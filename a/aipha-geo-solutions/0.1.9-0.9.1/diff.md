# Comparing `tmp/aipha_geo_solutions-0.1.9.tar.gz` & `tmp/aipha_geo_solutions-0.9.1.tar.gz`

## Comparing `aipha_geo_solutions-0.1.9.tar` & `aipha_geo_solutions-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0   190120 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.1.9/example.py` & `aipha_geo_solutions-0.9.1/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.9/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/webservice_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import grequests
 import requests
 import argparse
 import urllib
 import json
 import ssl
 import time
 
@@ -47,17 +48,22 @@
     instance_parameters = {}
     if 'instance_type' in parameters:
         instance_parameters['instance_type'] = parameters['instance_type']
     elif 'instance_type' in command_dict[command]:
         instance_parameters['instance_type'] = command_dict[command]['instance_type']['default_value']
     for parameter in valid_parameters:
         if parameter in parameters:
-            all_parameters[parameter] = parameters[parameter]
+            all_parameters[parameter] = str(parameters[parameter])
+            if len(all_parameters[parameter]) > 0 and all_parameters[parameter][0] != "'":
+                all_parameters[parameter] = "'" + all_parameters[parameter]
+            if len(all_parameters[parameter]) > 0 and all_parameters[parameter][-1] != "'":
+                all_parameters[parameter] = all_parameters[parameter] + "'"
+            all_parameters[parameter] = all_parameters[parameter].replace('"', '\\"')
         else:
-            all_parameters[parameter] = valid_parameters[parameter]['default_value']
+            all_parameters[parameter] = str(valid_parameters[parameter]['default_value'])
     return all_parameters, instance_parameters, image_name
 
 glob_commands = {}
 def import_commands(server_address,
                     verifySSL = True):
     url = "https://" + server_address + "/default_functions.json"
     global glob_commands
@@ -89,22 +95,20 @@
           'command': image_name, \
           'parameters': all_parameters, \
           'operator_name': command, \
           'instance_parameters': instance_parameters \
             }
   print("instance", instance_parameters)
   url = 'https://' + server_address +':443/run-operator'
-  r = requests.post(url, json=payload, verify=verifySSL)
-  try:
-    result = json.loads(r.text)
-    if 'error' in result:
-      raise RuntimeError('AIPHAProcessingError: ' + result['error'])
-  except:
-      raise RuntimeError('AIPHAProcessingError: ' + r.text)
-  return result
+  print(payload)
+  r = grequests.post(url, json=payload, verify=verifySSL, timeout=3600.)
+  return r
+
+def execute(requests):
+    return grequests.map(requests, size=10)
 
 def running_services_request(
         username,
         password,
         server_address,
         verifySSL = True):
   payload = { \
@@ -138,15 +142,16 @@
     running_services =  running_services_request(
         username,
         password,
         server_address,
         verifySSL
     )
     services_dict = json.loads(running_services['running_processes'])
-    for service_id in services:
+    for service_promise in services:
+      service_id = service_promise
       this_complete = True #ignore services that have been deleted
       for running_service in services_dict:
         if service_id.startswith(running_service['ID']):
           this_complete = False
           if '1/1 completed' in running_service['Replicas']:
               this_complete = True
               break
```

### Comparing `aipha_geo_solutions-0.1.9/LICENSE` & `aipha_geo_solutions-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.1.9/pyproject.toml` & `aipha_geo_solutions-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.1.9"
+version = "0.9.1"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
-requires-python = ">=3.5"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `aipha_geo_solutions-0.1.9/PKG-INFO` & `aipha_geo_solutions-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.1.9
+Version: 0.9.1
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # AIPHA Python API
 
 This package contains the AIPHA python API. You can install it via:
 
 	pip install aipha_geo_solutions
```

