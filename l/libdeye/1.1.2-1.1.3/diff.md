# Comparing `tmp/libdeye-1.1.2.tar.gz` & `tmp/libdeye-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdeye-1.1.2.tar", last modified: Thu Apr  6 14:23:12 2023, max compression
+gzip compressed data, was "libdeye-1.1.3.tar", last modified: Thu Jul  6 08:55:24 2023, max compression
```

## Comparing `libdeye-1.1.2.tar` & `libdeye-1.1.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.178732 libdeye-1.1.2/
--rw-r--r--   0 stackia    (501) staff       (20)      590 2023-02-26 14:57:53.000000 libdeye-1.1.2/.coveragerc
--rw-r--r--   0 stackia    (501) staff       (20)      571 2023-02-26 16:02:46.000000 libdeye-1.1.2/.gitignore
--rw-r--r--   0 stackia    (501) staff       (20)      856 2023-04-05 08:40:07.000000 libdeye-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 stackia    (501) staff       (20)      530 2023-02-26 14:57:53.000000 libdeye-1.1.2/.readthedocs.yml
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.173770 libdeye-1.1.2/.vscode/
--rw-r--r--   0 stackia    (501) staff       (20)      166 2023-03-19 19:27:54.000000 libdeye-1.1.2/.vscode/settings.json
--rw-r--r--   0 stackia    (501) staff       (20)       74 2023-02-26 14:57:53.000000 libdeye-1.1.2/AUTHORS.rst
--rw-r--r--   0 stackia    (501) staff       (20)      373 2023-03-19 19:46:01.000000 libdeye-1.1.2/CHANGELOG.rst
--rw-r--r--   0 stackia    (501) staff       (20)    11761 2023-02-26 15:37:09.000000 libdeye-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 stackia    (501) staff       (20)     1078 2023-02-26 14:57:53.000000 libdeye-1.1.2/LICENSE.txt
--rw-r--r--   0 stackia    (501) staff       (20)     3671 2023-04-06 14:23:12.178832 libdeye-1.1.2/PKG-INFO
--rw-r--r--   0 stackia    (501) staff       (20)     3088 2023-03-19 20:08:15.000000 libdeye-1.1.2/README.rst
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.175542 libdeye-1.1.2/docs/
--rw-r--r--   0 stackia    (501) staff       (20)     1154 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/Makefile
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.175674 libdeye-1.1.2/docs/_static/
--rw-r--r--   0 stackia    (501) staff       (20)       18 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/_static/.gitignore
--rw-r--r--   0 stackia    (501) staff       (20)       41 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/authors.rst
--rw-r--r--   0 stackia    (501) staff       (20)       43 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/changelog.rst
--rw-r--r--   0 stackia    (501) staff       (20)     9722 2023-02-26 16:45:33.000000 libdeye-1.1.2/docs/conf.py
--rw-r--r--   0 stackia    (501) staff       (20)       33 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/contributing.rst
--rw-r--r--   0 stackia    (501) staff       (20)     1329 2023-02-26 16:59:23.000000 libdeye-1.1.2/docs/index.rst
--rw-r--r--   0 stackia    (501) staff       (20)       67 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/license.rst
--rw-r--r--   0 stackia    (501) staff       (20)       39 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/readme.rst
--rw-r--r--   0 stackia    (501) staff       (20)      233 2023-02-26 14:57:53.000000 libdeye-1.1.2/docs/requirements.txt
--rw-r--r--   0 stackia    (501) staff       (20)      683 2023-02-26 16:44:23.000000 libdeye-1.1.2/mypy.ini
--rw-r--r--   0 stackia    (501) staff       (20)      378 2023-02-26 16:13:36.000000 libdeye-1.1.2/pyproject.toml
--rw-r--r--   0 stackia    (501) staff       (20)     1334 2023-04-06 14:23:12.179196 libdeye-1.1.2/setup.cfg
--rw-r--r--   0 stackia    (501) staff       (20)      702 2023-02-26 14:57:53.000000 libdeye-1.1.2/setup.py
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.170535 libdeye-1.1.2/src/
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.177145 libdeye-1.1.2/src/libdeye/
--rw-r--r--   0 stackia    (501) staff       (20)      700 2023-02-26 16:36:42.000000 libdeye-1.1.2/src/libdeye/__init__.py
--rw-r--r--   0 stackia    (501) staff       (20)     5633 2023-02-26 16:35:31.000000 libdeye-1.1.2/src/libdeye/cloud_api.py
--rw-r--r--   0 stackia    (501) staff       (20)     9906 2023-03-19 19:27:54.000000 libdeye-1.1.2/src/libdeye/const.py
--rw-r--r--   0 stackia    (501) staff       (20)     4263 2023-02-26 16:22:13.000000 libdeye-1.1.2/src/libdeye/device_state_command.py
--rw-r--r--   0 stackia    (501) staff       (20)     5026 2023-03-19 19:27:54.000000 libdeye-1.1.2/src/libdeye/mqtt_client.py
--rw-r--r--   0 stackia    (501) staff       (20)     2853 2023-04-06 14:22:10.000000 libdeye-1.1.2/src/libdeye/types.py
--rw-r--r--   0 stackia    (501) staff       (20)      503 2023-02-26 18:12:38.000000 libdeye-1.1.2/src/libdeye/utils.py
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.178034 libdeye-1.1.2/src/libdeye.egg-info/
--rw-r--r--   0 stackia    (501) staff       (20)     3671 2023-04-06 14:23:12.000000 libdeye-1.1.2/src/libdeye.egg-info/PKG-INFO
--rw-r--r--   0 stackia    (501) staff       (20)      837 2023-04-06 14:23:12.000000 libdeye-1.1.2/src/libdeye.egg-info/SOURCES.txt
--rw-r--r--   0 stackia    (501) staff       (20)        1 2023-04-06 14:23:12.000000 libdeye-1.1.2/src/libdeye.egg-info/dependency_links.txt
--rw-r--r--   0 stackia    (501) staff       (20)        1 2023-02-26 15:02:05.000000 libdeye-1.1.2/src/libdeye.egg-info/not-zip-safe
--rw-r--r--   0 stackia    (501) staff       (20)      174 2023-04-06 14:23:12.000000 libdeye-1.1.2/src/libdeye.egg-info/requires.txt
--rw-r--r--   0 stackia    (501) staff       (20)        8 2023-04-06 14:23:12.000000 libdeye-1.1.2/src/libdeye.egg-info/top_level.txt
-drwxr-xr-x   0 stackia    (501) staff       (20)        0 2023-04-06 14:23:12.178520 libdeye-1.1.2/tests/
--rw-r--r--   0 stackia    (501) staff       (20)      275 2023-02-26 14:57:53.000000 libdeye-1.1.2/tests/conftest.py
--rw-r--r--   0 stackia    (501) staff       (20)     1077 2023-02-26 16:09:26.000000 libdeye-1.1.2/tests/test_device_state_command.py
--rw-r--r--   0 stackia    (501) staff       (20)      516 2023-02-26 16:40:48.000000 libdeye-1.1.2/tests/test_utils.py
--rw-r--r--   0 stackia    (501) staff       (20)     2741 2023-02-26 16:05:12.000000 libdeye-1.1.2/tox.ini
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.764637 libdeye-1.1.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      590 2023-07-06 06:06:20.000000 libdeye-1.1.3/.coveragerc
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      571 2023-07-06 06:06:20.000000 libdeye-1.1.3/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      856 2023-07-06 06:06:20.000000 libdeye-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      530 2023-07-06 06:06:20.000000 libdeye-1.1.3/.readthedocs.yml
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.762637 libdeye-1.1.3/.vscode/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      301 2023-07-06 08:14:32.000000 libdeye-1.1.3/.vscode/settings.json
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       74 2023-07-06 06:06:20.000000 libdeye-1.1.3/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      518 2023-07-06 08:53:07.000000 libdeye-1.1.3/CHANGELOG.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11761 2023-07-06 06:06:20.000000 libdeye-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1078 2023-07-06 06:06:20.000000 libdeye-1.1.3/LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3671 2023-07-06 08:55:24.764637 libdeye-1.1.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3088 2023-07-06 06:06:20.000000 libdeye-1.1.3/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.763637 libdeye-1.1.3/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1154 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/Makefile
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.763637 libdeye-1.1.3/docs/_static/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       18 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/_static/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       41 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/authors.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       43 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/changelog.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9722 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1329 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       67 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/license.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      233 2023-07-06 06:06:20.000000 libdeye-1.1.3/docs/requirements.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      683 2023-07-06 06:06:20.000000 libdeye-1.1.3/mypy.ini
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      378 2023-07-06 07:01:22.000000 libdeye-1.1.3/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1377 2023-07-06 08:55:24.764637 libdeye-1.1.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      702 2023-07-06 06:06:20.000000 libdeye-1.1.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.761637 libdeye-1.1.3/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.763637 libdeye-1.1.3/src/libdeye/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      700 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5862 2023-07-06 08:31:45.000000 libdeye-1.1.3/src/libdeye/cloud_api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9906 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4263 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/device_state_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5026 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/mqtt_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-07-06 07:58:05.000000 libdeye-1.1.3/src/libdeye/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2853 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/types.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      503 2023-07-06 06:06:20.000000 libdeye-1.1.3/src/libdeye/utils.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.764637 libdeye-1.1.3/src/libdeye.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3671 2023-07-06 08:55:24.000000 libdeye-1.1.3/src/libdeye.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      858 2023-07-06 08:55:24.000000 libdeye-1.1.3/src/libdeye.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-06 08:55:24.000000 libdeye-1.1.3/src/libdeye.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-06 06:40:31.000000 libdeye-1.1.3/src/libdeye.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      174 2023-07-06 08:55:24.000000 libdeye-1.1.3/src/libdeye.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-06 08:55:24.000000 libdeye-1.1.3/src/libdeye.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-06 08:55:24.764637 libdeye-1.1.3/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      275 2023-07-06 06:06:20.000000 libdeye-1.1.3/tests/conftest.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1077 2023-07-06 06:06:20.000000 libdeye-1.1.3/tests/test_device_state_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      516 2023-07-06 06:06:20.000000 libdeye-1.1.3/tests/test_utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2741 2023-07-06 06:06:20.000000 libdeye-1.1.3/tox.ini
```

### Comparing `libdeye-1.1.2/.coveragerc` & `libdeye-1.1.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/.gitignore` & `libdeye-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/.pre-commit-config.yaml` & `libdeye-1.1.3/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     hooks:
       - id: flake8
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.1
     hooks:
       - id: mypy
         exclude: ^docs/
