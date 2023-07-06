# Comparing `tmp/fc-guarder-0.6.1.tar.gz` & `tmp/fc-guarder-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-guarder-0.6.1.tar", last modified: Thu Jul  6 05:55:13 2023, max compression
+gzip compressed data, was "dist/fc-guarder-0.6.2.tar", last modified: Thu Jul  6 08:49:04 2023, max compression
```

## Comparing `fc-guarder-0.6.1.tar` & `fc-guarder-0.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 05:53:39.000000 fc-guarder-0.6.1/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      671 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 05:53:39.000000 fc-guarder-0.6.1/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1928 2023-07-06 05:53:39.000000 fc-guarder-0.6.1/fc_guarder/guarder.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      671 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      265 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       55 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       17 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       11 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/fc_guarder.egg-info/top_level.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 05:55:13.000000 fc-guarder-0.6.1/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 05:53:39.000000 fc-guarder-0.6.1/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 08:48:52.000000 fc-guarder-0.6.2/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      671 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 08:48:52.000000 fc-guarder-0.6.2/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1928 2023-07-06 08:48:52.000000 fc-guarder-0.6.2/fc_guarder/guarder.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      671 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      265 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       55 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       17 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       11 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/fc_guarder.egg-info/top_level.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 08:49:04.000000 fc-guarder-0.6.2/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 08:48:52.000000 fc-guarder-0.6.2/setup.py
```

### Comparing `fc-guarder-0.6.1/LICENSE` & `fc-guarder-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.6.1/PKG-INFO` & `fc-guarder-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-guarder
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-guarder-0.6.1/README.rst` & `fc-guarder-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.6.1/fc_guarder/guarder.py` & `fc-guarder-0.6.2/fc_guarder/guarder.py`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.6.1/fc_guarder.egg-info/PKG-INFO` & `fc-guarder-0.6.2/fc_guarder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-guarder
-Version: 0.6.1
+Version: 0.6.2
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-guarder-0.6.1/setup.cfg` & `fc-guarder-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-guarder-0.6.1/setup.py` & `fc-guarder-0.6.2/setup.py`

 * *Files identical despite different names*

