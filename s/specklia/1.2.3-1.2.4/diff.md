# Comparing `tmp/specklia-1.2.3.tar.gz` & `tmp/specklia-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.2.3.tar", last modified: Thu Jul  6 12:45:31 2023, max compression
+gzip compressed data, was "specklia-1.2.4.tar", last modified: Thu Jul  6 14:14:28 2023, max compression
```

## Comparing `specklia-1.2.3.tar` & `specklia-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:45:31.566882 specklia-1.2.3/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-06 12:45:24.000000 specklia-1.2.3/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 12:45:31.566882 specklia-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-06 12:45:24.000000 specklia-1.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 12:45:31.570881 specklia-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-06 12:45:24.000000 specklia-1.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:45:31.566882 specklia-1.2.3/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-06 12:45:24.000000 specklia-1.2.3/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-07-06 12:45:24.000000 specklia-1.2.3/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    35189 2023-07-06 12:45:24.000000 specklia-1.2.3/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:45:31.566882 specklia-1.2.3/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 12:45:31.000000 specklia-1.2.3/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-06 12:45:31.000000 specklia-1.2.3/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 12:45:31.000000 specklia-1.2.3/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-06 12:45:31.000000 specklia-1.2.3/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 12:45:31.000000 specklia-1.2.3/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 12:45:31.566882 specklia-1.2.3/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-07-06 12:45:24.000000 specklia-1.2.3/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-07-06 12:45:24.000000 specklia-1.2.3/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-06 14:14:24.000000 specklia-1.2.4/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 14:14:28.043358 specklia-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-06 14:14:24.000000 specklia-1.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 14:14:28.043358 specklia-1.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2364 2023-07-06 14:14:24.000000 specklia-1.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.039358 specklia-1.2.4/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35378 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-06 14:14:28.000000 specklia-1.2.4/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/tests/
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-07-06 14:14:24.000000 specklia-1.2.4/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-07-06 14:14:24.000000 specklia-1.2.4/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.2.3/LICENCE` & `specklia-1.2.4/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.2.3/PKG-INFO` & `specklia-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.2.3/README.md` & `specklia-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.2.3/setup.py` & `specklia-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.3/specklia/_websocket_helpers.py` & `specklia-1.2.4/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.3/specklia/client.py` & `specklia-1.2.4/specklia/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             >>> with open("our_auth_token.jwt") as fh:
             ...     user_auth_token = fh.read()
             >>> client = Specklia(auth_token=user_auth_token)
         """
         self.server_url = url
         self.auth_token = auth_token
         self._data_streaming_timeout_s = 3600
+        self._user_id = None
         _log.info('New Specklia client created.')
 
     @property
     def user_id(self: Specklia) -> str:
         """
         Retrieve your unique user ID.
 
@@ -72,21 +73,24 @@
         Please quote this ID when contacting support@earthwave.co.uk.
 
         Returns
         -------
         str
             Your unique user ID.
         """
-        response = requests.post(
-            self.server_url + "/users",
-            headers={"Authorization": "Bearer " + self.auth_token})
-        _check_response_ok(response)
-        user_id = response.json()
-        _log.info('retrieved own user_id %s.', user_id)
-        return user_id
+        if self._user_id is None:
+            response = requests.post(
+                self.server_url + "/users",
+                headers={"Authorization": "Bearer " + self.auth_token})
+            _check_response_ok(response)
+            self._user_id = response.json()
+            _log.info('retrieved own user_id %s.', self._user_id)
+        else:
+            _log.info('returned buffered user_id %s.', self._user_id)
+        return self._user_id
 
     def list_users(self: Specklia, group_id: str) -> pd.DataFrame:
         """
         List users within a group.
 
         You must have ADMIN permissions within the group in order to do this.
```

### Comparing `specklia-1.2.3/specklia.egg-info/PKG-INFO` & `specklia-1.2.4/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
```

### Comparing `specklia-1.2.3/tests/test_client.py` & `specklia-1.2.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.3/tests/test_websocket_helpers.py` & `specklia-1.2.4/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

