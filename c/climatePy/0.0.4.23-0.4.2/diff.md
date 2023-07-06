# Comparing `tmp/climatePy-0.0.4.23.tar.gz` & `tmp/climatePy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.0.4.23.tar", last modified: Thu Jul  6 20:07:50 2023, max compression
+gzip compressed data, was "climatePy-0.4.2.tar", last modified: Thu Jul  6 21:05:04 2023, max compression
```

## Comparing `climatePy-0.0.4.23.tar` & `climatePy-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26691 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43848 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:04.261031 climatePy-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 21:05:01.000000 climatePy-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-06 21:05:04.261031 climatePy-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 21:05:01.000000 climatePy-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:04.217031 climatePy-0.4.2/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26691 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:04.217031 climatePy-0.4.2/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-06 21:05:01.000000 climatePy-0.4.2/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:04.217031 climatePy-0.4.2/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-06 21:05:04.000000 climatePy-0.4.2/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 21:05:04.000000 climatePy-0.4.2/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:05:04.000000 climatePy-0.4.2/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 21:05:04.000000 climatePy-0.4.2/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:05:04.000000 climatePy-0.4.2/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:05:04.261031 climatePy-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 21:05:03.000000 climatePy-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:04.261031 climatePy-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:05:01.000000 climatePy-0.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43848 2023-07-06 21:05:01.000000 climatePy-0.4.2/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 21:05:01.000000 climatePy-0.4.2/tests/test_utils.py
```

### Comparing `climatePy-0.0.4.23/LICENSE` & `climatePy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/PKG-INFO` & `climatePy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.0.4.23
+Version: 0.4.2
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.0.4.23/README.md` & `climatePy-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/__init__.py` & `climatePy-0.4.2/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/_climatepy_filter.py` & `climatePy-0.4.2/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/_dap.py` & `climatePy-0.4.2/climatePy/_dap.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/_netrc_utils.py` & `climatePy-0.4.2/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/_shortcuts.py` & `climatePy-0.4.2/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/_utils.py` & `climatePy-0.4.2/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy/data/catalog.csv` & `climatePy-0.4.2/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.2/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.0.4.23
+Version: 0.4.2
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.0.4.23/setup.py` & `climatePy-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
-    version="0.0.4.23",                        # version
+    # version="0.0.4.24",                        # version
+    version='0.4.2',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.0.4.23/tests/test_shortcuts.py` & `climatePy-0.4.2/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.23/tests/test_utils.py` & `climatePy-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

