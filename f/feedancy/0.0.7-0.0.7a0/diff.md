# Comparing `tmp/feedancy-0.0.7.tar.gz` & `tmp/feedancy-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.7.tar", max compression
+gzip compressed data, was "feedancy-0.0.7a0.tar", max compression
```

## Comparing `feedancy-0.0.7.tar` & `feedancy-0.0.7a0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.7/feedancy-client/README.md
--rw-r--r--   0        0        0     1016 2023-07-06 16:05:45.821142 feedancy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 feedancy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.7a0/feedancy-client/README.md
+-rw-r--r--   0        0        0     1034 2023-07-06 16:08:26.066387 feedancy-0.0.7a0/pyproject.toml
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 feedancy-0.0.7a0/PKG-INFO
```

### Comparing `feedancy-0.0.7/feedancy-client/README.md` & `feedancy-0.0.7a0/feedancy-client/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.7/pyproject.toml` & `feedancy-0.0.7a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,30 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.7"
+version = "0.0.7a"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
 readme = "./feedancy-client/README.md"
 packages = [
     { include = './feedancy/feedancy' }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
+poetry = ">=1.5"
 #djangorestframework = ">=3.14.0"
 #Django = ">=4"
 #gunicorn = ">=20.1.0"
 #psycopg2-binary = ">=2.9.6"
 #Pillow = ">=9.5.0"
 #django-filter = ">=23.2"
 #pydantic = ">=1.10.8"
```

### Comparing `feedancy-0.0.7/PKG-INFO` & `feedancy-0.0.7a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.7
+Version: 0.0.7a0
 Summary: сервис по сбору вакансий
 License: MIT
 Author: Alexey Ostanin
 Author-email: aostaninn@gmal.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bs4 (>=0.0.1)
+Requires-Dist: poetry (>=1.5)
 Requires-Dist: requests (>=2.31)
 Description-Content-Type: text/markdown
 
 # feedancy-client
 
 The client is provided with async and sync adapters.
```

