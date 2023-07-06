# Comparing `tmp/smbls-1.1.1.tar.gz` & `tmp/smbls-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smbls-1.1.1.tar", last modified: Fri Dec  2 15:36:27 2022, max compression
+gzip compressed data, was "smbls-1.1.2.tar", last modified: Thu Jul  6 21:14:26 2023, max compression
```

## Comparing `smbls-1.1.1.tar` & `smbls-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2022-12-02 15:36:27.516004 smbls-1.1.1/
--rw-r--r--   0 aralls    (1000) aralls    (1000)     1069 2022-12-02 15:36:11.000000 smbls-1.1.1/LICENSE
--rw-r--r--   0 aralls    (1000) aralls    (1000)     3661 2022-12-02 15:36:27.516004 smbls-1.1.1/PKG-INFO
--rw-r--r--   0 aralls    (1000) aralls    (1000)     3209 2022-12-02 15:36:11.000000 smbls-1.1.1/README.md
--rw-r--r--   0 aralls    (1000) aralls    (1000)      100 2022-10-05 19:52:10.000000 smbls-1.1.1/pyproject.toml
--rw-r--r--   0 aralls    (1000) aralls    (1000)      583 2022-12-02 15:36:27.516004 smbls-1.1.1/setup.cfg
-drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2022-12-02 15:36:27.516004 smbls-1.1.1/smbls/
--rwxr-xr-x   0 aralls    (1000) aralls    (1000)     9694 2022-12-02 15:36:11.000000 smbls-1.1.1/smbls/__init__.py
-drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2022-12-02 15:36:27.516004 smbls-1.1.1/smbls.egg-info/
--rw-r--r--   0 aralls    (1000) aralls    (1000)     3661 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/PKG-INFO
--rw-r--r--   0 aralls    (1000) aralls    (1000)      236 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/SOURCES.txt
--rw-r--r--   0 aralls    (1000) aralls    (1000)        1 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/dependency_links.txt
--rw-r--r--   0 aralls    (1000) aralls    (1000)       37 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/entry_points.txt
--rw-r--r--   0 aralls    (1000) aralls    (1000)        9 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/requires.txt
--rw-r--r--   0 aralls    (1000) aralls    (1000)        6 2022-12-02 15:36:27.000000 smbls-1.1.1/smbls.egg-info/top_level.txt
+drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2023-07-06 21:14:26.119463 smbls-1.1.2/
+-rw-r--r--   0 aralls    (1000) aralls    (1000)     1069 2023-07-06 20:50:51.000000 smbls-1.1.2/LICENSE
+-rw-r--r--   0 aralls    (1000) aralls    (1000)     3587 2023-07-06 21:14:26.119463 smbls-1.1.2/PKG-INFO
+-rw-r--r--   0 aralls    (1000) aralls    (1000)     3135 2023-07-06 20:50:51.000000 smbls-1.1.2/README.md
+-rw-r--r--   0 aralls    (1000) aralls    (1000)      100 2023-07-06 20:50:51.000000 smbls-1.1.2/pyproject.toml
+-rw-r--r--   0 aralls    (1000) aralls    (1000)      583 2023-07-06 21:14:26.119463 smbls-1.1.2/setup.cfg
+drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2023-07-06 21:14:26.116130 smbls-1.1.2/smbls/
+-rwxr-xr-x   0 aralls    (1000) aralls    (1000)     9769 2023-07-06 20:53:13.000000 smbls-1.1.2/smbls/__init__.py
+drwxr-xr-x   0 aralls    (1000) aralls    (1000)        0 2023-07-06 21:14:26.116130 smbls-1.1.2/smbls.egg-info/
+-rw-r--r--   0 aralls    (1000) aralls    (1000)     3587 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/PKG-INFO
+-rw-r--r--   0 aralls    (1000) aralls    (1000)      236 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/SOURCES.txt
+-rw-r--r--   0 aralls    (1000) aralls    (1000)        1 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/dependency_links.txt
+-rw-r--r--   0 aralls    (1000) aralls    (1000)       37 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/entry_points.txt
+-rw-r--r--   0 aralls    (1000) aralls    (1000)        9 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/requires.txt
+-rw-r--r--   0 aralls    (1000) aralls    (1000)        6 2023-07-06 21:14:26.000000 smbls-1.1.2/smbls.egg-info/top_level.txt
```

### Comparing `smbls-1.1.1/LICENSE` & `smbls-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smbls-1.1.1/PKG-INFO` & `smbls-1.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smbls
-Version: 1.1.1
+Version: 1.1.2
 Summary: list SMB shares
 Home-page: https://github.com/CarveSystems/smbls
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -74,20 +74,18 @@
 # Search for D drives
 jq -r 'path(..|select(.name?==$name))[0]' out.json --arg name D
 ```
 
 List hosts with corresponding readable shares:
 
 ```sh
