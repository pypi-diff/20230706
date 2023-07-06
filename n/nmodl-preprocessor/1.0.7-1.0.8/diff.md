# Comparing `tmp/nmodl_preprocessor-1.0.7.tar.gz` & `tmp/nmodl_preprocessor-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmodl_preprocessor-1.0.7.tar", last modified: Wed Jun 21 00:12:56 2023, max compression
+gzip compressed data, was "nmodl_preprocessor-1.0.8.tar", last modified: Thu Jul  6 16:33:52 2023, max compression
```

## Comparing `nmodl_preprocessor-1.0.7.tar` & `nmodl_preprocessor-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.7/.gitignore
--rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.7/DETAILS.pdf
--rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.7/LICENSE.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)     1899 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)     1158 2023-06-20 16:40:09.000000 nmodl_preprocessor-1.0.7/README.md
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nmodl_preprocessor/
--rw-rw-r--   0 dm        (1000) dm        (1000)     7434 2023-06-21 00:08:06.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/__main__.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/cpp_keywords.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     4592 2023-05-16 19:37:54.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/nmodl_to_python.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    21822 2023-06-20 15:54:47.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/optimize_nmodl.py
--rw-rw-r--   0 dm        (1000) dm        (1000)     5722 2023-05-15 17:49:58.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/rw_patterns.py
--rw-rw-r--   0 dm        (1000) dm        (1000)      710 2023-05-10 18:26:19.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor/utils.py
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/
--rw-rw-r--   0 dm        (1000) dm        (1000)     1899 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/PKG-INFO
--rw-rw-r--   0 dm        (1000) dm        (1000)      598 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/SOURCES.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/dependency_links.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/entry_points.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/requires.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-06-21 00:12:56.000000 nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/top_level.txt
-drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/
--rw-rw-r--   0 dm        (1000) dm        (1000)     1455 2023-06-20 23:34:46.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/diff_perf.py
--rw-rw-r--   0 dm        (1000) dm        (1000)    10774 2023-06-20 23:28:01.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/histogram.png
--rw-rw-r--   0 dm        (1000) dm        (1000)      489 2023-06-20 23:36:03.000000 nmodl_preprocessor-1.0.7/nrn-modeldb-ci/notes.txt
--rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-06-20 04:56:50.000000 nmodl_preprocessor-1.0.7/pyproject.toml
--rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-06-21 00:12:56.613682 nmodl_preprocessor-1.0.7/setup.cfg
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-06 16:33:52.822247 nmodl_preprocessor-1.0.8/
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-04-19 23:44:54.000000 nmodl_preprocessor-1.0.8/.gitignore
+-rw-rw-r--   0 dm        (1000) dm        (1000)    37883 2023-04-19 23:02:12.000000 nmodl_preprocessor-1.0.8/DETAILS.pdf
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1076 2023-03-28 16:31:04.000000 nmodl_preprocessor-1.0.8/LICENSE.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2031 2023-07-06 16:33:52.822247 nmodl_preprocessor-1.0.8/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1290 2023-07-02 02:20:53.000000 nmodl_preprocessor-1.0.8/README.md
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-06 16:33:52.818247 nmodl_preprocessor-1.0.8/nmodl_preprocessor/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     7434 2023-06-21 00:08:06.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/__main__.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1642 2023-04-29 16:57:39.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/cpp_keywords.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     4592 2023-05-16 19:37:54.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/nmodl_to_python.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    21822 2023-06-21 16:05:33.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/optimize_nmodl.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)     5722 2023-05-15 17:49:58.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/rw_patterns.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)      710 2023-05-10 18:26:19.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor/utils.py
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-06 16:33:52.818247 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     2031 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/PKG-INFO
+-rw-rw-r--   0 dm        (1000) dm        (1000)      598 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/SOURCES.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        1 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/dependency_links.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       80 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/entry_points.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)        6 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/requires.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)       19 2023-07-06 16:33:52.000000 nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/top_level.txt
+drwxrwxr-x   0 dm        (1000) dm        (1000)        0 2023-07-06 16:33:52.822247 nmodl_preprocessor-1.0.8/nrn-modeldb-ci/
+-rw-rw-r--   0 dm        (1000) dm        (1000)     1455 2023-06-20 23:34:46.000000 nmodl_preprocessor-1.0.8/nrn-modeldb-ci/diff_perf.py
+-rw-rw-r--   0 dm        (1000) dm        (1000)    10774 2023-06-20 23:28:01.000000 nmodl_preprocessor-1.0.8/nrn-modeldb-ci/histogram.png
+-rw-rw-r--   0 dm        (1000) dm        (1000)      489 2023-06-20 23:36:03.000000 nmodl_preprocessor-1.0.8/nrn-modeldb-ci/notes.txt
+-rw-rw-r--   0 dm        (1000) dm        (1000)      957 2023-07-05 18:28:15.000000 nmodl_preprocessor-1.0.8/pyproject.toml
+-rw-rw-r--   0 dm        (1000) dm        (1000)       38 2023-07-06 16:33:52.822247 nmodl_preprocessor-1.0.8/setup.cfg
```

### Comparing `nmodl_preprocessor-1.0.7/DETAILS.pdf` & `nmodl_preprocessor-1.0.8/DETAILS.pdf`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/LICENSE.txt` & `nmodl_preprocessor-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/PKG-INFO` & `nmodl_preprocessor-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl_preprocessor
-Version: 1.0.7
+Version: 1.0.8
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -53,13 +53,17 @@
 options:
   -h, --help   show this help message and exit
 
 ```
 
 ## Tips
 
