# Comparing `tmp/btimer-1.0.8.tar.gz` & `tmp/btimer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btimer-1.0.8.tar", last modified: Fri Jun 30 06:12:17 2023, max compression
+gzip compressed data, was "btimer-1.0.9.tar", last modified: Mon Jul  3 09:18:12 2023, max compression
```

## Comparing `btimer-1.0.8.tar` & `btimer-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,34 @@
-drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 06:12:17.427322 btimer-1.0.8/
--rw-r--r--   0 dylan      (502) staff       (20)     1075 2023-06-30 02:58:44.000000 btimer-1.0.8/LICENSE.txt
--rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 06:12:17.427173 btimer-1.0.8/PKG-INFO
--rw-r--r--   0 dylan      (502) staff       (20)      730 2023-06-30 02:58:44.000000 btimer-1.0.8/README.md
-drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-06-30 06:12:17.426961 btimer-1.0.8/btimer.egg-info/
--rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (502) staff       (20)      227 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (502) staff       (20)        1 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/entry_points.txt
--rw-r--r--   0 dylan      (502) staff       (20)       13 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/requires.txt
--rw-r--r--   0 dylan      (502) staff       (20)        6 2023-06-30 06:12:17.000000 btimer-1.0.8/btimer.egg-info/top_level.txt
--rw-r--r--   0 dylan      (502) staff       (20)      688 2023-06-30 06:11:40.000000 btimer-1.0.8/pyproject.toml
--rw-r--r--   0 dylan      (502) staff       (20)       38 2023-06-30 06:12:17.427363 btimer-1.0.8/setup.cfg
--rw-r--r--   0 dylan      (502) staff       (20)     1274 2023-06-30 03:25:13.000000 btimer-1.0.8/timer.py
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.388369 btimer-1.0.9/
+-rw-r--r--   0 dylan      (502) staff       (20)     6148 2023-06-30 02:58:44.000000 btimer-1.0.9/.DS_Store
+-rw-r--r--   0 dylan      (502) staff       (20)      482 2023-06-30 02:58:44.000000 btimer-1.0.9/.gitignore
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.384355 btimer-1.0.9/.idea/
+-rw-r--r--   0 dylan      (502) staff       (20)       47 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/.gitignore
+-rw-r--r--   0 dylan      (502) staff       (20)      395 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/buddhist.iml
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.384498 btimer-1.0.9/.idea/inspectionProfiles/
+-rw-r--r--   0 dylan      (502) staff       (20)      174 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 dylan      (502) staff       (20)      196 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/misc.xml
+-rw-r--r--   0 dylan      (502) staff       (20)      268 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/modules.xml
+-rw-r--r--   0 dylan      (502) staff       (20)      180 2023-06-30 02:58:44.000000 btimer-1.0.9/.idea/vcs.xml
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.384634 btimer-1.0.9/.vscode/
+-rw-r--r--   0 dylan      (502) staff       (20)      130 2023-06-30 02:58:44.000000 btimer-1.0.9/.vscode/settings.json
+-rw-r--r--   0 dylan      (502) staff       (20)     1075 2023-06-30 02:58:44.000000 btimer-1.0.9/LICENSE.txt
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-07-03 09:18:12.388222 btimer-1.0.9/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      730 2023-06-30 02:58:44.000000 btimer-1.0.9/README.md
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.385376 btimer-1.0.9/btimer/
+-rw-r--r--   0 dylan      (502) staff       (20)       45 2023-07-03 08:30:01.000000 btimer-1.0.9/btimer/__init__.py
+-rw-r--r--   0 dylan      (502) staff       (20)     1274 2023-07-03 08:47:03.000000 btimer-1.0.9/btimer/btimer.py
+-rw-r--r--   0 dylan      (502) staff       (20)      894 2023-07-03 08:03:39.000000 btimer-1.0.9/btimer/verses.json
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.386150 btimer-1.0.9/btimer.egg-info/
+-rw-r--r--   0 dylan      (502) staff       (20)     1240 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (502) staff       (20)      503 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        1 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       39 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/entry_points.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       13 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/requires.txt
+-rw-r--r--   0 dylan      (502) staff       (20)        7 2023-07-03 09:18:12.000000 btimer-1.0.9/btimer.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (502) staff       (20)        0 2023-07-03 09:18:12.386382 btimer-1.0.9/doc/
+-rw-r--r--   0 dylan      (502) staff       (20)     6148 2023-06-30 02:58:44.000000 btimer-1.0.9/doc/.DS_Store
+-rw-r--r--   0 dylan      (502) staff       (20)  1120133 2023-06-30 02:58:44.000000 btimer-1.0.9/doc/img01.png
+-rw-r--r--   0 dylan      (502) staff       (20)      828 2023-07-03 09:15:03.000000 btimer-1.0.9/pyproject.toml
+-rw-r--r--   0 dylan      (502) staff       (20)      131 2023-06-30 02:58:44.000000 btimer-1.0.9/requirements.txt
+-rw-r--r--   0 dylan      (502) staff       (20)       38 2023-07-03 09:18:12.388406 btimer-1.0.9/setup.cfg
+-rw-r--r--   0 dylan      (502) staff       (20)      894 2023-07-03 08:38:58.000000 btimer-1.0.9/verses.json
```

### Comparing `btimer-1.0.8/LICENSE.txt` & `btimer-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btimer-1.0.8/PKG-INFO` & `btimer-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.8/README.md` & `btimer-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `btimer-1.0.8/btimer.egg-info/PKG-INFO` & `btimer-1.0.9/btimer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btimer
-Version: 1.0.8
+Version: 1.0.9
 Summary: Help people get away from the computer
 Author-email: Dylan Ngo <it.tinhngo@gmail.com>
 Project-URL: Homepage, https://github.com/dylanngo95/timer
 Project-URL: Bug Tracker, https://github.com/dylanngo95/timer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btimer-1.0.8/pyproject.toml` & `btimer-1.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,22 @@
+[build-system]
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["btimer"]
+namespaces = true
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
+
 [project]
 name = "btimer"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Dylan Ngo", email="it.tinhngo@gmail.com" },
 ]
 description = "Help people get away from the computer"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -13,18 +25,12 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "rich==13.4.2"
 ]
 
 [project.scripts]
-btimer = "timer:main"
-
-[tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
-
-[tool.setuptools]
-include-package-data = true
+btimer = "btimer:main"
 
 [project.urls]
 "Homepage" = "https://github.com/dylanngo95/timer"
 "Bug Tracker" = "https://github.com/dylanngo95/timer/issues"
```

### Comparing `btimer-1.0.8/timer.py` & `btimer-1.0.9/btimer/btimer.py`

 * *Files identical despite different names*

