# Comparing `tmp/strawberry_azure_auth-2.0.0.tar.gz` & `tmp/strawberry_azure_auth-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_azure_auth-2.0.0.tar", max compression
+gzip compressed data, was "strawberry_azure_auth-2.1.0.tar", max compression
```

## Comparing `strawberry_azure_auth-2.0.0.tar` & `strawberry_azure_auth-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/LICENSE
--rw-r--r--   0        0        0     3466 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/README.md
--rw-r--r--   0        0        0      957 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      167 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/__init__.py
--rw-r--r--   0        0        0      154 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/__init__.py
--rw-r--r--   0        0        0     2020 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/context.py
--rw-r--r--   0        0        0     2059 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/handlers.py
--rw-r--r--   0        0        0     8623 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/schema.py
--rw-r--r--   0        0        0        0 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/__init__.py
--rw-r--r--   0        0        0      905 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/context.py
--rw-r--r--   0        0        0     9431 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/extension.py
--rw-r--r--   0        0        0     5569 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/openid.py
--rw-r--r--   0        0        0     1159 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/permissions.py
--rw-r--r--   0        0        0      579 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/types.py
--rw-r--r--   0        0        0     1585 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/utils.py
--rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 strawberry_azure_auth-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3466 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/README.md
+-rw-r--r--   0        0        0      958 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/__init__.py
+-rw-r--r--   0        0        0     2020 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/context.py
+-rw-r--r--   0        0        0     2059 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/handlers.py
+-rw-r--r--   0        0        0     8623 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/schema.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/django/__init__.py
+-rw-r--r--   0        0        0      905 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/django/context.py
+-rw-r--r--   0        0        0     9382 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/extension.py
+-rw-r--r--   0        0        0     6118 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/openid.py
+-rw-r--r--   0        0        0     1159 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/permissions.py
+-rw-r--r--   0        0        0      579 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/types.py
+-rw-r--r--   0        0        0     1585 2023-07-06 13:18:34.468121 strawberry_azure_auth-2.1.0/strawberry_azure_auth/utils.py
+-rw-r--r--   0        0        0     4206 1970-01-01 00:00:00.000000 strawberry_azure_auth-2.1.0/PKG-INFO
```

### Comparing `strawberry_azure_auth-2.0.0/LICENSE` & `strawberry_azure_auth-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/README.md` & `strawberry_azure_auth-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/context.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/handlers.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/handlers.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/schema.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/channels/schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/context.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/django/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/extension.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 __all__ = ["AzureAuthExtension"]
 
 import jwt
-import asyncio
 import logging
 import contextlib
 from uuid import UUID
 from typing import Any
 from graphql import GraphQLError, ExecutionResult
 from strawberry.extensions.base_extension import SchemaExtension
 from strawberry.utils.await_maybe import AsyncIteratorOrIterator
@@ -75,32 +74,33 @@
         super().__init__(execution_context=execution_context)  # type: ignore[arg-type]
         self._client_id: str = client_id
         self._tenant_id: str = tenant_id
         self._scopes: list[str] = scopes.split(" ") if isinstance(scopes, str) else scopes if scopes else []
         self._roles: list[str] | None = roles
         self._allow_introspection: bool = allow_introspection
         self._allow_unauthorized: bool = allow_unauthorized