+* Always check your results for accuracy and correctness.
+
+* Do not use this tool with neuron's graphical user interface "nrngui".
+
 * Keep your projects in separate directories.  
 
 * Use unique and descriptive variable names.  
 
 * Remove unnecessary VERBATIM statements.
```

### Comparing `nmodl_preprocessor-1.0.7/README.md` & `nmodl_preprocessor-1.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -33,13 +33,17 @@
 options:
   -h, --help   show this help message and exit
 
 ```
 
 ## Tips
 
+* Always check your results for accuracy and correctness.
+
+* Do not use this tool with neuron's graphical user interface "nrngui".
+
 * Keep your projects in separate directories.  
 
 * Use unique and descriptive variable names.  
 
 * Remove unnecessary VERBATIM statements.
```

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/__main__.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/cpp_keywords.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/cpp_keywords.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/nmodl_to_python.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/nmodl_to_python.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/optimize_nmodl.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/optimize_nmodl.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/rw_patterns.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/rw_patterns.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor/utils.py` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/PKG-INFO` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nmodl-preprocessor
-Version: 1.0.7
+Version: 1.0.8
 Summary: Optimize NMODL files for the NEURON simulator
 Author-email: David McDougall <dam1784@rit.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/ctrl-z-9000-times/nmodl_preprocessor
 Keywords: nmodl,neuron
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -53,13 +53,17 @@
 options:
   -h, --help   show this help message and exit
 
 ```
 
 ## Tips
 
+* Always check your results for accuracy and correctness.
+
+* Do not use this tool with neuron's graphical user interface "nrngui".
+
 * Keep your projects in separate directories.  
 
 * Use unique and descriptive variable names.  
 
 * Remove unnecessary VERBATIM statements.
```

### Comparing `nmodl_preprocessor-1.0.7/nmodl_preprocessor.egg-info/SOURCES.txt` & `nmodl_preprocessor-1.0.8/nmodl_preprocessor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nrn-modeldb-ci/diff_perf.py` & `nmodl_preprocessor-1.0.8/nrn-modeldb-ci/diff_perf.py`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/nrn-modeldb-ci/histogram.png` & `nmodl_preprocessor-1.0.8/nrn-modeldb-ci/histogram.png`

 * *Files identical despite different names*

### Comparing `nmodl_preprocessor-1.0.7/pyproject.toml` & `nmodl_preprocessor-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["nmodl_preprocessor"]
 
 [project]
 name = "nmodl_preprocessor"
-version = "1.0.7"
+version = "1.0.8"
 description = "Optimize NMODL files for the NEURON simulator"
 readme = "README.md"
 license = {text = "MIT"}
 authors = [
     {name = "David McDougall", email = "dam1784@rit.edu"},
 ]
 urls = {Homepage = "https://github.com/ctrl-z-9000-times/nmodl_preprocessor"}
```

