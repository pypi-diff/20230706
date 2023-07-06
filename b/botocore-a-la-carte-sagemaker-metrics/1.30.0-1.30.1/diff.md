# Comparing `tmp/botocore-a-la-carte-sagemaker-metrics-1.30.0.tar.gz` & `tmp/botocore-a-la-carte-sagemaker-metrics-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-sagemaker-metrics-1.30.0.tar", last modified: Tue Jul  4 01:45:04 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-sagemaker-metrics-1.30.1.tar", last modified: Thu Jul  6 01:45:30 2023, max compression
```

## Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0.tar` & `botocore-a-la-carte-sagemaker-metrics-1.30.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-04 01:44:02.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:45:04.694869 botocore-a-la-carte-sagemaker-metrics-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-04 01:45:04.000000 botocore-a-la-carte-sagemaker-metrics-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-07-06 01:44:40.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 01:44:40.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-06 01:44:40.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:30.919204 botocore-a-la-carte-sagemaker-metrics-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-06 01:45:30.000000 botocore-a-la-carte-sagemaker-metrics-1.30.1/setup.py
```

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/LICENSE.txt` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/PKG-INFO` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-metrics
-Version: 1.30.0
+Version: 1.30.1
 Summary: sagemaker-metrics data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/endpoint-rule-set-1.json` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore/data/sagemaker-metrics/2022-09-30/service-2.json` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore/data/sagemaker-metrics/2022-09-30/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/botocore_a_la_carte_sagemaker_metrics.egg-info/PKG-INFO` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/botocore_a_la_carte_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-sagemaker-metrics
-Version: 1.30.0
+Version: 1.30.1
 Summary: sagemaker-metrics data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-sagemaker-metrics-1.30.0/setup.py` & `botocore-a-la-carte-sagemaker-metrics-1.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-sagemaker-metrics',
-    version="1.30.0",
+    version="1.30.1",
     description='sagemaker-metrics data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/sagemaker-metrics/*/*.json'],
```

