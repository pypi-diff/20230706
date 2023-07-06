# Comparing `tmp/gdata-vaas-3.1.0.tar.gz` & `tmp/gdata-vaas-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-3.1.0.tar", last modified: Wed May 17 13:08:20 2023, max compression
+gzip compressed data, was "gdata-vaas-3.2.0.tar", last modified: Thu Jul  6 12:40:32 2023, max compression
```

## Comparing `gdata-vaas-3.1.0.tar` & `gdata-vaas-3.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.760342 gdata-vaas-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-17 13:08:20.000000 gdata-vaas-3.1.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      938 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11198 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:08:20.764343 gdata-vaas-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8305 2023-05-17 13:07:32.000000 gdata-vaas-3.1.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2545 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.003340 gdata-vaas-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.007341 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3089 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-07-06 12:40:32.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-06 12:40:31.000000 gdata-vaas-3.2.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11337 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 12:40:32.011341 gdata-vaas-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9579 2023-07-06 12:39:48.000000 gdata-vaas-3.2.0/tests/test_vaas.py
```

### Comparing `gdata-vaas-3.1.0/LICENSE` & `gdata-vaas-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.1.0/PKG-INFO` & `gdata-vaas-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.1.0
+Version: 3.2.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.1.0/README.md` & `gdata-vaas-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.1.0/setup.cfg` & `gdata-vaas-3.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 3.1.0
+version = 3.2.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls =
```

### Comparing `gdata-vaas-3.1.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata-vaas-3.2.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 3.1.0
+Version: 3.2.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-3.1.0/src/vaas/__init__.py` & `gdata-vaas-3.2.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.1.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata-vaas-3.2.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.1.0/src/vaas/vaas.py` & `gdata-vaas-3.2.0/src/vaas/vaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         self.session_id = None
         self.results = {}
         self.httpx_client: Optional[httpx.AsyncClient] = None
         self.options = options
         self.url = url
 
     def get_authenticated_websocket(self):
+        """Get authenticated websocket"""        
         if self.websocket is None:
             raise VaasInvalidStateError("connect() was not called")
         if not self.websocket.open:
             raise VaasConnectionClosedError(
                 "connection closed or connect() was not awaited"
             )
         if self.session_id is None:
@@ -151,32 +152,32 @@
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, traceback):
         await self.close()
 
-    async def for_sha256(self, sha256, verdict_request_attributes=None):
+    async def for_sha256(self, sha256, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a SHA256 checksum"""
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
         return {
             "Sha256": verdict_response.get("sha256"),
             "Guid": verdict_response.get("guid"),
             "Verdict": verdict_response.get("verdict"),
         }
 
-    async def __for_sha256(self, sha256, verdict_request_attributes=None):
+    async def __for_sha256(self, sha256, verdict_request_attributes=None, guid=None):
         if verdict_request_attributes is not None and not isinstance(
             verdict_request_attributes, dict
         ):
             raise TypeError("verdict_request_attributes has to be dict(str, str)")
 
         websocket = self.get_authenticated_websocket()
         start = time.time()
-        guid = str(uuid.uuid4())
+        guid = guid or str(uuid.uuid4())
         verdict_request = {
             "kind": "VerdictRequest",
             "sha256": sha256,
             "session_id": self.session_id,
             "guid": guid,
             "use_shed": self.options.use_shed,
             "use_cache": self.options.use_cache,
@@ -208,23 +209,23 @@
                     guid = vaas_message.get("guid")
                     future = self.results.get(guid)
                     if future is not None:
                         future.set_result(vaas_message)
         except Exception as error:
             raise VaasConnectionClosedError(error) from error
 
-    async def for_buffer(self, buffer, verdict_request_attributes=None):
+    async def for_buffer(self, buffer, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a buffer"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(
             None, lambda: hashlib.sha256(buffer).hexdigest()
         )
 
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             verdict_response = await self._for_unknown_buffer(
                 verdict_response, buffer, len(buffer)
             )
 
@@ -245,21 +246,21 @@
             verdict_response = await asyncio.wait_for(response_message, timeout=TIMEOUT)
         except asyncio.TimeoutError as ex:
             self.tracing.trace_upload_result_timeout(buffer_len)
             raise VaasTimeoutError() from ex
         self.tracing.trace_upload_request(time.time() - start, buffer_len)
         return verdict_response
 
-    async def for_file(self, path, verdict_request_attributes=None):
+    async def for_file(self, path, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a file"""
 
         loop = asyncio.get_running_loop()
         sha256 = await loop.run_in_executor(None, lambda: hash_file(path))
 
-        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes)
+        verdict_response = await self.__for_sha256(sha256, verdict_request_attributes, guid)
         verdict = verdict_response.get("verdict")
 
         if verdict == "Unknown":
             async with aiofiles.open(path, mode="rb") as file:
                 buffer = await file.read()
                 verdict_response = await self._for_unknown_buffer(
                     verdict_response, buffer, len(buffer)
@@ -286,24 +287,24 @@
                 },
                 timeout=UPLOAD_TIMEOUT,
             )
         except httpx.TimeoutException as ex:
             self.tracing.trace_upload_timeout(content_length)
             raise VaasTimeoutError() from ex
 
