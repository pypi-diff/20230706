# Comparing `tmp/stc-geck-1.2.9.tar.gz` & `tmp/stc-geck-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.9.tar", last modified: Thu Jul  6 10:33:31 2023, max compression
+gzip compressed data, was "stc-geck-1.3.0.tar", last modified: Thu Jul  6 10:45:43 2023, max compression
```

## Comparing `stc-geck-1.2.9.tar` & `stc-geck-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:33:31.642277 stc-geck-1.2.9/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.9/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:33:31.642022 stc-geck-1.2.9/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.9/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-06 10:33:21.000000 stc-geck-1.2.9/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.2.9/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 10:33:31.642370 stc-geck-1.2.9/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:33:31.639222 stc-geck-1.2.9/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)      913 2023-07-06 10:33:10.000000 stc-geck-1.2.9/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.2.9/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5950 2023-07-05 19:36:58.000000 stc-geck-1.2.9/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1640 2023-07-05 19:36:42.000000 stc-geck-1.2.9/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:33:31.641625 stc-geck-1.2.9/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-06 10:33:31.000000 stc-geck-1.2.9/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:45:43.275231 stc-geck-1.3.0/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.3.0/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:45:43.274986 stc-geck-1.3.0/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.3.0/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-06 10:45:26.000000 stc-geck-1.3.0/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.3.0/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 10:45:43.275321 stc-geck-1.3.0/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:45:43.272112 stc-geck-1.3.0/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)      913 2023-07-06 10:33:10.000000 stc-geck-1.3.0/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.3.0/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5950 2023-07-05 19:36:58.000000 stc-geck-1.3.0/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1640 2023-07-05 19:36:42.000000 stc-geck-1.3.0/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:45:43.274582 stc-geck-1.3.0/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-06 10:45:43.000000 stc-geck-1.3.0/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.9/PKG-INFO` & `stc-geck-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.9
+Version: 1.3.0
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.2.9/pyproject.toml` & `stc-geck-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.9"
+version = "1.3.0"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.9/stc_geck/advices.py` & `stc-geck-1.3.0/stc_geck/advices.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.9/stc_geck/cli.py` & `stc-geck-1.3.0/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.9/stc_geck/client.py` & `stc-geck-1.3.0/stc_geck/client.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.9/stc_geck/utils.py` & `stc-geck-1.3.0/stc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.9/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.3.0/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.9
+Version: 1.3.0
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