-        self._openid: OpenIDConfig = OpenIDConfig(
+        self._openid_config: OpenIDConfig = OpenIDConfig(
             client_id=client_id, tenant_id=tenant_id, enable_caching=enable_caching
         )
-        with contextlib.suppress(Exception):
-            asyncio.run_coroutine_threadsafe(coro=self._openid.load_config(), loop=asyncio.get_event_loop())
 
     async def on_operation(self) -> AsyncIteratorOrIterator[None]:
         """
         Hook that runs at the start/ end of every request/ operation:
         Authenticate incoming requests by validating the provided access tokens.
         """
         if not self.execution_context.context.authorized and (
             access_token := self.execution_context.context.access_token
         ):
             header: dict[str, str] = jwt.get_unverified_header(jwt=access_token)
             if kid := header.get("kid"):
-                await self._openid.load_config()
-                if (issuer := self._openid.issuer) and (signing_key := self._openid.signing_keys.get(kid)):
+                if not self._openid_config.up_to_date:
+                    await self._openid_config.update()
+                if (issuer := self._openid_config.issuer) and (
+                    signing_key := self._openid_config.signing_keys.get(kid)
+                ):
                     with contextlib.suppress(Exception):
                         claims: dict[str, Any] = self._validate_token(
                             token=access_token, signing_key=signing_key, issuer=issuer
                         )
                         self.execution_context.context.authorized = True
                         self.execution_context.context.upn = claims.get("upn")
                         self.execution_context.context.roles = claims.get("roles", [])
```

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/openid.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/openid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 __all__ = ["OpenIDConfig"]
 
 import httpx
 import logging
+import asyncio
 from typing import Final, TypedDict
 from datetime import datetime, timedelta
 from jwt.algorithms import RSAAlgorithm
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from django.core.cache import cache
 
 logger: logging.Logger = logging.getLogger(name="strawberry.auth")
@@ -62,14 +63,18 @@
 class JSONWebKeys(TypedDict):
     keys: list[JWK]
 
 
 # endregion
 
 
+# Asyncio lock used to handle concurrent calls to the `OpenIDConfig.update()` method.
+update_lock = asyncio.Lock()
+
+
 class OpenIDConfig:
     def __init__(self, client_id: str, tenant_id: str, enable_caching: bool = False) -> None:
         """
         :param client_id: Your Azure application's client ID.
         :param tenant_id: Your Azure tenant ID.
         :param enable_caching: Whether to cache the configuration using Django's built-in cache framework or not.
             Useful during development to avoid re-fetching the OpenID document every time the application restarts.
@@ -86,21 +91,26 @@
     @property
     def up_to_date(self) -> bool:
         if not self._last_update:
             return False
         expires: datetime = datetime.now() - timedelta(hours=24)
         return self._last_update > expires
 
-    async def load_config(self) -> None:
-        if bool(self.issuer and self.signing_keys and self.up_to_date):
-            return
-        try:
-            await self._load_openid_configuration()
-        except Exception as exc:
-            logger.error("Failed to update the OpenID configuration!", exc_info=exc)
+    async def update(self) -> None:
+        # lock the execution of this method to prevent multiple calls to the `_load_openid_configuration()` method:
+        # if multiple requests are made when the configuration is not up-to-date,
+        # the first one will update the config while the others will wait for the update to finish.
+        async with update_lock:
+            if bool(self.issuer and self.signing_keys and self.up_to_date):
+                return
+            try:
+                logger.info("Updating the OpenID configuration...")
+                await self._load_openid_configuration()
+            except Exception as exc:
+                logger.error("Failed to update the OpenID configuration!", exc_info=exc)
 
     async def _load_openid_configuration(self) -> None:
         if self._use_cache:
             try:
                 cached_config: CacheValues
                 if cached_config := await cache.aget(CACHE_KEY):
                     logger.debug("Using OpenID config from cache...")
```

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/permissions.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/types.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/strawberry_azure_auth/utils.py` & `strawberry_azure_auth-2.1.0/strawberry_azure_auth/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-2.0.0/PKG-INFO` & `strawberry_azure_auth-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strawberry-azure-auth
-Version: 2.0.0
+Version: 2.1.0
 Summary: Azure AD authentication for Strawberry GraphQL
 Home-page: https://github.com/skarre-r/strawberry-azure-auth
 License: MIT
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
-Requires-Dist: strawberry-graphql-django (>=0.9.5)
-Requires-Dist: strawberry-graphql[channels] (>=0.187.4)
+Requires-Dist: strawberry-graphql-django (>=0.10.2)
+Requires-Dist: strawberry-graphql[channels] (>=0.193.1)
 Project-URL: Repository, https://github.com/skarre-r/strawberry-azure-auth
 Description-Content-Type: text/markdown
 
 # strawberry-azure-auth
 
 Azure AD authentication for [Strawberry GraphQL](https://github.com/strawberry-graphql/strawberry),
 inspired by [fastapi-azure-auth](https://github.com/Intility/fastapi-azure-auth).
```

