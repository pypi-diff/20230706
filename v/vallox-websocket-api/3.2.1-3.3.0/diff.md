# Comparing `tmp/vallox_websocket_api-3.2.1.tar.gz` & `tmp/vallox_websocket_api-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vallox_websocket_api-3.2.1.tar", last modified: Thu Apr  6 20:19:21 2023, max compression
+gzip compressed data, was "vallox_websocket_api-3.3.0.tar", last modified: Thu Jul  6 16:32:50 2023, max compression
```

## Comparing `vallox_websocket_api-3.2.1.tar` & `vallox_websocket_api-3.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:19:21.174334 vallox_websocket_api-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-04-06 20:19:21.174334 vallox_websocket_api-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32687 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-06 20:19:21.178334 vallox_websocket_api-3.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:19:21.174334 vallox_websocket_api-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_vallox_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_vallox_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_vallox_next_filter_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_vallox_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/tests/test_vallox_temperatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:19:21.174334 vallox_websocket_api-3.2.1/vallox_websocket_api/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71638 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-06 20:19:08.000000 vallox_websocket_api-3.2.1/vallox_websocket_api/vallox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 20:19:21.174334 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-04-06 20:19:21.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-06 20:19:21.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 20:19:21.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-06 20:19:21.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-06 20:19:21.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 20:19:20.000000 vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:50.837653 vallox_websocket_api-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-07-06 16:32:50.837653 vallox_websocket_api-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32687 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-06 16:32:50.841653 vallox_websocket_api-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:50.837653 vallox_websocket_api-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_vallox_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_vallox_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_vallox_next_filter_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_vallox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/tests/test_vallox_temperatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:50.837653 vallox_websocket_api-3.3.0/vallox_websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12515 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71638 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-06 16:32:41.000000 vallox_websocket_api-3.3.0/vallox_websocket_api/vallox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:32:50.837653 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33640 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:32:50.000000 vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/zip-safe
```

### Comparing `vallox_websocket_api-3.2.1/LICENSE.txt` & `vallox_websocket_api-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/PKG-INFO` & `vallox_websocket_api-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallox_websocket_api
-Version: 3.2.1
+Version: 3.3.0
 Summary: Vallox WebSocket API
 Home-page: https://github.com/yozik04/vallox_websocket_api
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/vallox_websocket_api/issues
 Keywords: vallox api
```

### Comparing `vallox_websocket_api-3.2.1/README.md` & `vallox_websocket_api-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/pyproject.toml` & `vallox_websocket_api-3.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/setup.cfg` & `vallox_websocket_api-3.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_fetch_logs.py` & `vallox_websocket_api-3.3.0/tests/test_fetch_logs.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_messages.py` & `vallox_websocket_api-3.3.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_set_temperature.py` & `vallox_websocket_api-3.3.0/tests/test_set_temperature.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_vallox_fan_speed.py` & `vallox_websocket_api-3.3.0/tests/test_vallox_fan_speed.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_vallox_info.py` & `vallox_websocket_api-3.3.0/tests/test_vallox_info.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_vallox_next_filter_change.py` & `vallox_websocket_api-3.3.0/tests/test_vallox_next_filter_change.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_vallox_profile.py` & `vallox_websocket_api-3.3.0/tests/test_vallox_profile.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/tests/test_vallox_temperatures.py` & `vallox_websocket_api-3.3.0/tests/test_vallox_temperatures.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api/__init__.py` & `vallox_websocket_api-3.3.0/vallox_websocket_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "PROFILE_TO_SET_TEMPERATURE_METRIC_MAP",
     "ValloxException",
     "ValloxInvalidInputException",
     "ValloxApiException",
     "ValloxWebsocketException",
 ]
 
