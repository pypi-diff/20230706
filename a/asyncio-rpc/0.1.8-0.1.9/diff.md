# Comparing `tmp/asyncio_rpc-0.1.8.tar.gz` & `tmp/asyncio_rpc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncio_rpc-0.1.8.tar", last modified: Fri Feb  5 09:15:29 2021, max compression
+gzip compressed data, was "dist/asyncio_rpc-0.1.9.tar", last modified: Mon Feb 22 07:39:21 2021, max compression
```

## Comparing `asyncio_rpc-0.1.8.tar` & `asyncio_rpc-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/
--rw-r--r--   0 jprins    (1000) jprins    (1000)      237 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/AUTHORS.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)     3441 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/CONTRIBUTING.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1149 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/HISTORY.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1509 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/LICENSE
--rw-r--r--   0 jprins    (1000) jprins    (1000)      262 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/MANIFEST.in
--rw-r--r--   0 jprins    (1000) jprins    (1000)     3785 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/PKG-INFO
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1133 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/README.rst
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/
--rw-r--r--   0 jprins    (1000) jprins    (1000)       22 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/__init__.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     9032 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/client.py
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/commlayers/
--rw-r--r--   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/commlayers/__init__.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1111 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/commlayers/base.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     6009 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/commlayers/redis.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)      525 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/exceptions.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     2700 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/models.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     2810 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/pubsub.py
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/serialization/
--rw-r--r--   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/serialization/__init__.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     6991 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/serialization/msgpack.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     8626 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc/server.py
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/
--rw-r--r--   0 jprins    (1000) jprins    (1000)     3785 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/PKG-INFO
--rw-r--r--   0 jprins    (1000) jprins    (1000)      833 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 jprins    (1000) jprins    (1000)        1 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 jprins    (1000) jprins    (1000)        1 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/not-zip-safe
--rw-r--r--   0 jprins    (1000) jprins    (1000)       54 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/requires.txt
--rw-r--r--   0 jprins    (1000) jprins    (1000)       12 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/asyncio_rpc.egg-info/top_level.txt
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/docs/
--rw-r--r--   0 jprins    (1000) jprins    (1000)      247 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/docs/index.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1064 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/docs/installation.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)       27 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/docs/readme.rst
--rw-r--r--   0 jprins    (1000) jprins    (1000)      481 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/setup.cfg
--rw-r--r--   0 jprins    (1000) jprins    (1000)     2068 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/setup.py
-drwxr-xr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/
--rw-r--r--   0 jprins    (1000) jprins    (1000)        0 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/__init__.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     2803 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/test_msgpack_serialization.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     2095 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/test_pubsub.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     1030 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/test_rpc_client.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)      980 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/test_rpc_server.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     4789 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/test_simple_rpc_calls.py
--rw-r--r--   0 jprins    (1000) jprins    (1000)     4428 2021-02-05 09:15:29.000000 asyncio_rpc-0.1.8/tests/utils.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      237 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/AUTHORS.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     3441 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/CONTRIBUTING.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1347 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/HISTORY.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1509 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/LICENSE
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      262 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/MANIFEST.in
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4047 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/PKG-INFO
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1133 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/README.rst
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       22 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    10815 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/client.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/commlayers/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/commlayers/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1111 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/commlayers/base.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     6009 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/commlayers/redis.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      525 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/exceptions.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2700 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/models.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2810 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/pubsub.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/serialization/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/serialization/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     6991 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/serialization/msgpack.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)    10214 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc/server.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4047 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/PKG-INFO
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      833 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        1 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/not-zip-safe
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       54 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/requires.txt
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       12 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/asyncio_rpc.egg-info/top_level.txt
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/docs/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      247 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/docs/index.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1064 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/docs/installation.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)       27 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/docs/readme.rst
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      481 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/setup.cfg
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2068 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/setup.py
+drwxrwxr-x   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)        0 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/__init__.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2803 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/test_msgpack_serialization.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     2095 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/test_pubsub.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     1030 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/test_rpc_client.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)      980 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/test_rpc_server.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4789 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/test_simple_rpc_calls.py
+-rw-rw-r--   0 jprins    (1000) jprins    (1000)     4428 2021-02-22 07:39:21.000000 asyncio_rpc-0.1.9/tests/utils.py
```

### Comparing `asyncio_rpc-0.1.8/CONTRIBUTING.rst` & `asyncio_rpc-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/HISTORY.rst` & `asyncio_rpc-0.1.9/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.1.9 (2021-02-22)
+------------------
+
+- Bugfix: asyncio future that waits for return RPC message needs
+  to be created before sending RPC message to RPC server.
+
+- Added debug logging statements.
+
 0.1.8 (2021-02-05)
 ------------------
 
 - Add numpy int32 and int64 serializer.
 
 
 0.1.7 (2020-01-10)
