# Comparing `tmp/robotcode_jsonrpc2-0.45.0.tar.gz` & `tmp/robotcode_jsonrpc2-0.46.0.tar.gz`

## Comparing `robotcode_jsonrpc2-0.45.0.tar` & `robotcode_jsonrpc2-0.46.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/__version__.py
--rw-r--r--   0        0        0    30450 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/py.typed
--rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/LICENSE.txt
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/pyproject.toml
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.45.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/__version__.py
+-rw-r--r--   0        0        0    30454 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/py.typed
+-rw-r--r--   0        0        0     9709 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/LICENSE.txt
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/pyproject.toml
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 robotcode_jsonrpc2-0.46.0/PKG-INFO
```

### Comparing `robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/protocol.py` & `robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -457,15 +457,15 @@
         else:
             yield inner(data)
 
     def _handle_body(self, body: bytes, charset: str) -> None:
         try:
             b = body.decode(charset)
 
-            self._data_logger.trace(lambda: f"JSON Received: {b}")
+            self._data_logger.trace(lambda: f"JSON Received: {b!r}")
 
             self._handle_messages(self._generate_json_rpc_messages_from_dict(json.loads(b)))
         except (asyncio.CancelledError, SystemExit, KeyboardInterrupt):
             raise
         except BaseException as e:
             self.__logger.exception(e)
             self.send_error(JsonRPCErrors.PARSE_ERROR, f"{type(e).__name__}: {e}")
@@ -524,15 +524,15 @@
         header = (
             f"Content-Length: {len(body)}\r\nContent-Type: {self.CONTENT_TYPE}; charset={self.CHARSET}\r\n\r\n"
         ).encode("ascii")
 
         if self.write_transport is not None:
             msg = header + body
 
-            self._data_logger.trace(lambda: f"JSON send: {msg.decode()}")
+            self._data_logger.trace(lambda: f"JSON send: {msg.decode()!r}")
 
             if self._loop:
                 self._loop.call_soon_threadsafe(self.write_transport.write, msg)
 
     @__logger.call
     def send_request(
         self,
```

### Comparing `robotcode_jsonrpc2-0.45.0/src/robotcode/jsonrpc2/server.py` & `robotcode_jsonrpc2-0.46.0/src/robotcode/jsonrpc2/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.45.0/.gitignore` & `robotcode_jsonrpc2-0.46.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.45.0/LICENSE.txt` & `robotcode_jsonrpc2-0.46.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.45.0/README.md` & `robotcode_jsonrpc2-0.46.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_jsonrpc2-0.45.0/pyproject.toml` & `robotcode_jsonrpc2-0.46.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotcode-core==0.45.0"]
+dependencies = ["robotcode-core==0.46.0"]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
 Documentation = "https://github.com/d-biehl/robotcode#readme"
 Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
```

### Comparing `robotcode_jsonrpc2-0.45.0/PKG-INFO` & `robotcode_jsonrpc2-0.46.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-jsonrpc2
-Version: 0.45.0
+Version: 0.46.0
 Summary: JSONRPC Server for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-core==0.45.0
+Requires-Dist: robotcode-core==0.46.0
 Description-Content-Type: text/markdown
 
 # robotcode-jsonrpc2
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-jsonrpc2.svg)](https://pypi.org/project/robotcode-jsonrpc2)
 [![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
```

