# Comparing `tmp/misskey_python-1.1.tar.gz` & `tmp/misskey_python-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misskey_python-1.1.tar", max compression
+gzip compressed data, was "misskey_python-1.2.tar", max compression
```

## Comparing `misskey_python-1.1.tar` & `misskey_python-1.2.tar`

### file list

```diff
@@ -1,9 +1,17 @@
--rw-r--r--   0        0        0     1086 2023-06-15 06:34:58.016922 misskey_python-1.1/LICENSE
--rw-r--r--   0        0        0      133 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/__init__.py
--rw-r--r--   0        0        0      183 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/exceptions.py
--rw-r--r--   0        0        0     1300 2023-06-15 06:34:58.018447 misskey_python-1.1/MiPC/http.py
--rw-r--r--   0        0        0     1303 2023-06-15 06:34:58.017435 misskey_python-1.1/MiPC/MiAuth/__main__.py
--rw-r--r--   0        0        0    11502 2023-06-15 06:34:58.017435 misskey_python-1.1/MiPC/Misskey.py
--rw-r--r--   0        0        0      495 2023-06-15 06:34:58.025449 misskey_python-1.1/pyproject.toml
--rw-r--r--   0        0        0      634 2023-06-15 06:34:58.019447 misskey_python-1.1/README.md
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 misskey_python-1.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-06-28 08:45:04.592522 misskey_python-1.2/MiPC/__init__.py
+-rw-r--r--   0        0        0      273 2023-06-11 18:10:32.427114 misskey_python-1.2/MiPC/exceptions.py
+-rw-r--r--   0        0        0       26 2023-06-21 21:48:36.983223 misskey_python-1.2/MiPC/ext/__init__.py
+-rw-r--r--   0        0        0      198 2023-06-23 11:30:55.851342 misskey_python-1.2/MiPC/ext/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2664 2023-06-28 10:21:24.632093 misskey_python-1.2/MiPC/ext/__pycache__/MiAuth.cpython-311.pyc
+-rw-r--r--   0        0        0     1717 2023-06-28 10:21:19.794646 misskey_python-1.2/MiPC/ext/MiAuth.py
+-rw-r--r--   0        0        0       20 2023-06-21 21:48:58.869081 misskey_python-1.2/MiPC/ext/Streaming/__init__.py
+-rw-r--r--   0        0        0      205 2023-06-23 11:30:55.854885 misskey_python-1.2/MiPC/ext/Streaming/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12750 2023-06-23 11:30:55.859066 misskey_python-1.2/MiPC/ext/Streaming/__pycache__/Bot.cpython-311.pyc
+-rw-r--r--   0        0        0     8691 2023-06-21 21:48:46.902141 misskey_python-1.2/MiPC/ext/Streaming/Bot.py
+-rw-r--r--   0        0        0     2470 2023-06-28 08:44:03.408701 misskey_python-1.2/MiPC/mihttp.py
+-rw-r--r--   0        0        0     9371 2023-06-21 21:40:32.990728 misskey_python-1.2/MiPC/Misskey.py
+-rw-r--r--   0        0        0     9182 2023-06-28 08:44:52.702757 misskey_python-1.2/MiPC/Sync.py
+-rw-r--r--   0        0        0      498 2023-06-14 21:55:10.887744 misskey_python-1.2/MiPC/新規 Python File.py
+-rw-r--r--   0        0        0      516 2023-07-06 12:50:11.289632 misskey_python-1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-03 18:57:26.461287 misskey_python-1.2/README.md
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 misskey_python-1.2/PKG-INFO
```

### Comparing `misskey_python-1.1/MiPC/http.py` & `misskey_python-1.2/MiPC/mihttp.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,7 +29,39 @@
                     if response.status_code >= 400:
                         raise MisskeyAPIException(response.json())
 
                     if response.status_code == 204:
                         return True
                     else:
                         return response.json()
