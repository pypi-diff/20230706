# Comparing `tmp/botocore-a-la-carte-internetmonitor-1.30.0.tar.gz` & `tmp/botocore-a-la-carte-internetmonitor-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-internetmonitor-1.30.0.tar", last modified: Tue Jul  4 01:44:30 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-internetmonitor-1.30.1.tar", last modified: Thu Jul  6 01:45:03 2023, max compression
```

## Comparing `botocore-a-la-carte-internetmonitor-1.30.0.tar` & `botocore-a-la-carte-internetmonitor-1.30.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:29.000000 botocore-a-la-carte-internetmonitor-1.30.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-04 01:44:02.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-04 01:44:02.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-07-04 01:44:02.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-04 01:44:02.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-04 01:44:30.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-04 01:44:30.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:30.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:30.000000 botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:30.154546 botocore-a-la-carte-internetmonitor-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-04 01:44:29.000000 botocore-a-la-carte-internetmonitor-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.642778 botocore-a-la-carte-internetmonitor-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-06 01:44:40.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 01:44:40.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-07-06 01:44:40.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 01:44:40.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:03.638778 botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:03.642778 botocore-a-la-carte-internetmonitor-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-06 01:45:03.000000 botocore-a-la-carte-internetmonitor-1.30.1/setup.py
```

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/LICENSE.txt` & `botocore-a-la-carte-internetmonitor-1.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/PKG-INFO` & `botocore-a-la-carte-internetmonitor-1.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-internetmonitor
-Version: 1.30.0
+Version: 1.30.1
 Summary: internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/botocore/data/internetmonitor/2021-06-03/service-2.json` & `botocore-a-la-carte-internetmonitor-1.30.1/botocore/data/internetmonitor/2021-06-03/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO` & `botocore-a-la-carte-internetmonitor-1.30.1/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-internetmonitor
-Version: 1.30.0
+Version: 1.30.1
 Summary: internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-internetmonitor-1.30.0/setup.py` & `botocore-a-la-carte-internetmonitor-1.30.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-internetmonitor',
-    version="1.30.0",
+    version="1.30.1",
     description='internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/internetmonitor/*/*.json'],
```

