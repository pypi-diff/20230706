# Comparing `tmp/gestalt-cfg-3.3.0.tar.gz` & `tmp/gestalt-cfg-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gestalt-cfg-3.3.0.tar", last modified: Wed Jun 21 17:34:37 2023, max compression
+gzip compressed data, was "gestalt-cfg-3.3.1.tar", last modified: Thu Jul  6 18:37:03 2023, max compression
```

## Comparing `gestalt-cfg-3.3.0.tar` & `gestalt-cfg-3.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.277049 gestalt-cfg-3.3.0/gestalt/
--rw-r--r--   0 runner    (1001) docker     (123)    25398 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/gestalt/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:34:37.000000 gestalt-cfg-3.3.0/gestalt_cfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:37.281049 gestalt-cfg-3.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/test_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-21 17:34:10.000000 gestalt-cfg-3.3.0/tests/test_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.681786 gestalt-cfg-3.3.1/gestalt/
+-rw-r--r--   0 runner    (1001) docker     (123)    25382 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/gestalt/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 18:37:03.000000 gestalt-cfg-3.3.1/gestalt_cfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:37:03.685786 gestalt-cfg-3.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17698 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/test_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-06 18:36:34.000000 gestalt-cfg-3.3.1/tests/test_vault.py
```

### Comparing `gestalt-cfg-3.3.0/LICENSE` & `gestalt-cfg-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.0/PKG-INFO` & `gestalt-cfg-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.3.0
+Version: 3.3.1
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.3.0/README.md` & `gestalt-cfg-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.0/gestalt/__init__.py` & `gestalt-cfg-3.3.1/gestalt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from gestalt.vault import Vault  # noqa: E999
 from gestalt.provider import Provider
 import os
 import glob
 
-from typing import Dict, List, Type, Union, Optional, MutableMapping, Text, Any
+from typing import Dict, List, Type, Union, Optional, Text, Any
 import yaml
 import re
 import json
 
 from .utils import flatten
```

### Comparing `gestalt-cfg-3.3.0/gestalt/provider.py` & `gestalt-cfg-3.3.1/gestalt/provider.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.0/gestalt/utils.py` & `gestalt-cfg-3.3.1/gestalt/utils.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.0/gestalt/vault.py` & `gestalt-cfg-3.3.1/gestalt/vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime, timedelta
 from time import sleep
 from gestalt.provider import Provider
 import requests
 from jsonpath_ng import parse  # type: ignore
 from typing import Optional, Tuple, Any, Dict, Union, List
 import hvac  # type: ignore
-import asyncio
+from queue import Queue
 import os
 from threading import Thread
 from retry import retry
 
 
 class Vault(Provider):
     @retry(exceptions=RuntimeError, delay=2, tries=5)  # type: ignore
