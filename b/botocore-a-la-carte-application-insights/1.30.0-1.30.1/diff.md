# Comparing `tmp/botocore-a-la-carte-application-insights-1.30.0.tar.gz` & `tmp/botocore-a-la-carte-application-insights-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-application-insights-1.30.0.tar", last modified: Tue Jul  4 01:44:14 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-application-insights-1.30.1.tar", last modified: Thu Jul  6 01:44:50 2023, max compression
```

## Comparing `botocore-a-la-carte-application-insights-1.30.0.tar` & `botocore-a-la-carte-application-insights-1.30.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.222386 botocore-a-la-carte-application-insights-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:13.000000 botocore-a-la-carte-application-insights-1.30.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 01:44:14.222386 botocore-a-la-carte-application-insights-1.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.218386 botocore-a-la-carte-application-insights-1.30.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.218386 botocore-a-la-carte-application-insights-1.30.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.218386 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.222386 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-04 01:44:02.000000 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 01:44:02.000000 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 01:44:02.000000 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    76964 2023-07-04 01:44:02.000000 botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:14.222386 botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-04 01:44:14.000000 botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-04 01:44:14.000000 botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:14.000000 botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:14.000000 botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:14.222386 botocore-a-la-carte-application-insights-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-04 01:44:13.000000 botocore-a-la-carte-application-insights-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.890585 botocore-a-la-carte-application-insights-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 01:44:50.890585 botocore-a-la-carte-application-insights-1.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.886584 botocore-a-la-carte-application-insights-1.30.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.886584 botocore-a-la-carte-application-insights-1.30.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.886584 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.886584 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-07-06 01:44:40.000000 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 01:44:40.000000 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 01:44:40.000000 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76964 2023-07-06 01:44:40.000000 botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:44:50.886584 botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:44:50.890585 botocore-a-la-carte-application-insights-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 01:44:50.000000 botocore-a-la-carte-application-insights-1.30.1/setup.py
```

### Comparing `botocore-a-la-carte-application-insights-1.30.0/LICENSE.txt` & `botocore-a-la-carte-application-insights-1.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-application-insights-1.30.0/PKG-INFO` & `botocore-a-la-carte-application-insights-1.30.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-application-insights
-Version: 1.30.0
+Version: 1.30.1
 Summary: application-insights data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-application-insights-1.30.0/botocore/data/application-insights/2018-11-25/service-2.json` & `botocore-a-la-carte-application-insights-1.30.1/botocore/data/application-insights/2018-11-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/PKG-INFO` & `botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-application-insights
-Version: 1.30.0
+Version: 1.30.1
 Summary: application-insights data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-application-insights-1.30.0/botocore_a_la_carte_application_insights.egg-info/SOURCES.txt` & `botocore-a-la-carte-application-insights-1.30.1/botocore_a_la_carte_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-application-insights-1.30.0/setup.py` & `botocore-a-la-carte-application-insights-1.30.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-application-insights',
-    version="1.30.0",
+    version="1.30.1",
     description='application-insights data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/application-insights/*/*.json'],
```

