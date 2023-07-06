# Comparing `tmp/fastws-0.1.2.tar.gz` & `tmp/fastws-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastws-0.1.2.tar", max compression
+gzip compressed data, was "fastws-0.1.3.tar", max compression
```

## Comparing `fastws-0.1.2.tar` & `fastws-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-05 18:41:04.114466 fastws-0.1.2/LICENSE
--rw-r--r--   0        0        0     9804 2023-07-06 20:45:27.237817 fastws-0.1.2/README.md
--rw-r--r--   0        0        0      437 2023-07-06 19:26:33.618656 fastws-0.1.2/fastws/__init__.py
--rw-r--r--   0        0        0     6903 2023-07-06 20:45:38.807815 fastws-0.1.2/fastws/application.py
--rw-r--r--   0        0        0     1552 2023-07-06 16:34:25.530483 fastws-0.1.2/fastws/asyncapi.py
--rw-r--r--   0        0        0     4346 2023-07-06 16:34:17.230486 fastws-0.1.2/fastws/broker.py
--rw-r--r--   0        0        0     6172 2023-07-06 16:34:24.460484 fastws-0.1.2/fastws/docs.py
--rw-r--r--   0        0        0     6183 2023-07-06 19:26:36.358655 fastws-0.1.2/fastws/routing.py
--rw-r--r--   0        0        0     1231 2023-07-06 19:25:55.688662 fastws-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10922 1970-01-01 00:00:00.000000 fastws-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-06 20:53:23.287732 fastws-0.1.3/LICENSE
+-rw-r--r--   0        0        0    10110 2023-07-06 21:06:54.397590 fastws-0.1.3/README.md
+-rw-r--r--   0        0        0      437 2023-07-06 21:07:37.737582 fastws-0.1.3/fastws/__init__.py
+-rw-r--r--   0        0        0     6903 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/application.py
+-rw-r--r--   0        0        0     1552 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/asyncapi.py
+-rw-r--r--   0        0        0     4346 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/broker.py
+-rw-r--r--   0        0        0     6172 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/docs.py
+-rw-r--r--   0        0        0     6183 2023-07-06 20:53:23.287732 fastws-0.1.3/fastws/routing.py
+-rw-r--r--   0        0        0     1231 2023-07-06 21:07:37.597582 fastws-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11228 1970-01-01 00:00:00.000000 fastws-0.1.3/PKG-INFO
```

### Comparing `fastws-0.1.2/LICENSE` & `fastws-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/README.md` & `fastws-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # FastWS
 
-
-![FastWS Logo](assets/fastws.png)
+<p align="center">
+ <a href="https://github.com/endrekrohn/fastws">
+    <img src="https://raw.githubusercontent.com/endrekrohn/fastws/assets/assets/fastws.png" alt="FastWS"/>
+</a>
+</p>
 
 **Source Code**: <a href="https://github.com/endrekrohn/fastws" target="_blank">https://github.com/endrekrohn/fastws</a>
 
 ---
 
 FastWS is a wrapper around FastAPI to create better WebSocket applications with auto-documentation using <a href="https://www.asyncapi.com/" target="_blank">AsyncAPI</a>, in a similar fashion as FastAPIs existing use of OpenAPI.
 
@@ -69,15 +72,19 @@
 @app.websocket("/")
 async def fastws_stream(client: Annotated[Client, Depends(service.manage)]):
     await service.serve(client)
 ```
 
 We can look at the generated documentation at `http://localhost:<port>/asyncapi`.
 
-![AsyncAPI Logo](assets/asyncapi_example.png)
+<p align="center">
+ <a href="https://github.com/endrekrohn/fastws">
+    <img src="https://raw.githubusercontent.com/endrekrohn/fastws/assets/assets/asyncapi_example.png" alt="AsyncAPI Docs"/>
+</a>
+</p>
 
 ---
 
 ### Example breakdown
 
 First we import and initialize the service.
```

### Comparing `fastws-0.1.2/fastws/application.py` & `fastws-0.1.3/fastws/application.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/fastws/asyncapi.py` & `fastws-0.1.3/fastws/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/fastws/broker.py` & `fastws-0.1.3/fastws/broker.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/fastws/docs.py` & `fastws-0.1.3/fastws/docs.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/fastws/routing.py` & `fastws-0.1.3/fastws/routing.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.2/pyproject.toml` & `fastws-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastws"
-version = "0.1.2"
+version = "0.1.3"
 description = "FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI."
 authors = ["Endre Krohn <endre@skript.no>"]
 readme = "README.md"
 packages = [{ include = "fastws" }]
 repository = "https://github.com/endrekrohn/fastws"
 documentation = "https://github.com/endrekrohn/fastws"
 keywords = ["fastapi", "pydantic", "starlette", "websockets", "asyncapi"]
```

### Comparing `fastws-0.1.2/PKG-INFO` & `fastws-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastws
-Version: 0.1.2
+Version: 0.1.3
 Summary: FastWS framework. A WebSocket wrapper around FastAPI with auto-documentation using AsyncAPI.
 Home-page: https://github.com/endrekrohn/fastws
 Keywords: fastapi,pydantic,starlette,websockets,asyncapi
 Author: Endre Krohn
 Author-email: endre@skript.no
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -23,16 +23,19 @@
 Requires-Dist: fastapi (==0.100.0-beta3)
 Project-URL: Documentation, https://github.com/endrekrohn/fastws
 Project-URL: Repository, https://github.com/endrekrohn/fastws
 Description-Content-Type: text/markdown
 
 # FastWS
 
-
-![FastWS Logo](assets/fastws.png)
+<p align="center">
+ <a href="https://github.com/endrekrohn/fastws">
+    <img src="https://raw.githubusercontent.com/endrekrohn/fastws/assets/assets/fastws.png" alt="FastWS"/>
+</a>
+</p>
 
 **Source Code**: <a href="https://github.com/endrekrohn/fastws" target="_blank">https://github.com/endrekrohn/fastws</a>
 
 ---
 
 FastWS is a wrapper around FastAPI to create better WebSocket applications with auto-documentation using <a href="https://www.asyncapi.com/" target="_blank">AsyncAPI</a>, in a similar fashion as FastAPIs existing use of OpenAPI.
 
@@ -96,15 +99,19 @@
 @app.websocket("/")
 async def fastws_stream(client: Annotated[Client, Depends(service.manage)]):
     await service.serve(client)
 ```
 
 We can look at the generated documentation at `http://localhost:<port>/asyncapi`.
 
-![AsyncAPI Logo](assets/asyncapi_example.png)
+<p align="center">
+ <a href="https://github.com/endrekrohn/fastws">
+    <img src="https://raw.githubusercontent.com/endrekrohn/fastws/assets/assets/asyncapi_example.png" alt="AsyncAPI Docs"/>
+</a>
+</p>
 
 ---
 
 ### Example breakdown
 
 First we import and initialize the service.
```