+# JSON output
 jq -r '[.[] | select(.shares) | {ip: (.info.getRemoteHost), host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | {name: .name, type: .type, remark: .remark}]} | select(.readshares != [])]' out.json
-# With less output
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | .name]} | select(.readshares != [])' out.json
-# Excluding print$ and IPC$ shares:
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "" and ([.name] | inside($badsharenames) | not)) | .name]} | select(.readshares != [])' --argjson badsharenames '["print$", "IPC$"]' out.json
-
+# Formatted as a list of UNC paths, excluding a customizable list of shares
+jq -r '.[] | select(.shares) | .info.getServerDNSHostName as $host | .info.getRemoteHost as $ip | .shares[] | select(.access != "" and ([.name] | inside($exclude) | not)) | "\\\\" + (if $host == "" or $host == "\u0000" then $ip else $host end) + "\\" + .name' --argjson exclude '["print$", "IPC$"]' out.json
 ```
 
 List hosts that failed auth:
 
 ```sh
 jq -r 'path(.[]|select(.errtype == "auth"))[0]' out.json
 ```
```

### Comparing `smbls-1.1.1/README.md` & `smbls-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -59,20 +59,18 @@
 # Search for D drives
 jq -r 'path(..|select(.name?==$name))[0]' out.json --arg name D
 ```
 
 List hosts with corresponding readable shares:
 
 ```sh
+# JSON output
 jq -r '[.[] | select(.shares) | {ip: (.info.getRemoteHost), host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | {name: .name, type: .type, remark: .remark}]} | select(.readshares != [])]' out.json
-# With less output
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | .name]} | select(.readshares != [])' out.json
-# Excluding print$ and IPC$ shares:
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "" and ([.name] | inside($badsharenames) | not)) | .name]} | select(.readshares != [])' --argjson badsharenames '["print$", "IPC$"]' out.json
-
+# Formatted as a list of UNC paths, excluding a customizable list of shares
+jq -r '.[] | select(.shares) | .info.getServerDNSHostName as $host | .info.getRemoteHost as $ip | .shares[] | select(.access != "" and ([.name] | inside($exclude) | not)) | "\\\\" + (if $host == "" or $host == "\u0000" then $ip else $host end) + "\\" + .name' --argjson exclude '["print$", "IPC$"]' out.json
 ```
 
 List hosts that failed auth:
 
 ```sh
 jq -r 'path(.[]|select(.errtype == "auth"))[0]' out.json
 ```
```

