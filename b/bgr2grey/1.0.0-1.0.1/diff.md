# Comparing `tmp/bgr2grey-1.0.0.tar.gz` & `tmp/bgr2grey-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgr2grey-1.0.0.tar", last modified: Thu Jul  6 19:20:17 2023, max compression
+gzip compressed data, was "bgr2grey-1.0.1.tar", last modified: Thu Jul  6 19:23:05 2023, max compression
```

## Comparing `bgr2grey-1.0.0.tar` & `bgr2grey-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:20:17.360592 bgr2grey-1.0.0/
--rw-r--r--   0 divagar    (501) staff       (20)     1065 2023-07-06 18:06:32.000000 bgr2grey-1.0.0/LICENSE
--rw-r--r--   0 divagar    (501) staff       (20)      966 2023-07-06 19:20:17.360684 bgr2grey-1.0.0/PKG-INFO
--rw-r--r--   0 divagar    (501) staff       (20)      674 2023-07-06 19:19:13.000000 bgr2grey-1.0.0/README.md
-drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:20:17.359496 bgr2grey-1.0.0/bgr2grey/
--rw-r--r--   0 divagar    (501) staff       (20)      150 2023-07-06 19:14:05.000000 bgr2grey-1.0.0/bgr2grey/__init__.py
--rw-r--r--   0 divagar    (501) staff       (20)     1204 2023-07-06 19:13:02.000000 bgr2grey-1.0.0/bgr2grey/bgr2grey.py
-drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:20:17.360448 bgr2grey-1.0.0/bgr2grey.egg-info/
--rw-r--r--   0 divagar    (501) staff       (20)      966 2023-07-06 19:20:17.000000 bgr2grey-1.0.0/bgr2grey.egg-info/PKG-INFO
--rw-r--r--   0 divagar    (501) staff       (20)      243 2023-07-06 19:20:17.000000 bgr2grey-1.0.0/bgr2grey.egg-info/SOURCES.txt
--rw-r--r--   0 divagar    (501) staff       (20)        1 2023-07-06 19:20:17.000000 bgr2grey-1.0.0/bgr2grey.egg-info/dependency_links.txt
--rw-r--r--   0 divagar    (501) staff       (20)        6 2023-07-06 19:20:17.000000 bgr2grey-1.0.0/bgr2grey.egg-info/requires.txt
--rw-r--r--   0 divagar    (501) staff       (20)        9 2023-07-06 19:20:17.000000 bgr2grey-1.0.0/bgr2grey.egg-info/top_level.txt
--rw-r--r--   0 divagar    (501) staff       (20)      207 2023-07-06 19:15:39.000000 bgr2grey-1.0.0/pyproject.toml
--rw-r--r--   0 divagar    (501) staff       (20)      440 2023-07-06 19:20:17.361080 bgr2grey-1.0.0/setup.cfg
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:23:05.424889 bgr2grey-1.0.1/
+-rw-r--r--   0 divagar    (501) staff       (20)     1065 2023-07-06 18:06:32.000000 bgr2grey-1.0.1/LICENSE
+-rw-r--r--   0 divagar    (501) staff       (20)      966 2023-07-06 19:23:05.424980 bgr2grey-1.0.1/PKG-INFO
+-rw-r--r--   0 divagar    (501) staff       (20)      674 2023-07-06 19:19:13.000000 bgr2grey-1.0.1/README.md
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:23:05.423610 bgr2grey-1.0.1/bgr2grey/
+-rw-r--r--   0 divagar    (501) staff       (20)      150 2023-07-06 19:14:05.000000 bgr2grey-1.0.1/bgr2grey/__init__.py
+-rw-r--r--   0 divagar    (501) staff       (20)     1204 2023-07-06 19:13:02.000000 bgr2grey-1.0.1/bgr2grey/bgr2grey.py
+drwxr-xr-x   0 divagar    (501) staff       (20)        0 2023-07-06 19:23:05.424733 bgr2grey-1.0.1/bgr2grey.egg-info/
+-rw-r--r--   0 divagar    (501) staff       (20)      966 2023-07-06 19:23:05.000000 bgr2grey-1.0.1/bgr2grey.egg-info/PKG-INFO
+-rw-r--r--   0 divagar    (501) staff       (20)      243 2023-07-06 19:23:05.000000 bgr2grey-1.0.1/bgr2grey.egg-info/SOURCES.txt
+-rw-r--r--   0 divagar    (501) staff       (20)        1 2023-07-06 19:23:05.000000 bgr2grey-1.0.1/bgr2grey.egg-info/dependency_links.txt
+-rw-r--r--   0 divagar    (501) staff       (20)        6 2023-07-06 19:23:05.000000 bgr2grey-1.0.1/bgr2grey.egg-info/requires.txt
+-rw-r--r--   0 divagar    (501) staff       (20)        9 2023-07-06 19:23:05.000000 bgr2grey-1.0.1/bgr2grey.egg-info/top_level.txt
+-rw-r--r--   0 divagar    (501) staff       (20)      207 2023-07-06 19:15:39.000000 bgr2grey-1.0.1/pyproject.toml
+-rw-r--r--   0 divagar    (501) staff       (20)      440 2023-07-06 19:23:05.425469 bgr2grey-1.0.1/setup.cfg
```

### Comparing `bgr2grey-1.0.0/LICENSE` & `bgr2grey-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bgr2grey-1.0.0/PKG-INFO` & `bgr2grey-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bgr2grey
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for converting RGB images to grayscale
-Home-page: https://github.com/yourusername/bgr2grey
+Home-page: https://github.com/divagarn/bgr2grey.git
 Author: Divagar N
 Author-email: divagar2kn@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bgr2grey
```

### Comparing `bgr2grey-1.0.0/README.md` & `bgr2grey-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bgr2grey-1.0.0/bgr2grey/bgr2grey.py` & `bgr2grey-1.0.1/bgr2grey/bgr2grey.py`

 * *Files identical despite different names*

### Comparing `bgr2grey-1.0.0/bgr2grey.egg-info/PKG-INFO` & `bgr2grey-1.0.1/bgr2grey.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bgr2grey
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for converting RGB images to grayscale
-Home-page: https://github.com/yourusername/bgr2grey
+Home-page: https://github.com/divagarn/bgr2grey.git
 Author: Divagar N
 Author-email: divagar2kn@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bgr2grey
```

