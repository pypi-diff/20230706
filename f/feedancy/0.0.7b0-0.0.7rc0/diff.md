# Comparing `tmp/feedancy-0.0.7b0.tar.gz` & `tmp/feedancy-0.0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.7b0.tar", max compression
+gzip compressed data, was "feedancy-0.0.7rc0.tar", max compression
```

## Comparing `feedancy-0.0.7b0.tar` & `feedancy-0.0.7rc0.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.7b0/feedancy-client/README.md
--rw-r--r--   0        0        0     1017 2023-07-06 16:15:37.343962 feedancy-0.0.7b0/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 feedancy-0.0.7b0/PKG-INFO
+-rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.7rc0/feedancy-client/README.md
+-rw-r--r--   0        0        0     1016 2023-07-06 16:20:52.800364 feedancy-0.0.7rc0/pyproject.toml
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 feedancy-0.0.7rc0/PKG-INFO
```

### Comparing `feedancy-0.0.7b0/feedancy-client/README.md` & `feedancy-0.0.7rc0/feedancy-client/README.md`

 * *Files identical despite different names*

### Comparing `feedancy-0.0.7b0/pyproject.toml` & `feedancy-0.0.7rc0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.7b"
+version = "0.0.7c"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
@@ -32,15 +32,15 @@
     { include = './feedancy' }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.5"
 djangorestframework = ">=3.13.1"
-#Django = ">=4"
+Django = ">=4"
 gunicorn = ">=20.1.0"
 psycopg2-binary = ">=2.9.5"
 Pillow = ">=9.2.0"
 django-filter = ">=22.1"
 pydantic = ">=1.10"
 requests = ">=2.31"
 bs4 = ">=0.0.1"
```

### Comparing `feedancy-0.0.7b0/PKG-INFO` & `feedancy-0.0.7rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.7b0
+Version: 0.0.7rc0
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
+Requires-Dist: Django (>=4)
 Requires-Dist: Pillow (>=9.2.0)
 Requires-Dist: bs4 (>=0.0.1)
 Requires-Dist: django-filter (>=22.1)
 Requires-Dist: djangorestframework (>=3.13.1)
 Requires-Dist: gunicorn (>=20.1.0)
 Requires-Dist: poetry (>=1.5)
 Requires-Dist: psycopg2-binary (>=2.9.5)
```