```

### Comparing `asyncio_rpc-0.1.8/LICENSE` & `asyncio_rpc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/PKG-INFO` & `asyncio_rpc-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asyncio_rpc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asyncio RPC client/server with redis/msgpack/dataclasses
 Home-page: https://github.com/nens/asyncio_rpc
 Author: Jelle Prins
 Author-email: jelle.prins@nelen-schuurmans.nl
 License: BSD license
 Description: Asyncio-rpc: Remote procedure calling framework
         ===============================================
@@ -49,14 +49,22 @@
         
         
         Testing
         -------
             >>> docker-compose run pytest --cov=asyncio_rpc --cov-report=html
         
         
+        0.1.9 (2021-02-22)
+        ------------------
+        
+        - Bugfix: asyncio future that waits for return RPC message needs
+          to be created before sending RPC message to RPC server.
+        
+        - Added debug logging statements.
+        
         0.1.8 (2021-02-05)
         ------------------
         
         - Add numpy int32 and int64 serializer.
         
         
         0.1.7 (2020-01-10)
```

### Comparing `asyncio_rpc-0.1.8/README.rst` & `asyncio_rpc-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/client.py` & `asyncio_rpc-0.1.9/asyncio_rpc/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         assert isinstance(rpc_commlayer, AbstractRPCCommLayer)
         self.rpc_commlayer = rpc_commlayer
         self.futures = {}
         self.queue = asyncio.Queue()
         self.processing = False
         self.on_rpc_message = None
         self.subscriptions = {}
+        logger.debug("Initialized RPC client")
 
     def register_models(self, models: List):
         """
         Register all given models to the rpc_commlayer serialization
 
         Intended usage is to register dataclasses
         """
@@ -42,23 +43,25 @@
 
     async def _wait_for_result(
             self, uid: bytes) -> Union[RPCResult, RPCException]:
         """
         Internal helper function for stopping the rpc_commlayer subscription
         upon receiving a result from the RPC_server
         """
+        logger.debug("Start waiting for result with uid: %s", uid)
         result = None
         while True:
             event, channel = await self.queue.get()
 
             assert isinstance(event, RPCResult) or\
                 isinstance(event, RPCException)
 
             # Discard everything that we don't need...
             if event.uid == uid:
+                logger.debug("Received result for uid: %s, %s", uid, event)
                 result = event
                 break
 
         # Stop subscription, automatically stops
         # queue processing as well
         await self.rpc_commlayer.unsubscribe()
 
