# Comparing `tmp/threatmon-0.0.4-py3-none-any.whl.zip` & `tmp/threatmon-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4021 bytes, number of entries: 8
+Zip file size: 4778 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       42 b- defN 23-Jun-05 19:03 threatmon/__init__.py
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-15 21:04 threatmon/ioc.py
+-rw-r--r--  2.0 unx    10364 b- defN 23-Jul-06 10:23 threatmon/ioc.py
 -rw-r--r--  2.0 unx      597 b- defN 23-Jun-05 16:51 threatmon/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-15 21:37 threatmon-0.0.4.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-15 21:37 threatmon-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 21:37 threatmon-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-15 21:37 threatmon-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 23-Jun-15 21:37 threatmon-0.0.4.dist-info/RECORD
-8 files, 7162 bytes uncompressed, 2935 bytes compressed:  59.0%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jul-06 10:32 threatmon-0.0.5.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      443 b- defN 23-Jul-06 10:32 threatmon-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 10:32 threatmon-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-06 10:32 threatmon-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 23-Jul-06 10:32 threatmon-0.0.5.dist-info/RECORD
+8 files, 13240 bytes uncompressed, 3692 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: threatmon/ioc.py
 Comment: 
 
 Filename: threatmon/utils.py
 Comment: 
 
-Filename: threatmon-0.0.4.dist-info/LICENCE.txt
+Filename: threatmon-0.0.5.dist-info/LICENCE.txt
 Comment: 
 
-Filename: threatmon-0.0.4.dist-info/METADATA
+Filename: threatmon-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: threatmon-0.0.4.dist-info/WHEEL
+Filename: threatmon-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: threatmon-0.0.4.dist-info/top_level.txt
+Filename: threatmon-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: threatmon-0.0.4.dist-info/RECORD
+Filename: threatmon-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## threatmon/ioc.py

```diff
@@ -1,13 +1,23 @@
 import json
+from pprint import pprint
 import requests
 import time
 import re
 import socket
+from OTXv2 import OTXv2, IndicatorTypes
 from stix2 import Indicator
+import json
+from pandas.io.json import json_normalize
+import requests
+import urllib3
+from base64 import b64encode
+
+# Disable insecure https warnings (for self-signed SSL certificates)
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 class ioc():
     def __init__(self, api_token = "", limit = 10):
         self.api_token = api_token
         self.headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
@@ -110,8 +120,178 @@
                 json=request_body,
             )
             if microsof_api.status_code == 200:
                 print(time.strftime("%H:%M:%S") + " -- " + " (Finished) Imported IOCs to Sentinel (Success)" )
             else:
                 print(time.strftime("%H:%M:%S") + " -- " + "Could not POST IOCs to Sentinel (Failure)")
         except Exception as e:
-            print(e)
+            print(e)
+            
+    def CrowdStrikeIntegration(self,
+                               bearerToken,
+                               import_data):
+        # sourcery skip: avoid-builtin-shadow
+        
+        api_url = "https://api.crowdstrike.com/iocs/entities/indicators/v1"
+        
+        ioc_list = []
+        
+        headers = {
+            'Authorization': bearerToken,
+            'Content-Type': 'application/json',
+        }
+        
+        for iocs in import_data["entities"]:
+            for ioc in iocs["hashes"]:
+                if ioc["algorithm"] == "MD5":
+                    value = ioc["hash"]
+                    type = "md5"
+                    
+                if ioc["algorithm"] == "SHA-256":
+                    value = ioc["hash"]
+                    type = "sha256"
+                    
+                if ioc["algorithm"] == "Domain":
+                    type = "domain"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV4":
+                    type = "ipv4"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV6":
+                    type = "ipv6"
+                    value = ioc["hash"]
+                    
+                ioc_dict = {
+                    "type": type,
+                    "value": value,
+                    "policy": "none",
+                    "apply_globally": False,
+                }
+                
+                ioc_list.append(ioc_dict)
+            
+        response_data = {
+            "indicators" : ioc_list,
+        }
+            
+        try:
+            crowdstrike = requests.post(
+                url=api_url,
+                headers=headers,
+                json=response_data,
+            )
+            
+            if crowdstrike.status_code == 200:
+                print(time.strftime("%H:%M:%S") + " -- " + " (Finished) Imported IOCs to CrowdStrike (Success)" )
+            else:
+                print(time.strftime("%H:%M:%S") + " -- " + "Could not POST IOCs to CrowdStrike (Failure)")
+                
+        except Exception as e:
+            print(e)
+
+    def SplunkIntegration(self, token, import_data):
+        # sourcery skip: avoid-builtin-shadow
+        api_url = "https://api.trustar.co/api/2.0/submissions/indicators/upsert"
+        
+        ioc_list = []
+        
+        headers = {
+            'Authorization': token,
+            'Content-Type': 'application/json',
+        }
+        
+        for iocs in import_data["entities"]:
+            for ioc in iocs["hashes"]:
+                if ioc["algorithm"] == "MD5":
+                    value = ioc["hash"]
+                    type = "MD5"
+                    
+                if ioc["algorithm"] == "SHA-256":
+                    value = ioc["hash"]
+                    type = "SHA256"
+                    
+                if ioc["algorithm"] == "Domain":
+                    type = "DOMAIN"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV4":
+                    type = "IP4"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV6":
+                    type = "IP6"
+                    value = ioc["hash"]
+                    
+                ioc_dict = {
+                    "id": "",
+                    "title": "Indicator from ThreatMon API",
+                    "enclaveGuid": "ThreatMon",
+                    "tags":["ioc","threatmon"],
+                    "observable": {
+                            "type": type,
+                            "value": value
+                        }
+                }
+                
+                ioc_list.append(ioc_dict)
+            
+        response_data = ioc_list
+            
+        try:
+            splunk = requests.post(
+                url=api_url,
+                headers=headers,
+                json=response_data,
+            )
+            
+            if splunk.status_code == 200:
+                print(time.strftime("%H:%M:%S") + " -- " + " (Finished) Imported IOCs to Splunk (Success)" )
+            else:
+                print(time.strftime("%H:%M:%S") + " -- " + "Could not POST IOCs to Splunk (Failure)")
+                
+        except Exception as e:
+            print(e)
+
+
+    def AlienVaultIntegration(self, token, import_data):
+        # sourcery skip: avoid-builtin-shadow        
+        ioc_list = []
+        otx = OTXv2(token)
+        
+        for iocs in import_data["entities"]:
+            for ioc in iocs["hashes"]:
+                if ioc["algorithm"] == "MD5":
+                    value = ioc["hash"]
+                    type = "FileHash-MD5"
+                    
+                if ioc["algorithm"] == "SHA-256":
+                    value = ioc["hash"]
+                    type = "FileHash-SHA256"
+                    
+                if ioc["algorithm"] == "Domain":
+                    type = "domain"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV4":
+                    type = "IPv4"
+                    value = ioc["hash"]
+                    
+                if ioc["algorithm"] == "IPV6":
+                    type = "IPv6"
+                    value = ioc["hash"]
+                    
+                ioc_dict = {
+                    "indicator": value,
+                    "description": "",
+                    "type": type,
+                }
+                
+                ioc_list.append(ioc_dict)
+                
+        try:
+            new_pulse = otx.create_pulse(name="Threatmon IOCs", indicators=ioc_list, public=False)
+            pprint(json_normalize(new_pulse))
+            
+        except Exception as e:
+            print(e)
```