-__version__ = "3.2.1"
+__version__ = "3.3.0"
```

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api/client.py` & `vallox_websocket_api-3.3.0/vallox_websocket_api/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from functools import wraps
+import logging
 import re
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union, cast
 
 import websockets
 
 from .constants import vlxDevConstants, vlxOffsetObject
 from .exceptions import (
@@ -16,16 +17,22 @@
     LogReadResponse1,
     LogReadResponse2,
     ReadTableRequest,
     ReadTableResponse,
     WriteMessageRequest,
 )
 
+logger = logging.getLogger("vallox").getChild(__name__)
+
 KPageSize = 65536
 
+WEBSOCKETS_OPEN_TIMEOUT = 1
+WEBSOCKETS_RECV_TIMEOUT = 1
+WEBSOCKET_RETRY_DELAYS = [0.1, 0.2, 0.5, 1]
+
 
 def calculate_offset(aIndex: int) -> int:
     offset = 0
 
     if (aIndex > vlxDevConstants.RANGE_START_g_cyclone_general_info) and (
         aIndex <= vlxDevConstants.RANGE_END_g_cyclone_general_info
     ):
@@ -142,31 +149,52 @@
 def to_kelvin(value: float) -> int:
     return int(round(value * 10) * 10 + 27315)
 
 
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
-def _websocket_exception_handler(request_fn: FuncT) -> FuncT:
+def _websocket_retry_wrapper(request_fn: FuncT) -> FuncT:
+    retry_on_exceptions = (
+        websockets.InvalidHandshake,
+        websockets.InvalidState,
+        websockets.WebSocketProtocolError,
+        websockets.ConnectionClosed,
+        OSError,
+        asyncio.TimeoutError,
+    )
+
     @wraps(request_fn)
     async def wrapped(*args: Any, **kwargs: Any) -> Any:
         try:
-            return await request_fn(*args, **kwargs)
+            delays = WEBSOCKET_RETRY_DELAYS.copy()
+            while len(delays) >= 0:
+                try:
+                    return await request_fn(*args, **kwargs)
+                except Exception as e:
+                    if isinstance(e, retry_on_exceptions) and len(delays) > 0:
+                        await asyncio.sleep(delays.pop(0))
+                    else:
+                        raise e
         except websockets.InvalidHandshake as e:
             raise ValloxWebsocketException("Websocket handshake failed") from e
         except websockets.InvalidURI as e:
             raise ValloxWebsocketException("Websocket invalid URI") from e
         except websockets.PayloadTooBig as e:
             raise ValloxWebsocketException("Websocket payload too big") from e
         except websockets.InvalidState as e:
             raise ValloxWebsocketException("Websocket invalid state") from e
         except websockets.WebSocketProtocolError as e:
             raise ValloxWebsocketException("Websocket protocol error") from e
+        except websockets.ConnectionClosed as e:
+            raise ValloxWebsocketException("Websocket connection closed") from e
         except OSError as e:
             raise ValloxWebsocketException("Websocket connection failed") from e
+        except asyncio.TimeoutError as e:
+            raise ValloxWebsocketException("Websocket connection timed out") from e
 
     return cast(FuncT, wrapped)
 
 
 class Client:
     SETTABLE_INT_VALS = {
         re.compile("^A_CYC_MODE$"),
@@ -228,28 +256,34 @@
 
         assert (
             type(raw_value) == required_type
         ), f"{key}({address}) key needs to be an {required_type.__name__}, but {type(raw_value).__name__} passed"
 
         return address, raw_value
 
-    @_websocket_exception_handler
     async def _websocket_request(self, payload: bytes) -> bytes:
-        async with websockets.connect(f"ws://{self.ip_address}/") as ws:
-            await ws.send(payload)
-            r: bytes = await ws.recv()
-            return r
+        return (await self._websocket_request_multiple(payload, 1))[0]
 
-    @_websocket_exception_handler
+    @_websocket_retry_wrapper
     async def _websocket_request_multiple(
         self, payload: bytes, read_packets: int
     ) -> List[bytes]:
-        async with websockets.connect(f"ws://{self.ip_address}/") as ws:
+        async with websockets.connect(
+            f"ws://{self.ip_address}/",
+            open_timeout=WEBSOCKETS_OPEN_TIMEOUT,
+            logger=logger,
+        ) as ws:
             await ws.send(payload)
-            return await asyncio.gather(*[ws.recv() for _ in range(0, read_packets)])
+
+            async def _get_responses() -> List[bytes]:
+                return [await ws.recv() for _ in range(0, read_packets)]
+
+            return await asyncio.wait_for(
+                _get_responses(), timeout=WEBSOCKETS_RECV_TIMEOUT * read_packets
+            )
 
     async def fetch_metrics(
         self, metric_keys: Optional[List[str]] = None
     ) -> MetricDict:
         metrics = {}
         payload = ReadTableRequest.build({})
         result = await self._websocket_request(payload)
```

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api/constants.py` & `vallox_websocket_api-3.3.0/vallox_websocket_api/constants.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api/messages.py` & `vallox_websocket_api-3.3.0/vallox_websocket_api/messages.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api/vallox.py` & `vallox_websocket_api-3.3.0/vallox_websocket_api/vallox.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/PKG-INFO` & `vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallox-websocket-api
-Version: 3.2.1
+Version: 3.3.0
 Summary: Vallox WebSocket API
 Home-page: https://github.com/yozik04/vallox_websocket_api
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/vallox_websocket_api/issues
 Keywords: vallox api
```

### Comparing `vallox_websocket_api-3.2.1/vallox_websocket_api.egg-info/SOURCES.txt` & `vallox_websocket_api-3.3.0/vallox_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