@@ -104,52 +107,79 @@
         the default publish channel
         """
         assert isinstance(rpc_func_stack, RPCStack)
 
         # Make sure to be subscribed before publishing
         await self.rpc_commlayer.do_subscribe()
 
+        # Always create a future before sending the rpc_func_stack
+        # else the result can come back before the future is created
+        future = asyncio.get_event_loop().create_future()
+        self.futures[rpc_func_stack.uid] = future
+        logger.debug(
+            "Added future for rpc_func_stack: %s", rpc_func_stack.uid)
+
         # Publish RPCStack to RPCServer
         count = await self.rpc_commlayer.publish(
             rpc_func_stack, channel=channel)
 
+        logger.debug(
+            "RPC call rpc_func_stack: %s, %s (received=%s, channel=%s)",
+            rpc_func_stack.uid, rpc_func_stack, count, channel
+        )
+
         if count == 0:
+            self.futures.pop(rpc_func_stack.uid)
+            future.set_result(None)
             raise NotReceived(
                 f"rpc_call was not received "
                 f"by any subscriber {rpc_func_stack}")
 
         if self.processing:
             # client.serve() has been awaited, so
             # background processing is taken care of.
 
             # Create a future that should be resolved within
             # the given timeout. The background processing initialized
             # by client.serve() resolves the future when a result
             # is returned.
-            future = asyncio.get_event_loop().create_future()
-            self.futures[rpc_func_stack.uid] = future
             try:
                 result = await asyncio.wait_for(
                     future, timeout=rpc_func_stack.timeout)
+                logger.debug(
+                    "Retrieved result for rpc_func_stack %s, %s",
+                    rpc_func_stack.uid, result)
             except asyncio.TimeoutError:
+                logger.debug(
+                    "TimeoutError rpc_func_stack: %s", rpc_func_stack.uid)
                 raise RPCTimeoutError(f"rpc_func_stack: {rpc_func_stack}")
         else:
             # No background processing, so start the subscription
             # and wait for result via asyncio.gather
             # _wait_for_result is a helper function to unsubscribe
             # on a result.
+
+            # Don't need future here anymore
+            self.futures.pop(rpc_func_stack.uid)
+            future.set_result(None)
             try:
                 _, result = await asyncio.gather(
                     self.rpc_commlayer.subscribe(self._on_rpc_event),
                     self._wait_for_result(rpc_func_stack.uid)
                 )
+                logger.debug(
+                    "Retrieved result for rpc_func_stack %s, %s",
+                    rpc_func_stack.uid, result)
             except asyncio.TimeoutError:
+                logger.debug(
+                    "TimeoutError rpc_func_stack: %s", rpc_func_stack.uid)
                 raise RPCTimeoutError(f"rpc_func_stack: {rpc_func_stack}")
 
         if isinstance(result, RPCException):
+            logger.debug("RPC exception %s, %s", rpc_func_stack.uid, result)
             # Try to resolve builtin errors
             try:
                 exception_class = getattr(builtins, result.classname)
             except AttributeError:
                 # Default to WrappedException if
                 # returned exception is not a builtin error
                 exception_class = WrappedException
@@ -160,14 +190,15 @@
 
     async def _on_rpc_event(
             self, rpc_instance: RPCBase, channel: bytes = None):
         """
         Callback function sent to rpc_commlayer, is called
         when a message is received by the subscription.
         """
+        logger.debug("New RPC event %s", rpc_instance)
         assert isinstance(rpc_instance, RPCBase)
         # Put everything in a queue and process
         # it afterwards
         await self.queue.put((rpc_instance, channel))
 
     async def _process_queue(self, on_rpc_message: callable = None):
         """
@@ -190,29 +221,35 @@
             # 1) RPCResult or RPCException as a result from the RPCServer
             # 3) RPCMessage as a message from the RPCServer
             assert isinstance(event, RPCResult) or\
                 isinstance(event, RPCException) or\
                 isinstance(event, RPCMessage)
 
             if isinstance(event, RPCResult) or isinstance(event, RPCException):
+                logger.debug(
+                    "Received new queue item %s, %s", event.uid, event)
                 if event.uid in self.futures:
+                    logger.debug("Found event in futures %s", event.uid)
                     # A future is created & awaited in self.rpc_call
                     # resolve this future to proceed in the rpc_call function
                     # and return a result
                     future = self.futures.pop(event.uid)
                     if future is not None:
                         future.set_result(event)
                 elif event.uid in self.subscriptions:
