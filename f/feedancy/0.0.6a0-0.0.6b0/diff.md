# Comparing `tmp/feedancy-0.0.6a0.tar.gz` & `tmp/feedancy-0.0.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.6a0.tar", max compression
+gzip compressed data, was "feedancy-0.0.6b0.tar", max compression
```

## Comparing `feedancy-0.0.6a0.tar` & `feedancy-0.0.6b0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.6a0/feedancy-client/README.md
--rw-r--r--   0        0        0     1018 2023-07-03 17:33:21.022198 feedancy-0.0.6a0/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 feedancy-0.0.6a0/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.6b0/feedancy-client/README.md
+-rw-r--r--   0        0        0     1006 2023-07-06 15:47:43.313866 feedancy-0.0.6b0/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 feedancy-0.0.6b0/PKG-INFO
```

### Comparing `feedancy-0.0.6a0/feedancy-client/README.md` & `feedancy-0.0.6b0/feedancy-client/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.6a0/pyproject.toml` & `feedancy-0.0.6b0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -15,26 +15,26 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.6a"
+version = "0.0.6b"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
 readme = "./feedancy-client/README.md"
-#packages = [
-#    { include = 'feedancy/feedancy' }
-#]
+packages = [
+    { include = 'feedancy' }
+]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 #djangorestframework = ">=3.14.0"
 #Django = ">=4"
 #gunicorn = ">=20.1.0"
 #psycopg2-binary = ">=2.9.6"
```

### Comparing `feedancy-0.0.6a0/PKG-INFO` & `feedancy-0.0.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.6a0
+Version: 0.0.6b0
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