-    async def for_url(self, url, verdict_request_attributes=None):
+    async def for_url(self, url, verdict_request_attributes=None, guid=None):
         """Returns the verdict for a file from an url"""
         if verdict_request_attributes is not None and not isinstance(
             verdict_request_attributes, dict
         ):
             raise TypeError("verdict_request_attributes has to be dict(str, str)")
 
         websocket = self.get_authenticated_websocket()
         start = time.time()
-        guid = str(uuid.uuid4())
+        guid = guid or str(uuid.uuid4())
         verdict_request_for_url = {
             "kind": "VerdictRequestForUrl",
             "url": url,
             "session_id": self.session_id,
             "guid": guid,
             "use_shed": self.options.use_shed,
             "use_cache": self.options.use_cache,
```

### Comparing `gdata-vaas-3.1.0/tests/test_client_credentials_grant_authenticator.py` & `gdata-vaas-3.2.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-3.1.0/tests/test_vaas.py` & `gdata-vaas-3.2.0/tests/test_vaas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=C0114,C0116,C0115
 import base64
 import hashlib
 import os
 import unittest
 from unittest.mock import MagicMock, ANY
+import uuid
 
 import websockets.client
 from dotenv import load_dotenv
 
 from src.vaas import Vaas, VaasTracing, VaasOptions, ClientCredentialsGrantAuthenticator
 from src.vaas import get_ssl_context
 from src.vaas.vaas import hash_file
@@ -87,107 +88,140 @@
         with self.assertRaises(VaasInvalidStateError):
             await vaas.for_sha256(
                 "275a021bbfb6489e54d471899f7db9d1663fc695ec2fe2a2c4538aabf651fd0f"
             )
 
     async def test_for_sha256_returns_malicious_for_eicar(self):
         async with await create_and_connect() as vaas:
+            guid = str(uuid.uuid4())
             verdict = await vaas.for_sha256(
-                "275a021bbfb6489e54d471899f7db9d1663fc695ec2fe2a2c4538aabf651fd0f"
+                "275a021bbfb6489e54d471899f7db9d1663fc695ec2fe2a2c4538aabf651fd0f",
+                guid=guid
             )
             self.assertEqual(verdict["Verdict"], "Malicious")
             self.assertEqual(
                 verdict["Sha256"].casefold(),
                 "275a021bbfb6489e54d471899f7db9d1663fc695ec2fe2a2c4538aabf651fd0f".casefold(),
+            self.assertEqual(verdict["Guid"].casefold(), guid)
             )
 
     async def test_for_sha256_returns_pup_for_amtso(self):
         async with await create_and_connect() as vaas:
+            guid = str(uuid.uuid4())
             verdict = await vaas.for_sha256(
-                "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad"
+                "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad",
+                guid=guid
             )
             self.assertEqual(verdict["Verdict"], "Pup")
             self.assertEqual(
                 verdict["Sha256"].casefold(),
                 "d6f6c6b9fde37694e12b12009ad11ab9ec8dd0f193e7319c523933bdad8a50ad".casefold(),
             )
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_buffer_returns_malicious_for_eicar(self):
         async with await create_and_connect() as vaas:
             buffer = base64.b64decode(EICAR_BASE64)
             sha256 = hashlib.sha256(buffer).hexdigest()
-            verdict = await vaas.for_buffer(buffer)
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_buffer(buffer, guid=guid)
             self.assertEqual(verdict["Verdict"], "Malicious")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_buffer_returns_unknown_for_random_buffer(self):
         async with await create_and_connect() as vaas:
             buffer = os.urandom(1024)
             sha256 = hashlib.sha256(buffer).hexdigest()
-            verdict = await vaas.for_buffer(buffer)
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_buffer(buffer, guid=guid)
             self.assertEqual(verdict["Verdict"], "Clean")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_file_returns_verdict(self):
         async with await create_and_connect() as vaas:
             with open("eicar.txt", "wb") as f:
                 f.write(base64.b64decode(EICAR_BASE64))
             sha256 = hash_file("eicar.txt")
-            verdict = await vaas.for_file("eicar.txt")
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_file("eicar.txt", guid=guid)
             self.assertEqual(verdict["Verdict"], "Malicious")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_file_returns_verdict_if_no_cache_or_shed(self):
         options = get_disabled_options()
 
         async with await create_and_connect(options=options) as vaas:
             with open("eicar.txt", "wb") as f:
                 f.write(base64.b64decode(EICAR_BASE64))
             sha256 = hash_file("eicar.txt")
-            verdict = await vaas.for_file("eicar.txt")
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_file("eicar.txt", guid=guid)
             self.assertEqual(verdict["Verdict"], "Malicious")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_url_returns_malicious_for_eicar(self):
         options = get_disabled_options()
         async with await create_and_connect(options=options) as vaas:
-            verdict = await vaas.for_url("https://secure.eicar.org/eicarcom2.zip")
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_url("https://secure.eicar.org/eicarcom2.zip", guid=guid)
             self.assertEqual(verdict["Verdict"], "Malicious")
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_url_without_shed_and_cache_returns_clean_for_random_beer(self):
         options = get_disabled_options()
         async with await create_and_connect(options=options) as vaas:
-            verdict = await vaas.for_url("https://random-data-api.com/api/v2/beers")
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_url("https://random-data-api.com/api/v2/beers", guid=guid)
             self.assertEqual(verdict["Verdict"], "Clean")
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_url_without_cache_returns_clean_for_random_beer(self):
         options = VaasOptions()
         options.use_cache = False
         options.use_shed = True
         async with await create_and_connect(options=options) as vaas:
-            verdict = await vaas.for_url("https://random-data-api.com/api/v2/beers")
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_url("https://random-data-api.com/api/v2/beers", guid=guid)
             self.assertEqual(verdict["Verdict"], "Clean")
+            self.assertEqual(verdict["Guid"].casefold(), guid)
+
 
     async def test_for_buffer_traces(self):
         tracing = VaasTracing()
         tracing.trace_hash_request = MagicMock()
         tracing.trace_upload_request = MagicMock()
         async with await create_and_connect(tracing=tracing) as vaas:
             buffer = os.urandom(1024)
             sha256 = hashlib.sha256(buffer).hexdigest()
-            verdict = await vaas.for_buffer(buffer)
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_buffer(buffer, guid=guid)
             self.assertEqual(verdict["Verdict"], "Clean")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
             tracing.trace_hash_request.assert_called_with(ANY)
             tracing.trace_upload_request.assert_called_with(ANY, 1024)
 
+
     async def test_for_empty_buffer_returns_clean(self):
         async with await create_and_connect() as vaas:
             buffer = bytes("", "utf-8")
             sha256 = hashlib.sha256(buffer).hexdigest()
-            verdict = await vaas.for_buffer(buffer)
+            guid = str(uuid.uuid4())
+            verdict = await vaas.for_buffer(buffer, guid=guid)
             self.assertEqual(verdict["Verdict"], "Clean")
             self.assertEqual(verdict["Sha256"].casefold(), sha256.casefold())
+            self.assertEqual(verdict["Guid"].casefold(), guid)
 
 
 if __name__ == "__main__":
     unittest.main()
```

