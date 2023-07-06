# Comparing `tmp/Ruster-1.0.4.tar.gz` & `tmp/Ruster-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ruster-1.0.4.tar", last modified: Thu Jul  6 20:27:14 2023, max compression
+gzip compressed data, was "Ruster-1.0.5.tar", last modified: Thu Jul  6 20:31:13 2023, max compression
```

## Comparing `Ruster-1.0.4.tar` & `Ruster-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:27:14.609222 Ruster-1.0.4/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:27:14.607219 Ruster-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 20:27:14.562216 Ruster-1.0.4/Ruster/
--rw-rw-rw-   0        0        0        0 2023-07-06 20:26:54.000000 Ruster-1.0.4/Ruster/__init__.py
--rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.4/Ruster/app.py
--rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.4/Ruster/blueprints.py
--rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.4/Ruster/exceptions.py
--rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.4/Ruster/hasher.py
--rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.4/Ruster/jwt.py
--rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.4/Ruster/limiter.py
--rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.4/Ruster/mailer.py
--rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.4/Ruster/sanitizer.py
--rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.4/Ruster/session.py
--rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.4/Ruster/wtf.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:27:14.600221 Ruster-1.0.4/Ruster.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 20:27:14.000000 Ruster-1.0.4/Ruster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 20:27:14.609222 Ruster-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1275 2023-07-06 20:26:44.000000 Ruster-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:31:13.933033 Ruster-1.0.5/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:31:13.932033 Ruster-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 20:31:13.895032 Ruster-1.0.5/Ruster/
+-rw-rw-rw-   0        0        0      111 2023-07-06 20:30:47.000000 Ruster-1.0.5/Ruster/__init__.py
+-rw-rw-rw-   0        0        0    13107 2023-07-06 20:18:13.000000 Ruster-1.0.5/Ruster/app.py
+-rw-rw-rw-   0        0        0     1345 2023-07-06 08:52:07.000000 Ruster-1.0.5/Ruster/blueprints.py
+-rw-rw-rw-   0        0        0      182 2023-07-04 18:04:15.000000 Ruster-1.0.5/Ruster/exceptions.py
+-rw-rw-rw-   0        0        0     3761 2023-07-06 17:39:41.000000 Ruster-1.0.5/Ruster/hasher.py
+-rw-rw-rw-   0        0        0     7955 2023-07-06 17:39:59.000000 Ruster-1.0.5/Ruster/jwt.py
+-rw-rw-rw-   0        0        0     2664 2023-07-06 08:37:14.000000 Ruster-1.0.5/Ruster/limiter.py
+-rw-rw-rw-   0        0        0     2923 2023-07-06 17:39:05.000000 Ruster-1.0.5/Ruster/mailer.py
+-rw-rw-rw-   0        0        0     1087 2023-07-06 17:30:52.000000 Ruster-1.0.5/Ruster/sanitizer.py
+-rw-rw-rw-   0        0        0     1453 2023-07-05 18:45:57.000000 Ruster-1.0.5/Ruster/session.py
+-rw-rw-rw-   0        0        0     2679 2023-07-06 17:40:20.000000 Ruster-1.0.5/Ruster/wtf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 20:31:13.929034 Ruster-1.0.5/Ruster.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 20:31:13.000000 Ruster-1.0.5/Ruster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 20:31:13.934033 Ruster-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2023-07-06 20:30:55.000000 Ruster-1.0.5/setup.py
```

### Comparing `Ruster-1.0.4/PKG-INFO` & `Ruster-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.4
+Version: 1.0.5
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.4/Ruster/app.py` & `Ruster-1.0.5/Ruster/app.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/blueprints.py` & `Ruster-1.0.5/Ruster/blueprints.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/hasher.py` & `Ruster-1.0.5/Ruster/hasher.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/jwt.py` & `Ruster-1.0.5/Ruster/jwt.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/limiter.py` & `Ruster-1.0.5/Ruster/limiter.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/mailer.py` & `Ruster-1.0.5/Ruster/mailer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/sanitizer.py` & `Ruster-1.0.5/Ruster/sanitizer.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/session.py` & `Ruster-1.0.5/Ruster/session.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster/wtf.py` & `Ruster-1.0.5/Ruster/wtf.py`

 * *Files identical despite different names*

### Comparing `Ruster-1.0.4/Ruster.egg-info/PKG-INFO` & `Ruster-1.0.5/Ruster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ruster
-Version: 1.0.4
+Version: 1.0.5
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/ruster
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Ruster-1.0.4/setup.py` & `Ruster-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Ruster",
-    version="1.0.4",
+    version="1.0.5",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/ruster",
```

