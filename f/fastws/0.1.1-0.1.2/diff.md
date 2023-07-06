# Comparing `tmp/fastws-0.1.1.tar.gz` & `tmp/fastws-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastws-0.1.1.tar", max compression
+gzip compressed data, was "fastws-0.1.2.tar", max compression
```

## Comparing `fastws-0.1.1.tar` & `fastws-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1077 2023-07-05 18:41:04.114466 fastws-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-07-05 18:40:12.634470 fastws-0.1.1/README.md
--rw-r--r--   0        0        0      437 2023-07-06 16:36:48.210465 fastws-0.1.1/fastws/__init__.py
--rw-r--r--   0        0        0     6735 2023-07-06 16:33:42.550498 fastws-0.1.1/fastws/application.py
--rw-r--r--   0        0        0     1552 2023-07-06 16:34:25.530483 fastws-0.1.1/fastws/asyncapi.py
--rw-r--r--   0        0        0     4346 2023-07-06 16:34:17.230486 fastws-0.1.1/fastws/broker.py
--rw-r--r--   0        0        0     6172 2023-07-06 16:34:24.460484 fastws-0.1.1/fastws/docs.py
--rw-r--r--   0        0        0     6183 2023-07-06 16:02:50.890824 fastws-0.1.1/fastws/routing.py
--rw-r--r--   0        0        0      568 2023-07-06 16:36:41.650466 fastws-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 fastws-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-05 18:41:04.114466 fastws-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9804 2023-07-06 20:45:27.237817 fastws-0.1.2/README.md
+-rw-r--r--   0        0        0      437 2023-07-06 19:26:33.618656 fastws-0.1.2/fastws/__init__.py
+-rw-r--r--   0        0        0     6903 2023-07-06 20:45:38.807815 fastws-0.1.2/fastws/application.py
+-rw-r--r--   0        0        0     1552 2023-07-06 16:34:25.530483 fastws-0.1.2/fastws/asyncapi.py
+-rw-r--r--   0        0        0     4346 2023-07-06 16:34:17.230486 fastws-0.1.2/fastws/broker.py
+-rw-r--r--   0        0        0     6172 2023-07-06 16:34:24.460484 fastws-0.1.2/fastws/docs.py
+-rw-r--r--   0        0        0     6183 2023-07-06 19:26:36.358655 fastws-0.1.2/fastws/routing.py
+-rw-r--r--   0        0        0     1231 2023-07-06 19:25:55.688662 fastws-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10922 1970-01-01 00:00:00.000000 fastws-0.1.2/PKG-INFO
```

### Comparing `fastws-0.1.1/LICENSE` & `fastws-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastws-0.1.1/fastws/application.py` & `fastws-0.1.2/fastws/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import logging
 from typing import AsyncGenerator, AsyncIterator, Callable, Awaitable
 from uuid import uuid4
 from fastapi import Request, WebSocketException, status, FastAPI
-from fastapi.responses import HTMLResponse
+from fastapi.responses import HTMLResponse, JSONResponse
 from pydantic import BaseModel, ValidationError
 from starlette.websockets import WebSocket
 
 from fastws.routing import Message, NoMatchingOperation
 from fastws.broker import Broker
 from fastws.docs import get_asyncapi_html
 
@@ -45,16 +45,16 @@
         terms_of_service: str | None = None,
         contact: dict[str, str] | None = None,
         license_info: dict[str, str] | None = None,
         servers: dict | None = None,
         asyncapi_url: str | None = "/asyncapi.json",
         asyncapi_docs_url: str | None = "/asyncapi",
         debug: bool = False,
-        heartbeat_interval: int | None = 10,
-        max_connection_lifespan: int | None = None,
+        heartbeat_interval: float | None = None,
+        max_connection_lifespan: float | None = None,
         auth_handler: Callable[[WebSocket], Awaitable[bool]] | None = None,
         auto_ws_accept: bool = True,
     ) -> None:
         super().__init__(
             title=title,
             version=version,
             asyncapi_version=asyncapi_version,
@@ -95,15 +95,14 @@
         return await self.auth_handler(ws)
 
     async def manage(self, ws: WebSocket) -> AsyncGenerator[Client, None]:
         if not await self._auth(ws):
             return
         client = Client(ws)
         self._connect(client)
-        await client.send(client.uid)
         try:
             yield client
         except Exception:
             self.log("unknown disconnect")
         finally:
             self._disconnect(client)
 
@@ -133,51 +132,55 @@
             error.add_note(
                 "Connection timed out. "
                 + f"Heartbeat interval {self.heartbeat_interval or 'unset'}. "
                 + f"Max connection lifespan {self.max_connection_lifespan or 'unset'}"
             )
         raise exc
 
-    async def client(self, client: Client):
+    async def serve(self, client: Client):
         try:
             async with asyncio.timeout(
                 self.heartbeat_interval
             ) as heartbeat_cm, asyncio.timeout(
                 self.max_connection_lifespan,
             ):
                 async for message in client:
-                    await self.client_send(message, client=client)
                     if self.heartbeat_interval is not None:
                         heartbeat_cm.reschedule(
                             asyncio.get_running_loop().time() + self.heartbeat_interval
                         )
+                    await self.client_send(message, client=client)
         except (ValueError, ValidationError, NoMatchingOperation, TimeoutError) as exc:
             await self.handle_exception(exc)
 
     async def client_send(self, message: Message, *, client: Client):
         if (
-            reply := await self(message, method="SEND", client=client, manager=self)
+            reply := await self(message, method="SEND", client=client, app=self)
         ) is not None:
             await client.send(reply.model_dump_json())
 
-    async def server_send(self, message: Message, *, topic: str):
-        if (reply := await self(message, method="RECEIVE", manager=self)) is None:
+    async def server_send(self, message: Message, *, topic: str, **params):
+        if (reply := await self(message, method="RECEIVE", app=self, **params)) is None:
             return
         await self.broadcast(topic, reply)
 
     def setup(self, app: FastAPI) -> None:
         if self.asyncapi_url and self.asyncapi_docs_url:
-            self.asyncapi_url
 
             async def asyncapi_ui_html(req: Request) -> HTMLResponse:
                 root_path = req.scope.get("root_path", "").rstrip("/")
                 asyncapi_url = f"{root_path}{self.asyncapi_url}"
                 return HTMLResponse(
                     get_asyncapi_html(
                         title=f"{self.title} - AsyncAPI UI",
                         asyncapi_url=asyncapi_url,
                     )
                 )
 
             app.add_route(
                 self.asyncapi_docs_url, asyncapi_ui_html, include_in_schema=False
             )
+
+            async def asyncapi_json(_: Request) -> JSONResponse:
+                return JSONResponse(self.asyncapi())
+
+            app.add_route(self.asyncapi_url, asyncapi_json, include_in_schema=False)
```

### Comparing `fastws-0.1.1/fastws/asyncapi.py` & `fastws-0.1.2/fastws/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.1/fastws/broker.py` & `fastws-0.1.2/fastws/broker.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.1/fastws/docs.py` & `fastws-0.1.2/fastws/docs.py`

 * *Files identical despite different names*

### Comparing `fastws-0.1.1/fastws/routing.py` & `fastws-0.1.2/fastws/routing.py`

 * *Files identical despite different names*

