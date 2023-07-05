# Comparing `tmp/python-engineio-4.5.0.tar.gz` & `tmp/python-engineio-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-engineio-4.5.0.tar", last modified: Wed Jul  5 12:30:15 2023, max compression
+gzip compressed data, was "python-engineio-4.5.1.tar", last modified: Wed Jul  5 23:17:39 2023, max compression
```

## Comparing `python-engineio-4.5.0.tar` & `python-engineio-4.5.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-06-13 09:40:52.000000 python-engineio-4.5.0/LICENSE
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       26 2023-06-13 09:40:52.000000 python-engineio-4.5.0/MANIFEST.in
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 12:30:15.801900 python-engineio-4.5.0/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1288 2023-06-13 09:40:52.000000 python-engineio-4.5.0/README.md
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1012 2023-06-13 09:40:52.000000 python-engineio-4.5.0/README.rst
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      104 2023-06-13 09:40:52.000000 python-engineio-4.5.0/pyproject.toml
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      936 2023-07-05 12:30:15.801900 python-engineio-4.5.0/setup.cfg
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2023-06-13 09:40:52.000000 python-engineio-4.5.0/setup.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.797899 python-engineio-4.5.0/src/
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/engineio/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      747 2023-06-20 11:10:32.000000 python-engineio-4.5.0/src/engineio/__init__.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/engineio/async_drivers/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/async_drivers/__init__.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3768 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/aiohttp.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10189 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/asgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1042 2023-07-05 11:02:37.000000 python-engineio-4.5.0/src/engineio/async_drivers/eventlet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1807 2023-07-05 11:02:18.000000 python-engineio-4.5.0/src/engineio/async_drivers/gevent.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5916 2023-07-05 11:02:48.000000 python-engineio-4.5.0/src/engineio/async_drivers/gevent_uwsgi.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     4476 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/async_drivers/sanic.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1170 2023-07-05 10:55:29.000000 python-engineio-4.5.0/src/engineio/async_drivers/threading.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     5909 2023-07-05 11:03:10.000000 python-engineio-4.5.0/src/engineio/async_drivers/tornado.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    27033 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/asyncio_client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    22691 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/asyncio_server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10274 2023-07-05 10:50:32.000000 python-engineio-4.5.0/src/engineio/asyncio_socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    30109 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/client.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      292 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/exceptions.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)      405 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/json.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     3766 2023-07-05 11:03:29.000000 python-engineio-4.5.0/src/engineio/middleware.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2884 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/packet.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1547 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/payload.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    33757 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/server.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)    10325 2023-07-05 10:38:20.000000 python-engineio-4.5.0/src/engineio/socket.py
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     2064 2023-06-13 09:40:52.000000 python-engineio-4.5.0/src/engineio/static_files.py
-drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:30:15.801900 python-engineio-4.5.0/src/python_engineio.egg-info/
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/PKG-INFO
--rw-rw-r--   0 miguel    (1000) miguel    (1000)     1013 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/SOURCES.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/dependency_links.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-13 10:11:32.000000 python-engineio-4.5.0/src/python_engineio.egg-info/not-zip-safe
--rw-rw-r--   0 miguel    (1000) miguel    (1000)       98 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/requires.txt
--rw-rw-r--   0 miguel    (1000) miguel    (1000)        9 2023-07-05 12:30:15.000000 python-engineio-4.5.0/src/python_engineio.egg-info/top_level.txt
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 23:17:39.289574 python-engineio-4.5.1/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1082 2023-07-05 12:32:34.000000 python-engineio-4.5.1/LICENSE
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       26 2023-07-05 12:32:34.000000 python-engineio-4.5.1/MANIFEST.in
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 23:17:39.289574 python-engineio-4.5.1/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1288 2023-07-05 12:32:51.000000 python-engineio-4.5.1/README.md
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1012 2023-07-05 12:32:51.000000 python-engineio-4.5.1/README.rst
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      104 2023-07-05 12:32:51.000000 python-engineio-4.5.1/pyproject.toml
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      936 2023-07-05 23:17:39.289574 python-engineio-4.5.1/setup.cfg
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       38 2023-07-05 12:32:51.000000 python-engineio-4.5.1/setup.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 23:17:39.289574 python-engineio-4.5.1/src/
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 23:17:39.289574 python-engineio-4.5.1/src/engineio/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      747 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/__init__.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 23:17:39.289574 python-engineio-4.5.1/src/engineio/async_drivers/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        0 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/__init__.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3768 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/aiohttp.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10189 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/asgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1177 2023-07-05 23:16:42.000000 python-engineio-4.5.1/src/engineio/async_drivers/eventlet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1807 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/gevent.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5916 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/gevent_uwsgi.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     4476 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/sanic.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1170 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/threading.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     5909 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/async_drivers/tornado.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    27033 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/asyncio_client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    22691 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/asyncio_server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10274 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/asyncio_socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    30109 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/client.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      292 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/exceptions.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)      405 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/json.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     3766 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/middleware.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2884 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/packet.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1547 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/payload.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    33757 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/server.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)    10325 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/socket.py
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     2064 2023-07-05 12:32:51.000000 python-engineio-4.5.1/src/engineio/static_files.py
+drwxrwxr-x   0 miguel    (1000) miguel    (1000)        0 2023-07-05 23:17:39.289574 python-engineio-4.5.1/src/python_engineio.egg-info/
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1997 2023-07-05 23:17:39.000000 python-engineio-4.5.1/src/python_engineio.egg-info/PKG-INFO
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)     1013 2023-07-05 23:17:39.000000 python-engineio-4.5.1/src/python_engineio.egg-info/SOURCES.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-07-05 23:17:39.000000 python-engineio-4.5.1/src/python_engineio.egg-info/dependency_links.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        1 2023-06-13 10:11:32.000000 python-engineio-4.5.1/src/python_engineio.egg-info/not-zip-safe
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)       98 2023-07-05 23:17:39.000000 python-engineio-4.5.1/src/python_engineio.egg-info/requires.txt
+-rw-rw-r--   0 miguel    (1000) miguel    (1000)        9 2023-07-05 23:17:39.000000 python-engineio-4.5.1/src/python_engineio.egg-info/top_level.txt
```

### Comparing `python-engineio-4.5.0/LICENSE` & `python-engineio-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/PKG-INFO` & `python-engineio-4.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.5.0
+Version: 4.5.1
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python-engineio-4.5.0/README.md` & `python-engineio-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/README.rst` & `python-engineio-4.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/setup.cfg` & `python-engineio-4.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-engineio
-version = 4.5.0
+version = 4.5.1
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Engine.IO server and client for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/python-engineio
 project_urls =
