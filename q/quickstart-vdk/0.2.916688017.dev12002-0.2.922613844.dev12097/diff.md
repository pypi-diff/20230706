# Comparing `tmp/quickstart-vdk-0.2.916688017.dev12002.tar.gz` & `tmp/quickstart-vdk-0.2.922613844.dev12097.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.916688017.dev12002.tar", last modified: Fri Jun 30 04:23:17 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.922613844.dev12097.tar", last modified: Thu Jul  6 04:23:44 2023, max compression
```

## Comparing `quickstart-vdk-0.2.916688017.dev12002.tar` & `quickstart-vdk-0.2.922613844.dev12097.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 04:23:17.980330 quickstart-vdk-0.2.916688017.dev12002/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-30 04:23:17.980330 quickstart-vdk-0.2.916688017.dev12002/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-30 04:20:30.000000 quickstart-vdk-0.2.916688017.dev12002/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 04:23:17.976330 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-30 04:23:17.000000 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-30 04:23:17.000000 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 04:23:17.000000 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-30 04:23:17.000000 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-30 04:23:17.000000 quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 04:23:17.980330 quickstart-vdk-0.2.916688017.dev12002/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-30 04:23:06.000000 quickstart-vdk-0.2.916688017.dev12002/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 04:23:17.976330 quickstart-vdk-0.2.916688017.dev12002/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-30 04:20:30.000000 quickstart-vdk-0.2.916688017.dev12002/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:23:44.882405 quickstart-vdk-0.2.922613844.dev12097/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-06 04:23:44.882405 quickstart-vdk-0.2.922613844.dev12097/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-06 04:20:56.000000 quickstart-vdk-0.2.922613844.dev12097/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:23:44.878404 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-06 04:23:44.000000 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-06 04:23:44.000000 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:23:44.000000 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 04:23:44.000000 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 04:23:44.000000 quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 04:23:44.882405 quickstart-vdk-0.2.922613844.dev12097/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-06 04:23:34.000000 quickstart-vdk-0.2.922613844.dev12097/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:23:44.878404 quickstart-vdk-0.2.922613844.dev12097/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-06 04:20:56.000000 quickstart-vdk-0.2.922613844.dev12097/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.916688017.dev12002/PKG-INFO` & `quickstart-vdk-0.2.922613844.dev12097/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.916688017.dev12002
+Version: 0.2.922613844.dev12097
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.916688017.dev12002/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.922613844.dev12097/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.916688017.dev12002
+Version: 0.2.922613844.dev12097
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.916688017.dev12002/setup.py` & `quickstart-vdk-0.2.922613844.dev12097/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.916688017.dev12002"
+__version__ = "0.2.922613844.dev12097"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

