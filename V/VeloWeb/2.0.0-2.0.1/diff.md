# Comparing `tmp/VeloWeb-2.0.0.tar.gz` & `tmp/VeloWeb-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VeloWeb-2.0.0.tar", last modified: Thu Jul  6 18:35:15 2023, max compression
+gzip compressed data, was "VeloWeb-2.0.1.tar", last modified: Thu Jul  6 19:06:18 2023, max compression
```

## Comparing `VeloWeb-2.0.0.tar` & `VeloWeb-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 18:35:15.669050 VeloWeb-2.0.0/
--rw-rw-rw-   0        0        0      910 2023-07-06 18:35:15.661047 VeloWeb-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 18:35:15.661047 VeloWeb-2.0.0/VeloWeb.egg-info/
--rw-rw-rw-   0        0        0      910 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 18:35:15.669050 VeloWeb-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-07-06 18:34:05.000000 VeloWeb-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:06:18.316850 VeloWeb-2.0.1/
+-rw-rw-rw-   0        0        0      910 2023-07-06 19:06:18.284839 VeloWeb-2.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 19:06:18.204819 VeloWeb-2.0.1/VeloWeb.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 19:06:17.000000 VeloWeb-2.0.1/VeloWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 19:06:18.316850 VeloWeb-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-06 19:04:23.000000 VeloWeb-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 19:06:18.284839 VeloWeb-2.0.1/veloweb/
+-rw-rw-rw-   0        0        0       17 2023-07-06 19:06:12.000000 VeloWeb-2.0.1/veloweb/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-07-06 18:29:42.000000 VeloWeb-2.0.1/veloweb/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 VeloWeb-2.0.1/veloweb/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 VeloWeb-2.0.1/veloweb/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 VeloWeb-2.0.1/veloweb/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 VeloWeb-2.0.1/veloweb/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 VeloWeb-2.0.1/veloweb/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 VeloWeb-2.0.1/veloweb/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 VeloWeb-2.0.1/veloweb/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 VeloWeb-2.0.1/veloweb/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 VeloWeb-2.0.1/veloweb/wtf.py
```

### Comparing `VeloWeb-2.0.0/PKG-INFO` & `VeloWeb-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 2.0.0
+Version: 2.0.1
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-2.0.0/VeloWeb.egg-info/PKG-INFO` & `VeloWeb-2.0.1/VeloWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 2.0.0
+Version: 2.0.1
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-2.0.0/setup.py` & `VeloWeb-2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="VeloWeb",
-    version="2.0.0",
+    version="2.0.1",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/veloweb",
```

