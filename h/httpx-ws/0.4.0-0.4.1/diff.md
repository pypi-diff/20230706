# Comparing `tmp/httpx_ws-0.4.0.tar.gz` & `tmp/httpx_ws-0.4.1.tar.gz`

## Comparing `httpx_ws-0.4.0.tar` & `httpx_ws-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.all-contributorsrc
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.editorconfig
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/docs/index.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/docs/reference/httpx_ws.md
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/docs/usage/asgi.md
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/docs/usage/quickstart.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/docs/usage/subprotocols.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/httpx_ws/__init__.py
--rw-r--r--   0        0        0    43535 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/httpx_ws/_api.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/httpx_ws/_ping.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/httpx_ws/py.typed
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/httpx_ws/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0    31610 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/tests/test_api.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/tests/test_transport.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/LICENSE
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/README.md
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/PKG-INFO
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 httpx_ws-0.4.0/setup.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.all-contributorsrc
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.editorconfig
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/docs/index.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/docs/reference/httpx_ws.md
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/docs/usage/asgi.md
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/docs/usage/quickstart.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/docs/usage/subprotocols.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/httpx_ws/__init__.py
+-rw-r--r--   0        0        0    43521 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/httpx_ws/_api.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/httpx_ws/_ping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/httpx_ws/py.typed
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/httpx_ws/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0    31596 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/tests/test_api.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/tests/test_transport.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/README.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 httpx_ws-0.4.1/setup.py
```

### Comparing `httpx_ws-0.4.0/.all-contributorsrc` & `httpx_ws-0.4.1/.all-contributorsrc`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9083333333333333%*

 * *Differences: {"'commitType'": "'docs'",*

 * * "'contributors'": "{insert: [(4, OrderedDict([('login', 'saforem2'), ('name', 'Sam Foreman'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/5234251?v=4'), "*

 * *                   "('profile', 'https://samforeman.me'), ('contributions', ['bug'])]))]}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "commit": false,
     "commitConvention": "angular",
+    "commitType": "docs",
     "contributors": [
         {
             "avatar_url": "https://avatars.githubusercontent.com/u/1144727?v=4",
             "contributions": [
                 "maintenance",
                 "code"
             ],
@@ -34,14 +35,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/17018576?v=4",
             "contributions": [
                 "bug"
             ],
             "login": "ysmu",
             "name": "ysmu",
             "profile": "https://github.com/ysmu"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/5234251?v=4",
+            "contributions": [
+                "bug"
+            ],
+            "login": "saforem2",
+            "name": "Sam Foreman",
+            "profile": "https://samforeman.me"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `httpx_ws-0.4.0/mkdocs.yml` & `httpx_ws-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `httpx_ws-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/.github/workflows/build.yml` & `httpx_ws-0.4.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/.github/workflows/docs.yml` & `httpx_ws-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/docs/usage/asgi.md` & `httpx_ws-0.4.1/docs/usage/asgi.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/docs/usage/quickstart.md` & `httpx_ws-0.4.1/docs/usage/quickstart.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/docs/usage/subprotocols.md` & `httpx_ws-0.4.1/docs/usage/subprotocols.md`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/httpx_ws/__init__.py` & `httpx_ws-0.4.1/httpx_ws/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 from httpx_ws._api import (
     AsyncWebSocketSession,
     HTTPXWSException,
     JSONMode,
     WebSocketDisconnect,
     WebSocketInvalidTypeReceived,
```

### Comparing `httpx_ws-0.4.0/httpx_ws/_api.py` & `httpx_ws-0.4.1/httpx_ws/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import secrets
 import threading
 import typing
 
 import httpcore
 import httpx
 import wsproto
-from httpcore.backends.base import AsyncNetworkStream, NetworkStream
+from httpcore import AsyncNetworkStream, NetworkStream
 from wsproto.connection import CloseReason
 
 from httpx_ws._ping import AsyncPingManager, PingManager
 
 JSONMode = typing.Literal["text", "binary"]
 TaskFunction = typing.TypeVar("TaskFunction")
 TaskResult = typing.TypeVar("TaskResult")
```

### Comparing `httpx_ws-0.4.0/httpx_ws/_ping.py` & `httpx_ws-0.4.1/httpx_ws/_ping.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/httpx_ws/transport.py` & `httpx_ws-0.4.1/httpx_ws/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import contextlib
 import queue
 import typing
 from concurrent.futures import Future
 
 import anyio
 import wsproto
-from httpcore.backends.base import AsyncNetworkStream
+from httpcore import AsyncNetworkStream
 from httpx import ASGITransport, AsyncByteStream, Request, Response
 from wsproto.connection import CloseReason
 
 from httpx_ws._api import WebSocketDisconnect
 
 Scope = typing.Dict[str, typing.Any]
 Message = typing.Dict[str, typing.Any]
```

### Comparing `httpx_ws-0.4.0/tests/conftest.py` & `httpx_ws-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/tests/test_api.py` & `httpx_ws-0.4.1/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import typing
 from unittest.mock import MagicMock, call, patch
 
 import httpcore
 import httpx
 import pytest
 import wsproto
-from httpcore.backends.base import AsyncNetworkStream, NetworkStream
+from httpcore import AsyncNetworkStream, NetworkStream
 from starlette.websockets import WebSocket
 from starlette.websockets import WebSocketDisconnect as StarletteWebSocketDisconnect
 
 from httpx_ws import (
     AsyncWebSocketSession,
     JSONMode,
     WebSocketDisconnect,
```

### Comparing `httpx_ws-0.4.0/tests/test_transport.py` & `httpx_ws-0.4.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/.gitignore` & `httpx_ws-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/LICENSE` & `httpx_ws-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_ws-0.4.0/README.md` & `httpx_ws-0.4.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://samforeman.me"><img src="https://avatars.githubusercontent.com/u/5234251?v=4?s=100" width="100px;" alt="Sam Foreman"/><br /><sub><b>Sam Foreman</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Asaforem2" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -16,17 +16,17 @@
 This is a very young project. Expect bugs ð ```bash pip install httpx-ws ```
 ## Features * [X] Sync and async client * [X] Helper methods to send text,
 binary and JSON data * [X] Helper methods to receive text, binary and JSON data
 * [X] Automatic ping/pong answers * [X] HTTPX transport to test WebSockets
 defined in ASGI apps * [X] Automatic keepalive ping ## Contributors â¨ Thanks
 goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
 en/emoji-key)):
