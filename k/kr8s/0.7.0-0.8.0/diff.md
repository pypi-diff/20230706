# Comparing `tmp/kr8s-0.7.0.tar.gz` & `tmp/kr8s-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.7.0.tar", max compression
+gzip compressed data, was "kr8s-0.8.0.tar", max compression
```

## Comparing `kr8s-0.7.0.tar` & `kr8s-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1549 2023-07-03 10:38:10.325768 kr8s-0.7.0/LICENSE
--rw-r--r--   0        0        0     2571 2023-07-03 10:38:10.325768 kr8s-0.7.0/README.md
--rw-r--r--   0        0        0      541 2023-07-03 10:38:33.357956 kr8s-0.7.0/kr8s/__init__.py
--rw-r--r--   0        0        0    11094 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_api.py
--rw-r--r--   0        0        0     5879 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_auth.py
--rw-r--r--   0        0        0     1920 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_exceptions.py
--rw-r--r--   0        0        0     4294 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_io.py
--rw-r--r--   0        0        0    32623 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      709 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5503 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/conftest.py
--rw-r--r--   0        0        0     6001 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/objects.py
--rw-r--r--   0        0        0      152 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/portforward.py
--rw-r--r--   0        0        0       78 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/custom/evc.yaml
--rw-r--r--   0        0        0       61 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/serviceaccount.yaml
--rw-r--r--   0        0        0      369 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
--rw-r--r--   0        0        0      144 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nginx_pod.yaml
--rw-r--r--   0        0        0      435 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/resources/simple/nginx_pod_service.yaml
--rwxr-xr-x   0        0        0      614 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4567 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3402 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      824 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0      643 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_io.py
--rw-r--r--   0        0        0    17674 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-07-03 10:38:10.345768 kr8s-0.7.0/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2564 2023-07-03 10:38:33.357956 kr8s-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 kr8s-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-07-05 16:17:31.499512 kr8s-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2587 2023-07-05 16:17:31.499512 kr8s-0.8.0/README.md
+-rw-r--r--   0        0        0     1114 2023-07-05 16:17:56.447529 kr8s-0.8.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    14423 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4336 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_io.py
+-rw-r--r--   0        0        0    32661 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     8074 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0      248 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0     1110 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0     1681 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/asyncio/_helpers.py
+-rw-r--r--   0        0        0      827 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0      168 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5503 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     5238 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3394 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0     1710 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    17697 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-07-05 16:17:31.519512 kr8s-0.8.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2556 2023-07-05 16:17:56.443529 kr8s-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3323 1970-01-01 00:00:00.000000 kr8s-0.8.0/PKG-INFO
```

### Comparing `kr8s-0.7.0/LICENSE` & `kr8s-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/README.md` & `kr8s-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 A simple, extensible Python client library for Kubernetes that feels familiar for folks who already know how to use `kubectl`.
 
 ## Highlights
 
 - API inspired by `kubectl` to reduce developer learning curve.
 - [Sensible defaults](https://docs.kr8s.org/en/latest/authentication.html) to reduce boiler plate.
 - No swagger generated code, human readable code only.
-- Supports both [async/await](https://docs.kr8s.org/en/latest/asyncio.html) and sync APIs.
+- Also has an [asynchronous API](https://docs.kr8s.org/en/latest/asyncio.html) that can be used with `asyncio` and `trio`.
 - [Client caching](https://docs.kr8s.org/en/latest/client.html#client-caching) to reduce passing API objects around.
 - Batteries included by providing useful utilities and methods inspired by `kubectl`.
 
 ## Quickstart
 
 ### Installation
 
@@ -30,16 +30,15 @@
 ```
 
 ### Client API
 
 ```python
 import kr8s
 
-api = kr8s.api()
-pods = api.get("pods")
+pods = kr8s.get("pods")
 ```
 
 See the [Client API docs](https://docs.kr8s.org/en/latest/client.html) for more examples.
 
 ### Object API
 
 ```python
```

### Comparing `kr8s-0.7.0/kr8s/_api.py` & `kr8s-0.8.0/kr8s/_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
+from __future__ import annotations
+
 import contextlib
 import json
 import ssl
 import weakref
 from typing import Dict, List, Tuple, Union
 
 import aiohttp
-import asyncio_atexit
+import httpx
 
 from ._auth import KubeAuth
 from ._data_utils import dict_to_selector
 
 ALL = "all"
 
 
@@ -52,97 +54,165 @@
     def __await__(self):
         async def f():
             await self.auth
             return self
 
         return f().__await__()
 
-    async def _create_session(self) -> None:
-        headers = {"User-Agent": self.__version__, "content-type": "application/json"}
+    def _load_ssl_context(self) -> None:
         self._sslcontext = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
         if self.auth.client_key_file:
             self._sslcontext.load_cert_chain(
                 certfile=self.auth.client_cert_file,
                 keyfile=self.auth.client_key_file,
                 password=None,
             )
-
         if self.auth.server_ca_file:
             self._sslcontext.load_verify_locations(cafile=self.auth.server_ca_file)
+
+    async def _create_session(self) -> None:
+        headers = {"User-Agent": self.__version__, "content-type": "application/json"}
+        self._load_ssl_context()
         if self.auth.token:
             headers["Authorization"] = f"Bearer {self.auth.token}"
-        userauth = None
-        if self.auth.username and self.auth.password:
-            userauth = aiohttp.BasicAuth(self.auth.username, self.auth.password)
         if self._session:
-            asyncio_atexit.unregister(self._session.close)
-            await self._session.close()
+            with contextlib.suppress(RuntimeError):
+                await self._session.aclose()
             self._session = None
-        self._session = aiohttp.ClientSession(
+        userauth = None
+        if self.auth.username and self.auth.password:
+            userauth = httpx.BasicAuth(self.auth.username, self.auth.password)
+        self._session = httpx.AsyncClient(
             base_url=self.auth.server,
             headers=headers,
             auth=userauth,
+            verify=self._sslcontext,
         )
-        asyncio_atexit.register(self._session.close)
-
-    async def version(self) -> dict:
-        """Get the Kubernetes version"""
-        async with self.call_api(method="GET", version="", base="/version") as response:
-            return await response.json()
 
-    @contextlib.asynccontextmanager
-    async def call_api(
+    def _construct_url(
         self,
-        method: str = "GET",
         version: str = "v1",
         base: str = "",
         namespace: str = None,
         url: str = "",
-        raise_for_status: bool = True,
-        websocket: bool = False,
-        **kwargs,
-    ) -> aiohttp.ClientResponse:
-        """Make a Kubernetes API request."""
-        if not self._session or self._session.closed:
-            await self._create_session()
-
+    ) -> str:
         if not base:
             if version == "v1":
                 base = "/api"
             elif "/" in version:
                 base = "/apis"
             else:
                 raise ValueError("Unknown API version, base must be specified.")
         parts = [base]
         if version:
             parts.append(version)
         if namespace is not None:
             parts.extend(["namespaces", namespace])
         parts.append(url)
-        url = "/".join(parts)
-
-        call_method = self._session.ws_connect if websocket else self._session.request
-        kwargs.update(url=url, ssl=self._sslcontext)
-        if not websocket:
-            kwargs.update(method=method, raise_for_status=raise_for_status)
+        return "/".join(parts)
 
+    @contextlib.asynccontextmanager
+    async def call_api(
+        self,
+        method: str = "GET",
+        version: str = "v1",
+        base: str = "",
+        namespace: str = None,
+        url: str = "",
+        raise_for_status: bool = True,
+        stream: bool = False,
+        **kwargs,
+    ) -> httpx.Response:
+        """Make a Kubernetes API request."""
+        if not self._session or self._session.is_closed:
+            await self._create_session()
+        url = self._construct_url(version, base, namespace, url)
+        kwargs.update(url=url, method=method)
         auth_attempts = 0
         while True:
             try:
-                async with call_method(**kwargs) as response:
+                if stream:
+                    async with self._session.stream(**kwargs) as response:
+                        if raise_for_status:
+                            response.raise_for_status()
+                        yield response
+                else:
+                    response = await self._session.request(**kwargs)
+                    if raise_for_status:
+                        response.raise_for_status()
                     yield response
+            except httpx.HTTPStatusError as e:
+                if e.response.status_code in (401, 403) and auth_attempts < 3:
+                    auth_attempts += 1
+                    await self.auth.reauthenticate()
+                    await self._create_session()
+                    continue
+                else:
+                    raise
+            except RuntimeError as e:
+                if "Event loop is closed" in str(e):
+                    await self._create_session()
+                    continue
+                else:
+                    raise
+            break
+
+    @contextlib.asynccontextmanager
+    async def open_websocket(
+        self,
+        version: str = "v1",
+        base: str = "",
+        namespace: str = None,
+        url: str = "",
+        **kwargs,
+    ) -> aiohttp.ClientResponse:
+        """Open a websocket connection to a Kubernetes API endpoint."""
+        headers = {"User-Agent": self.__version__, "content-type": "application/json"}
+        self._load_ssl_context()
+        if self.auth.token:
+            headers["Authorization"] = f"Bearer {self.auth.token}"
+        userauth = None
+        if self.auth.username and self.auth.password:
+            userauth = aiohttp.BasicAuth(self.auth.username, self.auth.password)
+        url = self._construct_url(version, base, namespace, url)
+        kwargs.update(url=url, ssl=self._sslcontext)
+        auth_attempts = 0
+        while True:
+            try:
+                async with aiohttp.ClientSession(
+                    base_url=self.auth.server,
+                    headers=headers,
+                    auth=userauth,
+                ) as session:
+                    async with session.ws_connect(**kwargs) as response:
+                        yield response
             except aiohttp.ClientResponseError as e:
                 if e.status in (401, 403) and auth_attempts < 3:
                     auth_attempts += 1
                     await self.auth.reauthenticate()
                     continue
                 else:
                     raise
             break
 
+    async def version(self) -> dict:
+        """Get the Kubernetes version information from the API.
+
+        Returns
+        -------
+        dict
+            The Kubernetes version information.
+
+        """
+        return await self._version()
+
+    async def _version(self) -> dict:
+        async with self.call_api(method="GET", version="", base="/version") as response:
+            return response.json()
+
     async def reauthenticate(self) -> None:
         """Reauthenticate the API."""
         await self.auth.reauthenticate()
 
     @contextlib.asynccontextmanager
     async def _get_kind(
         self,
@@ -169,14 +239,15 @@
             params["labelSelector"] = label_selector
         if field_selector:
             if isinstance(field_selector, dict):
                 field_selector = dict_to_selector(field_selector)
             params["fieldSelector"] = field_selector
         if watch:
             params["watch"] = "true" if watch else "false"
+            kwargs["stream"] = True
         params = params or None
         obj_cls = get_class(kind)
         async with self.call_api(
             method="GET",
             url=kind,
             version=obj_cls.version,
             namespace=namespace if obj_cls.namespaced else None,
@@ -191,15 +262,39 @@
         *names: List[str],
         namespace: str = None,
         label_selector: Union[str, Dict] = None,
         field_selector: Union[str, Dict] = None,
         as_object: object = None,
         **kwargs,
     ) -> List[object]:
-        """Get a Kubernetes resource."""
+        """
+        Get Kubernetes resources.
+
+        Parameters
+        ----------
+        kind : str
+            The kind of resource to get.
+        *names : List[str], optional
+            The names of specific resources to get.
+        namespace : str, optional
+            The namespace to get the resource from.
+        label_selector : Union[str, Dict], optional
+            The label selector to filter the resources by.
+        field_selector : Union[str, Dict], optional
+            The field selector to filter the resources by.
+        as_object : object, optional
+            The object to return the resources as.
+        **kwargs
+            Additional keyword arguments to pass to the API call.
+
+        Returns
+        -------
+        List[object]
+            The resources.
+        """
         return await self._get(
             kind,
             *names,
             namespace=namespace,
             label_selector=label_selector,
             field_selector=field_selector,
             as_object=as_object,
@@ -226,15 +321,15 @@
             kind,
             namespace=namespace,
             label_selector=label_selector,
             field_selector=field_selector,
             headers=headers or None,
             **kwargs,
         ) as (obj_cls, response):
-            resourcelist = await response.json()
+            resourcelist = response.json()
             if (
                 as_object
                 and "kind" in resourcelist
                 and resourcelist["kind"] == as_object.kind
             ):
                 return as_object(resourcelist, api=self)
             else:
@@ -277,44 +372,48 @@
             kind,
             namespace=namespace,
             label_selector=label_selector,
             field_selector=field_selector,
             params={"resourceVersion": since} if since else None,
             watch=True,
         ) as (obj_cls, response):
-            async for line in response.content:
+            async for line in response.aiter_lines():
                 event = json.loads(line)
                 yield event["type"], obj_cls(event["object"], api=self)
 
     async def api_resources(self) -> dict:
         """Get the Kubernetes API resources."""
+        return await self._api_resources()
+
+    async def _api_resources(self) -> dict:
+        """Get the Kubernetes API resources."""
         resources = []
         async with self.call_api(method="GET", version="", base="/api") as response:
-            core_api_list = await response.json()
+            core_api_list = response.json()
 
         for version in core_api_list["versions"]:
             async with self.call_api(
                 method="GET", version="", base="/api", url=version
             ) as response:
-                resource = await response.json()
+                resource = response.json()
             resources.extend(
                 [
                     {"version": version, **r}
                     for r in resource["resources"]
                     if "/" not in r["name"]
                 ]
             )
         async with self.call_api(method="GET", version="", base="/apis") as response:
-            api_list = await response.json()
+            api_list = response.json()
         for api in sorted(api_list["groups"], key=lambda d: d["name"]):
             version = api["versions"][0]["groupVersion"]
             async with self.call_api(
                 method="GET", version="", base="/apis", url=version
             ) as response:
-                resource = await response.json()
+                resource = response.json()
             resources.extend(
                 [
                     {"version": version, **r}
                     for r in resource["resources"]
                     if "/" not in r["name"]
                 ]
             )
```

### Comparing `kr8s-0.7.0/kr8s/_auth.py` & `kr8s-0.8.0/kr8s/_auth.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/_data_utils.py` & `kr8s-0.8.0/kr8s/_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/_io.py` & `kr8s-0.8.0/kr8s/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,19 +35,21 @@
     -------
     result :
         Whatever the coroutine-function returns.
     """
 
     @wraps(coro)
     def wrapped(*args, **kwargs):
+        wrapped = partial(coro, *args, **kwargs)
+        wrapped.__doc__ = coro.__doc__
         with anyio.from_thread.start_blocking_portal() as portal:
             if inspect.iscoroutinefunction(coro):
-                return portal.call(partial(coro, *args, **kwargs))
+                return portal.call(wrapped)
             if inspect.isasyncgenfunction(coro):
-                return iter_over_async(partial(coro, *args, **kwargs))
+                return iter_over_async(wrapped)
             raise TypeError(
                 f"Expected coroutine function, got {coro.__class__.__name__}"
             )
 
     wrapped.__doc__ = coro.__doc__
     return wrapped
```

### Comparing `kr8s-0.7.0/kr8s/_objects.py` & `kr8s-0.8.0/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 import asyncio
 import json
 import pathlib
 import re
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
-import aiohttp
 import anyio
+import httpx
 import jsonpath
 import yaml
-from aiohttp import ClientResponse
 
 import kr8s
 import kr8s.asyncio
 from kr8s._api import Api
 from kr8s._data_utils import dict_to_selector, dot_to_nested_dict, list_dict_unpack
 from kr8s._exceptions import NotFoundError
 from kr8s.asyncio.portforward import PortForward as AsyncPortForward
@@ -194,15 +193,15 @@
         async with self.api.call_api(
             "GET",
             version=self.version,
             url=f"{self.endpoint}/{self.name}",
             namespace=self.namespace,
             raise_for_status=False,
         ) as resp:
-            status = resp.status
+            status = resp.status_code
         if status == 200:
             return True
         if ensure:
             raise NotFoundError(f"Object {self.name} does not exist")
         return False
 
     async def create(self) -> None:
@@ -210,49 +209,51 @@
         async with self.api.call_api(
             "POST",
             version=self.version,
             url=self.endpoint,
             namespace=self.namespace,
             data=json.dumps(self.raw),
         ) as resp:
-            self.raw = await resp.json()
+            self.raw = resp.json()
 
     async def delete(self, propagation_policy: str = None) -> None:
         """Delete this object from Kubernetes."""
         data = {}
         if propagation_policy:
             data["propagationPolicy"] = propagation_policy
         try:
             async with self.api.call_api(
                 "DELETE",
                 version=self.version,
                 url=f"{self.endpoint}/{self.name}",
                 namespace=self.namespace,
                 data=json.dumps(data),
             ) as resp:
-                self.raw = await resp.json()
-        except aiohttp.ClientResponseError as e:
-            raise NotFoundError(f"Object {self.name} does not exist") from e
+                self.raw = resp.json()
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == 404:
+                raise NotFoundError(f"Object {self.name} does not exist") from e
+            raise e
 
     async def refresh(self) -> None:
         """Refresh this object from Kubernetes."""
         await self._refresh()
 
     async def _refresh(self) -> None:
         """Refresh this object from Kubernetes."""
         try:
             async with self.api.call_api(
                 "GET",
                 version=self.version,
                 url=f"{self.endpoint}/{self.name}",
                 namespace=self.namespace,
             ) as resp:
-                self.raw = await resp.json()
-        except aiohttp.ClientResponseError as e:
-            if e.status == 404:
+                self.raw = resp.json()
+        except httpx.HTTPStatusError as e:
+            if e.response.status_code == 404:
                 raise NotFoundError(f"Object {self.name} does not exist") from e
             raise e
 
     async def patch(self, patch, *, subresource=None) -> None:
         """Patch this object in Kubernetes."""
         return await self._patch(patch, subresource=subresource)
 
@@ -265,15 +266,15 @@
             "PATCH",
             version=self.version,
             url=url,
             namespace=self.namespace,
             data=json.dumps(patch),
             headers={"Content-Type": "application/merge-patch+json"},
         ) as resp:
-            self.raw = await resp.json()
+            self.raw = resp.json()
 
     async def scale(self, replicas: int = None) -> None:
         """Scale this object in Kubernetes."""
         if not self.scalable:
             raise NotImplementedError(f"{self.kind} is not scalable")
         await self._exists(ensure=True)
         await self._patch({"spec": dot_to_nested_dict(self.scalable_spec, replicas)})
@@ -554,15 +555,15 @@
         async with self.api.call_api(
             "GET",
             version=self.version,
             url=f"{self.endpoint}/{self.name}/log",
             namespace=self.namespace,
             params=params,
         ) as resp:
-            return await resp.text()
+            return resp.text
 
     def portforward(self, remote_port: int, local_port: int = None) -> int:
         """Port forward a pod.
 
         Returns an instance of :class:`kr8s.portforward.PortForward` for this Pod.
 
         Example:
@@ -661,58 +662,58 @@
     kind = "Service"
     plural = "services"
     singular = "service"
     namespaced = True
 
     async def proxy_http_request(
         self, method: str, path: str, port: Optional[int] = None, **kwargs: Any
-    ) -> ClientResponse:
+    ) -> httpx.Response:
         """Issue a HTTP request with specific HTTP method to proxy of a Service.
 
         Args:
             method: HTTP method to use.
             path: Path to proxy.
             port: Port to proxy to. If not specified, the first port in the
                 Service's spec will be used.
             **kwargs: Additional keyword arguments to pass to the API call.
         """
         return await self._proxy_http_request(method, path, port, **kwargs)
 
     async def _proxy_http_request(
         self, method: str, path: str, port: Optional[int] = None, **kwargs: Any
-    ) -> ClientResponse:
+    ) -> httpx.Response:
         if port is None:
             port = self.raw["spec"]["ports"][0]["port"]
         async with self.api.call_api(
             method,
             version=self.version,
             url=f"{self.endpoint}/{self.name}:{port}/proxy/{path}",
             namespace=self.namespace,
             **kwargs,
         ) as response:
             return response
 
     async def proxy_http_get(
         self, path: str, port: Optional[int] = None, **kwargs
-    ) -> None:
+    ) -> httpx.Response:
         return await self._proxy_http_request("GET", path, port, **kwargs)
 
     async def proxy_http_post(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
         return await self._proxy_http_request("POST", path, port, **kwargs)
 
     async def proxy_http_put(
         self, path: str, port: Optional[int] = None, **kwargs
-    ) -> None:
+    ) -> httpx.Response:
         return await self._proxy_http_request("PUT", path, port, **kwargs)
 
     async def proxy_http_delete(
         self, path: str, port: Optional[int] = None, **kwargs
-    ) -> None:
+    ) -> httpx.Response:
         return await self._proxy_http_request("DELETE", path, port, **kwargs)
 
     async def ready_pods(self) -> List[Pod]:
         """Return a list of ready Pods for this Service."""
         return await self._ready_pods()
 
     async def _ready_pods(self) -> List[Pod]:
```

### Comparing `kr8s-0.7.0/kr8s/_portforward.py` & `kr8s-0.8.0/kr8s/_portforward.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import asyncio
 import random
 import socket
 from contextlib import asynccontextmanager
 from typing import TYPE_CHECKING, BinaryIO
 
 import aiohttp
+import sniffio
 
 from ._exceptions import ConnectionClosedError
 
 if TYPE_CHECKING:
     from .objects import APIObject
 
 
@@ -21,14 +22,17 @@
 
     You can either pass a :class:`kr8s.objects.Pod` or any resource with a ``ready_pods`` method
     such as a :class:`kr8s.objects.Service`.
 
     .. note::
         The ``ready_pods`` method should return a list of Pods that are ready to accept connections.
 
+    .. warning:
+        Currently Port Forwards only work when using ``asyncio`` and not ``trio``.
+
     Args:
         ``resource`` (Pod or Resource): The Pod or Resource to forward to.
 
         ``remote_port`` (int): The port on the Pod to forward to.
 
         ``local_port`` (int, optional): The local port to listen on. Defaults to 0, which will choose a random port.
 
@@ -52,14 +56,19 @@
 
 
     """
 
     def __init__(
         self, resource: APIObject, remote_port: int, local_port: int = None
     ) -> None:
+        if sniffio.current_async_library() != "asyncio":
+            raise RuntimeError(
+                "PortForward only works with asyncio, "
+                "see https://github.com/kr8s-org/kr8s/issues/104"
+            )
         self.running = True
         self.server = None
         self.websocket = None
         self.remote_port = remote_port
         self.local_port = local_port if local_port is not None else 0
         self._resource = resource
         from ._objects import Pod
@@ -126,19 +135,18 @@
             self.server.close()
             await self.server.wait_closed()
 
     async def _connect_websocket(self) -> None:
         while self.running:
             self.connection_attempts += 1
             try:
-                async with self.pod.api.call_api(
+                async with self.pod.api.open_websocket(
                     version=self.pod.version,
                     url=f"{self.pod.endpoint}/{self.pod.name}/portforward",
                     namespace=self.pod.namespace,
-                    websocket=True,
                     params={
                         "name": self.pod.name,
                         "namespace": self.pod.namespace,
                         "ports": f"{self.remote_port}",
                         "_preload_content": "false",
                     },
                 ) as websocket:
```

### Comparing `kr8s-0.7.0/kr8s/_testutils.py` & `kr8s-0.8.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/asyncio/_api.py` & `kr8s-0.8.0/kr8s/asyncio/_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
+# SPDX-License-Identifier: BSD 3-Clause License
 from kr8s._api import Api as _AsyncApi
 
 
 async def api(
     url: str = None,
     kubeconfig: str = None,
     serviceaccount: str = None,
```

### Comparing `kr8s-0.7.0/kr8s/asyncio/objects.py` & `kr8s-0.8.0/kr8s/asyncio/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
+# SPDX-License-Identifier: BSD 3-Clause License
 from kr8s._objects import (  # noqa
     APIObject,
     Binding,
     ClusterRole,
     ClusterRoleBinding,
     ComponentStatus,
     ConfigMap,
```

### Comparing `kr8s-0.7.0/kr8s/conftest.py` & `kr8s-0.8.0/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/objects.py` & `kr8s-0.8.0/kr8s/objects.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/tests/scripts/envexec.py` & `kr8s-0.8.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/tests/test_api.py` & `kr8s-0.8.0/kr8s/tests/test_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,14 +65,19 @@
 
 async def test_version():
     kubernetes = await kr8s.asyncio.api()
     version = await kubernetes.version()
     assert "major" in version
 
 
+def test_helper_version():
+    version = kr8s.version()
+    assert "major" in version
+
+
 async def test_concurrent_api_creation():
     async def get_api():
         api = await kr8s.asyncio.api()
         await api.version()
         return api
 
     apis = await asyncio.gather(*[get_api() for _ in range(10)])
@@ -84,35 +89,33 @@
     with pytest.raises(ValueError):
         async with kubernetes.call_api("GET", version="foo"):
             pass  # pragma: no cover
 
 
 @pytest.mark.parametrize("namespace", [kr8s.ALL, "kube-system"])
 async def test_get_pods(namespace):
-    kubernetes = await kr8s.asyncio.api()
-    pods = await kubernetes.get("pods", namespace=namespace)
+    pods = await kr8s.asyncio.get("pods", namespace=namespace)
     assert isinstance(pods, list)
     assert len(pods) > 0
     assert isinstance(pods[0], Pod)
 
 
 async def test_get_pods_as_table():
     kubernetes = await kr8s.asyncio.api()
     pods = await kubernetes.get("pods", namespace="kube-system", as_object=Table)
     assert isinstance(pods, Table)
     assert len(pods.rows) > 0
 
 
 async def test_watch_pods(example_pod_spec, ns):
-    kubernetes = await kr8s.asyncio.api()
     pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
-    async for event, obj in kubernetes.watch("pods", namespace=ns):
+    async for event, obj in kr8s.asyncio.watch("pods", namespace=ns):
         assert event in ["ADDED", "MODIFIED", "DELETED"]
         assert isinstance(obj, Pod)
         if obj.name == pod.name:
             if event == "ADDED":
                 await obj.patch({"metadata": {"labels": {"test": "test"}}})
             elif event == "MODIFIED" and "test" in obj.labels and await obj.exists():
                 await obj.delete()
@@ -125,16 +128,15 @@
 async def test_get_deployments():
     kubernetes = await kr8s.asyncio.api()
     deployments = await kubernetes.get("deployments")
     assert isinstance(deployments, list)
 
 
 async def test_api_resources():
-    kubernetes = await kr8s.asyncio.api()
-    resources = await kubernetes.api_resources()
+    resources = await kr8s.asyncio.api_resources()
 
     names = [r["name"] for r in resources]
     assert "nodes" in names
     assert "pods" in names
     assert "services" in names
     assert "namespaces" in names
 
@@ -154,7 +156,34 @@
 
 async def test_ns(ns):
     api = await kr8s.asyncio.api(namespace=ns)
     assert ns == api.namespace
 
     api.namespace = "foo"
     assert api.namespace == "foo"
+
+
+async def test_docstrings():
+    assert (
+        kr8s.Api.get.__doc__
+        == kr8s.asyncio.Api.get.__doc__
+        == kr8s.get.__doc__
+        == kr8s.asyncio.get.__doc__
+    )
+    assert (
+        kr8s.Api.version.__doc__
+        == kr8s.asyncio.Api.version.__doc__
+        == kr8s.version.__doc__
+        == kr8s.asyncio.version.__doc__
+    )
+    assert (
+        kr8s.Api.watch.__doc__
+        == kr8s.asyncio.Api.watch.__doc__
+        == kr8s.watch.__doc__
+        == kr8s.asyncio.watch.__doc__
+    )
+    assert (
+        kr8s.Api.api_resources.__doc__
+        == kr8s.asyncio.Api.api_resources.__doc__
+        == kr8s.api_resources.__doc__
+        == kr8s.asyncio.api_resources.__doc__
+    )
```

### Comparing `kr8s-0.7.0/kr8s/tests/test_auth.py` & `kr8s-0.8.0/kr8s/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import sys
 import tempfile
 from pathlib import Path
 
-import aiohttp
+import httpx
 import pytest
 import yaml
 
 import kr8s
 from kr8s._testutils import set_env
 
 HERE = Path(__file__).parent.resolve()
@@ -68,15 +68,15 @@
 
 async def test_bad_auth(serviceaccount):
     (Path(serviceaccount) / "token").write_text("abc123")
     kubernetes = await kr8s.asyncio.api(
         serviceaccount=serviceaccount, kubeconfig="/no/file/here"
     )
     serviceaccount = Path(serviceaccount)
-    with pytest.raises(aiohttp.ClientResponseError):
+    with pytest.raises(httpx.HTTPStatusError):
         await kubernetes.version()
 
 
 async def test_url(kubectl_proxy):
     kubernetes = await kr8s.asyncio.api(url=kubectl_proxy)
     version = await kubernetes.version()
     assert "major" in version
```

### Comparing `kr8s-0.7.0/kr8s/tests/test_data_utils.py` & `kr8s-0.8.0/kr8s/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/kr8s/tests/test_objects.py` & `kr8s-0.8.0/kr8s/tests/test_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import asyncio
 import pathlib
 import time
 
-import aiohttp
+import httpx
 import pytest
 
 import kr8s
 from kr8s.asyncio.objects import (
     APIObject,
     Deployment,
     Ingress,
@@ -18,15 +18,15 @@
     object_from_name_type,
     objects_from_files,
 )
 from kr8s.asyncio.portforward import PortForward
 from kr8s.objects import Pod as SyncPod
 from kr8s.objects import get_class, object_from_spec
 
-DEFAULT_TIMEOUT = aiohttp.ClientTimeout(30)
+DEFAULT_TIMEOUT = httpx.Timeout(30)
 CURRENT_DIR = pathlib.Path(__file__).parent
 
 
 @pytest.fixture
 async def nginx_pod(k8s_cluster, example_pod_spec, ns):
     example_pod_spec["metadata"]["name"] = (
         "nginx-" + example_pod_spec["metadata"]["name"]
@@ -129,14 +129,21 @@
     with pytest.raises(ValueError):
         pod.wait("foo=NotARealCondition")
     pod.delete()
     pod.wait("condition=Ready=False")
     pod.wait("delete")
 
 
+def test_pod_refresh_sync(example_pod_spec):
+    pod = SyncPod(example_pod_spec)
+    pod.create()
+    pod.refresh()
+    pod.delete()
+
+
 def test_pod_create_and_delete_sync(example_pod_spec):
     pod = SyncPod(example_pod_spec)
     pod.create()
     with pytest.raises(NotImplementedError):
         pod.replicas
     assert pod.exists()
     while not pod.ready():
@@ -412,15 +419,15 @@
 
 
 async def test_service_proxy():
     kubernetes = await kr8s.asyncio.api()
     [service] = await kubernetes.get("services", "kubernetes")
     assert service.name == "kubernetes"
     data = await service.proxy_http_get("/version", raise_for_status=False)
-    assert isinstance(data, aiohttp.ClientResponse)
+    assert isinstance(data, httpx.Response)
 
 
 async def test_pod_logs(example_pod_spec):
     pod = await Pod(example_pod_spec)
     await pod.create()
     while not await pod.ready():
         await asyncio.sleep(0.1)
@@ -428,22 +435,22 @@
     assert isinstance(log, str)
     await pod.delete()
 
 
 async def test_pod_port_forward_context_manager(nginx_service):
     [nginx_pod, *_] = await nginx_service.ready_pods()
     async with nginx_pod.portforward(80) as port:
-        async with aiohttp.ClientSession(timeout=DEFAULT_TIMEOUT) as session:
-            async with session.get(f"http://localhost:{port}/") as resp:
-                assert resp.status == 200
-            async with session.get(f"http://localhost:{port}/foo") as resp:
-                assert resp.status == 404
-            async with session.get(f"http://localhost:{port}/foo.dat") as resp:
-                assert resp.status == 200
-                await resp.read()
+        async with httpx.AsyncClient(timeout=DEFAULT_TIMEOUT) as session:
+            resp = await session.get(f"http://localhost:{port}/")
+            assert resp.status_code == 200
+            resp = await session.get(f"http://localhost:{port}/foo")
+            assert resp.status_code == 404
+            resp = await session.get(f"http://localhost:{port}/foo.dat")
+            assert resp.status_code == 200
+            resp.read()
 
 
 @pytest.mark.skip(reason="For manual testing only")
 async def test_pod_port_forward_context_manager_manual(nginx_service):
     [nginx_pod, *_] = await nginx_service.ready_pods()
     pf = nginx_pod.portforward(80, 8184)
     async with pf:
@@ -455,45 +462,47 @@
 
 async def test_pod_port_forward_start_stop(nginx_service):
     [nginx_pod, *_] = await nginx_service.ready_pods()
     pf = nginx_pod.portforward(80)
     assert pf._bg_task is None
     port = await pf.start()
     assert pf._bg_task is not None
-    async with aiohttp.ClientSession(timeout=DEFAULT_TIMEOUT) as session:
-        async with session.get(f"http://localhost:{port}/") as resp:
-            assert resp.status == 200
-        async with session.get(f"http://localhost:{port}/foo") as resp:
-            assert resp.status == 404
-        async with session.get(f"http://localhost:{port}/foo.dat") as resp:
-            assert resp.status == 200
-            await resp.read()
+    async with httpx.AsyncClient(timeout=DEFAULT_TIMEOUT) as session:
+        resp = await session.get(f"http://localhost:{port}/")
+        assert resp.status_code == 200
+        resp = await session.get(f"http://localhost:{port}/foo")
+        assert resp.status_code == 404
+        resp = await session.get(f"http://localhost:{port}/foo.dat")
+        assert resp.status_code == 200
+        resp.read()
     await pf.stop()
     assert pf._bg_task is None
 
 
 async def test_service_port_forward_context_manager(nginx_service):
     async with nginx_service.portforward(80) as port:
-        async with aiohttp.ClientSession(timeout=DEFAULT_TIMEOUT) as session:
-            async with session.get(f"http://localhost:{port}/") as resp:
-                assert resp.status == 200
-            async with session.get(f"http://localhost:{port}/foo") as resp:
-                assert resp.status == 404
+        async with httpx.AsyncClient(timeout=DEFAULT_TIMEOUT) as session:
+            resp = await session.get(f"http://localhost:{port}/")
+            assert resp.status_code == 200
+            resp = await session.get(f"http://localhost:{port}/foo")
+            assert resp.status_code == 404
 
 
 async def test_service_port_forward_start_stop(nginx_service):
     pf = nginx_service.portforward(80)
     assert pf._bg_task is None
     port = await pf.start()
     assert pf._bg_task is not None
-    async with aiohttp.ClientSession(timeout=DEFAULT_TIMEOUT) as session:
-        async with session.get(f"http://localhost:{port}/") as resp:
-            assert resp.status == 200
-        async with session.get(f"http://localhost:{port}/foo") as resp:
-            assert resp.status == 404
+
+    async with httpx.AsyncClient(timeout=DEFAULT_TIMEOUT) as session:
+        resp = await session.get(f"http://localhost:{port}/")
+        assert resp.status_code == 200
+        resp = await session.get(f"http://localhost:{port}/foo")
+        assert resp.status_code == 404
+
     await pf.stop()
     assert pf._bg_task is None
 
 
 async def test_unsupported_port_forward():
     pv = await PersistentVolume({})
     with pytest.raises(AttributeError):
```

### Comparing `kr8s-0.7.0/kr8s/tests/test_testutils.py` & `kr8s-0.8.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.7.0/pyproject.toml` & `kr8s-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.7.0"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.8.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
@@ -32,17 +32,17 @@
 [tool.poetry-dynamic-versioning.substitution]
 files = ["kr8s/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
-asyncio-atexit = "^1.0.1"
 python-jsonpath = "^0.7.1"
 anyio = "^3.7.0"
+httpx = "^0.24.1"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
```

### Comparing `kr8s-0.7.0/PKG-INFO` & `kr8s-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
-Requires-Dist: asyncio-atexit (>=1.0.1,<2.0.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: python-jsonpath (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
 [![Test](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml/badge.svg)](https://github.com/kr8s-org/kr8s/actions/workflows/test.yaml)
@@ -34,15 +34,15 @@
 A simple, extensible Python client library for Kubernetes that feels familiar for folks who already know how to use `kubectl`.
 
 ## Highlights
 
 - API inspired by `kubectl` to reduce developer learning curve.
 - [Sensible defaults](https://docs.kr8s.org/en/latest/authentication.html) to reduce boiler plate.
 - No swagger generated code, human readable code only.
-- Supports both [async/await](https://docs.kr8s.org/en/latest/asyncio.html) and sync APIs.
+- Also has an [asynchronous API](https://docs.kr8s.org/en/latest/asyncio.html) that can be used with `asyncio` and `trio`.
 - [Client caching](https://docs.kr8s.org/en/latest/client.html#client-caching) to reduce passing API objects around.
 - Batteries included by providing useful utilities and methods inspired by `kubectl`.
 
 ## Quickstart
 
 ### Installation
 
@@ -51,16 +51,15 @@
 ```
 
 ### Client API
 
 ```python
 import kr8s
 
-api = kr8s.api()
-pods = api.get("pods")
+pods = kr8s.get("pods")
 ```
 
 See the [Client API docs](https://docs.kr8s.org/en/latest/client.html) for more examples.
 
 ### Object API
 
 ```python
```

