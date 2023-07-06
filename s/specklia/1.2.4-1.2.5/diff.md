# Comparing `tmp/specklia-1.2.4.tar.gz` & `tmp/specklia-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.2.4.tar", last modified: Thu Jul  6 14:14:28 2023, max compression
+gzip compressed data, was "specklia-1.2.5.tar", last modified: Thu Jul  6 16:02:19 2023, max compression
```

## Comparing `specklia-1.2.4.tar` & `specklia-1.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-06 14:14:24.000000 specklia-1.2.4/LICENCE
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 14:14:28.043358 specklia-1.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-06 14:14:24.000000 specklia-1.2.4/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 14:14:28.043358 specklia-1.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2364 2023-07-06 14:14:24.000000 specklia-1.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.039358 specklia-1.2.4/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/_websocket_helpers.py
--rw-r--r--   0 root         (0) root         (0)    35378 2023-07-06 14:14:24.000000 specklia-1.2.4/specklia/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-07-06 14:14:28.000000 specklia-1.2.4/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 14:14:27.000000 specklia-1.2.4/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:14:28.043358 specklia-1.2.4/tests/
--rw-r--r--   0 root         (0) root         (0)    10184 2023-07-06 14:14:24.000000 specklia-1.2.4/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6632 2023-07-06 14:14:24.000000 specklia-1.2.4/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:02:19.899925 specklia-1.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-06 16:02:15.000000 specklia-1.2.5/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-06 16:02:19.899925 specklia-1.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-06 16:02:15.000000 specklia-1.2.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-07-06 16:02:19.899925 specklia-1.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-06 16:02:15.000000 specklia-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:02:19.899925 specklia-1.2.5/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-06 16:02:15.000000 specklia-1.2.5/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-07-06 16:02:15.000000 specklia-1.2.5/specklia/_websocket_helpers.py
+-rw-r--r--   0 root         (0) root         (0)    35318 2023-07-06 16:02:15.000000 specklia-1.2.5/specklia/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:02:19.899925 specklia-1.2.5/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-06 16:02:19.000000 specklia-1.2.5/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-07-06 16:02:19.000000 specklia-1.2.5/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:02:19.000000 specklia-1.2.5/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-06 16:02:19.000000 specklia-1.2.5/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 16:02:19.000000 specklia-1.2.5/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:02:19.899925 specklia-1.2.5/tests/
+-rw-r--r--   0 root         (0) root         (0)    10232 2023-07-06 16:02:15.000000 specklia-1.2.5/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6632 2023-07-06 16:02:15.000000 specklia-1.2.5/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.2.4/LICENCE` & `specklia-1.2.5/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.2.4/PKG-INFO` & `specklia-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
-Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
+Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/change_log.html
 Project-URL: Documentation, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Twitter, https://twitter.com/earth__wave
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `specklia-1.2.4/README.md` & `specklia-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.2.4/setup.py` & `specklia-1.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     url='https://specklia.earthwave.co.uk/static/docs/index.html',
     python_requires=">=3.9",
     license='MIT',
     packages=find_packages(),
     # These generate the icons in the sidebar on PyPI
     project_urls={
         'Homepage': 'https://specklia.earthwave.co.uk/static/docs/index.html',
-        'Changelog': 'https://specklia.earthwave.co.uk/static/docs/changelog.html',
+        'Changelog': 'https://specklia.earthwave.co.uk/static/docs/change_log.html',
         'Documentation': 'https://specklia.earthwave.co.uk/static/docs/index.html',
         'Twitter': 'https://twitter.com/earth__wave'
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 3.9',
         'Topic :: Database :: Front-Ends',
```

### Comparing `specklia-1.2.4/specklia/_websocket_helpers.py` & `specklia-1.2.5/specklia/_websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.2.4/specklia/client.py` & `specklia-1.2.5/specklia/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             auth_token: str,
             url: str = 'https://specklia.earthwave.co.uk') -> None:
         """
         Create a new Specklia client object.
 
         This object is a Python client for connecting to Specklia's API.
 
+        Giving the value of this object's user_id to another user will allow them to add you to private groups.
+        Please quote your user_id when contacting support@earthwave.co.uk.
+
         Parameters
         ----------
         auth_token : str
             The authentication token to use to authorise calls to Specklia.
             Obtained via https://specklia.earthwave.co.uk.
         url : str
             The url where Specklia is running, by default the URL of the Specklia server.
@@ -57,40 +60,31 @@
             >>> with open("our_auth_token.jwt") as fh:
             ...     user_auth_token = fh.read()
             >>> client = Specklia(auth_token=user_auth_token)
         """
         self.server_url = url
         self.auth_token = auth_token
         self._data_streaming_timeout_s = 3600
