# Comparing `tmp/fastapi-cors-0.0.4.tar.gz` & `tmp/fastapi-cors-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-cors-0.0.4.tar", last modified: Tue Jul  4 23:15:49 2023, max compression
+gzip compressed data, was "fastapi-cors-0.0.5.tar", last modified: Thu Jul  6 15:30:07 2023, max compression
```

## Comparing `fastapi-cors-0.0.4.tar` & `fastapi-cors-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/LICENSE
--rw-r--r--   0        0        0     2497 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/README.md
--rw-r--r--   0        0        0       55 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/fastapi_cors/__init__.py
--rw-r--r--   0        0        0      813 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/fastapi_cors/env.py
--rw-r--r--   0        0        0     2056 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/fastapi_cors/main.py
--rw-r--r--   0        0        0     2249 2023-07-04 23:15:22.453551 fastapi-cors-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3203 1970-01-01 00:00:00.000000 fastapi-cors-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2833 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/README.md
+-rw-r--r--   0        0        0       55 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/__init__.py
+-rw-r--r--   0        0        0      813 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/env.py
+-rw-r--r--   0        0        0     2056 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/fastapi_cors/main.py
+-rw-r--r--   0        0        0     2249 2023-07-06 15:29:43.034781 fastapi-cors-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3539 1970-01-01 00:00:00.000000 fastapi-cors-0.0.5/PKG-INFO
```

### Comparing `fastapi-cors-0.0.4/LICENSE` & `fastapi-cors-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.4/README.md` & `fastapi-cors-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -44,23 +44,31 @@
 | `PORT` | 8000 | Where to mount the static directory. Disabled if value is falsy. |
 | `LOG_LEVEL` | info | log level. |
 | `ALLOW_ORIGINS` | ["http://localhost","http://localhost:3000"] | A list of origins that should be permitted to make cross-origin requests. E.g. ['https://example.org', 'https://www.example.org']. You can use ['*'] to allow any origin.  *These are the URLs clients can make requests from* |
 | `ALLOWED_CREDENTIALS` | True | Indicate that cookies should be supported for cross-origin requests. Also, allow_origins cannot be set to ['*'] for credentials to be allowed, origins must be specified. |
 | `ALLOWED_METHODS` | ["*"] | A list of HTTP methods that should be allowed for cross-origin requests. Defaults to ['*'] to allow all standard methods. You can use ['GET'] to reduce the list. |
 | `ALLOWED_HEADERS` | ["Access-Control-Allow-Origin"] | A list of HTTP request headers that should be supported for cross-origin requests. You can use ['*'] to allow all headers. The Accept, Accept-Language, Content-Language and Content-Type headers are always allowed for [simple CORS requests](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#simple_requests) |
 
+> ⚠️ `allow_origins` default is `["http://localhost","http://localhost:3000"]`, not `[]` (80 -> docs, 3000 -> frontend)
+>
+> ⚠️ `allow_methods` default is `["*"]`, not `["GET"]`
+>
+> ⚠️ `allowed_credentials` default is `True`, not `False`
+>
 > See the [FastAPI documentation on CORS](https://fastapi.tiangolo.com/tutorial/cors/?h=cors) for more information
 
 ### Example Env
 
+Values will be cast into a `list` of `str`, as appropriate.
+
 ```env
 HOST=0.0.0.0
 PORT=8000
 LOG_LEVEL=info
 ALLOW_ORIGINS=http://localhost,http://localhost:3000
 ALLOWED_CREDENTIALS=True
-ALLOWED_METHODS=["*"]
-ALLOWED_HEADERS
+ALLOWED_METHODS=*
+ALLOWED_HEADERS=Access-Control-Allow-Origin
 
 ```
 
 *Note, this is not required unless you are changing a default or want to declare them all*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastapi-cors-0.0.4/fastapi_cors/env.py` & `fastapi-cors-0.0.5/fastapi_cors/env.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.4/fastapi_cors/main.py` & `fastapi-cors-0.0.5/fastapi_cors/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-cors-0.0.4/pyproject.toml` & `fastapi-cors-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 classifiers = [
     "Topic :: Software Development :: Code Generators",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.0.4"
+version = "0.0.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/iancleary/fastapi-cors"
 Repository = "https://github.com/iancleary/fastapi-cors"
```

### Comparing `fastapi-cors-0.0.4/PKG-INFO` & `fastapi-cors-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_cors
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple env support of CORS settings for Fastapi applications
 License: MIT
 Keywords: cors,python,fastapi,environs
 Author-email: Ian Cleary <github@iancleary.me>
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -61,23 +61,31 @@
 | `PORT` | 8000 | Where to mount the static directory. Disabled if value is falsy. |
 | `LOG_LEVEL` | info | log level. |
 | `ALLOW_ORIGINS` | ["http://localhost","http://localhost:3000"] | A list of origins that should be permitted to make cross-origin requests. E.g. ['https://example.org', 'https://www.example.org']. You can use ['*'] to allow any origin.  *These are the URLs clients can make requests from* |
 | `ALLOWED_CREDENTIALS` | True | Indicate that cookies should be supported for cross-origin requests. Also, allow_origins cannot be set to ['*'] for credentials to be allowed, origins must be specified. |
 | `ALLOWED_METHODS` | ["*"] | A list of HTTP methods that should be allowed for cross-origin requests. Defaults to ['*'] to allow all standard methods. You can use ['GET'] to reduce the list. |
 | `ALLOWED_HEADERS` | ["Access-Control-Allow-Origin"] | A list of HTTP request headers that should be supported for cross-origin requests. You can use ['*'] to allow all headers. The Accept, Accept-Language, Content-Language and Content-Type headers are always allowed for [simple CORS requests](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS#simple_requests) |
 
+> ⚠️ `allow_origins` default is `["http://localhost","http://localhost:3000"]`, not `[]` (80 -> docs, 3000 -> frontend)
+>
+> ⚠️ `allow_methods` default is `["*"]`, not `["GET"]`
+>
+> ⚠️ `allowed_credentials` default is `True`, not `False`
+>
 > See the [FastAPI documentation on CORS](https://fastapi.tiangolo.com/tutorial/cors/?h=cors) for more information
 
 ### Example Env
 
+Values will be cast into a `list` of `str`, as appropriate.
+
 ```env
 HOST=0.0.0.0
 PORT=8000
 LOG_LEVEL=info
 ALLOW_ORIGINS=http://localhost,http://localhost:3000
 ALLOWED_CREDENTIALS=True
-ALLOWED_METHODS=["*"]
-ALLOWED_HEADERS
+ALLOWED_METHODS=*
+ALLOWED_HEADERS=Access-Control-Allow-Origin
 
 ```
 
 *Note, this is not required unless you are changing a default or want to declare them all*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

