# Comparing `tmp/omnivoreql-0.1.2.tar.gz` & `tmp/omnivoreql-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.1.2.tar", last modified: Wed Jul  5 21:49:13 2023, max compression
+gzip compressed data, was "omnivoreql-0.1.3.tar", last modified: Wed Jul  5 22:24:29 2023, max compression
```

## Comparing `omnivoreql-0.1.2.tar` & `omnivoreql-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:49:13.596272 omnivoreql-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 21:49:13.596272 omnivoreql-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:49:13.592271 omnivoreql-0.1.2/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/omnivoreql/__init__,py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/omnivoreql/omnivoreql.py
--rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/omnivoreql/schema.gql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:49:13.596272 omnivoreql-0.1.2/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 21:49:13.000000 omnivoreql-0.1.2/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 21:49:13.000000 omnivoreql-0.1.2/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:49:13.000000 omnivoreql-0.1.2/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 21:49:13.000000 omnivoreql-0.1.2/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 21:49:13.000000 omnivoreql-0.1.2/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:49:13.596272 omnivoreql-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 21:49:09.000000 omnivoreql-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:24:29.312725 omnivoreql-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 22:24:29.312725 omnivoreql-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:24:29.312725 omnivoreql-0.1.3/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/omnivoreql/__init__,py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/omnivoreql/omnivoreql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/omnivoreql/schema.gql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:24:29.312725 omnivoreql-0.1.3/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-05 22:24:29.000000 omnivoreql-0.1.3/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-05 22:24:29.000000 omnivoreql-0.1.3/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:24:29.000000 omnivoreql-0.1.3/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-05 22:24:29.000000 omnivoreql-0.1.3/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 22:24:29.000000 omnivoreql-0.1.3/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:24:29.312725 omnivoreql-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-05 22:24:24.000000 omnivoreql-0.1.3/setup.py
```

### Comparing `omnivoreql-0.1.2/LICENSE` & `omnivoreql-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.2/PKG-INFO` & `omnivoreql-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.1.2/README.md` & `omnivoreql-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.2/omnivoreql/omnivoreql.py` & `omnivoreql-0.1.3/omnivoreql/omnivoreql.py`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.2/omnivoreql/schema.gql` & `omnivoreql-0.1.3/omnivoreql/schema.gql`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.1.2/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.1.3/omnivoreql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.1.2
+Version: 0.1.3
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.1.2/setup.py` & `omnivoreql-0.1.3/setup.py`

 * *Files identical despite different names*