@@ -27,16 +27,16 @@
             client_config (HVAC_ClientConfig): initializes vault. URL can be set in VAULT_ADDR
                 environment variable, token can be set to VAULT_TOKEN environment variable.
                 These will be picked by default if not set to empty string
             auth_config (HVAC_ClientAuthentication): authenticates the initialized vault client
                 with role and jwt string from kubernetes
         """
         self._scheme: str = scheme
-        self.dynamic_token_queue: asyncio.Queue[Any] = asyncio.Queue(maxsize=0)
-        self.kubes_token_queue: asyncio.Queue[Any] = asyncio.Queue(maxsize=0)
+        self.dynamic_token_queue: Queue[Tuple[str, str, str]] = Queue()
+        self.kubes_token_queue: Queue[Tuple[str, str, str]] = Queue()
 
         self.vault_client = hvac.Client(url=url,
                                         token=token,
                                         cert=cert,
                                         verify=verify)
         self._secret_expiry_times: Dict[str, datetime] = dict()
         self._secret_values: Dict[str, Union[str, int, float, bool,
@@ -62,24 +62,23 @@
                     self.kubes_token_queue.put(kubes_token)
             except hvac.exceptions.InvalidPath:
                 raise RuntimeError(
                     "Gestalt Error: Kubernetes auth couldn't be performed")
             except requests.exceptions.ConnectionError:
                 raise RuntimeError("Gestalt Error: Couldn't connect to Vault")
 
-            dynamic_ttl_renew = Thread(name='dynamic-token-renew',
-                                       target=asyncio.run,
-                                       daemon=True,
-                                       args=(self.worker(
-                                           self.dynamic_token_queue), ))
+            dynamic_ttl_renew = Thread(
+                name='dynamic-token-renew',
+                target=self.worker,
+                daemon=True,
+                args=(self.dynamic_token_queue, ))  # noqa: F841
             kubernetes_ttl_renew = Thread(name="kubes-token-renew",
-                                          target=asyncio.run,
+                                          target=self.worker,
                                           daemon=True,
-                                          args=(self.worker(
-                                              self.kubes_token_queue), ))
+                                          args=(self.kubes_token_queue, ))
             kubernetes_ttl_renew.start()
 
     @retry(RuntimeError, delay=3, tries=3)  # type: ignore
     def get(
         self,
         key: str,
         path: str,
@@ -150,23 +149,23 @@
             ".")[0]  # to the nearest second
         last_vault_rotation_dt = datetime.strptime(last_vault_rotation_str,
                                                    '%Y-%m-%dT%H:%M:%S')
         ttl = requested_data["ttl"]
         secret_expires_dt = last_vault_rotation_dt + timedelta(seconds=ttl)
         self._secret_expiry_times[key] = secret_expires_dt
 
-    async def worker(self, token_queue: Any) -> None:
+    def worker(self, token_queue: Queue) -> None:  # type: ignore
         """
         Worker function to renew lease on expiry
         """
 
         try:
             while True:
                 if not token_queue.empty():
-                    token_type, token_id, token_duration = token = await token_queue.get(
+                    token_type, token_id, token_duration = token = token_queue.get(
                     )
                     if token_type == "kubernetes":
                         self.vault_client.auth.token.renew(token_id)
                         print("kubernetes token for the app has been renewed")
                     elif token_type == "dynamic":
                         self.vault_client.sys.renew_lease(token_id)
                         print("dynamic token for the app has been renewed")
```

### Comparing `gestalt-cfg-3.3.0/gestalt_cfg.egg-info/PKG-INFO` & `gestalt-cfg-3.3.1/gestalt_cfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gestalt-cfg
-Version: 3.3.0
+Version: 3.3.1
 Summary: A sensible configuration library for Python
 Home-page: https://github.com/clear-street/gestalt
 Author: Clear Street
 Author-email: engineering@clearstreet.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `gestalt-cfg-3.3.0/setup.py` & `gestalt-cfg-3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 with open("requirements.txt") as reqs_file:
     reqs = filter(lambda x: not x.startswith("-"), reqs_file.readlines())
     reqs_list = list(map(lambda x: x.rstrip(), reqs))
 
 setup(name='gestalt-cfg',
-      version='3.3.0',
+      version='3.3.1',
       description='A sensible configuration library for Python',
       long_description=readme(),
       long_description_content_type="text/markdown",
       url='https://github.com/clear-street/gestalt',
       author='Clear Street',
       author_email='engineering@clearstreet.io',
       license='MIT',
```

### Comparing `gestalt-cfg-3.3.0/tests/conftest.py` & `gestalt-cfg-3.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gestalt-cfg-3.3.0/tests/test_gestalt.py` & `gestalt-cfg-3.3.1/tests/test_gestalt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # type: ignore
 
 from unittest.mock import patch, Mock
 
 from gestalt.vault import Vault
 from gestalt import merge_into
-import asyncio
 import pytest
 import os
 import gestalt
 import hvac
+from queue import Queue
 
 
 # Testing member function
 def test_merge_into():
     combine1 = {}
     combine2 = {}
     combine3 = {"local": 1234, "pg": {"host": "dict1_pg", "pass": "dict1_pg"}}
@@ -537,16 +537,15 @@
     g.set_string(key="test",
                  value="ref+vault://secret/data/testnested#.slack.token")
     g.build_config()
     secret = g.get_string("test")
     assert secret == "ref+vault://secret/data/testnested#.slack.token"
 
 
-@pytest.mark.asyncio
-async def test_vault_worker_dynamic(mock_vault_workers, mock_vault_k8s_auth):
+def test_vault_worker_dynamic(mock_vault_workers, mock_vault_k8s_auth):
     mock_dynamic_renew, mock_k8s_renew = mock_vault_workers
 
     mock_sleep = None
 
     def except_once(self, **kwargs):
         # side effect used to exit the worker loop after one call
         if mock_sleep.call_count == 1:
@@ -556,30 +555,29 @@
                autospec=True) as mock_sleep:
 
         with patch("gestalt.vault.hvac.Client") as mock_client:
             v = Vault(role="test-role", jwt="test-jwt")
 
             mock_k8s_renew.start.assert_called()
 
-            test_token_queue = asyncio.Queue(maxsize=0)
-            await test_token_queue.put(("dynamic", 1, 100))
+            test_token_queue = Queue(maxsize=0)
+            test_token_queue.put(("dynamic", 1, 100))
 
             with pytest.raises(RuntimeError):
-                await v.worker(test_token_queue)
+                v.worker(test_token_queue)
 
             mock_sleep.assert_called()
             mock_client().sys.renew_lease.assert_called()
             mock_k8s_renew.start.assert_called_once()
 
             mock_dynamic_renew.stop()
             mock_k8s_renew.stop()
 
 
-@pytest.mark.asyncio
-async def test_vault_worker_k8s(mock_vault_workers):
+def test_vault_worker_k8s(mock_vault_workers):
     mock_dynamic_renew, mock_k8s_renew = mock_vault_workers
 
     mock_sleep = None
 
     def except_once(self, **kwargs):
         # side effect used to exit the worker loop after one call
         if mock_sleep.call_count == 1:
@@ -588,45 +586,44 @@
     with patch("gestalt.vault.sleep", side_effect=except_once,
                autospec=True) as mock_sleep:
         with patch("gestalt.vault.hvac.Client") as mock_client:
             v = Vault(role="test-role", jwt="test-jwt")
 
             mock_k8s_renew.start.assert_called()
 
-            test_token_queue = asyncio.Queue(maxsize=0)
-            await test_token_queue.put(("kubernetes", 1, 100))
+            test_token_queue = Queue(maxsize=0)
+            test_token_queue.put(("kubernetes", 1, 100))
 
             with pytest.raises(RuntimeError):
-                await v.worker(test_token_queue)
+                v.worker(test_token_queue)
 
             mock_sleep.assert_called()
             mock_client().auth.token.renew.assert_called()
             mock_k8s_renew.start.assert_called_once()
 
             mock_dynamic_renew.stop()
             mock_k8s_renew.stop()
 
 
-@pytest.mark.asyncio
-async def test_vault_start_dynamic_lease(mock_vault_workers):
+def test_vault_start_dynamic_lease(mock_vault_workers):
     mock_response = {
         "lease_id": "1",
         "lease_duration": 5,
         "data": {
             "data": "mock_data"
         }
     }
 
     mock_vault_client_patch = patch("gestalt.vault.hvac.Client.read",
                                     return_value=mock_response)
     with mock_vault_client_patch as mock_vault_client_read:
         mock_dynamic_token_queue = Mock()
         mock_kube_token_queue = Mock()
         with patch(
-                "gestalt.vault.asyncio.Queue",
+                "gestalt.vault.Queue",
                 side_effect=[mock_dynamic_token_queue,
                              mock_kube_token_queue]) as mock_queues:
 
             v = Vault(role=None, jwt=None)
             g = gestalt.Gestalt()
             g.add_config_file("./tests/testvault/testmount.json")
             g.configure_provider("vault", v)
```

### Comparing `gestalt-cfg-3.3.0/tests/test_vault.py` & `gestalt-cfg-3.3.1/tests/test_vault.py`

 * *Files identical despite different names*