-[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]
- FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu
-    ð§ ð�     ð»        ð¦     ð
+[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]  [Sam_Foreman]
+ FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu    Sam_Foreman
+    ð§ ð�     ð»        ð¦     ð�    ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment We use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it's installed on your system. ### Run unit tests You
 can run all the tests with: ```bash hatch run test ``` ### Format the code
 Execute the following command to apply linting and check typing: ```bash hatch
```

### Comparing `httpx_ws-0.4.0/pyproject.toml` & `httpx_ws-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,14 @@
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "anyio",
     "httpx>=0.23.1",
-    "httpcore>=0.16.1",
+    "httpcore>=0.17.3,<0.18",
     "wsproto",
 ]
 
 [project.urls]
 Documentation = "https://frankie567.github.io/httpx-ws/"
 Source = "https://github.com/frankie567/httpx-ws"
```

### Comparing `httpx_ws-0.4.0/PKG-INFO` & `httpx_ws-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-ws
-Version: 0.4.0
+Version: 0.4.1
 Summary: WebSockets support for HTTPX
 Project-URL: Documentation, https://frankie567.github.io/httpx-ws/
 Project-URL: Source, https://github.com/frankie567/httpx-ws
 Author-email: François Voron <fvoron@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
 Requires-Python: >=3.8
 Requires-Dist: anyio
-Requires-Dist: httpcore>=0.16.1
+Requires-Dist: httpcore<0.18,>=0.17.3
 Requires-Dist: httpx>=0.23.1
 Requires-Dist: wsproto
 Description-Content-Type: text/markdown
 
 # HTTPX WS
 
 <p align="center">
@@ -75,14 +75,15 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://samforeman.me"><img src="https://avatars.githubusercontent.com/u/5234251?v=4?s=100" width="100px;" alt="Sam Foreman"/><br /><sub><b>Sam Foreman</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Asaforem2" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: httpx-ws Version: 0.4.0 Summary: WebSockets support
+Metadata-Version: 2.1 Name: httpx-ws Version: 0.4.1 Summary: WebSockets support
 for HTTPX Project-URL: Documentation, https://frankie567.github.io/httpx-ws/
 Project-URL: Source, https://github.com/frankie567/httpx-ws Author-email:
 FranÃ§ois Voron
 gmail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Python: >=3.8 Requires-Dist: anyio Requires-Dist: httpcore>=0.16.1
