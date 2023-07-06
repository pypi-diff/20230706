# Comparing `tmp/lobster-tools-0.0.1.tar.gz` & `tmp/lobster-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lobster-tools-0.0.1.tar", last modified: Thu Jul  6 15:01:16 2023, max compression
+gzip compressed data, was "lobster-tools-0.0.2.tar", last modified: Thu Jul  6 15:52:10 2023, max compression
```

## Comparing `lobster-tools-0.0.1.tar` & `lobster-tools-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:01:16.265382 lobster-tools-0.0.1/
--rw-rw-r--   0 petit     (1001) petit     (1001)     1064 2023-05-10 18:13:46.000000 lobster-tools-0.0.1/LICENSE
--rw-rw-r--   0 petit     (1001) petit     (1001)      111 2023-04-27 10:12:58.000000 lobster-tools-0.0.1/MANIFEST.in
--rw-rw-r--   0 petit     (1001) petit     (1001)     5808 2023-07-06 15:01:16.265382 lobster-tools-0.0.1/PKG-INFO
--rw-rw-r--   0 petit     (1001) petit     (1001)     5146 2023-05-17 16:12:56.000000 lobster-tools-0.0.1/README.md
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:01:16.265382 lobster-tools-0.0.1/lobster_tools/
--rw-rw-r--   0 petit     (1001) petit     (1001)       85 2023-07-06 14:58:25.000000 lobster-tools-0.0.1/lobster_tools/__init__.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    12734 2023-07-06 14:51:44.000000 lobster-tools-0.0.1/lobster_tools/_modidx.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    16944 2023-07-06 14:51:44.000000 lobster-tools-0.0.1/lobster_tools/flow_decomposition.py
--rw-rw-r--   0 petit     (1001) petit     (1001)    12809 2023-07-06 14:51:44.000000 lobster-tools-0.0.1/lobster_tools/preprocessing.py
--rw-rw-r--   0 petit     (1001) petit     (1001)     4153 2023-07-06 14:51:44.000000 lobster-tools-0.0.1/lobster_tools/querying.py
--rw-rw-r--   0 petit     (1001) petit     (1001)      178 2023-05-15 22:05:13.000000 lobster-tools-0.0.1/lobster_tools/transformation.py
--rw-rw-r--   0 petit     (1001) petit     (1001)      184 2023-05-15 22:05:13.000000 lobster-tools-0.0.1/lobster_tools/visualisation.py
-drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:01:16.265382 lobster-tools-0.0.1/lobster_tools.egg-info/
--rw-rw-r--   0 petit     (1001) petit     (1001)     5808 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 petit     (1001) petit     (1001)      518 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)      163 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/entry_points.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-05-12 13:35:10.000000 lobster-tools-0.0.1/lobster_tools.egg-info/not-zip-safe
--rw-rw-r--   0 petit     (1001) petit     (1001)       33 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/requires.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)       14 2023-07-06 15:01:16.000000 lobster-tools-0.0.1/lobster_tools.egg-info/top_level.txt
--rw-rw-r--   0 petit     (1001) petit     (1001)     1265 2023-07-06 14:48:12.000000 lobster-tools-0.0.1/settings.ini
--rw-rw-r--   0 petit     (1001) petit     (1001)       38 2023-07-06 15:01:16.265382 lobster-tools-0.0.1/setup.cfg
--rw-rw-r--   0 petit     (1001) petit     (1001)     2601 2023-07-06 11:07:01.000000 lobster-tools-0.0.1/setup.py
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:52:10.838072 lobster-tools-0.0.2/
+-rw-rw-r--   0 petit     (1001) petit     (1001)     1064 2023-05-10 18:13:46.000000 lobster-tools-0.0.2/LICENSE
+-rw-rw-r--   0 petit     (1001) petit     (1001)      111 2023-04-27 10:12:58.000000 lobster-tools-0.0.2/MANIFEST.in
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5808 2023-07-06 15:52:10.838072 lobster-tools-0.0.2/PKG-INFO
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5146 2023-05-17 16:12:56.000000 lobster-tools-0.0.2/README.md
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:52:10.838072 lobster-tools-0.0.2/lobster_tools/
+-rw-rw-r--   0 petit     (1001) petit     (1001)       85 2023-07-06 15:49:28.000000 lobster-tools-0.0.2/lobster_tools/__init__.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    12734 2023-07-06 15:49:28.000000 lobster-tools-0.0.2/lobster_tools/_modidx.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    16944 2023-07-06 15:49:28.000000 lobster-tools-0.0.2/lobster_tools/flow_decomposition.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)    12809 2023-07-06 15:49:28.000000 lobster-tools-0.0.2/lobster_tools/preprocessing.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)     4153 2023-07-06 15:49:28.000000 lobster-tools-0.0.2/lobster_tools/querying.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)      178 2023-05-15 22:05:13.000000 lobster-tools-0.0.2/lobster_tools/transformation.py
+-rw-rw-r--   0 petit     (1001) petit     (1001)      184 2023-05-15 22:05:13.000000 lobster-tools-0.0.2/lobster_tools/visualisation.py
+drwxrwxr-x   0 petit     (1001) petit     (1001)        0 2023-07-06 15:52:10.838072 lobster-tools-0.0.2/lobster_tools.egg-info/
+-rw-rw-r--   0 petit     (1001) petit     (1001)     5808 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 petit     (1001) petit     (1001)      518 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)      163 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)        1 2023-05-12 13:35:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 petit     (1001) petit     (1001)       49 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/requires.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)       14 2023-07-06 15:52:10.000000 lobster-tools-0.0.2/lobster_tools.egg-info/top_level.txt
+-rw-rw-r--   0 petit     (1001) petit     (1001)     1281 2023-07-06 15:51:39.000000 lobster-tools-0.0.2/settings.ini
+-rw-rw-r--   0 petit     (1001) petit     (1001)       38 2023-07-06 15:52:10.838072 lobster-tools-0.0.2/setup.cfg
+-rw-rw-r--   0 petit     (1001) petit     (1001)     2601 2023-07-06 11:07:01.000000 lobster-tools-0.0.2/setup.py
```

### Comparing `lobster-tools-0.0.1/LICENSE` & `lobster-tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/PKG-INFO` & `lobster-tools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobster-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for working with LOBSTER data, the Nasdaq limit order book data.
 Home-page: https://github.com/n-petit/lobster-tools
 Author: nic
 Author-email: nicolas.petit@keble.ox.ac.uk
 License: MIT License
 Keywords: LOBSTER LOB nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.1 Summary: Python
+Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.2 Summary: Python
 package for working with LOBSTER data, the Nasdaq limit order book data. Home-
 page: https://github.com/n-petit/lobster-tools Author: nic Author-email:
 nicolas.petit@keble.ox.ac.uk License: MIT License Keywords: LOBSTER LOB nbdev
 jupyter notebook python Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `lobster-tools-0.0.1/README.md` & `lobster-tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/lobster_tools/_modidx.py` & `lobster-tools-0.0.2/lobster_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/lobster_tools/flow_decomposition.py` & `lobster-tools-0.0.2/lobster_tools/flow_decomposition.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/lobster_tools/preprocessing.py` & `lobster-tools-0.0.2/lobster_tools/preprocessing.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/lobster_tools/querying.py` & `lobster-tools-0.0.2/lobster_tools/querying.py`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/lobster_tools.egg-info/PKG-INFO` & `lobster-tools-0.0.2/lobster_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lobster-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for working with LOBSTER data, the Nasdaq limit order book data.
 Home-page: https://github.com/n-petit/lobster-tools
 Author: nic
 Author-email: nicolas.petit@keble.ox.ac.uk
 License: MIT License
 Keywords: LOBSTER LOB nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.1 Summary: Python
+Metadata-Version: 2.1 Name: lobster-tools Version: 0.0.2 Summary: Python
 package for working with LOBSTER data, the Nasdaq limit order book data. Home-
 page: https://github.com/n-petit/lobster-tools Author: nic Author-email:
 nicolas.petit@keble.ox.ac.uk License: MIT License Keywords: LOBSTER LOB nbdev
 jupyter notebook python Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.11 Description-Content-Type: text/
```

### Comparing `lobster-tools-0.0.1/lobster_tools.egg-info/SOURCES.txt` & `lobster-tools-0.0.2/lobster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lobster-tools-0.0.1/settings.ini` & `lobster-tools-0.0.2/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = lobster-tools
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.11
 license = MIT
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = lobster_tools
@@ -38,11 +38,11 @@
 description = Python package for working with LOBSTER data, the Nasdaq limit order book data.
 keywords = LOBSTER LOB nbdev jupyter notebook python
 language = English
 status = 3
 user = n-petit
 
 ### Optional ###
-requirements = pandas numpy scikit-learn
+requirements = pandas==2.0 numpy==1.25 scikit-learn==1.3
 # dev_requirements = black_formatting 
 console_scripts =   testa=lobster_tools.preprocessing:testa 
                     cli_example=lobster_tools.preprocessing:cli_example
```

### Comparing `lobster-tools-0.0.1/setup.py` & `lobster-tools-0.0.2/setup.py`

 * *Files identical despite different names*

