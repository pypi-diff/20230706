# Comparing `tmp/Ruster-1.0.2.tar.gz` & `tmp/Ruster-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-1.0.2.tar", last modified: Thu Jul  6 20:14:46 2023, max compression
+gzip compressed data, was "Ruster-1.0.3.tar", last modified: Thu Jul  6 20:23:07 2023, max compression
```

## Comparing `Ruster-1.0.2.tar` & `Ruster-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.419914 Ruster-1.0.2/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:14:46.414913 Ruster-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.366912 Ruster-1.0.2/Ruster/
--rw-rw-rw-   0        0        0        0 2023-07-06 20:11:06.000000 Ruster-1.0.2/Ruster/__init__.py
--rw-rw-rw-   0        0        0    13107 2023-07-06 18:29:42.000000 Ruster-1.0.2/Ruster/app.py
--rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.2/Ruster/blueprints.py
--rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.2/Ruster/exceptions.py
--rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.2/Ruster/hasher.py
--rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.2/Ruster/jwt.py
--rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.2/Ruster/limiter.py
--rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.2/Ruster/mailer.py
--rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.2/Ruster/sanitizer.py
--rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.2/Ruster/session.py
--rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.2/Ruster/wtf.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.413913 Ruster-1.0.2/Ruster.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 20:14:46.420913 Ruster-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-07-06 20:10:46.000000 Ruster-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:23:07.800253 Ruster-1.0.3/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:23:07.798253 Ruster-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 20:23:07.738249 Ruster-1.0.3/Ruster/
+-rw-rw-rw-   0        0        0       18 2023-07-06 20:21:57.000000 Ruster-1.0.3/Ruster/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.3/Ruster/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.3/Ruster/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.3/Ruster/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.3/Ruster/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.3/Ruster/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.3/Ruster/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.3/Ruster/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.3/Ruster/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.3/Ruster/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.3/Ruster/wtf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:23:07.793250 Ruster-1.0.3/Ruster.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 20:23:07.000000 Ruster-1.0.3/Ruster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 20:23:07.801251 Ruster-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-06 20:23:04.000000 Ruster-1.0.3/setup.py
```

### Comparing `Ruster-1.0.2/PKG-INFO` & `Ruster-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.2/Ruster/app.py` & `Ruster-1.0.3/Ruster/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import asyncio
 from session import session_manager
 from limiter import Limiter
 import traceback
 import os
 import importlib.util
 
-class Velo:
+class Rust:
     def __init__(self):
         self.url_map = Map()
         self.error_handlers = {}
         self.before_request_funcs = []
         self.after_request_funcs = []
         self.template_env = Environment(loader=FileSystemLoader('templates'))
         self.host = '127.0.0.1'
@@ -239,15 +239,15 @@
 
 
 class VeloRequest(Request):
     @property
     def session(self):
         return session_manager.get_session(self.cookies.get('session_id'))
 
-crust = Velo()
+crust = Rust()
 request = VeloRequest
 
 
 def jsonify(data):
     return Response(json.dumps(data), mimetype='application/json')
```

### Comparing `Ruster-1.0.2/Ruster/blueprints.py` & `Ruster-1.0.3/Ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/hasher.py` & `Ruster-1.0.3/Ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/jwt.py` & `Ruster-1.0.3/Ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/limiter.py` & `Ruster-1.0.3/Ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/mailer.py` & `Ruster-1.0.3/Ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/sanitizer.py` & `Ruster-1.0.3/Ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/session.py` & `Ruster-1.0.3/Ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster/wtf.py` & `Ruster-1.0.3/Ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.2/Ruster.egg-info/PKG-INFO` & `Ruster-1.0.3/Ruster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.2
+Version: 1.0.3
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.2/setup.py` & `Ruster-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Ruster",
-    version="1.0.2",
+    version="1.0.3",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/ruster",
@@ -23,15 +23,15 @@
         "jinja2",
         "uuid",
         "rustadmin",
         "uuid"
     ],
     entry_points={
     'console_scripts': [
-    'ruster = Ruster:app'
+    'ruster = Ruster:app',
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

