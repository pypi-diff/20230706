# Comparing `tmp/testdwg-1.2.0.tar.gz` & `tmp/testdwg-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testdwg-1.2.0.tar", max compression
+gzip compressed data, was "testdwg-1.2.1.tar", max compression
```

## Comparing `testdwg-1.2.0.tar` & `testdwg-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-06 13:41:53.409567 testdwg-1.2.0/LICENSE
--rw-r--r--   0        0        0        9 2023-07-06 13:41:53.409567 testdwg-1.2.0/README.md
--rw-r--r--   0        0        0      639 2023-07-06 13:42:06.453694 testdwg-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-07-06 13:41:53.409567 testdwg-1.2.0/testdwg/__init__.py
--rw-r--r--   0        0        0       29 2023-07-06 13:41:53.409567 testdwg-1.2.0/testdwg/main.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 testdwg-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 13:45:50.839113 testdwg-1.2.1/LICENSE
+-rw-r--r--   0        0        0        9 2023-07-06 13:45:50.839113 testdwg-1.2.1/README.md
+-rw-r--r--   0        0        0      639 2023-07-06 13:46:06.583140 testdwg-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-07-06 13:45:50.839113 testdwg-1.2.1/testdwg/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-06 13:45:50.839113 testdwg-1.2.1/testdwg/main.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 testdwg-1.2.1/PKG-INFO
```

### Comparing `testdwg-1.2.0/LICENSE` & `testdwg-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `testdwg-1.2.0/pyproject.toml` & `testdwg-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testdwg"
-version = "1.2.0"  # not used
+version = "1.2.1"  # not used
 description = ""
 license = "MIT"
 authors = ["yatmanov <yatmanov@megaputer.ru>"]
 readme = "README.md"
 repository = "https://github.com/yatmanov/testdwg"
 documentation = "https://yatmanov.github.io/testdwg/"
```

### Comparing `testdwg-1.2.0/PKG-INFO` & `testdwg-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testdwg
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Home-page: https://github.com/yatmanov/testdwg
 License: MIT
 Author: yatmanov
 Author-email: yatmanov@megaputer.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

