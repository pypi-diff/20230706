# Comparing `tmp/feedancy-0.0.8a0.tar.gz` & `tmp/feedancy-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.8a0.tar", max compression
+gzip compressed data, was "feedancy-0.0.8b0.tar", max compression
```

## Comparing `feedancy-0.0.8a0.tar` & `feedancy-0.0.8b0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      615 2023-07-03 17:31:45.058158 feedancy-0.0.8a0/feedancy/README.md
--rw-r--r--   0        0        0     1006 2023-07-06 16:29:17.102576 feedancy-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 feedancy-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-07-03 17:31:45.058158 feedancy-0.0.8b0/feedancy/README.md
+-rw-r--r--   0        0        0     1009 2023-07-06 16:31:30.374333 feedancy-0.0.8b0/pyproject.toml
+-rw-r--r--   0        0        0     1476 1970-01-01 00:00:00.000000 feedancy-0.0.8b0/PKG-INFO
```

### Comparing `feedancy-0.0.8a0/feedancy/README.md` & `feedancy-0.0.8b0/feedancy/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.8a0/pyproject.toml` & `feedancy-0.0.8b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,26 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.8a"
+version = "0.0.8b"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
 readme = "feedancy/README.md"
-packages = [
-    { include = 'feedancy' }
-]
+#packages = [
+#    { include = 'feedancy' }
+#]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.5.1"
 djangorestframework = ">=3.14"
 #Django = ">=4"
 gunicorn = ">=20.1.0"
```

### Comparing `feedancy-0.0.8a0/PKG-INFO` & `feedancy-0.0.8b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.8a0
+Version: 0.0.8b0
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

