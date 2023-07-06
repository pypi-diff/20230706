# Comparing `tmp/weave-py-api-1.2.0.tar.gz` & `tmp/weave-py-api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-py-api-1.2.0.tar", last modified: Wed Jun  7 09:23:48 2023, max compression
+gzip compressed data, was "weave-py-api-1.2.1.tar", last modified: Thu Jul  6 11:54:10 2023, max compression
```

## Comparing `weave-py-api-1.2.0.tar` & `weave-py-api-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.694781 weave-py-api-1.2.0/
--rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.2.0/LICENSE
--rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2648 2023-06-07 09:23:48.693780 weave-py-api-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-06-07 09:20:21.000000 weave-py-api-1.2.0/README.md
--rw-rw-rw-   0        0        0     1436 2023-06-07 09:23:13.000000 weave-py-api-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 09:23:48.694781 weave-py-api-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.662789 weave-py-api-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.680781 weave-py-api-1.2.0/src/weave_py_api.egg-info/
--rw-rw-rw-   0        0        0     2648 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 09:23:48.000000 weave-py-api-1.2.0/src/weave_py_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 09:23:48.693780 weave-py-api-1.2.0/src/weaveapi/
--rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/__init__.py
--rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.2.0/src/weaveapi/apicontext.py
--rw-rw-rw-   0        0        0    34203 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/clienthttp.py
--rw-rw-rw-   0        0        0    40963 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/clientws.py
--rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.2.0/src/weaveapi/filter.py
--rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/futures.py
--rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.2.0/src/weaveapi/javarandom.py
--rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.2.0/src/weaveapi/keys.py
--rw-rw-rw-   0        0        0    14919 2023-05-09 11:29:57.000000 weave-py-api-1.2.0/src/weaveapi/nodeapi.py
--rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.2.0/src/weaveapi/options.py
--rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.2.0/src/weaveapi/records.py
--rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.2.0/src/weaveapi/session.py
--rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.2.0/src/weaveapi/setup.py
--rw-rw-rw-   0        0        0     4282 2023-01-25 16:39:28.000000 weave-py-api-1.2.0/src/weaveapi/utils.py
--rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.2.0/src/weaveapi/weaveapi.py
--rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.2.0/src/weaveapi/weaveh.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:54:10.905799 weave-py-api-1.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-07 05:54:07.000000 weave-py-api-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-06-07 06:24:55.000000 weave-py-api-1.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2642 2023-07-06 11:54:10.903799 weave-py-api-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2023-06-08 14:14:22.000000 weave-py-api-1.2.1/README.md
+-rw-rw-rw-   0        0        0     1436 2023-07-06 11:46:51.000000 weave-py-api-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 11:54:10.905799 weave-py-api-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 11:54:10.866543 weave-py-api-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 11:54:10.876570 weave-py-api-1.2.1/src/weave_py_api.egg-info/
+-rw-rw-rw-   0        0        0     2642 2023-07-06 11:54:10.000000 weave-py-api-1.2.1/src/weave_py_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-07-06 11:54:10.000000 weave-py-api-1.2.1/src/weave_py_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 11:54:10.000000 weave-py-api-1.2.1/src/weave_py_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-07-06 11:54:10.000000 weave-py-api-1.2.1/src/weave_py_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 11:54:10.000000 weave-py-api-1.2.1/src/weave_py_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 11:54:10.903799 weave-py-api-1.2.1/src/weaveapi/
+-rw-rw-rw-   0        0        0        0 2022-03-20 14:22:30.000000 weave-py-api-1.2.1/src/weaveapi/__init__.py
+-rw-rw-rw-   0        0        0     3817 2023-01-27 18:40:16.000000 weave-py-api-1.2.1/src/weaveapi/apicontext.py
+-rw-rw-rw-   0        0        0    34202 2023-06-27 04:34:57.000000 weave-py-api-1.2.1/src/weaveapi/clienthttp.py
+-rw-rw-rw-   0        0        0    40958 2023-06-27 11:11:41.000000 weave-py-api-1.2.1/src/weaveapi/clientws.py
+-rw-rw-rw-   0        0        0     3968 2023-02-28 07:27:53.000000 weave-py-api-1.2.1/src/weaveapi/filter.py
+-rw-rw-rw-   0        0        0      363 2022-03-20 14:22:30.000000 weave-py-api-1.2.1/src/weaveapi/futures.py
+-rw-rw-rw-   0        0        0     5015 2022-12-30 12:27:54.000000 weave-py-api-1.2.1/src/weaveapi/javarandom.py
+-rw-rw-rw-   0        0        0     3455 2022-12-12 12:20:08.000000 weave-py-api-1.2.1/src/weaveapi/keys.py
+-rw-rw-rw-   0        0        0    14919 2023-05-09 11:29:57.000000 weave-py-api-1.2.1/src/weaveapi/nodeapi.py
+-rw-rw-rw-   0        0        0    14300 2023-04-05 10:54:57.000000 weave-py-api-1.2.1/src/weaveapi/options.py
+-rw-rw-rw-   0        0        0      984 2022-12-30 12:27:54.000000 weave-py-api-1.2.1/src/weaveapi/records.py
+-rw-rw-rw-   0        0        0      884 2023-01-23 13:53:04.000000 weave-py-api-1.2.1/src/weaveapi/session.py
+-rw-rw-rw-   0        0        0      894 2022-03-28 18:45:18.000000 weave-py-api-1.2.1/src/weaveapi/setup.py
+-rw-rw-rw-   0        0        0     4302 2023-07-06 11:46:23.000000 weave-py-api-1.2.1/src/weaveapi/utils.py
+-rw-rw-rw-   0        0        0       81 2022-03-20 14:22:30.000000 weave-py-api-1.2.1/src/weaveapi/weaveapi.py
+-rw-rw-rw-   0        0        0     4980 2023-03-15 09:17:36.000000 weave-py-api-1.2.1/src/weaveapi/weaveh.py
```

### Comparing `weave-py-api-1.2.0/LICENSE` & `weave-py-api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/PKG-INFO` & `weave-py-api-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,15 +40,15 @@
 
 #### How to install
 
 ```sh
 pip install weave-py-api
 ```
 
