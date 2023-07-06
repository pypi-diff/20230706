# Comparing `tmp/pytket-projectq-0.8.0.tar.gz` & `tmp/pytket-projectq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-projectq-0.8.0.tar", last modified: Thu Apr  1 10:56:47 2021, max compression
+gzip compressed data, was "pytket-projectq-0.9.0.tar", last modified: Wed Apr 28 13:28:55 2021, max compression
```

## Comparing `pytket-projectq-0.8.0.tar` & `pytket-projectq-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      606 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/pytket/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/pytket/extensions/projectq/
--rw-r--r--   0 runner    (1001) docker     (121)      920 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/pytket/extensions/projectq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket/extensions/projectq/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/pytket/extensions/projectq/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/pytket/extensions/projectq/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9672 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/pytket/extensions/projectq/backends/projectq_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    12982 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/pytket/extensions/projectq/projectq_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/pytket_projectq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-01 10:56:47.000000 pytket-projectq-0.8.0/pytket_projectq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-01 10:56:47.507523 pytket-projectq-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-04-01 10:54:45.000000 pytket-projectq-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.865154 pytket-projectq-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-04-28 13:28:55.865154 pytket-projectq-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.861154 pytket-projectq-0.9.0/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.861154 pytket-projectq-0.9.0/pytket/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.861154 pytket-projectq-0.9.0/pytket/extensions/projectq/
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/pytket/extensions/projectq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket/extensions/projectq/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.861154 pytket-projectq-0.9.0/pytket/extensions/projectq/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/pytket/extensions/projectq/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9672 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/pytket/extensions/projectq/backends/projectq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12982 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/pytket/extensions/projectq/projectq_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-28 13:28:55.865154 pytket-projectq-0.9.0/pytket_projectq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1653 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-28 13:28:55.000000 pytket-projectq-0.9.0/pytket_projectq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-28 13:28:55.865154 pytket-projectq-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2078 2021-04-28 13:26:53.000000 pytket-projectq-0.9.0/setup.py
```

### Comparing `pytket-projectq-0.8.0/PKG-INFO` & `pytket-projectq-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-projectq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the ProjectQ framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Luca Mondada
 Author-email: luca.mondada@cambridgequantum.com
 License: Apache 2
 Description: # pytket-projectq
```

### Comparing `pytket-projectq-0.8.0/README.md` & `pytket-projectq-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pytket-projectq-0.8.0/pytket/extensions/projectq/__init__.py` & `pytket-projectq-0.9.0/pytket/extensions/projectq/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-projectq-0.8.0/pytket/extensions/projectq/backends/__init__.py` & `pytket-projectq-0.9.0/pytket/extensions/projectq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pytket-projectq-0.8.0/pytket/extensions/projectq/backends/projectq_backend.py` & `pytket-projectq-0.9.0/pytket/extensions/projectq/backends/projectq_backend.py`

 * *Files identical despite different names*

### Comparing `pytket-projectq-0.8.0/pytket/extensions/projectq/projectq_convert.py` & `pytket-projectq-0.9.0/pytket/extensions/projectq/projectq_convert.py`

 * *Files identical despite different names*

### Comparing `pytket-projectq-0.8.0/pytket_projectq.egg-info/PKG-INFO` & `pytket-projectq-0.9.0/pytket_projectq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-projectq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing translation to and from the ProjectQ framework
 Home-page: https://github.com/CQCL/pytket-extensions
 Author: Luca Mondada
 Author-email: luca.mondada@cambridgequantum.com
 License: Apache 2
 Description: # pytket-projectq
```

### Comparing `pytket-projectq-0.8.0/setup.py` & `pytket-projectq-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     description="Extension for pytket, providing translation to and from the ProjectQ "
     "framework",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache 2",
     packages=find_namespace_packages(include=["pytket.*"]),
     include_package_data=True,
-    install_requires=["pytket ~= 0.9.0", "projectq ~= 0.5.0"],
+    install_requires=["pytket ~= 0.10.0", "projectq ~= 0.5.0"],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: Other/Proprietary License",
         "Operating System :: MacOS :: MacOS X",
```

