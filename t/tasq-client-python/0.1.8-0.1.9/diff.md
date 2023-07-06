# Comparing `tmp/tasq-client-python-0.1.8.tar.gz` & `tmp/tasq-client-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasq-client-python-0.1.8.tar", last modified: Fri Nov  4 23:30:30 2022, max compression
+gzip compressed data, was "tasq-client-python-0.1.9.tar", last modified: Thu Feb  9 20:23:39 2023, max compression
```

## Comparing `tasq-client-python-0.1.8.tar` & `tasq-client-python-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-11-04 23:30:30.057997 tasq-client-python-0.1.8/
--rw-r--r--   0 alex       (502) staff       (20)       62 2022-11-04 23:30:30.057649 tasq-client-python-0.1.8/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)       38 2022-11-04 23:30:30.058081 tasq-client-python-0.1.8/setup.cfg
--rw-r--r--   0 alex       (502) staff       (20)      156 2022-11-04 23:29:39.000000 tasq-client-python-0.1.8/setup.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-11-04 23:30:30.053374 tasq-client-python-0.1.8/tasq_client/
--rw-r--r--   0 alex       (502) staff       (20)      277 2022-10-12 16:53:46.000000 tasq-client-python-0.1.8/tasq_client/__init__.py
--rw-r--r--   0 alex       (502) staff       (20)     2583 2022-10-12 16:53:13.000000 tasq-client-python-0.1.8/tasq_client/check_type.py
--rw-r--r--   0 alex       (502) staff       (20)     1433 2022-08-19 23:03:05.000000 tasq-client-python-0.1.8/tasq_client/check_type_test.py
--rw-r--r--   0 alex       (502) staff       (20)    11135 2022-11-04 23:29:09.000000 tasq-client-python-0.1.8/tasq_client/client.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-11-04 23:30:30.057128 tasq-client-python-0.1.8/tasq_client_python.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)       62 2022-11-04 23:30:29.000000 tasq-client-python-0.1.8/tasq_client_python.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)      320 2022-11-04 23:30:29.000000 tasq-client-python-0.1.8/tasq_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2022-11-04 23:30:29.000000 tasq-client-python-0.1.8/tasq_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (502) staff       (20)        9 2022-11-04 23:30:29.000000 tasq-client-python-0.1.8/tasq_client_python.egg-info/requires.txt
--rw-r--r--   0 alex       (502) staff       (20)       12 2022-11-04 23:30:29.000000 tasq-client-python-0.1.8/tasq_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-02-09 20:23:39.547421 tasq-client-python-0.1.9/
+-rw-r--r--   0 alex       (502) staff       (20)      143 2023-02-09 20:23:39.547117 tasq-client-python-0.1.9/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)      968 2023-02-09 20:16:22.000000 tasq-client-python-0.1.9/README.md
+-rw-r--r--   0 alex       (502) staff       (20)       38 2023-02-09 20:23:39.547497 tasq-client-python-0.1.9/setup.cfg
+-rw-r--r--   0 alex       (502) staff       (20)      156 2023-02-09 20:22:15.000000 tasq-client-python-0.1.9/setup.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-02-09 20:23:39.542391 tasq-client-python-0.1.9/tasq_client/
+-rw-r--r--   0 alex       (502) staff       (20)      277 2022-10-12 16:53:46.000000 tasq-client-python-0.1.9/tasq_client/__init__.py
+-rw-r--r--   0 alex       (502) staff       (20)     2583 2022-10-12 16:53:13.000000 tasq-client-python-0.1.9/tasq_client/check_type.py
+-rw-r--r--   0 alex       (502) staff       (20)     1433 2022-08-19 23:03:05.000000 tasq-client-python-0.1.9/tasq_client/check_type_test.py
+-rw-r--r--   0 alex       (502) staff       (20)    11229 2023-02-09 20:20:41.000000 tasq-client-python-0.1.9/tasq_client/client.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-02-09 20:23:39.546457 tasq-client-python-0.1.9/tasq_client_python.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)      143 2023-02-09 20:23:39.000000 tasq-client-python-0.1.9/tasq_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)      330 2023-02-09 20:23:39.000000 tasq-client-python-0.1.9/tasq_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2023-02-09 20:23:39.000000 tasq-client-python-0.1.9/tasq_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (502) staff       (20)        9 2023-02-09 20:23:39.000000 tasq-client-python-0.1.9/tasq_client_python.egg-info/requires.txt
+-rw-r--r--   0 alex       (502) staff       (20)       12 2023-02-09 20:23:39.000000 tasq-client-python-0.1.9/tasq_client_python.egg-info/top_level.txt
```

### Comparing `tasq-client-python-0.1.8/tasq_client/check_type.py` & `tasq-client-python-0.1.9/tasq_client/check_type.py`

 * *Files identical despite different names*

### Comparing `tasq-client-python-0.1.8/tasq_client/check_type_test.py` & `tasq-client-python-0.1.9/tasq_client/check_type_test.py`

 * *Files identical despite different names*

### Comparing `tasq-client-python-0.1.8/tasq_client/client.py` & `tasq-client-python-0.1.9/tasq_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import multiprocessing
 import sys
 import time
 import urllib.parse
 from contextlib import contextmanager
 from dataclasses import dataclass
