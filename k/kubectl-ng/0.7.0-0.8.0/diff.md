# Comparing `tmp/kubectl_ng-0.7.0.tar.gz` & `tmp/kubectl_ng-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubectl_ng-0.7.0.tar", max compression
+gzip compressed data, was "kubectl_ng-0.8.0.tar", max compression
```

## Comparing `kubectl_ng-0.7.0.tar` & `kubectl_ng-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       80 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/README.md
--rw-r--r--   0        0        0      185 2023-07-03 10:38:25.719257 kubectl_ng-0.7.0/kubectl_ng/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/_api_resources.py
--rw-r--r--   0        0        0      769 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/_formatters.py
--rw-r--r--   0        0        0     4285 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/_get.py
--rw-r--r--   0        0        0     1981 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/_version.py
--rw-r--r--   0        0        0     5464 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/_wait.py
--rw-r--r--   0        0        0      758 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/cli.py
--rw-r--r--   0        0        0     1029 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/tests/test_formatters.py
--rw-r--r--   0        0        0      818 2023-07-03 10:38:10.271012 kubectl_ng-0.7.0/kubectl_ng/tests/test_version.py
--rw-r--r--   0        0        0      623 2023-07-03 10:38:25.715257 kubectl_ng-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       80 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/README.md
+-rw-r--r--   0        0        0      185 2023-07-05 16:17:59.026904 kubectl_ng-0.8.0/kubectl_ng/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/_api_resources.py
+-rw-r--r--   0        0        0      769 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/_formatters.py
+-rw-r--r--   0        0        0     4285 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/_get.py
+-rw-r--r--   0        0        0     1981 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/_version.py
+-rw-r--r--   0        0        0     5464 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/_wait.py
+-rw-r--r--   0        0        0      758 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/cli.py
+-rw-r--r--   0        0        0     1029 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/tests/test_formatters.py
+-rw-r--r--   0        0        0      818 2023-07-05 16:17:37.250991 kubectl_ng-0.8.0/kubectl_ng/tests/test_version.py
+-rw-r--r--   0        0        0      623 2023-07-05 16:17:59.026904 kubectl_ng-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 kubectl_ng-0.8.0/PKG-INFO
```

### Comparing `kubectl_ng-0.7.0/kubectl_ng/_api_resources.py` & `kubectl_ng-0.8.0/kubectl_ng/_api_resources.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/_formatters.py` & `kubectl_ng-0.8.0/kubectl_ng/_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/_get.py` & `kubectl_ng-0.8.0/kubectl_ng/_get.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/_version.py` & `kubectl_ng-0.8.0/kubectl_ng/_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/_wait.py` & `kubectl_ng-0.8.0/kubectl_ng/_wait.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/cli.py` & `kubectl_ng-0.8.0/kubectl_ng/cli.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/tests/test_formatters.py` & `kubectl_ng-0.8.0/kubectl_ng/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/kubectl_ng/tests/test_version.py` & `kubectl_ng-0.8.0/kubectl_ng/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `kubectl_ng-0.7.0/pyproject.toml` & `kubectl_ng-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubectl-ng"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 readme = "README.md"
 packages = [{include = "kubectl_ng"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `kubectl_ng-0.7.0/PKG-INFO` & `kubectl_ng-0.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubectl-ng
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