```

### Comparing `libdeye-1.1.2/.readthedocs.yml` & `libdeye-1.1.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/CONTRIBUTING.rst` & `libdeye-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/LICENSE.txt` & `libdeye-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/PKG-INFO` & `libdeye-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdeye
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library to connect to Deye Cloud and control Deye dehumidifier devices.
 Home-page: https://github.com/stackia/libdeye/
 Author: Stackie Jia
 Author-email: jsq2627@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stackia/libdeye/
 Platform: any
```

### Comparing `libdeye-1.1.2/README.rst` & `libdeye-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/docs/Makefile` & `libdeye-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/docs/conf.py` & `libdeye-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/docs/index.rst` & `libdeye-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/mypy.ini` & `libdeye-1.1.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/setup.cfg` & `libdeye-1.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	aiohttp>=3.8,<4.0
 	PyJWT>=2.0,<3.0
 	paho-mqtt>=1.6,<2
 
+[options.package_data]
+libdeye = py.typed
+
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 testing =
```

### Comparing `libdeye-1.1.2/setup.py` & `libdeye-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye/__init__.py` & `libdeye-1.1.3/src/libdeye/__init__.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye/cloud_api.py` & `libdeye-1.1.3/src/libdeye/cloud_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,25 +102,30 @@
                 f"{DEYE_API_END_USER_ENDPOINT}/refreshToken/",
                 data={"token": self.auth_token},
             )
             result: DeyeApiResponseEnvelope = await response.json()
         except ClientError as err:
             raise DeyeCloudApiCannotConnectError from err
 
