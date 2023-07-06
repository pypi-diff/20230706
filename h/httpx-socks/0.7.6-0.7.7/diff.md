# Comparing `tmp/httpx-socks-0.7.6.tar.gz` & `tmp/httpx-socks-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpx-socks-0.7.6.tar", last modified: Sun Apr 16 05:43:39 2023, max compression
+gzip compressed data, was "dist/httpx-socks-0.7.7.tar", last modified: Thu Jul  6 11:57:51 2023, max compression
```

## Comparing `httpx-socks-0.7.6.tar` & `httpx-socks-0.7.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/
--rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 httpx-socks-0.7.6/LICENSE.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 httpx-socks-0.7.6/MANIFEST.in
--rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)     2409 2022-02-12 08:51:18.000000 httpx-socks-0.7.6/README.md
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/httpx_socks/
--rw-rw-r--   0 roman     (1000) roman     (1000)      448 2023-04-16 05:31:37.000000 httpx-socks-0.7.6/httpx_socks/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     8125 2021-11-25 11:27:42.000000 httpx-socks-0.7.6/httpx_socks/_async_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3400 2021-11-25 11:17:09.000000 httpx-socks-0.7.6/httpx_socks/_async_transport.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     6195 2021-11-25 11:29:34.000000 httpx-socks-0.7.6/httpx_socks/_sync_proxy.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     1420 2021-11-25 12:08:29.000000 httpx-socks-0.7.6/httpx_socks/_sync_stream.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3265 2021-11-25 11:27:33.000000 httpx-socks-0.7.6/httpx_socks/_sync_transport.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/httpx_socks.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      401 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      120 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/requires.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)       12 2023-04-16 05:43:38.000000 httpx-socks-0.7.6/httpx_socks.egg-info/top_level.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)      209 2022-02-06 06:27:51.000000 httpx-socks-0.7.6/pyproject.toml
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-04-16 05:43:39.000000 httpx-socks-0.7.6/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)     1330 2023-04-16 05:29:16.000000 httpx-socks-0.7.6/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/
+-rw-rw-r--   0 roman     (1000) roman     (1000)    11357 2020-11-30 04:28:18.000000 httpx-socks-0.7.7/LICENSE.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       47 2020-11-30 04:28:18.000000 httpx-socks-0.7.7/MANIFEST.in
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2409 2022-02-12 08:51:18.000000 httpx-socks-0.7.7/README.md
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      448 2023-07-06 11:38:13.000000 httpx-socks-0.7.7/httpx_socks/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     8107 2023-07-06 11:49:46.000000 httpx-socks-0.7.7/httpx_socks/_async_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3400 2021-11-25 11:17:09.000000 httpx-socks-0.7.7/httpx_socks/_async_transport.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     6195 2021-11-25 11:29:34.000000 httpx-socks-0.7.7/httpx_socks/_sync_proxy.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1421 2023-07-06 11:39:18.000000 httpx-socks-0.7.7/httpx_socks/_sync_stream.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3265 2021-11-25 11:27:33.000000 httpx-socks-0.7.7/httpx_socks/_sync_transport.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     2828 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      401 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      120 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/requires.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)       12 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/httpx_socks.egg-info/top_level.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)      209 2022-02-06 06:27:51.000000 httpx-socks-0.7.7/pyproject.toml
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-07-06 11:57:51.000000 httpx-socks-0.7.7/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1330 2023-07-06 11:37:39.000000 httpx-socks-0.7.7/setup.py
```

### Comparing `httpx-socks-0.7.6/LICENSE.txt` & `httpx-socks-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.6/PKG-INFO` & `httpx-socks-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-socks
-Version: 0.7.6
+Version: 0.7.7
 Summary: Proxy (HTTP, SOCKS) transports for httpx
 Home-page: https://github.com/romis2012/httpx-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: httpx asyncio socks socks5 socks4 http proxy
 Platform: UNKNOWN
```

### Comparing `httpx-socks-0.7.6/README.md` & `httpx-socks-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.6/httpx_socks/_async_proxy.py` & `httpx-socks-0.7.7/httpx_socks/_async_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     AsyncConnectionInterface,
     Request,
     Response,
     default_ssl_context,
     AsyncHTTP11Connection,
     ConnectionNotAvailable,
 )
