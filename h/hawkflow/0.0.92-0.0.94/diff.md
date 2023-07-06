# Comparing `tmp/hawkflow-0.0.92.tar.gz` & `tmp/hawkflow-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-fci3zisu/hawkflow-0.0.92.tar", last modified: Wed Jul  5 08:46:22 2023, max compression
+gzip compressed data, was "/Users/felbus/github/hawkflow-py/dist/.tmp-4s1mscg3/hawkflow-0.0.94.tar", last modified: Thu Jul  6 08:48:59 2023, max compression
```

## Comparing `hawkflow-0.0.92.tar` & `hawkflow-0.0.94.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/
--rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.92/LICENSE
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-05 08:46:22.000000 hawkflow-0.0.92/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.92/README.md
--rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-05 08:44:15.000000 hawkflow-0.0.92/pyproject.toml
--rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-05 08:46:22.000000 hawkflow-0.0.92/setup.cfg
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/
--rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/PKG-INFO
--rw-r--r--   0 felbus     (501) staff       (20)      556 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/SOURCES.txt
--rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/dependency_links.txt
--rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/requires.txt
--rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflow.egg-info/top_level.txt
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflowclient/
--rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.92/src/hawkflowclient/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)      879 2023-02-27 16:57:39.000000 hawkflow-0.0.92/src/hawkflowclient/_endpoints.py
--rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/_hawkflow_exceptions.py
--rw-r--r--   0 felbus     (501) staff       (20)     3463 2023-07-05 08:45:37.000000 hawkflow-0.0.92/src/hawkflowclient/_validation.py
--rw-r--r--   0 felbus     (501) staff       (20)     2714 2023-03-03 15:36:38.000000 hawkflow-0.0.92/src/hawkflowclient/hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/hawkflow_decorators.py
-drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-05 08:46:22.000000 hawkflow-0.0.92/src/hawkflowclient/tests/
--rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/tests/__init__.py
--rw-r--r--   0 felbus     (501) staff       (20)     3276 2023-02-20 15:32:46.000000 hawkflow-0.0.92/src/hawkflowclient/tests/test_hawkflow_api.py
--rw-r--r--   0 felbus     (501) staff       (20)     4518 2023-07-05 08:45:23.000000 hawkflow-0.0.92/src/hawkflowclient/tests/test_validation.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:48:59.000000 hawkflow-0.0.94/
+-rw-r--r--   0 felbus     (501) staff       (20)     1054 2023-02-20 15:32:46.000000 hawkflow-0.0.94/LICENSE
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-06 08:48:59.000000 hawkflow-0.0.94/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)     1264 2023-03-15 18:47:38.000000 hawkflow-0.0.94/README.md
+-rw-r--r--   0 felbus     (501) staff       (20)      843 2023-07-06 07:15:19.000000 hawkflow-0.0.94/pyproject.toml
+-rw-r--r--   0 felbus     (501) staff       (20)       38 2023-07-06 08:48:59.000000 hawkflow-0.0.94/setup.cfg
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/
+-rw-r--r--   0 felbus     (501) staff       (20)     1956 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/PKG-INFO
+-rw-r--r--   0 felbus     (501) staff       (20)      510 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 felbus     (501) staff       (20)        1 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       17 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/requires.txt
+-rw-r--r--   0 felbus     (501) staff       (20)       15 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflow.egg-info/top_level.txt
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflowclient/
+-rw-r--r--   0 felbus     (501) staff       (20)      199 2023-03-03 15:13:44.000000 hawkflow-0.0.94/src/hawkflowclient/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)      910 2023-07-06 07:19:23.000000 hawkflow-0.0.94/src/hawkflowclient/_endpoints.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1045 2023-02-20 15:32:46.000000 hawkflow-0.0.94/src/hawkflowclient/_hawkflow_exceptions.py
+-rw-r--r--   0 felbus     (501) staff       (20)     4980 2023-07-06 07:19:23.000000 hawkflow-0.0.94/src/hawkflowclient/_validation.py
+-rw-r--r--   0 felbus     (501) staff       (20)     2724 2023-07-06 07:19:23.000000 hawkflow-0.0.94/src/hawkflowclient/hawkflow_api.py
+-rw-r--r--   0 felbus     (501) staff       (20)     1816 2023-02-20 15:32:46.000000 hawkflow-0.0.94/src/hawkflowclient/hawkflow_decorators.py
+drwxr-xr-x   0 felbus     (501) staff       (20)        0 2023-07-06 08:48:59.000000 hawkflow-0.0.94/src/hawkflowclient/tests/
+-rw-r--r--   0 felbus     (501) staff       (20)        0 2023-02-20 15:32:46.000000 hawkflow-0.0.94/src/hawkflowclient/tests/__init__.py
+-rw-r--r--   0 felbus     (501) staff       (20)     8702 2023-07-06 07:14:36.000000 hawkflow-0.0.94/src/hawkflowclient/tests/test_validation.py
```

### Comparing `hawkflow-0.0.92/LICENSE` & `hawkflow-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.92/PKG-INFO` & `hawkflow-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.92
+Version: 0.0.94
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.92/README.md` & `hawkflow-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.92/pyproject.toml` & `hawkflow-0.0.94/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="hawkflow"
-version="0.0.92"
+version="0.0.94"
 description="HawkFlow.ai"
 readme = "README.md"
 keywords=["hawkflow", "hawkflowclient", "monitoring"]
 license = {text = "LICENSE"}
 requires-python = ">=3.7"
 dependencies=[
     "requests>=2.25.1"
```

### Comparing `hawkflow-0.0.92/src/hawkflow.egg-info/PKG-INFO` & `hawkflow-0.0.94/src/hawkflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hawkflow
-Version: 0.0.92
+Version: 0.0.94
 Summary: HawkFlow.ai
 License: LICENSE
 Project-URL: Homepage, https://github.com/hawkflow/hawkflow-py
 Keywords: hawkflow,hawkflowclient,monitoring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `hawkflow-0.0.92/src/hawkflowclient/_endpoints.py` & `hawkflow-0.0.94/src/hawkflowclient/_endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,21 +14,22 @@
         "meta": meta,
         "uid": uid
     })
 
     return x
 
 
-def _metric_data(process: str, meta: str, items: dict) -> str:
-    _validate_metric_data(process, meta, items)
+def _metric_data(process: str, meta: str, items: dict, df: int) -> str:
+    _validate_metric_data(process, meta, items, df)
 
     x = json.dumps({
         "process": process,
         "meta": meta,
-        "items": items
+        "items": items,
+        "df": df
     })
 
     return x
 
 
 def _exception_data(process: str, meta: str, exception_text: str) -> str:
     _validate_exception_data(process, meta, exception_text)
```

### Comparing `hawkflow-0.0.92/src/hawkflowclient/_hawkflow_exceptions.py` & `hawkflow-0.0.94/src/hawkflowclient/_hawkflow_exceptions.py`

 * *Files identical despite different names*

### Comparing `hawkflow-0.0.92/src/hawkflowclient/_validation.py` & `hawkflow-0.0.94/src/hawkflowclient/_validation.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 
 
 def _validate_timed_data(process: str, meta: str, uid: str):
     _validate_core(process, meta)
     _validate_uid(uid)
 
 
-def _validate_metric_data(process: str, meta: str, items: dict):
+def _validate_metric_data(process: str, meta: str, items: dict, df: int):
     _validate_core(process, meta)
-    _validate_metric_items(items)
+
+    if df == 1:
+        _validate_metric_items_df(items)
+    else:
+        _validate_metric_items(items)
 
 
 def _validate_exception_data(process: str, meta: str, exception_text: str):
     _validate_core(process, meta)
     _validate_exception_text(exception_text)
 
 
@@ -102,7 +106,35 @@
             raise HawkFlowDataTypesException(_metric_text)
 
         if key == "":
             raise HawkFlowDataTypesException("metric items parameter dictionary key cannot be empty")
 
         if not re.match(METRIC_KEY_REGEX, key):
             raise HawkFlowDataTypesException("metric items parameter dictionary key contains illegal characters")
+
+
+def _validate_metric_items_df(items):
+    _metric_text = "metric items df parameter should be a dict {STR:{str:FLOAT or INT}, {str:FLOAT or INT}}"
+
+    if not isinstance(items, dict):
+        raise HawkFlowDataTypesException("metric items parameter must be type dict {STR:FLOAT or INT}")
+
+    if not items:
+        raise HawkFlowDataTypesException("metric items cannot be empty")
+
+    for key, value in items.items():
+        if not re.match(METRIC_KEY_REGEX, key):
+            raise HawkFlowDataTypesException("metric items parameter dictionary key contains illegal characters")
+        if key == "":
+            raise HawkFlowDataTypesException("metric items parameter dictionary key cannot be empty")
+        # Check if each item in the dictionary is also a dictionary
+        if not isinstance(value, dict):
+            raise HawkFlowDataTypesException(_metric_text)
+
+        for sub_key, sub_value in value.items():
+            if not re.match(METRIC_KEY_REGEX, sub_key):
+                raise HawkFlowDataTypesException("metric items parameter dictionary key contains illegal characters")
+            if sub_key == "":
+                raise HawkFlowDataTypesException("metric items parameter dictionary key cannot be empty")
+            # Check if each value in the sub-dictionaries is an integer (or a float)
+            if not isinstance(sub_value, (int, float)):
+                raise HawkFlowDataTypesException(_metric_text)
```

### Comparing `hawkflow-0.0.92/src/hawkflowclient/hawkflow_api.py` & `hawkflow-0.0.94/src/hawkflowclient/hawkflow_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 class HawkflowAPI:
     def __init__(self, api_key="", max_retries=3, wait_time=1):
         self.api_key = api_key
         self.max_retries = max_retries
         self.wait_time = wait_time
 
-    def metrics(self, process: str, meta: str = "", items=None):
+    def metrics(self, process: str, meta: str = "", items=None, df=0):
         try:
             if items is None:
                 items = []
 
             url = f"{_hawkflow_api_url}/metrics"
-            data = _metric_data(process, meta, items)
+            data = _metric_data(process, meta, items, df)
             return self._hawkflow_post(url, data)
         except HawkFlowException as he:
             logging.error(f"HawkFlowException - {str(he)}")
 
     def exception(self, process: str, meta: str = "", exception_text: str = ""):
         try:
             url = f"{_hawkflow_api_url}/exception"
```

### Comparing `hawkflow-0.0.92/src/hawkflowclient/hawkflow_decorators.py` & `hawkflow-0.0.94/src/hawkflowclient/hawkflow_decorators.py`

 * *Files identical despite different names*

