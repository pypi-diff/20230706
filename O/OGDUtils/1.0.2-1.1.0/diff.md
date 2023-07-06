# Comparing `tmp/OGDUtils-1.0.2.tar.gz` & `tmp/OGDUtils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OGDUtils-1.0.2.tar", last modified: Thu Jul  6 06:20:36 2023, max compression
+gzip compressed data, was "OGDUtils-1.1.0.tar", last modified: Thu Jul  6 16:05:30 2023, max compression
```

## Comparing `OGDUtils-1.0.2.tar` & `OGDUtils-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.892951 OGDUtils-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 06:20:36.892951 OGDUtils-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 06:20:36.892951 OGDUtils-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.888951 OGDUtils-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.888951 OGDUtils-1.0.2/src/OGDUtils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.888951 OGDUtils-1.0.2/src/OGDUtils/JOWILDER/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/JOWILDER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37301 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/JOWILDER/jowilder_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.888951 OGDUtils-1.0.2/src/OGDUtils/LAKELAND/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/LAKELAND/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/LAKELAND/lakeland_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.892951 OGDUtils-1.0.2/src/OGDUtils/WAVES/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/WAVES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/WAVES/waves_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.892951 OGDUtils-1.0.2/src/OGDUtils/general/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/FeatureSetOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24764 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-06 06:19:53.000000 OGDUtils-1.0.2/src/OGDUtils/general/ogd_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:20:36.888951 OGDUtils-1.0.2/src/OGDUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 06:20:36.000000 OGDUtils-1.0.2/src/OGDUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 06:20:36.000000 OGDUtils-1.0.2/src/OGDUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:20:36.000000 OGDUtils-1.0.2/src/OGDUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 06:20:36.000000 OGDUtils-1.0.2/src/OGDUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.254112 OGDUtils-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 16:05:30.254112 OGDUtils-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:05:30.254112 OGDUtils-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/OGDUtils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/OGDUtils/JOWILDER/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/JOWILDER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37301 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/JOWILDER/jowilder_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/OGDUtils/LAKELAND/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/LAKELAND/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/LAKELAND/lakeland_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/OGDUtils/WAVES/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/WAVES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/WAVES/waves_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.250112 OGDUtils-1.1.0/src/OGDUtils/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/FeatureSetOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24764 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-06 16:04:40.000000 OGDUtils-1.1.0/src/OGDUtils/general/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:05:30.246112 OGDUtils-1.1.0/src/OGDUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-06 16:05:30.000000 OGDUtils-1.1.0/src/OGDUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-06 16:05:30.000000 OGDUtils-1.1.0/src/OGDUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:05:30.000000 OGDUtils-1.1.0/src/OGDUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 16:05:30.000000 OGDUtils-1.1.0/src/OGDUtils.egg-info/top_level.txt
```

### Comparing `OGDUtils-1.0.2/LICENSE` & `OGDUtils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/PKG-INFO` & `OGDUtils-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OGDUtils
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package with utilities for working with output data from the Open Game Data core
 Author: John McCloskey
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/OGDUtils
 Project-URL: Bug Tracker, https://github.com/opengamedata/OGDUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OGDUtils-1.0.2/README.md` & `OGDUtils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/pyproject.toml` & `OGDUtils-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/JOWILDER/jowilder_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/JOWILDER/jowilder_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/LAKELAND/lakeland_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/LAKELAND/lakeland_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/WAVES/waves_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/WAVES/waves_utils.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/general/FeatureSetOptions.py` & `OGDUtils-1.1.0/src/OGDUtils/general/FeatureSetOptions.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/general/Workflow.py` & `OGDUtils-1.1.0/src/OGDUtils/general/Workflow.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/general/feature_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/general/features.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/general/import_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/general/fileio.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils/general/ogd_utils.py` & `OGDUtils-1.1.0/src/OGDUtils/general/general.py`

 * *Files identical despite different names*

### Comparing `OGDUtils-1.0.2/src/OGDUtils.egg-info/PKG-INFO` & `OGDUtils-1.1.0/src/OGDUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OGDUtils
-Version: 1.0.2
+Version: 1.1.0
 Summary: A package with utilities for working with output data from the Open Game Data core
 Author: John McCloskey
 Author-email: Luke Swanson <superscription58@gmail.com>
 Project-URL: Homepage, https://github.com/opengamedata/OGDUtils
 Project-URL: Bug Tracker, https://github.com/opengamedata/OGDUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OGDUtils-1.0.2/src/OGDUtils.egg-info/SOURCES.txt` & `OGDUtils-1.1.0/src/OGDUtils.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 src/OGDUtils/LAKELAND/__init__.py
 src/OGDUtils/LAKELAND/lakeland_utils.py
 src/OGDUtils/WAVES/__init__.py
 src/OGDUtils/WAVES/waves_utils.py
 src/OGDUtils/general/FeatureSetOptions.py
 src/OGDUtils/general/Workflow.py
 src/OGDUtils/general/__init__.py
-src/OGDUtils/general/feature_utils.py
-src/OGDUtils/general/import_utils.py
-src/OGDUtils/general/ogd_utils.py
+src/OGDUtils/general/features.py
+src/OGDUtils/general/fileio.py
+src/OGDUtils/general/general.py
```

