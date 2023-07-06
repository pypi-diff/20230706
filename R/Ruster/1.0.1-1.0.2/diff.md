# Comparing `tmp/Ruster-1.0.1.tar.gz` & `tmp/Ruster-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-1.0.1.tar", last modified: Thu Jul  6 19:58:35 2023, max compression
+gzip compressed data, was "Ruster-1.0.2.tar", last modified: Thu Jul  6 20:14:46 2023, max compression
```

## Comparing `Ruster-1.0.1.tar` & `Ruster-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 19:58:35.340868 Ruster-1.0.1/
--rw-rw-rw-   0        0        0      908 2023-07-06 19:58:35.339869 Ruster-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 19:58:35.336867 Ruster-1.0.1/Ruster.egg-info/
--rw-rw-rw-   0        0        0      908 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 19:58:35.000000 Ruster-1.0.1/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 19:58:35.341868 Ruster-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1274 2023-07-06 19:57:53.000000 Ruster-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.419914 Ruster-1.0.2/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:14:46.414913 Ruster-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.366912 Ruster-1.0.2/Ruster/
+-rw-rw-rw-   0        0        0        0 2023-07-06 20:11:06.000000 Ruster-1.0.2/Ruster/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-07-06 18:29:42.000000 Ruster-1.0.2/Ruster/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.2/Ruster/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.2/Ruster/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.2/Ruster/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.2/Ruster/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.2/Ruster/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.2/Ruster/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.2/Ruster/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.2/Ruster/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.2/Ruster/wtf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:14:46.413913 Ruster-1.0.2/Ruster.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 20:14:46.000000 Ruster-1.0.2/Ruster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 20:14:46.420913 Ruster-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2023-07-06 20:10:46.000000 Ruster-1.0.2/setup.py
```

### Comparing `Ruster-1.0.1/PKG-INFO` & `Ruster-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Python VeloWEB
+# Python Ruster
 
-A light weight and fully functional web framework for python, achive a quality code and rich functions with VeloWEB.
+A light weight and fully functional web framework for python, achive a quality code and rich functions with Ruster.
 
 ## Installation
 
-You can install veloweb using pip:
+You can install Ruster using pip:
 
 ```shell
-pip install veloweb
+pip install ruster
```

### Comparing `Ruster-1.0.1/Ruster.egg-info/PKG-INFO` & `Ruster-1.0.2/Ruster.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,17 +12,17 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Python VeloWEB
+# Python Ruster
 
-A light weight and fully functional web framework for python, achive a quality code and rich functions with VeloWEB.
+A light weight and fully functional web framework for python, achive a quality code and rich functions with Ruster.
 
 ## Installation
 
-You can install veloweb using pip:
+You can install Ruster using pip:
 
 ```shell
-pip install veloweb
+pip install ruster
```

### Comparing `Ruster-1.0.1/setup.py` & `Ruster-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Ruster",
-    version="1.0.1",
+    version="1.0.2",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/ruster",
```

