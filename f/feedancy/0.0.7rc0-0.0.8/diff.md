# Comparing `tmp/feedancy-0.0.7rc0.tar.gz` & `tmp/feedancy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedancy-0.0.7rc0.tar", max compression
+gzip compressed data, was "feedancy-0.0.8.tar", max compression
```

## Comparing `feedancy-0.0.7rc0.tar` & `feedancy-0.0.8.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      657 2023-07-03 17:16:29.011425 feedancy-0.0.7rc0/feedancy-client/README.md
--rw-r--r--   0        0        0     1016 2023-07-06 16:20:52.800364 feedancy-0.0.7rc0/pyproject.toml
--rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 feedancy-0.0.7rc0/PKG-INFO
+-rw-r--r--   0        0        0      615 2023-07-03 17:31:45.058158 feedancy-0.0.8/feedancy/README.md
+-rw-r--r--   0        0        0     1009 2023-07-06 16:23:37.141461 feedancy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 feedancy-0.0.8/PKG-INFO
```

### Comparing `feedancy-0.0.7rc0/feedancy-client/README.md` & `feedancy-0.0.8/feedancy/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# feedancy-client
+# feedancy
 
 The client is provided with async and sync adapters.
 
 To install the async version with all its dependencies use:
 ```bash
-pip install feedancy-client[asyncio]
+pip install feedancy[asyncio]
 ```
 
 To install the sync version with all its dependencies use:
 ```bash
-pip install feedancy-client[sync]
+pip install feedancy[sync]
 ```
 
 To install both versions with all their dependencies use:
 ```bash
-pip install feedancy-client[asyncio,sync]
+pip install feedancy[asyncio,sync]
 ```
 
 ## Client instantiation example
 
 ```python
 
-from feedancy_client import new_client, Configuration
-from feedancy_client.lib.adapter.requests import RequestsAdapter
+from feedancy import new_client, Configuration
+from feedancy.lib.adapter.requests import RequestsAdapter
 
 client = new_client(RequestsAdapter(), Configuration(host="<your openapi server URL>"))
 ```
```

### Comparing `feedancy-0.0.7rc0/pyproject.toml` & `feedancy-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
   | build
   | dist
 )/
 '''
 
 [tool.poetry]
 name = "feedancy"
-version = "0.0.7c"
+version = "0.0.8"
 description = "сервис по сбору вакансий"
 authors = [
     "Alexey Ostanin <aostaninn@gmal.com>",
     "Stanislav Losev <stanislav_losev@protonmail.com>",
     "Tatiana Zimina <tratatatanya@gmail.com>"
 ]
 license = "MIT"
-readme = "./feedancy-client/README.md"
+readme = "./feedancy/README.md"
 packages = [
     { include = './feedancy' }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 poetry = ">=1.5"
 djangorestframework = ">=3.13.1"
-Django = ">=4"
+#Django = ">=4"
 gunicorn = ">=20.1.0"
 psycopg2-binary = ">=2.9.5"
 Pillow = ">=9.2.0"
 django-filter = ">=22.1"
 pydantic = ">=1.10"
 requests = ">=2.31"
 bs4 = ">=0.0.1"
```

### Comparing `feedancy-0.0.7rc0/PKG-INFO` & `feedancy-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 Metadata-Version: 2.1
 Name: feedancy
-Version: 0.0.7rc0
+Version: 0.0.8
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
-Requires-Dist: Django (>=4)
 Requires-Dist: Pillow (>=9.2.0)
 Requires-Dist: bs4 (>=0.0.1)
 Requires-Dist: django-filter (>=22.1)
 Requires-Dist: djangorestframework (>=3.13.1)
 Requires-Dist: gunicorn (>=20.1.0)
 Requires-Dist: poetry (>=1.5)
 Requires-Dist: psycopg2-binary (>=2.9.5)
 Requires-Dist: pydantic (>=1.10)
 Requires-Dist: requests (>=2.31)
 Description-Content-Type: text/markdown
 
-# feedancy-client
+# feedancy
 
 The client is provided with async and sync adapters.
 
 To install the async version with all its dependencies use:
 ```bash
-pip install feedancy-client[asyncio]
+pip install feedancy[asyncio]
 ```
 
 To install the sync version with all its dependencies use:
 ```bash
-pip install feedancy-client[sync]
+pip install feedancy[sync]
 ```
 
 To install both versions with all their dependencies use:
 ```bash
-pip install feedancy-client[asyncio,sync]
+pip install feedancy[asyncio,sync]
 ```
 
 ## Client instantiation example
 
 ```python
 
-from feedancy_client import new_client, Configuration
-from feedancy_client.lib.adapter.requests import RequestsAdapter
+from feedancy import new_client, Configuration
+from feedancy.lib.adapter.requests import RequestsAdapter
 
 client = new_client(RequestsAdapter(), Configuration(host="<your openapi server URL>"))
 ```
```

