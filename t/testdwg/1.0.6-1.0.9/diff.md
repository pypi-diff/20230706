# Comparing `tmp/testdwg-1.0.6.tar.gz` & `tmp/testdwg-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-1.0.6.tar", max compression
+gzip compressed data, was "testdwg-1.0.9.tar", max compression
```

## Comparing `testdwg-1.0.6.tar` & `testdwg-1.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-06 10:53:41.324177 testdwg-1.0.6/LICENSE
--rw-r--r--   0        0        0        9 2023-07-06 10:53:41.324177 testdwg-1.0.6/README.md
--rw-r--r--   0        0        0      639 2023-07-06 10:53:59.908355 testdwg-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-06 10:53:41.324177 testdwg-1.0.6/testdwg/__init__.py
--rw-r--r--   0        0        0       29 2023-07-06 10:53:41.324177 testdwg-1.0.6/testdwg/main.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 testdwg-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 11:02:44.423426 testdwg-1.0.9/LICENSE
+-rw-r--r--   0        0        0        9 2023-07-06 11:02:44.423426 testdwg-1.0.9/README.md
+-rw-r--r--   0        0        0      639 2023-07-06 11:03:02.451514 testdwg-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-06 11:02:44.427426 testdwg-1.0.9/testdwg/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-06 11:02:44.427426 testdwg-1.0.9/testdwg/main.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 testdwg-1.0.9/PKG-INFO
```

### Comparing `testdwg-1.0.6/LICENSE` & `testdwg-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `testdwg-1.0.6/pyproject.toml` & `testdwg-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testdwg"
-version = "1.0.6"  # not used
+version = "1.0.9"  # not used
 description = ""
 license = "MIT"
 authors = ["yatmanov <yatmanov@megaputer.ru>"]
 readme = "README.md"
 repository = "https://github.com/yatmanov/testdwg"
 documentation = "https://yatmanov.github.io/testdwg/"
```

### Comparing `testdwg-1.0.6/PKG-INFO` & `testdwg-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdwg
-Version: 1.0.6
+Version: 1.0.9
 Summary: 
 Home-page: https://github.com/yatmanov/testdwg
 License: MIT
 Author: yatmanov
 Author-email: yatmanov@megaputer.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