+                    logger.debug("Found event in subscriptions %s", event.uid)
                     subscription = self.subscriptions[event.uid]
                     await subscription.enqueue(event)
                 else:
                     # FUTURE NOT FOUND FOR EVENT
-                    # TODO: how to handle this??
-                    pass  # pragma: nocover
+                    logger.exception(
+                        "Future not found for %s, %s", event.uid, event)
             elif isinstance(event, RPCMessage) and on_rpc_message:
+                logger.debug(
+                    "RPCMessage received: %s", event)
                 await on_rpc_message(event, channel)
 
         self.processing = False
 
     async def serve(self, on_rpc_message=None):
         """
         Start RPCClient background processing, blocks
```

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/commlayers/base.py` & `asyncio_rpc-0.1.9/asyncio_rpc/commlayers/base.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/commlayers/redis.py` & `asyncio_rpc-0.1.9/asyncio_rpc/commlayers/redis.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/exceptions.py` & `asyncio_rpc-0.1.9/asyncio_rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/models.py` & `asyncio_rpc-0.1.9/asyncio_rpc/models.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/pubsub.py` & `asyncio_rpc-0.1.9/asyncio_rpc/pubsub.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/serialization/msgpack.py` & `asyncio_rpc-0.1.9/asyncio_rpc/serialization/msgpack.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc/server.py` & `asyncio_rpc-0.1.9/asyncio_rpc/server.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self._alive = True
 
         # Allow multiple executors to be registered by
         # namespace
         self.registry = {}
         self.publishers = {}
         self.rpc_commlayer = rpc_commlayer
+        logger.debug("Initialized RPCServer")
 
     def register_models(self, models):
         """
         Register all given models to the rpc_commlayer serialization
 
         Intended usage is to register dataclasses
         """
@@ -58,39 +59,57 @@
 
     async def rpc_call(self, rpc_func_stack: RPCStack):
         """
         Incoming rpc_call, execute it via the registered
         executor and return the result or exception
         """
         assert isinstance(rpc_func_stack, RPCStack)
+        logger.debug(
+            "Received RPC call rpc_func_stack %s, %s",
+            rpc_func_stack.uid, rpc_func_stack)
 
         # Create a default result
         result = RPCResult(
             uid=rpc_func_stack.uid,
             namespace=rpc_func_stack.namespace,
             data=None)
 
         if rpc_func_stack.namespace not in self.registry:
+            logger.debug(
+                "Unknown namespace for rpc_func_stack: %s", rpc_func_stack.uid
+            )
             raise NamespaceError("Unknown namespace")
 
         executor = self.registry[rpc_func_stack.namespace]
 
         try:
             # Wait for result from executor
+            logger.debug(
+                "Going to run executor for rpc_func_stack: %s",
+                rpc_func_stack.uid
+            )
             result.data = await asyncio.wait_for(
                 executor.rpc_call(rpc_func_stack.stack),
                 timeout=rpc_func_stack.timeout)
+            logger.debug(
+                "Got result for rpc_func_stack: %s, %s",
+                rpc_func_stack.uid, result
+            )
         except Exception as e:
             # For now catch all exceptions here...
             # TODO: debug mode with stacktrace
             result = RPCException(
                 uid=rpc_func_stack.uid,
                 namespace=rpc_func_stack.namespace,
                 classname=e.__class__.__name__,
                 exc_args=e.args)
+            logger.debug(
+                "Exception occurred for rpc_funct_stack: %s, %s",
+                rpc_func_stack.uid, e
+            )
 
         return result
 
     async def subscribe_call(self, rpc_sub_stack: RPCSubStack):
         assert isinstance(rpc_sub_stack, RPCSubStack)
         if rpc_sub_stack.namespace not in self.registry:
             raise NamespaceError("Unknown namespace")
@@ -132,19 +151,28 @@
             if item == b'END':
                 break
 
             rpc_func_stack, channel = item
 
             assert isinstance(rpc_func_stack, RPCStack)
 
+            logger.debug(
+                "Processing rpcstack %s, %s",
+                rpc_func_stack.uid, rpc_func_stack
+            )
+
             if isinstance(rpc_func_stack, RPCSubStack):
                 try:
                     # Process rpc_func_call_stack
                     await self.subscribe_call(rpc_func_stack)
                 except Exception as e:
+                    # Log everything that is not an
+                    # instance of RPCException
+                    if not isinstance(e, RPCException):
+                        logger.exception(e)
                     result = RPCException(
                         uid=rpc_func_stack.uid,
                         namespace=rpc_func_stack.namespace,
                         classname=e.__class__.__name__,
                         exc_args=e.args)
                     # Publish exception
                     await self.rpc_commlayer.publish(
@@ -153,19 +181,30 @@
                 publisher = self.publishers.pop(rpc_func_stack.uid, None)
                 if publisher is not None:
                     publisher.set_is_active(False)
             else:
                 try:
                     # Process rpc_func_call_stack
                     result = await self.rpc_call(rpc_func_stack)
+
+                    logger.debug(
+                        "Publishing result for %s, %s",
+                        rpc_func_stack.uid, rpc_func_stack)
                     # Publish result of rpc call
                     await self.rpc_commlayer.publish(
                         result, channel=rpc_func_stack.respond_to)
-
+                    logger.debug("Publishing done for %s", rpc_func_stack.uid)
                 except Exception as e:
+                    logger.debug(
+                        "Error occured for %s: %s", rpc_func_stack.uid, e)
+                    # Log everything that is not an
+                    # instance of RPCException
+                    if not isinstance(e, RPCException):
+                        logger.exception(e)
+
                     result = RPCException(
                         uid=rpc_func_stack.uid,
                         namespace=rpc_func_stack.namespace,
                         classname=e.__class__.__name__,
                         exc_args=e.args)
                     # Try to publish error
                     await self.rpc_commlayer.publish(
```

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc.egg-info/PKG-INFO` & `asyncio_rpc-0.1.9/asyncio_rpc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: asyncio-rpc
-Version: 0.1.8
+Version: 0.1.9
 Summary: Asyncio RPC client/server with redis/msgpack/dataclasses
 Home-page: https://github.com/nens/asyncio_rpc
 Author: Jelle Prins
 Author-email: jelle.prins@nelen-schuurmans.nl
 License: BSD license
 Description: Asyncio-rpc: Remote procedure calling framework
         ===============================================
@@ -49,14 +49,22 @@
         
         
         Testing
         -------
             >>> docker-compose run pytest --cov=asyncio_rpc --cov-report=html
         
         
+        0.1.9 (2021-02-22)
+        ------------------
+        
+        - Bugfix: asyncio future that waits for return RPC message needs
+          to be created before sending RPC message to RPC server.
+        
+        - Added debug logging statements.
+        
         0.1.8 (2021-02-05)
         ------------------
         
         - Add numpy int32 and int64 serializer.
         
         
         0.1.7 (2020-01-10)
```

### Comparing `asyncio_rpc-0.1.8/asyncio_rpc.egg-info/SOURCES.txt` & `asyncio_rpc-0.1.9/asyncio_rpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/docs/installation.rst` & `asyncio_rpc-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/setup.py` & `asyncio_rpc-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/test_msgpack_serialization.py` & `asyncio_rpc-0.1.9/tests/test_msgpack_serialization.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/test_pubsub.py` & `asyncio_rpc-0.1.9/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/test_rpc_client.py` & `asyncio_rpc-0.1.9/tests/test_rpc_client.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/test_rpc_server.py` & `asyncio_rpc-0.1.9/tests/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/test_simple_rpc_calls.py` & `asyncio_rpc-0.1.9/tests/test_simple_rpc_calls.py`

 * *Files identical despite different names*

### Comparing `asyncio_rpc-0.1.8/tests/utils.py` & `asyncio_rpc-0.1.9/tests/utils.py`

 * *Files identical despite different names*

