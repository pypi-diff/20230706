# Comparing `tmp/spaces-0.6.1.tar.gz` & `tmp/spaces-0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.6.1.tar", max compression
+gzip compressed data, was "spaces-0.6b1.tar", max compression
```

## Comparing `spaces-0.6.1.tar` & `spaces-0.6b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.6.1/README.md
--rw-r--r--   0        0        0     1505 2023-07-06 15:35:51.087356 spaces-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.6.1/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.6.1/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.6.1/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     2204 2023-07-06 15:35:07.994466 spaces-0.6.1/spaces/gpu/client.py
--rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.6.1/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.6.1/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6778 2023-07-06 15:35:14.742606 spaces-0.6.1/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.6.1/spaces/gradio.py
--rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.6.1/spaces/utils.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.6.1/setup.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.6b1/README.md
+-rw-r--r--   0        0        0     1489 2023-06-30 16:02:24.855918 spaces-0.6b1/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.6b1/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.6b1/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.6b1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-29 12:42:06.802062 spaces-0.6b1/spaces/gpu/client.py
+-rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.6b1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.6b1/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.6b1/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.6b1/spaces/gradio.py
+-rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.6b1/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.6b1/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.6b1/PKG-INFO
```

### Comparing `spaces-0.6.1/pyproject.toml` & `spaces-0.6b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "spaces"
-version = "0.6.1"
+version = "0.6b1"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 psutil = "^5.9.5"
 typing-extensions = "^4.5.0"
 requests = "^2.29.0"
 pydantic = "^1.10.8"
-gradio = "^3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-dotenv = "^0.5.2"
 pytest-mock = "^3.10.0"
 requests-mock = "^1.10.0"
 pytest-timeout = "^2.1.0"
```

### Comparing `spaces-0.6.1/spaces/gpu/client.py` & `spaces-0.6b1/spaces/gpu/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 """
 from __future__ import annotations
 
-import time
 from http import HTTPStatus
 
-import gradio as gr
 import requests
 from pydantic import BaseModel
 
 from .. import utils
 from ..config import Config
 
 
@@ -35,31 +33,27 @@
 
 
 def post(path: str, params: BaseModel | None = None) -> requests.Response:
     return requests.post(base_url() + path, params=params.dict() if params else None)
 
 
 def startup_report():
-    retries, max_retries = 0, 2
-    while (status := post('/startup-report').status_code) == HTTPStatus.NOT_FOUND: # pragma: no cover
-        time.sleep(1)
-        if (retries := retries + 1) > max_retries:
-            raise RuntimeError("Error while initializing ZeroGPU: NotFound")
-    if status != HTTPStatus.OK: # pragma: no cover
-        raise RuntimeError("Error while initializing ZeroGPU: Unknown")
+    res = post('/startup-report')
+    if res.status_code != HTTPStatus.OK: # pragma: no cover
+        raise RuntimeError("Error while initializing ZeroGPU")
 
 
 def schedule() -> ScheduleResponse:
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
     ))
 
     if res.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise gr.Error("No GPU is currently available")
+        raise RuntimeError("GPU already in use")
 
     try:
         data = res.json()
     except requests.JSONDecodeError: # pragma: no cover
         data = {}
 
     if not res.ok: # pragma: no cover
@@ -77,11 +71,10 @@
     ))
 
     if not res.ok:
         try:
             data = res.json()
         except requests.JSONDecodeError: # pragma: no cover
             data = {}
-        # TODO: use future gr.Warning() if /release didn't detect GPU usage
         raise RuntimeError(f"ZeroGPU API /release error: {data.get('detail')}")
 
     return None
```

### Comparing `spaces-0.6.1/spaces/gpu/decorator.py` & `spaces-0.6b1/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.1/spaces/gpu/torch.py` & `spaces-0.6b1/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.1/spaces/gpu/wrappers.py` & `spaces-0.6b1/spaces/gpu/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 """
 from __future__ import annotations
 
-import gradio as gr
 import multiprocessing
 import os
 import signal
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from pickle import PicklingError
@@ -90,15 +89,15 @@
             release(fail=True)
             raise
 
         try:
             res = worker.res_queue.get()
         except EOFError:
             release(fail=True)
-            raise gr.Error("GPU task aborted")
+            raise RuntimeError("Operation aborted")
         if isinstance(res, Exception):
             release(fail=True)
             raise res
         release()
         return res[0]
 
 
@@ -115,15 +114,15 @@
         signal.signal(signal.SIGTERM, drop_params(arg_queue.close))
         while True:
             try:
                 args, kwargs = arg_queue.get()
             except OSError:
                 break
             with ThreadPoolExecutor() as executor:
-                future = executor.submit(task, *args, **kwargs) # type: ignore
+                future = executor.submit(task, *args, **kwargs)
             try:
                 res = [future.result()]
             except Exception as e:
                 traceback.print_exc()
                 res = e
             try:
                 res_queue.put(res)
@@ -178,15 +177,15 @@
 
         with ThreadPoolExecutor() as e:
             e.submit(fill_yield_queue, worker)
             while True:
                 try:
                     res = yield_queue.get()
                 except Exception:
-                    raise gr.Error("GPU task aborted")
+                    raise RuntimeError("Operation aborted")
                 if isinstance(res, Exception):
                     raise res
                 if res is None:
                     break
                 yield res[0]
```

### Comparing `spaces-0.6.1/spaces/gradio.py` & `spaces-0.6b1/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.1/spaces/utils.py` & `spaces-0.6b1/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.6.1/setup.py` & `spaces-0.6b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 packages = \
 ['spaces', 'spaces.gpu']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['gradio>=3.2,<4.0',
- 'psutil>=5.9.5,<6.0.0',
+['psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.6.1',
+    'version': '0.6b1',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.6.1/PKG-INFO` & `spaces-0.6b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.6.1
+Version: 0.6b1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gradio (>=3.2,<4.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: requests (>=2.29.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/huggingface/huggingface_hub
 Description-Content-Type: text/markdown
```

