# Comparing `tmp/proteus_runtime-0.2.9.tar.gz` & `tmp/proteus_runtime-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_runtime-0.2.9.tar", max compression
+gzip compressed data, was "proteus_runtime-0.3.0.tar", max compression
```

## Comparing `proteus_runtime-0.2.9.tar` & `proteus_runtime-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/LICENSE
--rw-r--r--   0        0        0     2851 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/__init__.py
--rw-r--r--   0        0        0     7519 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/api.py
--rw-r--r--   0        0        0        0 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/__init__.py
--rw-r--r--   0        0        0      258 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/calculator.py
--rw-r--r--   0        0        0      518 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/grammar.py
--rw-r--r--   0        0        0     2150 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/operations.py
--rw-r--r--   0        0        0      371 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/calculator/parser.py
--rw-r--r--   0        0        0      507 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/config.py
--rw-r--r--   0        0        0     1109 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/logger.py
--rw-r--r--   0        0        0     6652 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/oidc.py
--rw-r--r--   0        0        0     2595 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/proteus/reporting.py
--rw-r--r--   0        0        0     1462 2023-02-01 12:35:34.887855 proteus_runtime-0.2.9/pyproject.toml
--rw-r--r--   0        0        0      825 1970-01-01 00:00:00.000000 proteus_runtime-0.2.9/setup.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 proteus_runtime-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3967 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/__init__.py
+-rw-r--r--   0        0        0     9635 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/api.py
+-rw-r--r--   0        0        0     3009 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/bin/runs_workflow.py
+-rw-r--r--   0        0        0     8619 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/bucket.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/calculator/__init__.py
+-rw-r--r--   0        0        0      258 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/calculator/calculator.py
+-rw-r--r--   0        0        0      521 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/calculator/grammar.py
+-rw-r--r--   0        0        0     2184 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/calculator/operations.py
+-rw-r--r--   0        0        0      371 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/calculator/parser.py
+-rw-r--r--   0        0        0      815 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/config.py
+-rw-r--r--   0        0        0     1580 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/logger.py
+-rw-r--r--   0        0        0     6727 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/oidc.py
+-rw-r--r--   0        0        0     3367 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/reporting.py
+-rw-r--r--   0        0        0     2594 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/runs.py
+-rw-r--r--   0        0        0     2549 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/proteus/vault.py
+-rw-r--r--   0        0        0     1479 2023-07-06 16:19:51.950641 proteus_runtime-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 proteus_runtime-0.3.0/PKG-INFO
```

### Comparing `proteus_runtime-0.2.9/LICENSE` & `proteus_runtime-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteus_runtime-0.2.9/proteus/calculator/grammar.py` & `proteus_runtime-0.3.0/proteus/calculator/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 grammar_str = (
     e_str  # noqa: W503
     + c_str  # noqa: W503
     + r"""
 terminals
 number: /\-?\d+(\.\d+)?/;
-array: /\$[a-zA-Z_][a-zA-Z0-9_]*/;
+array: /\$?\$[a-zA-Z_][a-zA-Z0-9_]*/;
 """  # noqa: W503
 )
 
 grammar = Grammar.from_string(grammar_str)
```

### Comparing `proteus_runtime-0.2.9/proteus/calculator/operations.py` & `proteus_runtime-0.3.0/proteus/calculator/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 import re
 import math
 
 
 def _get(ref, ctx):