-#### Simple read sample
+#### Data read sample
 
 ```python
 from weaveapi import weaveapi
 from weaveapi.records import *
 from weaveapi.options import *
 from weaveapi.weaveh import *
 
@@ -60,14 +60,14 @@
 organization = "weavedemo"
 scope = "shared"
 table = "directory"
 
 cfg = weave_client_config(pub, pvk, node, organization)
 nodeApi, session = connect_weave_api(cfg)
 
-reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_MUX_NO_CHAIN).get()
+reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_NO_CHAIN).get()
 print(reply["data"])
 ```
 
 #### Docs
 
 [https://docs.weavechain.com](https://docs.weavechain.com)
```

### Comparing `weave-py-api-1.2.0/README.md` & `weave-py-api-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #### How to install
 
 ```sh
 pip install weave-py-api
 ```
 
-#### Simple read sample
+#### Data read sample
 
 ```python
 from weaveapi import weaveapi
 from weaveapi.records import *
 from weaveapi.options import *
 from weaveapi.weaveh import *
 
@@ -24,14 +24,14 @@
 organization = "weavedemo"
 scope = "shared"
 table = "directory"
 
 cfg = weave_client_config(pub, pvk, node, organization)
 nodeApi, session = connect_weave_api(cfg)
 
-reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_MUX_NO_CHAIN).get()
+reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_NO_CHAIN).get()
 print(reply["data"])
 ```
 
 #### Docs
 
 [https://docs.weavechain.com](https://docs.weavechain.com)
```

### Comparing `weave-py-api-1.2.0/pyproject.toml` & `weave-py-api-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "weave-py-api"
-version = "1.2.0"
+version = "1.2.1"
 description = "Weavechain Python API"
 readme = "README.md"
 authors = [{ name = "Weavechain", email = "support@weavechain.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `weave-py-api-1.2.0/src/weave_py_api.egg-info/PKG-INFO` & `weave-py-api-1.2.1/src/weave_py_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-py-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Weavechain Python API
 Author-email: Weavechain <support@weavechain.com>
 License: MIT License
         
         Copyright (c) 2023 Weavechain
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,15 +40,15 @@
 
 #### How to install
 
 ```sh
 pip install weave-py-api
 ```
 
-#### Simple read sample
+#### Data read sample
 
 ```python
 from weaveapi import weaveapi
 from weaveapi.records import *
 from weaveapi.options import *
 from weaveapi.weaveh import *
 
@@ -60,14 +60,14 @@
 organization = "weavedemo"
 scope = "shared"
 table = "directory"
 
 cfg = weave_client_config(pub, pvk, node, organization)
 nodeApi, session = connect_weave_api(cfg)
 
-reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_MUX_NO_CHAIN).get()
+reply = nodeApi.read(session, scope, table, None, READ_DEFAULT_NO_CHAIN).get()
 print(reply["data"])
 ```
 
 #### Docs
 
 [https://docs.weavechain.com](https://docs.weavechain.com)
```

### Comparing `weave-py-api-1.2.0/src/weave_py_api.egg-info/SOURCES.txt` & `weave-py-api-1.2.1/src/weave_py_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/apicontext.py` & `weave-py-api-1.2.1/src/weaveapi/apicontext.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/clienthttp.py` & `weave-py-api-1.2.1/src/weaveapi/clienthttp.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
 
     def taskLineage(self, session, taskId):
         data = {"taskId": taskId}
 
         return self.authPost(session, "task_lineage", data)
 
     def verifyTaskLineage(self, session, lineageData):
-        data = {"task_lineage": task_lineage}
+        data = {"task_lineage": lineageData}
 
         return self.authPost(session, "verify_task_lineage", data)
 
     def taskOutputData(self, session, taskId, options):
         data = {"taskId": taskId, "options": options.toJson()}
 
         return self.authPost(session, "task_output_data", data)
```

### Comparing `weave-py-api-1.2.0/src/weaveapi/clientws.py` & `weave-py-api-1.2.1/src/weaveapi/clientws.py`

 * *Files 0% similar despite different names*

```diff
@@ -864,15 +864,15 @@
         data = {
             "type": "get_scopes",
         }
         return self.authPost(session, data)
 
     def getTables(self, session, scope):
         data = {
-            "type": "get_node_config",
+            "type": "get_tables",
             "scope": scope
         }
         return self.authPost(session, data)
 
     def getNodeConfig(self, session, nodePublicKey):
         data = {
             "type": "get_node_config",
```

### Comparing `weave-py-api-1.2.0/src/weaveapi/filter.py` & `weave-py-api-1.2.1/src/weaveapi/filter.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/javarandom.py` & `weave-py-api-1.2.1/src/weaveapi/javarandom.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/keys.py` & `weave-py-api-1.2.1/src/weaveapi/keys.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/nodeapi.py` & `weave-py-api-1.2.1/src/weaveapi/nodeapi.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/options.py` & `weave-py-api-1.2.1/src/weaveapi/options.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/records.py` & `weave-py-api-1.2.1/src/weaveapi/records.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/session.py` & `weave-py-api-1.2.1/src/weaveapi/session.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/setup.py` & `weave-py-api-1.2.1/src/weaveapi/setup.py`

 * *Files identical despite different names*

### Comparing `weave-py-api-1.2.0/src/weaveapi/utils.py` & `weave-py-api-1.2.1/src/weaveapi/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             salt = bytes(seedHex, encoding='utf-8')
 
             idBuffer = ""
             hashBuffer = ""
             first = True
             for r in records.records:
                 record = standardizeRecord(r, layout)
-                data = record.toJson() if isinstance(record, Record) else json.dumps(record, separators=(',', ':'))
+                data = record.toJson() if isinstance(record, Record) else json.dumps(record, separators=(',', ':'), ensure_ascii=False)
                 hash = hashFn(salt, data)
 
                 if first:
                     first = False
                 else:
                     idBuffer += " "
                     hashBuffer += "\n"
```

### Comparing `weave-py-api-1.2.0/src/weaveapi/weaveh.py` & `weave-py-api-1.2.1/src/weaveapi/weaveh.py`

 * *Files identical despite different names*

