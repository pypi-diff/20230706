# Comparing `tmp/runweb-0.2.0.tar.gz` & `tmp/runweb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runweb-0.2.0.tar", last modified: Wed Jun 21 15:50:23 2023, max compression
+gzip compressed data, was "runweb-0.3.0.tar", last modified: Thu Jul  6 11:37:27 2023, max compression
```

## Comparing `runweb-0.2.0.tar` & `runweb-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11341 2023-06-21 15:50:04.971581 runweb-0.2.0/LICENSE
--rw-r--r--   0        0        0      729 2023-06-21 15:50:04.971581 runweb-0.2.0/README.md
--rw-r--r--   0        0        0     1218 2023-06-21 15:50:23.816752 runweb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__init__.py
--rw-r--r--   0        0        0       29 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__main__.py
--rw-r--r--   0        0        0       22 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/__version__.py
--rw-r--r--   0        0        0     3544 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/main.py
--rw-r--r--   0        0        0     2171 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/multiprocess.py
--rw-r--r--   0        0        0     2110 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/parse.py
--rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/__init__.py
--rw-r--r--   0        0        0      798 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/uvicorn.py
--rw-r--r--   0        0        0      787 2023-06-21 15:50:04.971581 runweb-0.2.0/runweb/runner/waitress.py
--rw-r--r--   0        0        0        0 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      930 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/test_uvicorn.py
--rw-r--r--   0        0        0      934 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/test_waitress.py
--rw-r--r--   0        0        0      866 2023-06-21 15:50:04.971581 runweb-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-06 11:37:10.609843 runweb-0.3.0/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-06 11:37:10.609843 runweb-0.3.0/README.md
+-rw-r--r--   0        0        0     1230 2023-07-06 11:37:27.082029 runweb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/__version__.py
+-rw-r--r--   0        0        0     3544 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/main.py
+-rw-r--r--   0        0        0     2171 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/multiprocess.py
+-rw-r--r--   0        0        0     2120 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/parse.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/__init__.py
+-rw-r--r--   0        0        0      837 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/uvicorn.py
+-rw-r--r--   0        0        0      814 2023-07-06 11:37:10.609843 runweb-0.3.0/runweb/runner/waitress.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/test_uvicorn.py
+-rw-r--r--   0        0        0      934 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/test_waitress.py
+-rw-r--r--   0        0        0      866 2023-07-06 11:37:10.609843 runweb-0.3.0/tests/utils.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 runweb-0.3.0/PKG-INFO
```

### Comparing `runweb-0.2.0/LICENSE` & `runweb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/README.md` & `runweb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/pyproject.toml` & `runweb-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "click>=8.1.3",
 ]
 description = "Run web server with one command."
 dynamic = []
 name = "runweb"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.2.0"
+version = "0.3.0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 tui = [
     "trogon>=0.4.0",
@@ -54,14 +54,14 @@
 [tool.pdm.scripts.lint]
 shell = "ruff --fix ."
 
 [tool.pdm.scripts.test]
 shell = "pytest tests"
 
 [tool.pdm.scripts.push-tag]
-shell = "git add runweb/__version__.py && git commit -m v`pdm show --version` && git tag v`pdm show --version` && git push --tags"
+shell = "git add runweb/__version__.py && git commit -m v`pdm show --version` && git tag v`pdm show --version` && git push && git push --tags"
 
 [build-system]
 build-backend = "pdm.backend"
 requires = [
     "pdm-backend",
 ]
```

### Comparing `runweb-0.2.0/runweb/main.py` & `runweb-0.3.0/runweb/main.py`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/runweb/multiprocess.py` & `runweb-0.3.0/runweb/multiprocess.py`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/runweb/parse.py` & `runweb-0.3.0/runweb/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import ipaddress
 from functools import reduce
 from typing import Any
 
 import click
 
 
-def parse_bind(value) -> socket.socket:
+def parse_bind(value: str) -> socket.socket:
     if value.startswith("unix:"):
         path = value[5:]
         sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         sock.bind(path)
 
         uds_perms = 0o666
         os.chmod(path, uds_perms)
@@ -39,15 +39,15 @@
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
     else:  # In windows, SO_REUSEPORT is not available
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.bind((str(address), port))
     return sock
 
 
-def parse_application(value) -> Any:
+def parse_application(value: str) -> Any:
     module_str, _, attrs_str = value.partition(":")
     if not module_str or not attrs_str:
         message = (
             'Import string "{import_str}" must be in format "<module>:<attribute>".'
         )
         raise click.BadParameter(message.format(import_str=value))
```

### Comparing `runweb-0.2.0/tests/test_uvicorn.py` & `runweb-0.3.0/tests/test_uvicorn.py`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/tests/test_waitress.py` & `runweb-0.3.0/tests/test_waitress.py`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/tests/utils.py` & `runweb-0.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `runweb-0.2.0/PKG-INFO` & `runweb-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runweb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Run web server with one command.
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache-2.0
 Requires-Python: >=3.7
 Requires-Dist: click>=8.1.3
 Requires-Dist: trogon>=0.4.0; extra == "tui"
 Requires-Dist: waitress; extra == "waitress"
```