-        self._user_id = None
+        # immediately retrieve the user's ID. This serves as a check that their API token is valid.
+        self._fetch_user_id()
+
         _log.info('New Specklia client created.')
 
-    @property
-    def user_id(self: Specklia) -> str:
+    def _fetch_user_id(self: Specklia) -> None:
         """
-        Retrieve your unique user ID.
-
-        Giving this to another user will allow them to add you to private groups.
-        Please quote this ID when contacting support@earthwave.co.uk.
+        Set the client's User ID.
 
-        Returns
-        -------
-        str
-            Your unique user ID.
+        We've separated this out for testing reasons.
         """
-        if self._user_id is None:
-            response = requests.post(
-                self.server_url + "/users",
-                headers={"Authorization": "Bearer " + self.auth_token})
-            _check_response_ok(response)
-            self._user_id = response.json()
-            _log.info('retrieved own user_id %s.', self._user_id)
-        else:
-            _log.info('returned buffered user_id %s.', self._user_id)
-        return self._user_id
+        response = requests.post(
+            self.server_url + "/users",
+            headers={"Authorization": "Bearer " + self.auth_token})
+        _check_response_ok(response)
+        self.user_id = response.json()
+        _log.info('fetched User ID for client, was %s', self.user_id)
 
     def list_users(self: Specklia, group_id: str) -> pd.DataFrame:
         """
         List users within a group.
 
         You must have ADMIN permissions within the group in order to do this.
```

### Comparing `specklia-1.2.4/specklia.egg-info/PKG-INFO` & `specklia-1.2.5/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/static/docs/index.html
 Author: Earthwave Ltd
 Author-email: support@earthwave.co.uk
 License: MIT
 Project-URL: Homepage, https://specklia.earthwave.co.uk/static/docs/index.html
-Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/changelog.html
+Project-URL: Changelog, https://specklia.earthwave.co.uk/static/docs/change_log.html
 Project-URL: Documentation, https://specklia.earthwave.co.uk/static/docs/index.html
 Project-URL: Twitter, https://twitter.com/earth__wave
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `specklia-1.2.4/tests/test_client.py` & `specklia-1.2.5/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,28 @@
         'geometry': [Point(lon, lat) for lon, lat in zip([1, 2, 3, 4, 5], [0, 1, 2, 3, 4])],
         'timestamp': [2, 3, 4, 5, 6]},
         crs="EPSG:4326")
 
 
 @pytest.fixture()
 def test_client():
-    return Specklia(auth_token='fake_token', url='https://localhost')
+    with patch.object(Specklia, '_fetch_user_id'):
+        return Specklia(auth_token='fake_token', url='https://localhost')
 
 
 def test_create_client(test_client: Specklia):
     assert test_client is not None
 
 
 def test_user_id(test_client: Specklia, patched_requests_with_response: Dict[str, MagicMock]):
     patched_requests_with_response['response'].json.return_value = 'fake_user_id'
-    returned_user_id = test_client.user_id
+    test_client._fetch_user_id()
     patched_requests_with_response['requests'].post.assert_has_calls([
         call('https://localhost/users', headers={'Authorization': 'Bearer fake_token'})])
-    assert returned_user_id == 'fake_user_id'
+    assert test_client.user_id == 'fake_user_id'
 
 
 def test_list_users(test_client: Specklia, patched_requests_with_response: Dict[str, MagicMock]):
     patched_requests_with_response['response'].json.return_value = [{'name': 'fred', 'email': 'fred@fred.fred'}]
     test_client.list_users(group_id='hazbin')
     patched_requests_with_response['requests'].get.assert_has_calls([
         call('https://localhost/users', headers={'Authorization': 'Bearer fake_token'},
```

### Comparing `specklia-1.2.4/tests/test_websocket_helpers.py` & `specklia-1.2.5/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

