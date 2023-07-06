# Comparing `tmp/pyawskit-0.1.73.tar.gz` & `tmp/pyawskit-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.73.tar", last modified: Tue May  9 08:54:44 2023, max compression
+gzip compressed data, was "pyawskit-0.1.74.tar", last modified: Thu Jul  6 15:32:11 2023, max compression
```

## Comparing `pyawskit-0.1.73.tar` & `pyawskit-0.1.74.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-09 08:54:44.177167 pyawskit-0.1.73/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-05-09 08:54:33.000000 pyawskit-0.1.73/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-05-09 08:54:44.177167 pyawskit-0.1.73/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-05-09 08:54:33.000000 pyawskit-0.1.73/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-09 08:54:44.176167 pyawskit-0.1.73/pyawskit/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:33:09.000000 pyawskit-0.1.73/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2022-06-13 04:33:09.000000 pyawskit-0.1.73/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-17 07:19:49.000000 pyawskit-0.1.73/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-17 07:19:49.000000 pyawskit-0.1.73/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1826 2023-05-09 08:54:16.000000 pyawskit-0.1.73/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-12 10:00:43.000000 pyawskit-0.1.73/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-20 09:56:53.000000 pyawskit-0.1.73/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14829 2023-05-02 09:34:27.000000 pyawskit-0.1.73/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-09-11 10:30:52.000000 pyawskit-0.1.73/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      185 2023-05-09 08:54:33.000000 pyawskit-0.1.73/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-09-11 10:30:52.000000 pyawskit-0.1.73/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-05-09 08:54:44.177167 pyawskit-0.1.73/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-05-09 08:54:44.000000 pyawskit-0.1.73/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-05-09 08:54:44.177167 pyawskit-0.1.73/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1761 2023-05-09 08:54:33.000000 pyawskit-0.1.73/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 15:32:11.467062 pyawskit-0.1.74/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-07-06 15:31:53.000000 pyawskit-0.1.74/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-06 15:32:11.467062 pyawskit-0.1.74/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      415 2023-07-06 15:31:53.000000 pyawskit-0.1.74/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 15:32:11.467062 pyawskit-0.1.74/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.74/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.74/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3499 2023-04-16 18:29:08.000000 pyawskit-0.1.74/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.74/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2039 2023-07-06 15:31:39.000000 pyawskit-0.1.74/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.74/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2093 2023-04-19 19:52:43.000000 pyawskit-0.1.74/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14829 2023-04-27 08:16:18.000000 pyawskit-0.1.74/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.74/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      185 2023-07-06 15:31:53.000000 pyawskit-0.1.74/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.74/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 15:32:11.467062 pyawskit-0.1.74/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1375 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)      104 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-07-06 15:32:11.000000 pyawskit-0.1.74/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-07-06 15:32:11.467062 pyawskit-0.1.74/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1761 2023-07-06 15:31:53.000000 pyawskit-0.1.74/setup.py
```

### Comparing `pyawskit-0.1.73/LICENSE` & `pyawskit-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/PKG-INFO` & `pyawskit-0.1.74/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.73
+Version: 0.1.74
 Summary: Pyawskit is your AWS Swiss Army Knife
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.73
+version: 0.1.74
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.73/pyawskit/aws.py` & `pyawskit-0.1.74/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.74/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.74/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/aws_ecr_login_code.py` & `pyawskit-0.1.74/pyawskit/aws_ecr_login_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import sys
 import datetime
-
 import base64
+
+import requests.exceptions
 import docker
 import boto3
 import pyapikey
 
 KEY = "ecr_password"
 
 
 def handle_data(user: str, password: str, proxyEndpoint: str) -> None:
     """ really do something with the data """
     client = docker.Client()
-    client.login(
-        username=user,
-        password=password,
-        registry=proxyEndpoint,
-    )
+    try:
+        client.login(
+            username=user,
+            password=password,
+            registry=proxyEndpoint,
+        )
+    except requests.exceptions.ConnectionError:
+        print(f"ConnectionError for {user} {password} {proxyEndpoint}", file=sys.stderr)
+        sys.exit(1)
 
 
 def run() -> None:
     temp_store = pyapikey.core.TempStore()
     if temp_store.has(KEY):
         data = temp_store.get(KEY)
         expiration = data["expiration"]
```

### Comparing `pyawskit-0.1.73/pyawskit/common.py` & `pyawskit-0.1.74/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/configs.py` & `pyawskit-0.1.74/pyawskit/configs.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/main.py` & `pyawskit-0.1.74/pyawskit/main.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/os_utils.py` & `pyawskit-0.1.74/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit/utils.py` & `pyawskit-0.1.74/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.73/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.74/pyawskit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.73
+Version: 0.1.74
 Summary: Pyawskit is your AWS Swiss Army Knife
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.73
+version: 0.1.74
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.73/setup.py` & `pyawskit-0.1.74/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.73",
+    version="0.1.74",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="Pyawskit is your AWS Swiss Army Knife",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

