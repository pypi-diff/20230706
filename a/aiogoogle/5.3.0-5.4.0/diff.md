# Comparing `tmp/aiogoogle-5.3.0.tar.gz` & `tmp/aiogoogle-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogoogle-5.3.0.tar", last modified: Thu Apr  6 07:01:10 2023, max compression
+gzip compressed data, was "aiogoogle-5.4.0.tar", last modified: Thu Jul  6 04:09:48 2023, max compression
```

## Comparing `aiogoogle-5.3.0.tar` & `aiogoogle-5.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:01:10.794875 aiogoogle-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-06 07:01:10.794875 aiogoogle-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:01:10.790875 aiogoogle-5.3.0/aiogoogle/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:01:10.790875 aiogoogle-5.3.0/aiogoogle/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/auth/creds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/auth/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    49567 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/auth/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/auth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/excs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    35691 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:01:10.790875 aiogoogle-5.3.0/aiogoogle/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/aiohttp_session.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/curio_asks_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/sessions/trio_asks_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/aiogoogle/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:01:10.790875 aiogoogle-5.3.0/aiogoogle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-06 07:01:10.000000 aiogoogle-5.3.0/aiogoogle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-06 07:01:10.000000 aiogoogle-5.3.0/aiogoogle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 07:01:10.000000 aiogoogle-5.3.0/aiogoogle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-06 07:01:10.000000 aiogoogle-5.3.0/aiogoogle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 07:01:10.000000 aiogoogle-5.3.0/aiogoogle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-06 07:01:10.794875 aiogoogle-5.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-06 07:00:47.000000 aiogoogle-5.3.0/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/aiogoogle/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/aiogoogle/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/auth/creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/auth/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49567 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/auth/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/auth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14847 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/excs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15440 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35691 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/aiogoogle/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/aiohttp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/curio_asks_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/sessions/trio_asks_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/aiogoogle/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/aiogoogle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 04:09:48.000000 aiogoogle-5.4.0/aiogoogle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-06 04:09:48.000000 aiogoogle-5.4.0/aiogoogle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:09:48.000000 aiogoogle-5.4.0/aiogoogle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 04:09:48.000000 aiogoogle-5.4.0/aiogoogle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 04:09:48.000000 aiogoogle-5.4.0/aiogoogle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-06 04:09:48.564487 aiogoogle-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 04:09:39.000000 aiogoogle-5.4.0/test_requirements.txt
```

### Comparing `aiogoogle-5.3.0/LICENSE` & `aiogoogle-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/PKG-INFO` & `aiogoogle-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogoogle
-Version: 5.3.0
+Version: 5.4.0
 Summary: Async Google API client
 Home-page: https://github.com/omarryhan/aiogoogle
 Author: Omar Ryhan
 Author-email: omarryhan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiogoogle Version: 5.3.0 Summary: Async Google API
+Metadata-Version: 2.1 Name: aiogoogle Version: 5.4.0 Summary: Async Google API
 client Home-page: https://github.com/omarryhan/aiogoogle Author: Omar Ryhan
 Author-email: omarryhan@gmail.com License: MIT Classifier: Programming Language
 :: Python :: 3.7 Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown Provides-Extra: curio_asks Provides-Extra:
 trio_asks License-File: LICENSE
                                     [Logo]
   [Build_Status] [Software_License] [Code_style:_black] [Downloads] [Monthly
```

### Comparing `aiogoogle-5.3.0/README.md` & `aiogoogle-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/__init__.py` & `aiogoogle-5.4.0/aiogoogle/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/auth/creds.py` & `aiogoogle-5.4.0/aiogoogle/auth/creds.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/auth/data.py` & `aiogoogle-5.4.0/aiogoogle/auth/data.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/auth/managers.py` & `aiogoogle-5.4.0/aiogoogle/auth/managers.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/auth/utils.py` & `aiogoogle-5.4.0/aiogoogle/auth/utils.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/client.py` & `aiogoogle-5.4.0/aiogoogle/client.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/data.py` & `aiogoogle-5.4.0/aiogoogle/data.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/models.py` & `aiogoogle-5.4.0/aiogoogle/models.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/resource.py` & `aiogoogle-5.4.0/aiogoogle/resource.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/sessions/abc.py` & `aiogoogle-5.4.0/aiogoogle/sessions/abc.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/sessions/aiohttp_session.py` & `aiogoogle-5.4.0/aiogoogle/sessions/aiohttp_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             else:
                 if response.status != 204:  # If no (no content)
                     try:
                         json = await response.json()
                     except (JSONDecodeError, ContentTypeError):
                         try:
                             data = await response.text()
-                        except ContentTypeError:
+                        except (ContentTypeError, UnicodeDecodeError):
                             try:
                                 data = await response.read()
                             except ContentTypeError:
                                 data = None
 
             if request.media_upload:
                 upload_file = request.media_upload.file_path
```

### Comparing `aiogoogle-5.3.0/aiogoogle/sessions/curio_asks_session.py` & `aiogoogle-5.4.0/aiogoogle/sessions/curio_asks_session.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/sessions/trio_asks_session.py` & `aiogoogle-5.4.0/aiogoogle/sessions/trio_asks_session.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/utils.py` & `aiogoogle-5.4.0/aiogoogle/utils.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle/validate.py` & `aiogoogle-5.4.0/aiogoogle/validate.py`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/aiogoogle.egg-info/PKG-INFO` & `aiogoogle-5.4.0/aiogoogle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogoogle
-Version: 5.3.0
+Version: 5.4.0
 Summary: Async Google API client
 Home-page: https://github.com/omarryhan/aiogoogle
 Author: Omar Ryhan
 Author-email: omarryhan@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiogoogle Version: 5.3.0 Summary: Async Google API
+Metadata-Version: 2.1 Name: aiogoogle Version: 5.4.0 Summary: Async Google API
 client Home-page: https://github.com/omarryhan/aiogoogle Author: Omar Ryhan
 Author-email: omarryhan@gmail.com License: MIT Classifier: Programming Language
 :: Python :: 3.7 Classifier: Operating System :: OS Independent Description-
 Content-Type: text/markdown Provides-Extra: curio_asks Provides-Extra:
 trio_asks License-File: LICENSE
                                     [Logo]
   [Build_Status] [Software_License] [Code_style:_black] [Downloads] [Monthly
```

### Comparing `aiogoogle-5.3.0/aiogoogle.egg-info/SOURCES.txt` & `aiogoogle-5.4.0/aiogoogle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiogoogle-5.3.0/setup.py` & `aiogoogle-5.4.0/setup.py`

 * *Files identical despite different names*

