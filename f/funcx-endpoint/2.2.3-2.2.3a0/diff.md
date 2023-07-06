# Comparing `tmp/funcx-endpoint-2.2.3.tar.gz` & `tmp/funcx-endpoint-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.2.3.tar", last modified: Thu Jul  6 20:23:05 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.2.3a0.tar", last modified: Wed Jul  5 15:37:57 2023, max compression
```

## Comparing `funcx-endpoint-2.2.3.tar` & `funcx-endpoint-2.2.3a0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.180897 funcx-endpoint-2.2.3/
--rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/LICENSE
--rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/MANIFEST.in
--rw-r--r--   0 yadu       (501) staff       (20)     2040 2023-07-06 20:23:05.181023 funcx-endpoint-2.2.3/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)     1115 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/PyPI.md
--rw-r--r--   0 yadu       (501) staff       (20)      430 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/README.md
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.177862 funcx-endpoint-2.2.3/funcx_endpoint/
--rw-r--r--   0 yadu       (501) staff       (20)      122 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.179027 funcx-endpoint-2.2.3/funcx_endpoint/endpoint/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.179563 funcx-endpoint-2.2.3/funcx_endpoint/endpoint/utils/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)       73 2023-06-12 16:33:52.000000 funcx-endpoint-2.2.3/funcx_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.180040 funcx-endpoint-2.2.3/funcx_endpoint/executors/
--rw-r--r--   0 yadu       (501) staff       (20)      107 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/executors/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.180664 funcx-endpoint-2.2.3/funcx_endpoint/executors/high_throughput/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)      101 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/executors/high_throughput/funcx_manager.py
--rw-r--r--   0 yadu       (501) staff       (20)      114 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3/funcx_endpoint/executors/high_throughput/funcx_worker.py
--rw-r--r--   0 yadu       (501) staff       (20)      243 2023-07-06 20:21:28.000000 funcx-endpoint-2.2.3/funcx_endpoint/version.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:23:05.178860 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/
--rw-r--r--   0 yadu       (501) staff       (20)     2040 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)      662 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 yadu       (501) staff       (20)      329 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 yadu       (501) staff       (20)       31 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 yadu       (501) staff       (20)       15 2023-07-06 20:23:05.000000 funcx-endpoint-2.2.3/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 yadu       (501) staff       (20)      305 2023-07-06 20:23:05.181900 funcx-endpoint-2.2.3/setup.cfg
--rw-r--r--   0 yadu       (501) staff       (20)     2030 2023-07-06 20:21:28.000000 funcx-endpoint-2.2.3/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.077800 funcx-endpoint-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     2042 2023-07-05 15:37:57.077897 funcx-endpoint-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     1115 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/PyPI.md
+-rw-r--r--   0 yadu       (501) staff       (20)      430 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/README.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.074712 funcx-endpoint-2.2.3a0/funcx_endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)      122 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.076078 funcx-endpoint-2.2.3a0/funcx_endpoint/endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.076468 funcx-endpoint-2.2.3a0/funcx_endpoint/endpoint/utils/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)       73 2023-06-12 16:33:52.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.076894 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/
+-rw-r--r--   0 yadu       (501) staff       (20)      107 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.077559 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      101 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/high_throughput/funcx_manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)      114 2023-04-21 14:48:17.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/executors/high_throughput/funcx_worker.py
+-rw-r--r--   0 yadu       (501) staff       (20)      245 2023-07-05 15:22:07.000000 funcx-endpoint-2.2.3a0/funcx_endpoint/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:57.075907 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     2042 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      662 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      329 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       33 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       15 2023-07-05 15:37:57.000000 funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      305 2023-07-05 15:37:57.078253 funcx-endpoint-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     2032 2023-07-05 15:24:44.000000 funcx-endpoint-2.2.3a0/setup.py
```

### Comparing `funcx-endpoint-2.2.3/LICENSE` & `funcx-endpoint-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.3/PKG-INFO` & `funcx-endpoint-2.2.3a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.2.3/PyPI.md` & `funcx-endpoint-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.3/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-endpoint-2.2.3/funcx_endpoint.egg-info/SOURCES.txt` & `funcx-endpoint-2.2.3a0/funcx_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.2.3/setup.py` & `funcx-endpoint-2.2.3a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint==2.2.3",
+    "globus-compute-endpoint==2.2.3a0",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
```

