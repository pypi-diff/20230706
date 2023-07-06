# Comparing `tmp/lobster-tools-0.0.3.tar.gz` & `tmp/lobster-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lobster-tools-0.0.3.tar", last modified: Thu Jul  6 16:00:09 2023, max compression
+gzip compressed data, was "lobster-tools-0.0.4.tar", last modified: Thu Jul  6 16:06:33 2023, max compression
```

## Comparing `lobster-tools-0.0.3.tar` & `lobster-tools-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:00:09.282685 lobster-tools-0.0.3/
--rw-rw-r--   0 petit     (1001) petit     (1001)     1064 2023-05-10 18:13:46.000000 lobster-tools-0.0.3/LICENSE
--rw-rw-r--   0 petit     (1001) petit     (1001)      111 2023-04-27 10:12:58.000000 lobster-tools-0.0.3/MANIFEST.in
--rw-rw-r--   0 petit     (1001) petit     (1001)     5809 2023-07-06 16:00:09.282685 lobster-tools-0.0.3/PKG-INFO
--rw-rw-r--   0 petit     (1001) petit     (1001)     5146 2023-05-17 16:12:56.000000 lobster-tools-0.0.3/README.md
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:00:09.282685 lobster-tools-0.0.3/lobster_tools/
--rw-rw-r--   0 petit     (1001) petit     (1001)       85 2023-07-06 15:49:28.000000 lobster-tools-0.0.3/lobster_tools/__init__.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    12734 2023-07-06 15:49:28.000000 lobster-tools-0.0.3/lobster_tools/_modidx.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    16944 2023-07-06 15:49:28.000000 lobster-tools-0.0.3/lobster_tools/flow_decomposition.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    12809 2023-07-06 15:49:28.000000 lobster-tools-0.0.3/lobster_tools/preprocessing.py
--rw-rw-r--   0 petit     (1001) petit     (1001)     4153 2023-07-06 15:49:28.000000 lobster-tools-0.0.3/lobster_tools/querying.py
--rw-rw-r--   0 petit     (1001) petit     (1001)      178 2023-05-15 22:05:13.000000 lobster-tools-0.0.3/lobster_tools/transformation.py
--rw-rw-r--   0 petit     (1001) petit     (1001)      184 2023-05-15 22:05:13.000000 lobster-tools-0.0.3/lobster_tools/visualisation.py
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:00:09.282685 lobster-tools-0.0.3/lobster_tools.egg-info/
--rw-rw-r--   0 petit     (1001) petit     (1001)     5809 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 petit     (1001) petit     (1001)      518 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)      163 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/entry_points.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-05-12 13:35:10.000000 lobster-tools-0.0.3/lobster_tools.egg-info/not-zip-safe
--rw-rw-r--   0 petit     (1001) petit     (1001)       49 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/requires.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)       14 2023-07-06 16:00:09.000000 lobster-tools-0.0.3/lobster_tools.egg-info/top_level.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)     1281 2023-07-06 15:59:31.000000 lobster-tools-0.0.3/settings.ini
--rw-rw-r--   0 petit     (1001) petit     (1001)       38 2023-07-06 16:00:09.282685 lobster-tools-0.0.3/setup.cfg
--rw-rw-r--   0 petit     (1001) petit     (1001)     2621 2023-07-06 15:58:14.000000 lobster-tools-0.0.3/setup.py
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:06:33.887169 lobster-tools-0.0.4/
+-rw-rw-r--   0 petit     (1001) petit     (1001)     1064 2023-05-10 18:13:46.000000 lobster-tools-0.0.4/LICENSE
+-rw-rw-r--   0 petit     (1001) petit     (1001)      111 2023-04-27 10:12:58.000000 lobster-tools-0.0.4/MANIFEST.in
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5809 2023-07-06 16:06:33.887169 lobster-tools-0.0.4/PKG-INFO
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5146 2023-05-17 16:12:56.000000 lobster-tools-0.0.4/README.md
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:06:33.883169 lobster-tools-0.0.4/lobster_tools/
+-rw-rw-r--   0 petit     (1001) petit     (1001)       85 2023-07-06 16:06:03.000000 lobster-tools-0.0.4/lobster_tools/__init__.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    12734 2023-07-06 16:06:03.000000 lobster-tools-0.0.4/lobster_tools/_modidx.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    16944 2023-07-06 16:06:03.000000 lobster-tools-0.0.4/lobster_tools/flow_decomposition.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    12809 2023-07-06 16:06:03.000000 lobster-tools-0.0.4/lobster_tools/preprocessing.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)     4153 2023-07-06 16:06:03.000000 lobster-tools-0.0.4/lobster_tools/querying.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)      178 2023-05-15 22:05:13.000000 lobster-tools-0.0.4/lobster_tools/transformation.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)      184 2023-05-15 22:05:13.000000 lobster-tools-0.0.4/lobster_tools/visualisation.py
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 16:06:33.887169 lobster-tools-0.0.4/lobster_tools.egg-info/
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5809 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 petit     (1001) petit     (1001)      518 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)      163 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-05-12 13:35:10.000000 lobster-tools-0.0.4/lobster_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 petit     (1001) petit     (1001)       49 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/requires.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)       14 2023-07-06 16:06:33.000000 lobster-tools-0.0.4/lobster_tools.egg-info/top_level.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)     1281 2023-07-06 16:05:58.000000 lobster-tools-0.0.4/settings.ini
+-rw-rw-r--   0 petit     (1001) petit     (1001)       38 2023-07-06 16:06:33.887169 lobster-tools-0.0.4/setup.cfg
+-rw-rw-r--   0 petit     (1001) petit     (1001)     2621 2023-07-06 15:58:14.000000 lobster-tools-0.0.4/setup.py
```

### Comparing `lobster-tools-0.0.3/LICENSE` & `lobster-tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/PKG-INFO` & `lobster-tools-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobster-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for working with LOBSTER data, the Nasdaq limit order book data.
 Home-page: https://github.com/n-petit/lobster-tools
 Author: nic
 Author-email: nicolas.petit@keble.ox.ac.uk
 License: MIT License
 Keywords: LOBSTER LOB nbdev jupyter notebook python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.3 Summary: Python
+Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.4 Summary: Python
 package for working with LOBSTER data, the Nasdaq limit order book data. Home-
 page: https://github.com/n-petit/lobster-tools Author: nic Author-email:
 nicolas.petit@keble.ox.ac.uk License: MIT License Keywords: LOBSTER LOB nbdev
 jupyter notebook python Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `lobster-tools-0.0.3/README.md` & `lobster-tools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/lobster_tools/_modidx.py` & `lobster-tools-0.0.4/lobster_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/lobster_tools/flow_decomposition.py` & `lobster-tools-0.0.4/lobster_tools/flow_decomposition.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/lobster_tools/preprocessing.py` & `lobster-tools-0.0.4/lobster_tools/preprocessing.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/lobster_tools/querying.py` & `lobster-tools-0.0.4/lobster_tools/querying.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/lobster_tools.egg-info/PKG-INFO` & `lobster-tools-0.0.4/lobster_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobster-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for working with LOBSTER data, the Nasdaq limit order book data.
 Home-page: https://github.com/n-petit/lobster-tools
 Author: nic
 Author-email: nicolas.petit@keble.ox.ac.uk
 License: MIT License
 Keywords: LOBSTER LOB nbdev jupyter notebook python
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.3 Summary: Python
+Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.4 Summary: Python
 package for working with LOBSTER data, the Nasdaq limit order book data. Home-
 page: https://github.com/n-petit/lobster-tools Author: nic Author-email:
 nicolas.petit@keble.ox.ac.uk License: MIT License Keywords: LOBSTER LOB nbdev
 jupyter notebook python Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `lobster-tools-0.0.3/lobster_tools.egg-info/SOURCES.txt` & `lobster-tools-0.0.4/lobster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.3/settings.ini` & `lobster-tools-0.0.4/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lobster-tools
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.11
 license = MIT
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lobster_tools
```

### Comparing `lobster-tools-0.0.3/setup.py` & `lobster-tools-0.0.4/setup.py`

 * *Files identical despite different names*