```

### Comparing `python-engineio-4.5.0/src/engineio/__init__.py` & `python-engineio-4.5.1/src/engineio/__init__.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/aiohttp.py` & `python-engineio-4.5.1/src/engineio/async_drivers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/asgi.py` & `python-engineio-4.5.1/src/engineio/async_drivers/asgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/eventlet.py` & `python-engineio-4.5.1/src/engineio/async_drivers/eventlet.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 from eventlet import queue
 from eventlet import sleep
 from eventlet.websocket import WebSocketWSGI as _WebSocketWSGI
 
 
 class WebSocketWSGI(_WebSocketWSGI):
     def __init__(self, handler, server):
-        print(server.max_http_buffer_size)
-        super().__init__(
-            handler, max_frame_length=int(server.max_http_buffer_size))
+        try:
+            super().__init__(
+                handler, max_frame_length=int(server.max_http_buffer_size))
+        except TypeError:  # pragma: no cover
+            # older versions of eventlet do not support a max frame size
+            super().__init__(handler)
         self._sock = None
 
     def __call__(self, environ, start_response):
         if 'eventlet.input' not in environ:
             raise RuntimeError('You need to use the eventlet server. '
                                'See the Deployment section of the '
                                'documentation for more information.')
```

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/gevent.py` & `python-engineio-4.5.1/src/engineio/async_drivers/gevent.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/gevent_uwsgi.py` & `python-engineio-4.5.1/src/engineio/async_drivers/gevent_uwsgi.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/sanic.py` & `python-engineio-4.5.1/src/engineio/async_drivers/sanic.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/threading.py` & `python-engineio-4.5.1/src/engineio/async_drivers/threading.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/async_drivers/tornado.py` & `python-engineio-4.5.1/src/engineio/async_drivers/tornado.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/asyncio_client.py` & `python-engineio-4.5.1/src/engineio/asyncio_client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/asyncio_server.py` & `python-engineio-4.5.1/src/engineio/asyncio_server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/asyncio_socket.py` & `python-engineio-4.5.1/src/engineio/asyncio_socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/client.py` & `python-engineio-4.5.1/src/engineio/client.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/middleware.py` & `python-engineio-4.5.1/src/engineio/middleware.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/packet.py` & `python-engineio-4.5.1/src/engineio/packet.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/payload.py` & `python-engineio-4.5.1/src/engineio/payload.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/server.py` & `python-engineio-4.5.1/src/engineio/server.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/socket.py` & `python-engineio-4.5.1/src/engineio/socket.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/engineio/static_files.py` & `python-engineio-4.5.1/src/engineio/static_files.py`

 * *Files identical despite different names*

### Comparing `python-engineio-4.5.0/src/python_engineio.egg-info/PKG-INFO` & `python-engineio-4.5.1/src/python_engineio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-engineio
-Version: 4.5.0
+Version: 4.5.1
 Summary: Engine.IO server and client for Python
 Home-page: https://github.com/miguelgrinberg/python-engineio
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/python-engineio/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `python-engineio-4.5.0/src/python_engineio.egg-info/SOURCES.txt` & `python-engineio-4.5.1/src/python_engineio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