-    if re.match(r"\$[a-zA-Z_]\w*", str(ref)):
-        return ctx.get(ref[1:])
+    result = re.search(r"\$?\$([a-zA-Z_]\w*)", str(ref))
+    if result:
+        return ctx.get(result.group(1))
     elif re.match(r"\-?\d+(\.\d+)?", str(ref)):
         return ref
     else:
         return ref(ctx)
 
 
 operations = {
```

### Comparing `proteus_runtime-0.2.9/proteus/logger.py` & `proteus_runtime-0.3.0/proteus/logger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 import logging
 import logging.config
 import logging.handlers
 import os
+import shutil
 
 from pathlib import Path
 
+FALLBACK_LOGGING_PATH = os.path.join(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")), "logging.ini")
+
 
 def initialize_logger(log_loc=None):
     # Discover logging.ini path
     if log_loc:
         logging_path = log_loc if os.path.isabs(log_loc) else os.path.abspath(os.path.join(os.curdir, log_loc))
 
-        logging_path = os.path.join(logging_path, "logging.ini")
-
-        if not os.path.exists(logging_path):
+        if not logging_path.endswith("logging.ini"):
+            logging_path = os.path.join(logging_path, "logging.ini")
+            if not os.path.exists(logging_path):
+                shutil.copy(FALLBACK_LOGGING_PATH, logging_path)
+        elif not os.path.exists(logging_path):
             raise FileNotFoundError(f"Proteus runtime - log_log path not found: {logging_path}")
     else:
         # Fallback to runtime logger
-        logging_path = os.path.join(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")), "logging.ini")
-
-    # Create logs folder. See logging.ini
-    Path(os.path.join(os.path.dirname(logging_path), "logs")).mkdir(parents=True, exist_ok=True)
+        logging_path = FALLBACK_LOGGING_PATH
 
-    # Init logger
-    logging.config.fileConfig(logging_path, disable_existing_loggers=False)
+    try:
+        # Create logs folder. See logging.ini
+        Path(os.path.join(os.path.dirname(logging_path), "logs")).mkdir(parents=True, exist_ok=True)
+        # Init logger
+        logging.config.fileConfig(logging_path, disable_existing_loggers=False)
+    except PermissionError:
+        print(
+            f"There are no permissions to create log files in {os.path.dirname(logging_path)}"
+            ", will continue without storing logs on the machine"
+        )
 
     # Disable known noisy loggers
     azure_logger = logging.getLogger("azure.core.pipeline.policies.http_logging_policy")
     azure_logger.setLevel(logging.WARNING)
 
     return logging.getLogger(__name__)
```

### Comparing `proteus_runtime-0.2.9/proteus/oidc.py` & `proteus_runtime-0.3.0/proteus/oidc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import json
 import re
-from copy import deepcopy
 from threading import Timer, Lock
 
 import certifi
 import requests
 
 
 class RepeatTimer(Timer):
@@ -20,26 +19,24 @@
 def is_worker_username(username):
     return WORKER_USERNAME_RE.match(username) is not None
 
 
 class OIDC:
     def __init__(
         self,
-        config,
         proteus,
     ):
-        host = config.auth_host
+        host = proteus.config.auth_host
 
-        self.config = deepcopy(config)
         self.proteus = proteus
-        self.username = config.username
+        self.username = proteus.config.username
         self.host = host if host.endswith("/auth") else host + "/auth"
-        self.realm = config.realm
-        self.client_id = config.client_id
-        self.client_secret = config.client_secret
+        self.realm = proteus.config.realm
+        self.client_id = proteus.config.client_id
+        self.client_secret = proteus.config.client_secret
         self._access_token_locked = Lock()
         self._last_res = None
         self._refresh_timer = None
         self._when_login_callback = None
         self._when_refresh_callback = None
         self._update_credentials()
         self._i_am_robot = False
@@ -59,15 +56,14 @@
         self._access_token = access_token
         self._refresh_token = refresh_token
         self._expires_in = expires_in
         self._resfresh_expires_in = refresh_expires_in
 
     @property
     def access_token(self):
-        self.do_refresh()
         self._access_token_locked.acquire()
         result = self._access_token
         self._access_token_locked.release()
         return result
 
     @property
     def access_token_parsed(self):
@@ -105,27 +101,26 @@
             data=login,
             verify=certifi.where(),
             headers={"Content-Type": "application/x-www-form-urlencoded"},
         )
         if response.status_code == 401:
             # No need to be blunt
             return None
-        response.raise_for_status()
+        self.proteus.api.raise_for_status(response)
         return response
 
     def do_login(self, password=None, username=None, auto_update=True):
         login = {
             "grant_type": "password",
             "username": self.username if username is None else username,
-            "password": password or self.config.password,
+            "password": password or self.proteus.config.password,
             "client_id": self.client_id,
         }
         if self.client_secret is not None:
             login["client_secret"] = self.client_secret
-
         response = self.send_login_request(login)
         self.proteus.api.raise_for_status(response)
 
         credentials = response.json()
         assert "access_token" in credentials
         if self._when_login_callback is not None:
             self._when_login_callback()
@@ -143,26 +138,26 @@
 
     def prepare_refresh(self):
         assert self.expires_in is not None
 
         def perform_refresh():
             self.do_refresh()
 
-        self._refresh_timer = RepeatTimer(self.expires_in - self.config.refresh_gap, perform_refresh)
+        self._refresh_timer = RepeatTimer(self.expires_in - self.proteus.config.refresh_gap, perform_refresh)
         self._refresh_timer.start()
 
     # @may_insist_up_to(5, delay_in_secs=1)
     def send_refresh_request(self, refresh):
         response = requests.post(
             self.url,
             data=refresh,
             verify=certifi.where(),
             headers={"Content-Type": "application/x-www-form-urlencoded"},
         )
-        response.raise_for_status()
+        self.proteus.api.raise_for_status(response)
         return response
 
     def do_refresh(self):
         assert self.refresh_token is not None
         self._access_token_locked.acquire()
         refresh = {
             "grant_type": "refresh_token",
@@ -200,13 +195,15 @@
         if self.am_i_robot:
             unit_name = parsed_token.get("preferred_username")
             return f"unit {unit_name}"
         return parsed_token.get("given_name")
 
     @property
     def worker_uuid(self):
+        if self.proteus.config.worker_uuid:
+            return self.proteus.config.worker_uuid
         if self.am_i_robot:
             username = self.access_token_parsed.get("preferred_username")
             robot_match = WORKER_USERNAME_RE.match(username)
             if robot_match is not None:
                 return robot_match.groupdict().get("uuid")
         return None
```

### Comparing `proteus_runtime-0.2.9/proteus/reporting.py` & `proteus_runtime-0.3.0/proteus/reporting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,40 @@
+from functools import wraps
+
+
 class Reporting:
     """Unifies logging and reporting to status API"""
 
-    def __init__(self, logger, api=None):
-        self.logger = logger
-        self.api = api
+    def __init__(self, proteus):
+        self.proteus = proteus
+
+    def ensure_failed_is_reported(self, fn):
+        @wraps(fn)
+        def _(*args, **kwargs):
+            try:
+                return fn(*args, **kwargs)
+            except SystemExit as error:
+                if error.code != 0:
+                    self.send(status="failed", message="Exit status different than 0")
+                raise
+            except BaseException as error:
+                self.send(status="failed", message=str(error))
+                raise
+
+        return _
+
+    def ensure_finished_is_reported(self, fn):
+        @wraps(fn)
+        def _(*args, **kwargs):
+            fn(*args, **kwargs)
+            self.send(
+                "Begin configuration validation process",
+                status="completed",
+                progress=100,
+            )
 
     def send(
         self,
         message,
         status="processing",
         progress=0,
         result=None,
@@ -22,28 +49,28 @@
             status (str): The status to report
             progress (int): The progress of the job
             result (dict): The result of the job
             total (int): The total elements of the job
             number (int): The number of actual elements completed
         """
         assert status is not None, "Status can't be set to None"
-        self.logger.info(
+        self.proteus.logger.info(
             message,
             extra={"status": status, "progress": progress, "result": result},
         )
-        if self.api:
-            self._report(
-                self.api.auth.worker_uuid,
-                set_status=str(status),
-                message=message,
-                progress=progress,
-                result=result,
-                total=total,
-                number=number,
-            )
+
+        self._report(
+            self.proteus.auth.worker_uuid,
+            set_status=str(status),
+            message=message,
+            progress=progress,
+            result=result,
+            total=total,
+            number=number,
+        )
 
     def _report(
         self,
         worker_uuid,
         set_status="processing",
         message=None,
         progress=0,
@@ -75,10 +102,10 @@
         if message is not None:
             report["message"] = message
         if result is not None:
             report["result"] = result
         report["number"] = number
         report["total"] = total
         data["report"] = report
-        response = self.api.post(status_url, data)
-        response.raise_for_status()
+        response = self.proteus.api.post(status_url, data, retry=True)
+        self.proteus.api.raise_for_status(response)
         return response
```

### Comparing `proteus_runtime-0.2.9/pyproject.toml` & `proteus_runtime-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "proteus-runtime"
-version = "0.2.9"
+version = "0.3.0"
 description = ""
 authors = []
 packages = [
     { include = "proteus" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-json-logger = "^2.0.4"
 requests = "^2.28.1"
 certifi = "^2022.12.07"
-setuptools = "^65.0.0"
+setuptools = "^67.0.0"
 parglare = "^0.16.0"
 numpy = "^1.23.3"
 azure-storage-blob = "^12.14.1"
 multipart = "^0.2.4"
+tqdm = "^4.65.0"
 
 [tool.poetry.dev-dependencies]
 python-dotenv = "^0.19.2"
 black = "^22.6.0"
 pre-commit = "^2.9.3"
 pytest = "^7.2.0"
 pytest-mock = "^3.5.1"
```

### Comparing `proteus_runtime-0.2.9/PKG-INFO` & `proteus_runtime-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: proteus-runtime
-Version: 0.2.9
+Version: 0.3.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-storage-blob (>=12.14.1,<13.0.0)
 Requires-Dist: certifi (>=2022.12.07,<2023.0.0)
 Requires-Dist: multipart (>=0.2.4,<0.3.0)
 Requires-Dist: numpy (>=1.23.3,<2.0.0)
 Requires-Dist: parglare (>=0.16.0,<0.17.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: setuptools (>=65.0.0,<66.0.0)
+Requires-Dist: setuptools (>=67.0.0,<68.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