-from multiprocessing import Process
+from multiprocessing.context import BaseContext
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 
 from .check_type import CheckTypeException, OptionalKey, check_type
 
 
@@ -65,14 +66,15 @@
         self.keepalive_interval = keepalive_interval
         self.context = context
         self.username = username
         self.password = password
         self.max_timeout = max_timeout
         self.task_timeout = task_timeout
         self.session = requests.Session()
+        self.mp_context = multiprocessing.get_context("spawn")
         if username is not None or password is not None:
             assert username is not None and password is not None
             self.session.auth = (username, password)
 
     def push(self, contents: str) -> str:
         """Push a task and get its resulting ID."""
         return self._post_form("/task/push", dict(contents=contents), type_template=str)
@@ -169,15 +171,17 @@
         This is meant to be used in a `with` clause. When the `with` clause is
         exited, the keepalive loop is stopped, and the task will be marked as
         completed unless the with clause is exited with an exception.
         """
         while True:
             task, timeout = self.pop()
             if task is not None:
-                rt = RunningTask(self, id=task.id, contents=task.contents)
+                rt = RunningTask(
+                    self, id=task.id, contents=task.contents, mp_context=self.mp_context
+                )
                 try:
                     yield rt
                     rt.completed()
                 finally:
                     rt.cancel()
                 return
             elif timeout is not None:
@@ -195,14 +199,27 @@
                 running=int,
                 expired=int,
                 completed=int,
             ),
         )
         return QueueCounts(**data)
 
+    def __getstate__(
+        self,
+    ):
+        res = self.__dict__.copy()
+        del res["session"]
+        return res
+
+    def __setstate__(self, state: Dict[str, Any]):
+        self.__dict__ = state
+        self.session = requests.Session()
+        if self.username is not None:
+            self.session.auth = (self.username, self.password)
+
     def _get(
         self, path: str, type_template: Optional[Any] = None, supports_timeout: bool = False
     ) -> Any:
         return _process_response(
             self.session.get(self._url_for_path(path, supports_timeout)), type_template
         )
 
@@ -238,27 +255,24 @@
 @dataclass
 class RunningTask(Task):
     """
     A task object that periodically sends keepalives in the background until
     cancel() or completed() is called.
     """
 
-    def __init__(self, client: TasqClient, *args, **kwargs):
+    def __init__(
+        self, client: TasqClient, *args, mp_context: Optional[BaseContext] = None, **kwargs
+    ):
         super().__init__(*args, **kwargs)
         self.client = client
-        self._proc = Process(
+        self._proc = (mp_context or multiprocessing).Process(
             target=RunningTask._keepalive_worker,
             name="tasq-keepalive-worker",
             args=(
-                client.base_url,
-                client.context,
-                client.username,
-                client.password,
-                client.task_timeout,
-                client.keepalive_interval,
+                client,
                 self.id,
             ),
             daemon=True,
         )
         self._proc.start()
 
     def cancel(self):
@@ -270,35 +284,23 @@
 
     def completed(self):
         self.cancel()
         self.client.completed(self.id)
 
     @staticmethod
     def _keepalive_worker(
-        base_url: str,
-        context: str,
-        username: Optional[str],
-        password: Optional[str],
-        task_timeout: Optional[float],
-        interval: float,
+        client: TasqClient,
         task_id: str,
     ):
-        client = TasqClient(
-            base_url,
-            context=context,
-            username=username,
-            password=password,
-            task_timeout=task_timeout,
-        )
         while True:
             try:
                 client.keepalive(task_id)
             except Exception as exc:  # pylint: disable=broad-except
                 print(f"exception in tasq keepalive worker: {exc}", file=sys.stderr)
-            time.sleep(interval)
+            time.sleep(client.keepalive_interval)
 
 
 class TasqRemoteError(Exception):
     """An error returned by a remote server."""
 
 
 class TasqMisbehavingServerError(Exception):
```