+
+class sync_mihttp:
+    
+    def __init__(self, base_url):
+        self.__base = base_url
+    
+    def request(
+        self, endpoint, data, file=None
+    ):
+        head = {
+            "Content-Type": "application/json"
+        }
+        if file is not None:
+            with httpx.Client(base_url=self.__base) as client:
+                with client.post(endpoint, json=data, headers=head, files=file) as response:
+                    if response.status_code >= 400:
+                        raise MisskeyAPIException(response.json())
+
+                    if response.status_code == 204:
+                        return True
+                    else:
+                        return response.json()
+        else:
+            with httpx.Client(base_url=self.__base) as client:
+                with client.post(endpoint, json=data, headers=head) as response:
+                    if response.status_code >= 400:
+                        raise MisskeyAPIException(response.json())
+
+                    if response.status_code == 204:
+                        return True
+                    else:
+                        return response.json()
```

### Comparing `misskey_python-1.1/MiPC/MiAuth/__main__.py` & `misskey_python-1.2/MiPC/ext/MiAuth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import uuid
 import asyncio
 import json
+import warnings
+import re
 
 import httpx
 
 from MiPC.exceptions import MisskeyMiAuthFailedException
 
 class MiAuth:
 
-    def __init__(self, server="misskey.io", name="MiPC App"):
-        self.server = server
+    def __init__(
+        self, 
+        server="misskey.io", 
+        name="MiPC Application"
+    ):
+        self.__pattern = "http?://[\w/:%#\$&\?\(\)~\.=\+\-]+"
+        self.__pattern_ws = "^ws:\/\/.*"
+        if re.match(self.__pattern_ws, server):
+            raise TypeError("Websocket procotr is not available within the Misskey class.")
+        if re.match(self.__pattern, server):
+            self.server = server
+        else:
+            self.server = "https://" + server
         self.name = name
     