## Comparing `threatmon-0.0.4.dist-info/LICENCE.txt` & `threatmon-0.0.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `threatmon-0.0.4.dist-info/RECORD` & `threatmon-0.0.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 threatmon/__init__.py,sha256=nXlXBoxbxeXzEDK0JXVCkIi47kcoch2e0GirpfTyquU,42
-threatmon/ioc.py,sha256=71zeZDve29TbLbfo0hz2KnyMRkK6RhCEEu9sLvWR7og,4308
+threatmon/ioc.py,sha256=sF3XBf_rRAIpKV-ej_RZl-KC-gFq3vGm3XwfIkpvCdM,10364
 threatmon/utils.py,sha256=SydslOhqSkZo6ppgSiYrDyP7ZIJd7h4pNXD3Gu6_9Tc,597
-threatmon-0.0.4.dist-info/LICENCE.txt,sha256=Kj1QsVeBn9NHAhuxP4DmX8ksX3OHTCzMVVV8NG6nW1o,1069
-threatmon-0.0.4.dist-info/METADATA,sha256=xq-hIkRBx2GGYeW0gQmpbYBoPRIs2tmP9Eccd5pDp7Y,422
-threatmon-0.0.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-threatmon-0.0.4.dist-info/top_level.txt,sha256=0m-UKHGwuR6fmNQ5DZTLtl7jOOC9RJjh0nqy91Dm6oE,10
-threatmon-0.0.4.dist-info/RECORD,,
+threatmon-0.0.5.dist-info/LICENCE.txt,sha256=Kj1QsVeBn9NHAhuxP4DmX8ksX3OHTCzMVVV8NG6nW1o,1069
+threatmon-0.0.5.dist-info/METADATA,sha256=5-1WWkcvaww5dpG6kGy20yG9bUCUvbQg0MqBnKon49U,443
+threatmon-0.0.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+threatmon-0.0.5.dist-info/top_level.txt,sha256=0m-UKHGwuR6fmNQ5DZTLtl7jOOC9RJjh0nqy91Dm6oE,10
+threatmon-0.0.5.dist-info/RECORD,,
```

