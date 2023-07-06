# Comparing `tmp/botocore-a-la-carte-s3-1.30.0.tar.gz` & `tmp/botocore-a-la-carte-s3-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-s3-1.30.0.tar", last modified: Tue Jul  4 01:45:01 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-s3-1.30.1.tar", last modified: Thu Jul  6 01:45:28 2023, max compression
```

## Comparing `botocore-a-la-carte-s3-1.30.0.tar` & `botocore-a-la-carte-s3-1.30.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.582842 botocore-a-la-carte-s3-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 01:45:01.582842 botocore-a-la-carte-s3-1.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.574842 botocore-a-la-carte-s3-1.30.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.574842 botocore-a-la-carte-s3-1.30.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.574842 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.578842 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)  1674528 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    57596 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)   852245 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-04 01:44:02.000000 botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:01.582842 botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:01.582842 botocore-a-la-carte-s3-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-04 01:45:01.000000 botocore-a-la-carte-s3-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.435168 botocore-a-la-carte-s3-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 01:45:28.435168 botocore-a-la-carte-s3-1.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.431168 botocore-a-la-carte-s3-1.30.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.431168 botocore-a-la-carte-s3-1.30.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.431168 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.435168 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)  1674528 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57596 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)   852245 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-06 01:44:40.000000 botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:28.435168 botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:28.435168 botocore-a-la-carte-s3-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-06 01:45:28.000000 botocore-a-la-carte-s3-1.30.1/setup.py
```

### Comparing `botocore-a-la-carte-s3-1.30.0/LICENSE.txt` & `botocore-a-la-carte-s3-1.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/PKG-INFO` & `botocore-a-la-carte-s3-1.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-s3
-Version: 1.30.0
+Version: 1.30.1
 Summary: s3 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/examples-1.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/paginators-1.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/paginators-1.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/service-2.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore/data/s3/2006-03-01/waiters-2.json` & `botocore-a-la-carte-s3-1.30.1/botocore/data/s3/2006-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-s3-1.30.0/botocore_a_la_carte_s3.egg-info/PKG-INFO` & `botocore-a-la-carte-s3-1.30.1/botocore_a_la_carte_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-s3
-Version: 1.30.0
+Version: 1.30.1
 Summary: s3 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-s3-1.30.0/setup.py` & `botocore-a-la-carte-s3-1.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-s3',
-    version="1.30.0",
+    version="1.30.1",
     description='s3 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/s3/*/*.json'],
```