-    def generate_url(
+    def generate(
             self, 
             permission=["read:account", "write:account", "read:blocks", "write:blocks", "read:drive", "write:drive", "read:favorites", "write:favorites", "read:following", "write:following", "read:messaging", "write:messaging", "read:mutes", "write:mutes", "write:notes", "read:notifications", "write:notifications", "write:reactions", "write:votes", "read:pages", "write:pages", "write:page-likes", "read:page-likes", "write:gallery-likes", "read:gallery-likes"]
     ):
         self.session_id = uuid.uuid4()
         url = f"{self.server}/miauth/{self.session_id}?name={self.name}&permission={','.join(permission)}"
         return url
     
-    def get_token(
+    def token(
             self
     ):
         url = f"{self.server}/api/miauth/{self.session_id}/check"
         response = httpx.post(url)
         response_json = response.json()
         if response_json["ok"]:
             return response_json["token"]
         else:
-            raise MisskeyMiAuthFailedException("ログイン失敗")
+            raise MisskeyMiAuthFailedException(response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `misskey_python-1.1/MiPC/Misskey.py` & `misskey_python-1.2/MiPC/Misskey.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 import websockets
 import aiofiles
 from colorama import Fore, Back, Style
 from websockets import connect, exceptions
 import orjson
 
 from MiPC.exceptions import MisskeyMiAuthFailedException, MisskeyAPIException
-from MiPC import mihttp
+import MiPC
+
+Arry = list
 
 class user:
     pass
 
 class Misskey:
     
     def __init__(
@@ -40,15 +42,15 @@
         if re.match(self.__pattern_ws, server):
             raise TypeError("Websocket procotr is not available within the Misskey class.")
         if re.match(self.__pattern, server):
             self.__server = server
         else:
             self.__server = "https://" + server
         self.__token = token
-        self.http = mihttp(server)
+        self.http = MiPC.mihttp(server)
 
     async def meta(
         self):
         class metadata:
             pass
         params = {
             "i" : self.__token,
@@ -96,15 +98,31 @@
         self,
         file_id: str
     ):
         return self.http.request('drive/files/delete', data={
             "fileId": file_id
         })
 
-    async def send(self, text, visibility="public", visibleUserIds: list=None, replyid=None, fileid=None, channelId=None, localOnly=False):
+    async def update(
+        self, 
+        dct: dict
+    ):
+        dct["i"] = self.__token
+        return self.http.request('i/update', data=dct)
+
+    async def send(
+        self, 
+        text, 
+        visibility="public", 
+        visibleUserIds: list=None, 
+        replyid=None, 
+        fileid=None, 
+        channelId=None, 
+        localOnly=False
+    ):
         url = f"{self.__server}/api/notes/create"
         if replyid is not None:
             if fileid is not None:
                 params = {
                     "i" : self.__token,
                     "replyId": replyid,
                     "fileIds": fileid,
@@ -235,73 +253,27 @@
                 async with httpx.AsyncClient() as client:
                     r = await client.post(
                         url=url, 
                         json=params,
                         headers=head
                     )
                     return r.json()
-                
-class StreamingClient():
 
-    class context:
-        pass
-
-    def __init__(self, server, token):
-        self.__token = token
-        self.__pattern = "^ws:\/\/.*"
-        if re.match(self.__pattern, server):
-            self.__server = server
+    def app_create(
+        self, 
+        name, 
+        description, 
+        permission=["read:account", "write:account", "read:blocks", "write:blocks", "read:drive", "write:drive", "read:favorites", "write:favorites", "read:following", "write:following", "read:messaging", "write:messaging", "read:mutes", "write:mutes", "write:notes", "read:notifications", "write:notifications", "write:reactions", "write:votes", "read:pages", "write:pages", "write:page-likes", "read:page-likes", "write:gallery-likes", "read:gallery-likes"],
+        callback=None
+    ):
+        if callback is None:
+            r = self.http.request(
+                "app/create", 
+                {"name": name, "description": description, "permission": permission}
+            )
         else:
-            self.__server = "wss://" + server
-
-    def run(self):
-        async def runner(self):
-            self.__ws = await websockets.connect(f{self.__server}/streaming?i={self.__token}')
-            try:
-                await self.on_ready()
-            except AttributeError:
-                pass
-            while True:
-                response = await self.recv()
-                response = json.loads(response)
-                if response["body"]["type"] == "note":
-                    try:
-                        ctx = self.context()
-                        ctx.note.id = response["body"]["body"]["id"]
-                        ctx.author.id = response["body"]["body"]["userId"]
-                        ctx.author.name = response["body"]["body"]["user"]["name"]
-                        ctx.author.username = response["body"]["body"]["user"]["username"]
-                        ctx.text = response["body"]["body"]["text"]
-                        ctx.reactions = response["body"]["body"]["reactions"]
-                        ctx.files = response["body"]["body"]["files"]
-                        ctx.fileId = response["body"]["body"]["fileIds"]
-                        ctx.reply.id = response["body"]["body"]["replyId"]
-                        ctx.renote.id = response["body"]["body"]["renoteId"]
-                        ctx.uri = response["body"]["body"]["uri"]
-                        ctx.url = response["body"]["body"]["url"]
-                        if response["body"]["body"]["user"]["host"] is not None:
-                            ctx.author.host = response["body"]["body"]["user"]["host"]
-                            ctx.author.host.name = response["body"]["body"]["user"]["instance"]["name"]
-                            ctx.author.host.software = response["body"]["body"]["user"]["instance"]["softwareName"]
-                            ctx.author.host.softwareversion = response["body"]["body"]["user"]["instance"]["softwareVersion"]
-                            ctx.author.host.icon = response["body"]["body"]["user"]["instance"]["iconUrl"]
-                            ctx.author.host.favicon = response["body"]["body"]["user"]["instance"]["faviconUrl"]
-                            ctx.author.host.color = response["body"]["body"]["user"]["instance"]["themeColor"]
-                        else:
-                            ctx.author.host = None
-                        await self.on_note(ctx)
-                    except AttributeError:
-                        pass
-        asyncio.run(runner(self))
-
-    async def send(self, message):
-        await self.__ws.send(json.dumps(message, indent=4, ensure_ascii=False))
-
-    async def connect(self, channel):
-        await self.__ws.send(json.dumps({"type": "connect", "body": {"channel": channel, "id": channel}}, indent=4, ensure_ascii=False))
-
-    async def disconnect(self, channel):
-        await self.__ws.send(json.dumps({"type": "disconnect", "body": {"id": channel}}, indent=4, ensure_ascii=False))
-
+            r = self.http.request(
+                "app/create", 
+                {"name": name, "description": description, "permission": permission, "callbackUrl": callback}
+            )
 
-    async def recv(self):
-        return await self.__ws.recv()
+        return r
```