### Comparing `smbls-1.1.1/setup.cfg` & `smbls-1.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = smbls
-version = 1.1.1
+version = 1.1.2
 description = list SMB shares
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CarveSystems/smbls
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `smbls-1.1.1/smbls/__init__.py` & `smbls-1.1.2/smbls/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
 import json
 import re
-from enum import IntFlag
 from multiprocessing import Pool
 from pathlib import Path
 from typing import Any, Dict, List, Tuple
 
 from impacket.dcerpc.v5 import srvs
 from impacket.smbconnection import SessionError, SMBConnection
 from impacket.nmb import NetBIOSTimeout
@@ -21,29 +20,14 @@
 
 password_regex = re.compile(r"(?P<domain>[^/:]*)/(?P<username>[^:]*):(?P<password>.*)")
 hash_regex = re.compile(
     r"(?P<domain>[^/:]*)/(?P<username>[^#]*)#(?P<lmhash>[a-fA-F0-9]{32}):(?P<nthash>[a-fA-F0-9]{32})"
 )
 
 
-class STypes(IntFlag):
-    """Share Types"""
-
-    DISKTREE = srvs.STYPE_DISKTREE
-    PRINTQ = srvs.STYPE_PRINTQ
-    DEVICE = srvs.STYPE_DEVICE
-    IPC = srvs.STYPE_IPC
-    CLUSTER_FS = srvs.STYPE_CLUSTER_FS
-    CLUSTER_SOFS = srvs.STYPE_CLUSTER_SOFS
-    CLUSTER_DFS = srvs.STYPE_CLUSTER_DFS
-
-    SPECIAL = srvs.STYPE_SPECIAL
-    TEMPORARY = srvs.STYPE_TEMPORARY
-
-
 def list_shares_multicred(
     argbundle: Tuple[List[Creds], str]
 ) -> Tuple[str, Dict[str, Scan]]:
     creds_list, host = argbundle
     res = dict()
     timed_out = False
     for creds in creds_list:
@@ -104,38 +88,47 @@
 
         # Get shares
         admin = False
         try:
             shares = list()
             for share in smbconn.listShares():
                 share_name = share["shi1_netname"][:-1]
+                if share["shi1_type"] & srvs.STYPE_MASK == srvs.STYPE_DISKTREE:
+                    share_type = "DISKTREE"
+                elif share["shi1_type"] & srvs.STYPE_MASK == srvs.STYPE_PRINTQ:
+                    share_type = "PRINTQ"
+                elif share["shi1_type"] & srvs.STYPE_MASK == srvs.STYPE_DEVICE:
+                    share_type = "DEVICE"
+                elif share["shi1_type"] & srvs.STYPE_MASK == srvs.STYPE_IPC:
+                    share_type = "IPC"
+                else:
+                    share_type = "error_unknown"
+                if share["shi1_type"] & srvs.STYPE_CLUSTER_FS:
+                    share_type += "|CLUSTER_FS"
+                if share["shi1_type"] & srvs.STYPE_CLUSTER_SOFS:
+                    share_type += "|CLUSTER_SOFS"
+                if share["shi1_type"] & srvs.STYPE_CLUSTER_DFS:
+                    share_type += "|CLUSTER_DFS"
+                if share["shi1_type"] & srvs.STYPE_SPECIAL:
+                    share_type += "|SPECIAL"
+                if share["shi1_type"] & srvs.STYPE_TEMPORARY:
+                    share_type += "|TEMPORARY"
                 try:
                     smbconn.listPath(share_name, "*")
                     access = "READ"
                     access_error = ""
                 except SessionError as e:
                     access_error = str(e)
                     access = ""
                 if (share_name == "C$" or share_name == "ADMIN$") and access:
                     admin = True
                 shares.append(
                     {
                         "name": share_name,
-                        "type_raw": STypes(share["shi1_type"]),
-                        # STYPE has a flag of 0 that is valid when the masked
-                        # value is 0, which IntFlag doesn't look for. This
-                        # adds the 0 flag (DISKTREE) iff there's a masked
-                        # value.
-                        "type": str(STypes(share["shi1_type"])).removeprefix("STypes.")
-                        + (
-                            "|DISKTREE"
-                            if STypes(share["shi1_type"]) & srvs.STYPE_MASK == 0
-                            and STypes(share["shi1_type"]) != 0
-                            else ""
-                        ),
+                        "type": share_type,
                         "remark": share["shi1_remark"][:-1],
                         "access": access,
                         "access_error": access_error,
                     }
                 )
         except Exception as e:
             return {"errtype": "shares", "error": str(e)}
```

### Comparing `smbls-1.1.1/smbls.egg-info/PKG-INFO` & `smbls-1.1.2/smbls.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smbls
-Version: 1.1.1
+Version: 1.1.2
 Summary: list SMB shares
 Home-page: https://github.com/CarveSystems/smbls
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -74,20 +74,18 @@
 # Search for D drives
 jq -r 'path(..|select(.name?==$name))[0]' out.json --arg name D
 ```
 
 List hosts with corresponding readable shares:
 
 ```sh
+# JSON output
 jq -r '[.[] | select(.shares) | {ip: (.info.getRemoteHost), host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | {name: .name, type: .type, remark: .remark}]} | select(.readshares != [])]' out.json
-# With less output
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "") | .name]} | select(.readshares != [])' out.json
-# Excluding print$ and IPC$ shares:
-jq -r '.[] | select(.shares) | {host: (.info.getServerDNSHostName), readshares: [.shares[] | select(.access != "" and ([.name] | inside($badsharenames) | not)) | .name]} | select(.readshares != [])' --argjson badsharenames '["print$", "IPC$"]' out.json
-
+# Formatted as a list of UNC paths, excluding a customizable list of shares
+jq -r '.[] | select(.shares) | .info.getServerDNSHostName as $host | .info.getRemoteHost as $ip | .shares[] | select(.access != "" and ([.name] | inside($exclude) | not)) | "\\\\" + (if $host == "" or $host == "\u0000" then $ip else $host end) + "\\" + .name' --argjson exclude '["print$", "IPC$"]' out.json
 ```
 
 List hosts that failed auth:
 
 ```sh
 jq -r 'path(.[]|select(.errtype == "auth"))[0]' out.json
 ```
```

