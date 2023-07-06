# Comparing `tmp/unbelievaboat-1.1.3.tar.gz` & `tmp/unbelievaboat-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.1.3.tar", last modified: Tue Jul  4 11:43:45 2023, max compression
+gzip compressed data, was "unbelievaboat-1.1.4.tar", last modified: Thu Jul  6 18:04:10 2023, max compression
```

## Comparing `unbelievaboat-1.1.3.tar` & `unbelievaboat-1.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.144811 unbelievaboat-1.1.3/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-04 11:43:45.143782 unbelievaboat-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-04 11:43:45.145835 unbelievaboat-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-04 11:43:08.000000 unbelievaboat-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:44.983973 unbelievaboat-1.1.3/unbelievaboat/
--rw-rw-rw-   0        0        0     7923 2023-07-04 11:42:36.000000 unbelievaboat-1.1.3/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.3/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.3/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.046474 unbelievaboat-1.1.3/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.3/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.3/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.3/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.057619 unbelievaboat-1.1.3/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      750 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.3/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1306 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2103 2023-07-04 11:42:22.000000 unbelievaboat-1.1.3/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.3/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.110528 unbelievaboat-1.1.3/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.3/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.141247 unbelievaboat-1.1.3/unbelievaboat/util/
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.3/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.3/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.3/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 11:43:45.017591 unbelievaboat-1.1.3/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-04 11:43:44.000000 unbelievaboat-1.1.3/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.379710 unbelievaboat-1.1.4/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3940 2023-07-06 18:04:10.378696 unbelievaboat-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-07-06 17:33:53.000000 unbelievaboat-1.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:04:10.379710 unbelievaboat-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-06 18:03:53.000000 unbelievaboat-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.324300 unbelievaboat-1.1.4/unbelievaboat/
+-rw-rw-rw-   0        0        0     7923 2023-07-04 11:42:36.000000 unbelievaboat-1.1.4/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3961 2023-07-06 18:02:48.000000 unbelievaboat-1.1.4/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.4/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.351711 unbelievaboat-1.1.4/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.4/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.4/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.4/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.361830 unbelievaboat-1.1.4/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.4/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-04 11:42:22.000000 unbelievaboat-1.1.4/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.4/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.4/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-04 11:42:22.000000 unbelievaboat-1.1.4/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2103 2023-07-06 17:44:57.000000 unbelievaboat-1.1.4/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.4/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.372069 unbelievaboat-1.1.4/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.4/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.376443 unbelievaboat-1.1.4/unbelievaboat/util/
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.4/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.4/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.4/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:04:10.347597 unbelievaboat-1.1.4/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3940 2023-07-06 18:04:10.000000 unbelievaboat-1.1.4/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-07-06 18:04:10.000000 unbelievaboat-1.1.4/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:04:10.000000 unbelievaboat-1.1.4/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 18:04:10.000000 unbelievaboat-1.1.4/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 18:04:10.000000 unbelievaboat-1.1.4/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.1.3/LICENSE` & `unbelievaboat-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/PKG-INFO` & `unbelievaboat-1.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
-[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&color=yellowgreen&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/unbelievaboat?style=for-the-badge&color=blueviolet&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
 
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
```

### Comparing `unbelievaboat-1.1.3/README.md` & `unbelievaboat-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
-[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&color=yellowgreen&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/unbelievaboat?style=for-the-badge&color=blueviolet&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
 
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
```

### Comparing `unbelievaboat-1.1.3/setup.py` & `unbelievaboat-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.1.3",
+    version="1.1.4",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.1.3/unbelievaboat/Client.py` & `unbelievaboat-1.1.4/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.1.4/unbelievaboat/RequestHandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,75 @@
 import asyncio
 import time
 from typing import Any, Dict, Optional
 
 from .errors import APIError, HTTPError
+import re
 
 
 class RequestHandler:
     def __init__(self, client) -> None:
         self._client = client
         self.locks: Dict[str, asyncio.Lock] = {}
+        self.timeouts: Dict[str, float] = {}
 
     def __str__(self) -> str:
         return "<RequestHandler>"
 
+    def get_route(self, method: str, endpoint: str) -> str:
+        major_params = ["guilds"]
+        route = re.sub(
+            r"/([a-z-]+)/(?:(\d+))",
+            lambda match: match.group()
+            if match.group(1) in major_params
+            else f"/{match.group(1)}/:id",
+            endpoint,
+        )
+        return f"{method}/{route}"
+
+    def get_url(self, endpoint: str) -> str:
+        return "{}/{}/{}".format(self._client.base_url, self._client.version, endpoint)
+
+    def get_data(
+        self,
+        url: str,
+        method: str,
+        data: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        return {
+            "headers": {
+                "Authorization": self._client.token,
+                "Content-Type": "application/json",
+            },
+            "url": url,
+            "method": method,
+            "json": data,
+            "params": params,
+        }
+
+    async def check_ratelimit(self, route: str) -> None:
+        if route in self.timeouts:
+            timeout = self.timeouts[route] - time.time()
+            if timeout > 0:
+                await asyncio.sleep(timeout)
+            del self.timeouts[route]
+
+    def handle_ratelimit(self, route: str, response: Dict[str, Any]) -> None:
+        remaining = int(response.headers.get("x-ratelimit-remaining", 0))
+        if remaining <= 0:
+            if response.headers.get("retry-after"):
+                self.timeouts[route] = (
+                    time.time() + float(response.headers.get("retry-after", 0)) / 1000
+                )
+            else:
+                self.timeouts[route] = (
+                    float(response.headers.get("x-ratelimit-reset", 0)) / 1000
+                )
+
     async def request(
         self,
         method: str,
         endpoint: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
         _attempts: int = 0,
@@ -35,67 +88,32 @@
         method: str,
         endpoint: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
         _attempts: int = 0,
     ):
         async with self.locks[route]:
-            url = "{}/{}/{}".format(
-                self._client.base_url, self._client.version, endpoint
-            )
-            options = {
-                "headers": {
-                    "Authorization": self._client.token,
-                    "Content-Type": "application/json",
-                },
-                "url": url,
-                "method": method,
-                "json": data,
-                "params": params,
-            }
+            await self.check_ratelimit(route)
+
+            url = self.get_url(endpoint)
+            options = self.get_data(url, method, data, params)
 
             async with self._client._session.request(
                 **options
             ) as response:  # type: ClientResponse
                 _attempts += 1
 
-                # Handle rate limits
-                await self.parse_rate_limit_headers(response.headers)
+                self.handle_ratelimit(route, response)
 
                 if response.status >= 200 and response.status < 300:
                     try:
                         return await response.json()
                     except Exception as e:
                         return await response.text()
 
                 if response.status == 429:
                     if _attempts >= self._client._max_retries:
                         raise APIError(await response.json(), response)
                     else:
                         await self.request(method, endpoint, data, params, _attempts)
 
                 raise HTTPError(await response.json(), response)
-
-    def get_route(self, method: str, endpoint: str) -> str:
-        import re
-
-        major_params = ["guilds"]
-        route = re.sub(
-            r"/([a-z-]+)/(?:(\d+))",
-            lambda match: match.group()
-            if match.group(1) in major_params
-            else f"/{match.group(1)}/:id",
-            endpoint,
-        )
-        return f"{method}/{route}"
-
-    async def parse_rate_limit_headers(self, headers: Dict[str, str]) -> None:
-        remaining = int(headers.get("x-ratelimit-remaining", 0))
-        if remaining <= 0:
-            if headers.get("retry-after"):
-                retry_after = float(headers.get("retry-after", 0)) / 1000
-                await asyncio.sleep(retry_after)
-            else:
-                reset_after = (
-                    float(headers.get("x-ratelimit-reset", 0)) / 1000 - time.time()
-                )
-                await asyncio.sleep(reset_after)
```

### Comparing `unbelievaboat-1.1.3/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.1.4/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/Store.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/UserInventory.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/items/InventoryItem.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/items/InventoryItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.1.4/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.1.4/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.3/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.1.4/unbelievaboat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.3
+Version: 1.1.4
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UnbelievaBoat API Python Wrapper
 
 [![Discord Server](https://img.shields.io/discord/746360067632136222?label=discord&style=for-the-badge&logo=discord&color=5865F2&logoColor=white)](https://discord.gg/yoggies)
 [![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/downloads/release/python-380/)
-[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Version](https://img.shields.io/pypi/v/unbelievaboat.svg?style=for-the-badge&color=yellowgreen&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/unbelievaboat?style=for-the-badge&color=blueviolet&logo=pypi&logoColor=white)](https://pypi.org/project/unbelievaboat/)
+
 
 This is a Python wrapper for the UnbelievaBoat API, which provides access to the UnbelievaBoat Discord bot functionality. It allows you to interact with the API endpoints to retrieve guild information, user balances, leaderboard data, and more.
 
 ## Requirements
 
 - Python 3.8 or higher
```

### Comparing `unbelievaboat-1.1.3/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.1.4/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

