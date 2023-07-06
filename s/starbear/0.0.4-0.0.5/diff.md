# Comparing `tmp/starbear-0.0.4.tar.gz` & `tmp/starbear-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.0.4.tar", max compression
+gzip compressed data, was "starbear-0.0.5.tar", max compression
```

## Comparing `starbear-0.0.4.tar` & `starbear-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      786 2023-06-26 19:37:39.133159 starbear-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.4/starbear/__init__.py
--rw-r--r--   0        0        0     4988 2023-05-31 16:06:31.359436 starbear-0.0.4/starbear/base-lib.js
--rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.4/starbear/base-template.html
--rw-r--r--   0        0        0     5126 2023-06-08 20:37:34.926744 starbear-0.0.4/starbear/page.py
--rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.4/starbear/repr.py
--rw-r--r--   0        0        0    10916 2023-06-26 19:28:58.244359 starbear-0.0.4/starbear/serve.py
--rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.4/starbear/utils.py
--rw-r--r--   0        0        0       18 2023-06-26 19:37:39.166090 starbear-0.0.4/starbear/version.py
--rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.4/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      786 2023-07-06 19:07:03.623417 starbear-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-01-22 18:07:37.078561 starbear-0.0.5/starbear/__init__.py
+-rw-r--r--   0        0        0     4988 2023-05-31 16:06:31.359436 starbear-0.0.5/starbear/base-lib.js
+-rw-r--r--   0        0        0      552 2023-01-22 20:51:07.514209 starbear-0.0.5/starbear/base-template.html
+-rw-r--r--   0        0        0     5126 2023-06-08 20:37:34.926744 starbear-0.0.5/starbear/page.py
+-rw-r--r--   0        0        0     6759 2023-01-22 18:36:53.392128 starbear-0.0.5/starbear/repr.py
+-rw-r--r--   0        0        0    11184 2023-07-06 19:05:48.953462 starbear-0.0.5/starbear/serve.py
+-rw-r--r--   0        0        0     2525 2023-01-23 07:23:44.113526 starbear-0.0.5/starbear/utils.py
+-rw-r--r--   0        0        0       18 2023-07-06 19:07:03.658607 starbear-0.0.5/starbear/version.py
+-rw-r--r--   0        0        0      731 1970-01-01 00:00:00.000000 starbear-0.0.5/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 starbear-0.0.5/PKG-INFO
```

### Comparing `starbear-0.0.4/pyproject.toml` & `starbear-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starbear"
-version = "0.0.4"
+version = "0.0.5"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = "^0.17.6"
```

### Comparing `starbear-0.0.4/starbear/base-lib.js` & `starbear-0.0.5/starbear/base-lib.js`

 * *Files identical despite different names*

### Comparing `starbear-0.0.4/starbear/base-template.html` & `starbear-0.0.5/starbear/base-template.html`

 * *Files identical despite different names*

### Comparing `starbear-0.0.4/starbear/page.py` & `starbear-0.0.5/starbear/page.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.4/starbear/repr.py` & `starbear-0.0.5/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.4/starbear/serve.py` & `starbear-0.0.5/starbear/serve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import asyncio as aio
 import base64
 import inspect
 import json
 import traceback
-from functools import wraps
+from functools import cached_property, wraps
 from itertools import count
 from pathlib import Path
 from uuid import uuid4 as uuid
 
 from hrepr import Tag
 from starlette.exceptions import HTTPException
 from starlette.responses import (
     FileResponse,
     HTMLResponse,
     JSONResponse,
     RedirectResponse,
     Response,
 )
-from starlette.routing import Route, WebSocketRoute
+from starlette.routing import Mount, Route, WebSocketRoute
 from starlette.websockets import WebSocketDisconnect
 
 from .page import Page
 from .repr import Representer
 from .utils import keyword_decorator
 
 here = Path(__file__).parent
@@ -220,14 +220,15 @@
 
     return fwd
 
 
 class MotherBear:
     def __init__(self, fn, process_timeout=60, hide_processes=True):
         self.fn = fn
+        self.doc = getattr(fn, "__doc__", None)
         self.router = None
         self.process_timeout = process_timeout
         self.hide_processes = hide_processes
         self.cubs = {}
         self.appid = next(_count)
 
     def _get(self, proc, query_params={}, session={}, ensure=False):
@@ -343,11 +344,18 @@
             self._make_route("file", "/{process:str}/file/{path:path}"),
             self._make_route("vfile", "/{process:str}/vfile/{path:path}"),
             self._make_route("post", "/{process:str}/post", methods=["POST"]),
             self._make_route("queue", "/{process:str}/queue", methods=["POST"]),
             self._make_route("socket", "/{process:str}/socket", cls=WebSocketRoute),
         ]
 
+    @cached_property
+    def _mnt(self):
+        return Mount("/", routes=self.routes())
+
+    async def __call__(self, scope, receive, send):
+        await self._mnt.handle(scope, receive, send)
+
 
 @keyword_decorator
 def bear(fn, **kwargs):
     return MotherBear(fn, **kwargs)
```

### Comparing `starbear-0.0.4/starbear/utils.py` & `starbear-0.0.5/starbear/utils.py`

 * *Files identical despite different names*

### Comparing `starbear-0.0.4/setup.py` & `starbear-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['hrepr>=0.5.0,<0.6.0',
  'starlette>=0.20.3,<0.21.0',
  'uvicorn>=0.17.6,<0.18.0',
  'websockets>=10.3,<11.0']
 
 setup_kwargs = {
     'name': 'starbear',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Framework for easy small local web apps or programs',
     'long_description': 'None',
     'author': 'Olivier Breuleux',
     'author_email': 'breuleux@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `starbear-0.0.4/PKG-INFO` & `starbear-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.0.4
+Version: 0.0.5
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