+from httpcore import AsyncNetworkStream
 from httpcore._synchronization import AsyncLock
-from httpcore.backends.base import AsyncNetworkStream
 from python_socks import ProxyType, parse_proxy_url
 
 
 class AsyncProxy(AsyncConnectionPool):
     def __init__(
         self,
         *,
@@ -170,15 +170,15 @@
         # Curio support has been dropped in httpcore 0.14.0
         # if backend == 'curio':
         #     return await self._open_curio_stream(host, port, connect_timeout, ssl_context)
 
         raise RuntimeError(f'Unsupported concurrency backend {backend!r}')  # pragma: no cover
 
     async def _open_aio_stream(self, host, port, connect_timeout, ssl_context):
-        from httpcore.backends.asyncio import AsyncIOStream
+        from httpcore._backends.anyio import AnyIOStream
         from python_socks.async_.anyio import Proxy
 
         proxy = Proxy.create(
             proxy_type=self._proxy_type,
             host=self._proxy_host,
             port=self._proxy_port,
             username=self._username,
@@ -190,18 +190,18 @@
         proxy_stream = await proxy.connect(
             host,
             port,
             dest_ssl=ssl_context,
             timeout=connect_timeout,
         )
 
-        return AsyncIOStream(proxy_stream.anyio_stream)
+        return AnyIOStream(proxy_stream.anyio_stream)
 
     async def _open_trio_stream(self, host, port, connect_timeout, ssl_context):
-        from httpcore.backends.trio import TrioStream
+        from httpcore._backends.trio import TrioStream
         from python_socks.async_.trio.v2 import Proxy
 
         proxy = Proxy.create(
             proxy_type=self._proxy_type,
             host=self._proxy_host,
             port=self._proxy_port,
             username=self._username,
```

### Comparing `httpx-socks-0.7.6/httpx_socks/_async_transport.py` & `httpx-socks-0.7.7/httpx_socks/_async_transport.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.6/httpx_socks/_sync_proxy.py` & `httpx-socks-0.7.7/httpx_socks/_sync_proxy.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.6/httpx_socks/_sync_stream.py` & `httpx-socks-0.7.7/httpx_socks/_sync_stream.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import ssl
 import typing
 
-from httpcore.backends.sync import SyncStream as CoreSyncStream
+from httpcore._backends.sync import SyncStream as CoreSyncStream
 from httpcore._utils import is_socket_readable
 from python_socks.sync.v2._ssl_transport import SSLTransport
 
 
 class SyncStream(CoreSyncStream):
     def get_extra_info(self, info: str) -> typing.Any:
         if info == "ssl_object":
```

### Comparing `httpx-socks-0.7.6/httpx_socks/_sync_transport.py` & `httpx-socks-0.7.7/httpx_socks/_sync_transport.py`

 * *Files identical despite different names*

### Comparing `httpx-socks-0.7.6/httpx_socks.egg-info/PKG-INFO` & `httpx-socks-0.7.7/httpx_socks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-socks
-Version: 0.7.6
+Version: 0.7.7
 Summary: Proxy (HTTP, SOCKS) transports for httpx
 Home-page: https://github.com/romis2012/httpx-socks
 Author: Roman Snegirev
 Author-email: snegiryev@gmail.com
 License: Apache 2
 Keywords: httpx asyncio socks socks5 socks4 http proxy
 Platform: UNKNOWN
```

### Comparing `httpx-socks-0.7.6/setup.py` & `httpx-socks-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description='Proxy (HTTP, SOCKS) transports for httpx',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['httpx_socks'],
     keywords='httpx asyncio socks socks5 socks4 http proxy',
     install_requires=[
         'httpx>=0.21.0,<0.25.0',
-        'httpcore>=0.14.0,<0.18.0',
+        'httpcore>=0.17.3,<0.18.0',
         'python-socks>=2.0.0',
     ],
     extras_require={
         'asyncio': ['async-timeout>=3.0.1'],
         'trio': ['trio>=0.16.0'],
     }
 )
```

