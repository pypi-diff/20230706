# Comparing `tmp/aipha_geo_solutions-0.9.1.tar.gz` & `tmp/aipha_geo_solutions-0.9.2.tar.gz`

## Comparing `aipha_geo_solutions-0.9.1.tar` & `aipha_geo_solutions-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/example.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/__init__.py
--rw-r--r--   0        0        0   190120 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/operators.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/webservice_api.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/LICENSE
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/example.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/src/aipha_geo_solutions/__init__.py
+-rw-r--r--   0        0        0   190120 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/src/aipha_geo_solutions/operators.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/src/aipha_geo_solutions/webservice_api.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/LICENSE
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aipha_geo_solutions-0.9.2/PKG-INFO
```

### Comparing `aipha_geo_solutions-0.9.1/example.py` & `aipha_geo_solutions-0.9.2/example.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/operators.py` & `aipha_geo_solutions-0.9.2/src/aipha_geo_solutions/operators.py`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.1/src/aipha_geo_solutions/webservice_api.py` & `aipha_geo_solutions-0.9.2/src/aipha_geo_solutions/webservice_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   print("instance", instance_parameters)
   url = 'https://' + server_address +':443/run-operator'
   print(payload)
   r = grequests.post(url, json=payload, verify=verifySSL, timeout=3600.)
   return r
 
 def execute(requests):
-    return grequests.map(requests, size=10)
+    return grequests.map(requests, size=7)
 
 def running_services_request(
         username,
         password,
         server_address,
         verifySSL = True):
   payload = { \
```

### Comparing `aipha_geo_solutions-0.9.1/LICENSE` & `aipha_geo_solutions-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aipha_geo_solutions-0.9.1/pyproject.toml` & `aipha_geo_solutions-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aipha_geo_solutions"
-version = "0.9.1"
+version = "0.9.2"
 authors = [
   { name="Timo Hackel", email="timo.hackel@aipha.ch" },
 ]
 description = "A python API to the AIPHA webservices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `aipha_geo_solutions-0.9.1/PKG-INFO` & `aipha_geo_solutions-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipha_geo_solutions
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python API to the AIPHA webservices
 Project-URL: Homepage, https://github.com/AIPHA-Geo-Solutions/
 Project-URL: Bug Tracker, https://github.com/AIPHA-Geo-Solutions/AIPHAPythonAPI/issues
 Author-email: Timo Hackel <timo.hackel@aipha.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