-Requires-Dist: httpx>=0.23.1 Requires-Dist: wsproto Description-Content-Type:
-text/markdown # HTTPX WS
+Requires-Python: >=3.8 Requires-Dist: anyio Requires-Dist:
+httpcore<0.18,>=0.17.3 Requires-Dist: httpx>=0.23.1 Requires-Dist: wsproto
+Description-Content-Type: text/markdown # HTTPX WS
                          WebSockets support for HTTPX
 [![build](https://github.com/frankie567/httpx-ws/workflows/Build/badge.svg)]
 (https://github.com/frankie567/httpx-ws/actions) [![codecov](https://
 codecov.io/gh/frankie567/httpx-ws/branch/main/graph/
 badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws) [![All
 Contributors](https://img.shields.io/badge/all_contributors-2-
 orange.svg?style=flat-square)](#contributors-) [![PyPI version](https://
@@ -28,17 +28,17 @@
 This is a very young project. Expect bugs ð ```bash pip install httpx-ws ```
 ## Features * [X] Sync and async client * [X] Helper methods to send text,
 binary and JSON data * [X] Helper methods to receive text, binary and JSON data
 * [X] Automatic ping/pong answers * [X] HTTPX transport to test WebSockets
 defined in ASGI apps * [X] Automatic keepalive ping ## Contributors â¨ Thanks
 goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
 en/emoji-key)):
-[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]
- FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu
-    ð§ ð�     ð»        ð¦     ð
+[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]  [Sam_Foreman]
+ FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu    Sam_Foreman
+    ð§ ð�     ð»        ð¦     ð�    ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment We use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it's installed on your system. ### Run unit tests You
 can run all the tests with: ```bash hatch run test ``` ### Format the code
 Execute the following command to apply linting and check typing: ```bash hatch
```

### Comparing `httpx_ws-0.4.0/setup.py` & `httpx_ws-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='httpx-ws',
-    version='0.4.0',
+    version='0.4.1',
     description='WebSockets support for HTTPX',
-    long_description='# HTTPX WS\n\n<p align="center">\n    <em>WebSockets support for HTTPX</em>\n</p>\n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https://codecov.io/gh/frankie567/httpx-ws/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)\n[![PyPI version](https://badge.fury.io/py/httpx-ws.svg)](https://badge.fury.io/py/httpx-ws)\n[![Downloads](https://pepy.tech/badge/httpx-ws)](https://pepy.tech/project/httpx-ws)\n\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://frankie567.github.io/httpx-ws/" target="_blank">https://frankie567.github.io/httpx-ws/</a>\n\n**Source Code**: <a href="https://github.com/frankie567/httpx-ws" target="_blank">https://github.com/frankie567/httpx-ws</a>\n\n---\n\n## Installation\n\n> **Warning**\n>\n> This is a very young project. Expect bugs 🐛\n\n```bash\npip install httpx-ws\n```\n\n## Features\n\n* [X] Sync and async client\n* [X] Helper methods to send text, binary and JSON data\n* [X] Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/pong answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n* [X] Automatic keepalive ping\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply linting and check typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
+    long_description='# HTTPX WS\n\n<p align="center">\n    <em>WebSockets support for HTTPX</em>\n</p>\n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https://codecov.io/gh/frankie567/httpx-ws/branch/main/graph/badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)\n[![PyPI version](https://badge.fury.io/py/httpx-ws.svg)](https://badge.fury.io/py/httpx-ws)\n[![Downloads](https://pepy.tech/badge/httpx-ws)](https://pepy.tech/project/httpx-ws)\n\n<p align="center">\n<a href="https://github.com/sponsors/frankie567"><img src="https://md-buttons.francoisvoron.com/button.svg?text=Buy%20me%20a%20coffee%20%E2%98%95%EF%B8%8F&bg=ef4444&w=200&h=50"></a>\n</p>\n\n---\n\n**Documentation**: <a href="https://frankie567.github.io/httpx-ws/" target="_blank">https://frankie567.github.io/httpx-ws/</a>\n\n**Source Code**: <a href="https://github.com/frankie567/httpx-ws" target="_blank">https://github.com/frankie567/httpx-ws</a>\n\n---\n\n## Installation\n\n> **Warning**\n>\n> This is a very young project. Expect bugs 🐛\n\n```bash\npip install httpx-ws\n```\n\n## Features\n\n* [X] Sync and async client\n* [X] Helper methods to send text, binary and JSON data\n* [X] Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/pong answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n* [X] Automatic keepalive ping\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="http://francoisvoron.com"><img src="https://avatars.githubusercontent.com/u/1144727?v=4?s=100" width="100px;" alt="François Voron"/><br /><sub><b>François Voron</b></sub></a><br /><a href="#maintenance-frankie567" title="Maintenance">🚧</a> <a href="https://github.com/frankie567/httpx-ws/commits?author=frankie567" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://kousikmitra.github.io"><img src="https://avatars.githubusercontent.com/u/15109533?v=4?s=100" width="100px;" alt="Kousik Mitra"/><br /><sub><b>Kousik Mitra</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/commits?author=kousikmitra" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/davidbrochart"><img src="https://avatars.githubusercontent.com/u/4711805?v=4?s=100" width="100px;" alt="David Brochart"/><br /><sub><b>David Brochart</b></sub></a><br /><a href="#platform-davidbrochart" title="Packaging/porting to new platform">📦</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ysmu"><img src="https://avatars.githubusercontent.com/u/17018576?v=4?s=100" width="100px;" alt="ysmu"/><br /><sub><b>ysmu</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Aysmu" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://samforeman.me"><img src="https://avatars.githubusercontent.com/u/5234251?v=4?s=100" width="100px;" alt="Sam Foreman"/><br /><sub><b>Sam Foreman</b></sub></a><br /><a href="https://github.com/frankie567/httpx-ws/issues?q=author%3Asaforem2" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://hatch.pypa.io/latest/install/) to manage the development environment and production build. Ensure it\'s installed on your system.\n\n### Run unit tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n### Format the code\n\nExecute the following command to apply linting and check typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
     author_email='François Voron <fvoron@gmail.com>',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: AsyncIO',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP :: Session',
     ],
     install_requires=[
         'anyio',
-        'httpcore>=0.16.1',
+        'httpcore<0.18,>=0.17.3',
         'httpx>=0.23.1',
         'wsproto',
     ],
     packages=[
         'httpx_ws',
         'tests',
     ],
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*- from setuptools import setup setup( name='httpx-ws',
-version='0.4.0', description='WebSockets support for HTTPX',
+version='0.4.1', description='WebSockets support for HTTPX',
 long_description='# HTTPX WS\n\n
                        \n WebSockets support for HTTPX\n
 \n\n[![build](https://github.com/frankie567/httpx-ws/workflows/Build/
 badge.svg)](https://github.com/frankie567/httpx-ws/actions)\n[![codecov](https:
 //codecov.io/gh/frankie567/httpx-ws/branch/main/graph/
 badge.svg?token=fL49kIvrj6)](https://codecov.io/gh/frankie567/httpx-ws)\n[![All
 Contributors](https://img.shields.io/badge/all_contributors-2-
@@ -19,26 +19,26 @@
 ð\n\n```bash\npip install httpx-ws\n```\n\n## Features\n\n* [X] Sync and
 async client\n* [X] Helper methods to send text, binary and JSON data\n* [X]
 Helper methods to receive text, binary and JSON data\n* [X] Automatic ping/pong
 answers\n* [X] HTTPX transport to test WebSockets defined in ASGI apps\n* [X]
 Automatic keepalive ping\n\n## Contributors â¨\n\nThanks goes to these
 wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 \n\n\n\n\n
-[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]
- FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu
-    ð§ ð�     ð»        ð¦     ð
+[FranÃ§ois_Voron[Kousik_Mitra] [David_Brochart]  [ysmu]  [Sam_Foreman]
+ FranÃ§ois_Voron Kousik_Mitra   David_Brochart    ysmu    Sam_Foreman
+    ð§ ð�     ð»        ð¦     ð�    ð
 \n\n\n\n\n\n\nThis project follows the [all-contributors](https://github.com/
 all-contributors/all-contributors) specification. Contributions of any kind
 welcome!\n\n## Development\n\n### Setup environment\n\nWe use [Hatch](https://
 hatch.pypa.io/latest/install/) to manage the development environment and
 production build. Ensure it\'s installed on your system.\n\n### Run unit
 tests\n\nYou can run all the tests with:\n\n```bash\nhatch run test\n```\n\n###
 Format the code\n\nExecute the following command to apply linting and check
 typing:\n\n```bash\nhatch run lint\n```\n\n## License\n\nThis project is
 licensed under the terms of the MIT license.\n', author_email='FranÃ§ois Voron
 gmail.com>', classifiers=[ 'Development Status :: 4 - Beta', 'Framework ::
 AsyncIO', 'Intended Audience :: Developers', 'License :: OSI Approved :: MIT
 License', 'Programming Language :: Python :: 3 :: Only', 'Programming Language
 :: Python :: 3.8', 'Programming Language :: Python :: 3.9', 'Programming
 Language :: Python :: 3.10', 'Topic :: Internet :: WWW/HTTP :: Session', ],
-install_requires=[ 'anyio', 'httpcore>=0.16.1', 'httpx>=0.23.1', 'wsproto', ],
-packages=[ 'httpx_ws', 'tests', ], )
+install_requires=[ 'anyio', 'httpcore<0.18,>=0.17.3', 'httpx>=0.23.1',
+'wsproto', ], packages=[ 'httpx_ws', 'tests', ], )
```