-        ensure_valid_response_code(result)
-
         try:
+            ensure_valid_response_code(result)
             token = result["data"]["token"]
             if token:
                 self.auth_token = token
                 if self.on_auth_token_refreshed:
                     self.on_auth_token_refreshed(token)
-                return
+            return
+        except DeyeCloudApiInvalidAuthError:
+            await self.authenticate()
+            if self.auth_token and self.on_auth_token_refreshed:
+                self.on_auth_token_refreshed(self.auth_token)
+            return
         except KeyError:
             pass
+
         raise DeyeCloudApiInvalidAuthError
 
     async def get_device_list(self) -> list[DeyeApiResponseDeviceInfo]:
         """Get all connected devices for current user"""
         await self.refresh_token_if_near_expiry()
 
         try:
```

### Comparing `libdeye-1.1.2/src/libdeye/const.py` & `libdeye-1.1.3/src/libdeye/const.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye/device_state_command.py` & `libdeye-1.1.3/src/libdeye/device_state_command.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye/mqtt_client.py` & `libdeye-1.1.3/src/libdeye/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye/types.py` & `libdeye-1.1.3/src/libdeye/types.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/src/libdeye.egg-info/PKG-INFO` & `libdeye-1.1.3/src/libdeye.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdeye
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Python library to connect to Deye Cloud and control Deye dehumidifier devices.
 Home-page: https://github.com/stackia/libdeye/
 Author: Stackie Jia
 Author-email: jsq2627@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/stackia/libdeye/
 Platform: any
```

### Comparing `libdeye-1.1.2/src/libdeye.egg-info/SOURCES.txt` & `libdeye-1.1.3/src/libdeye.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/requirements.txt
 docs/_static/.gitignore
 src/libdeye/__init__.py
 src/libdeye/cloud_api.py
 src/libdeye/const.py
 src/libdeye/device_state_command.py
 src/libdeye/mqtt_client.py
+src/libdeye/py.typed
 src/libdeye/types.py
 src/libdeye/utils.py
 src/libdeye.egg-info/PKG-INFO
 src/libdeye.egg-info/SOURCES.txt
 src/libdeye.egg-info/dependency_links.txt
 src/libdeye.egg-info/not-zip-safe
 src/libdeye.egg-info/requires.txt
```

### Comparing `libdeye-1.1.2/tests/test_device_state_command.py` & `libdeye-1.1.3/tests/test_device_state_command.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/tests/test_utils.py` & `libdeye-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libdeye-1.1.2/tox.ini` & `libdeye-1.1.3/tox.ini`

 * *Files identical despite different names*

