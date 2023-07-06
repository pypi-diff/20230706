# Comparing `tmp/funcx-2.2.3.tar.gz` & `tmp/funcx-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.2.3.tar", last modified: Thu Jul  6 20:22:51 2023, max compression
+gzip compressed data, was "funcx-2.2.3a0.tar", last modified: Wed Jul  5 15:37:39 2023, max compression
```

## Comparing `funcx-2.2.3.tar` & `funcx-2.2.3a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.135659 funcx-2.2.3/
--rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 funcx-2.2.3/LICENSE
--rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 funcx-2.2.3/MANIFEST.in
--rw-r--r--   0 yadu       (501) staff       (20)     1995 2023-07-06 20:22:51.135744 funcx-2.2.3/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)     1051 2023-04-21 14:48:17.000000 funcx-2.2.3/PyPI.md
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.133299 funcx-2.2.3/funcx/
--rw-r--r--   0 yadu       (501) staff       (20)      467 2023-04-21 14:48:17.000000 funcx-2.2.3/funcx/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.135006 funcx-2.2.3/funcx/sdk/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-2.2.3/funcx/sdk/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)       78 2023-06-12 16:33:52.000000 funcx-2.2.3/funcx/sdk/client.py
--rw-r--r--   0 yadu       (501) staff       (20)       84 2023-06-12 16:33:52.000000 funcx-2.2.3/funcx/sdk/executor.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.135222 funcx-2.2.3/funcx/sdk/login_manager/
--rw-r--r--   0 yadu       (501) staff       (20)      445 2023-04-21 14:48:17.000000 funcx-2.2.3/funcx/sdk/login_manager/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)       88 2023-04-21 14:48:17.000000 funcx-2.2.3/funcx/sdk/web_client.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.135480 funcx-2.2.3/funcx/serialize/
--rw-r--r--   0 yadu       (501) staff       (20)      110 2023-04-21 14:48:17.000000 funcx-2.2.3/funcx/serialize/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1144 2023-07-06 20:21:28.000000 funcx-2.2.3/funcx/version.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:51.134098 funcx-2.2.3/funcx.egg-info/
--rw-r--r--   0 yadu       (501) staff       (20)     1995 2023-07-06 20:22:51.000000 funcx-2.2.3/funcx.egg-info/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)      377 2023-07-06 20:22:51.000000 funcx-2.2.3/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-06 20:22:51.000000 funcx-2.2.3/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 yadu       (501) staff       (20)       26 2023-07-06 20:22:51.000000 funcx-2.2.3/funcx.egg-info/requires.txt
--rw-r--r--   0 yadu       (501) staff       (20)        6 2023-07-06 20:22:51.000000 funcx-2.2.3/funcx.egg-info/top_level.txt
--rw-r--r--   0 yadu       (501) staff       (20)      305 2023-07-06 20:22:51.136087 funcx-2.2.3/setup.cfg
--rw-r--r--   0 yadu       (501) staff       (20)     1913 2023-07-06 20:21:28.000000 funcx-2.2.3/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.265185 funcx-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 funcx-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       16 2023-04-21 14:48:17.000000 funcx-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     1997 2023-07-05 15:37:39.265266 funcx-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     1051 2023-04-21 14:48:17.000000 funcx-2.2.3a0/PyPI.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.262743 funcx-2.2.3a0/funcx/
+-rw-r--r--   0 yadu       (501) staff       (20)      467 2023-04-21 14:48:17.000000 funcx-2.2.3a0/funcx/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.264513 funcx-2.2.3a0/funcx/sdk/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 funcx-2.2.3a0/funcx/sdk/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)       78 2023-06-12 16:33:52.000000 funcx-2.2.3a0/funcx/sdk/client.py
+-rw-r--r--   0 yadu       (501) staff       (20)       84 2023-06-12 16:33:52.000000 funcx-2.2.3a0/funcx/sdk/executor.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.264723 funcx-2.2.3a0/funcx/sdk/login_manager/
+-rw-r--r--   0 yadu       (501) staff       (20)      445 2023-04-21 14:48:17.000000 funcx-2.2.3a0/funcx/sdk/login_manager/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)       88 2023-04-21 14:48:17.000000 funcx-2.2.3a0/funcx/sdk/web_client.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.265002 funcx-2.2.3a0/funcx/serialize/
+-rw-r--r--   0 yadu       (501) staff       (20)      110 2023-04-21 14:48:17.000000 funcx-2.2.3a0/funcx/serialize/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1146 2023-07-05 15:22:25.000000 funcx-2.2.3a0/funcx/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:37:39.263547 funcx-2.2.3a0/funcx.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     1997 2023-07-05 15:37:39.000000 funcx-2.2.3a0/funcx.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      377 2023-07-05 15:37:39.000000 funcx-2.2.3a0/funcx.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:37:39.000000 funcx-2.2.3a0/funcx.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       28 2023-07-05 15:37:39.000000 funcx-2.2.3a0/funcx.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        6 2023-07-05 15:37:39.000000 funcx-2.2.3a0/funcx.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      305 2023-07-05 15:37:39.265638 funcx-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     1915 2023-07-05 15:24:28.000000 funcx-2.2.3a0/setup.py
```

### Comparing `funcx-2.2.3/LICENSE` & `funcx-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.2.3/PKG-INFO` & `funcx-2.2.3a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.2.3/PyPI.md` & `funcx-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-2.2.3/funcx/version.py` & `funcx-2.2.3a0/funcx/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.3"
+__version__ = "2.2.3a0"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.2.3/funcx.egg-info/PKG-INFO` & `funcx-2.2.3a0/funcx.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `funcx-2.2.3/setup.py` & `funcx-2.2.3a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-sdk==2.2.3",
+    "globus-compute-sdk==2.2.3a0",
 ]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
```

