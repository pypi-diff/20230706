# Comparing `tmp/VeloWeb-1.0.3.tar.gz` & `tmp/VeloWeb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VeloWeb-1.0.3.tar", last modified: Mon Jul  3 18:02:19 2023, max compression
+gzip compressed data, was "VeloWeb-2.0.0.tar", last modified: Thu Jul  6 18:35:15 2023, max compression
```

## Comparing `VeloWeb-1.0.3.tar` & `VeloWeb-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.759226 VeloWeb-1.0.3/
--rw-rw-rw-   0        0        0      910 2023-07-03 18:02:19.756225 VeloWeb-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.714220 VeloWeb-1.0.3/VeloWeb.egg-info/
--rw-rw-rw-   0        0        0      910 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 18:02:19.000000 VeloWeb-1.0.3/VeloWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 18:02:19.759226 VeloWeb-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-03 18:02:15.000000 VeloWeb-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 18:02:19.752225 VeloWeb-1.0.3/veloweb/
--rw-rw-rw-   0        0        0     3648 2023-07-03 07:50:31.000000 VeloWeb-1.0.3/veloweb/VeloHasher.py
--rw-rw-rw-   0        0        0     7776 2023-07-03 18:01:44.000000 VeloWeb-1.0.3/veloweb/VeloJWT.py
--rw-rw-rw-   0        0        0     2847 2023-07-01 16:49:03.000000 VeloWeb-1.0.3/veloweb/VeloMailer.py
--rw-rw-rw-   0        0        0     2594 2023-07-01 16:49:12.000000 VeloWeb-1.0.3/veloweb/VeloWTF.py
--rw-rw-rw-   0        0        0       27 2023-07-01 20:25:18.000000 VeloWeb-1.0.3/veloweb/__init__.py
--rw-rw-rw-   0        0        0    14356 2023-07-03 17:58:50.000000 VeloWeb-1.0.3/veloweb/veloweb.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:35:15.669050 VeloWeb-2.0.0/
+-rw-rw-rw-   0        0        0      910 2023-07-06 18:35:15.661047 VeloWeb-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 18:35:15.661047 VeloWeb-2.0.0/VeloWeb.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 18:35:14.000000 VeloWeb-2.0.0/VeloWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:35:15.669050 VeloWeb-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-06 18:34:05.000000 VeloWeb-2.0.0/setup.py
```

### Comparing `VeloWeb-1.0.3/PKG-INFO` & `VeloWeb-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.3
+Version: 2.0.0
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.3/VeloWeb.egg-info/PKG-INFO` & `VeloWeb-2.0.0/VeloWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.3
+Version: 2.0.0
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.3/setup.py` & `VeloWeb-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="VeloWeb",
-    version="1.0.3",
+    version="2.0.0",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/veloweb",
     packages=find_packages(),
     py_modules=['veloweb'],
     install_requires=[
         "itsdangerous",
         "werkzeug",
         "PyJWT",
-        "pyaes",
+        "cryptography"
         "jinja2",
         "uuid",
         "veloadmin"
+        "uuid"
     ],
     entry_points={
     'console_scripts': [
-    'veloweb = veloweb:veloweb',
+    'veloweb = veloweb:app',
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

