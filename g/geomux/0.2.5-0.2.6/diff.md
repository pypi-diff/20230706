# Comparing `tmp/geomux-0.2.5.tar.gz` & `tmp/geomux-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomux-0.2.5.tar", last modified: Wed Jul  5 20:26:47 2023, max compression
+gzip compressed data, was "geomux-0.2.6.tar", max compression
```

## Comparing `geomux-0.2.5.tar` & `geomux-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,8 @@
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/
--rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-07-05 20:26:47.535847 geomux-0.2.5/PKG-INFO
--rw-r--r--   0 noam      (1000) noam      (1000)     3282 2023-06-30 23:52:39.000000 geomux-0.2.5/README.md
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/geomux/
--rw-r--r--   0 noam      (1000) noam      (1000)       71 2023-06-23 19:19:47.000000 geomux-0.2.5/geomux/__init__.py
--rw-r--r--   0 noam      (1000) noam      (1000)     2482 2023-06-30 23:52:39.000000 geomux-0.2.5/geomux/__main__.py
--rw-r--r--   0 noam      (1000) noam      (1000)    10177 2023-07-05 20:26:30.000000 geomux-0.2.5/geomux/geomux.py
--rw-r--r--   0 noam      (1000) noam      (1000)     1005 2023-06-28 20:47:48.000000 geomux-0.2.5/geomux/utils.py
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/geomux.egg-info/
--rw-r--r--   0 noam      (1000) noam      (1000)     3548 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/PKG-INFO
--rw-r--r--   0 noam      (1000) noam      (1000)      309 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/SOURCES.txt
--rw-r--r--   0 noam      (1000) noam      (1000)        1 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/dependency_links.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       52 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/entry_points.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       36 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/requires.txt
--rw-r--r--   0 noam      (1000) noam      (1000)        7 2023-07-05 20:26:47.000000 geomux-0.2.5/geomux.egg-info/top_level.txt
--rw-r--r--   0 noam      (1000) noam      (1000)       38 2023-07-05 20:26:47.535847 geomux-0.2.5/setup.cfg
--rw-r--r--   0 noam      (1000) noam      (1000)      658 2023-07-05 20:26:30.000000 geomux-0.2.5/setup.py
-drwxr-xr-x   0 noam      (1000) noam      (1000)        0 2023-07-05 20:26:47.535847 geomux-0.2.5/tests/
--rw-r--r--   0 noam      (1000) noam      (1000)     3160 2023-06-30 23:52:39.000000 geomux-0.2.5/tests/test_geomux.py
--rw-r--r--   0 noam      (1000) noam      (1000)     1110 2023-06-28 20:47:48.000000 geomux-0.2.5/tests/test_io.py
+-rw-r--r--   0        0        0     1070 2023-07-06 16:28:36.932248 geomux-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3282 2023-07-06 15:32:39.788448 geomux-0.2.6/README.md
+-rw-r--r--   0        0        0       71 2023-07-06 15:32:39.815115 geomux-0.2.6/geomux/__init__.py
+-rw-r--r--   0        0        0     2482 2023-07-06 15:32:39.815115 geomux-0.2.6/geomux/__main__.py
+-rw-r--r--   0        0        0    10177 2023-07-06 15:32:39.815115 geomux-0.2.6/geomux/geomux.py
+-rw-r--r--   0        0        0     1005 2023-07-06 15:32:39.815115 geomux-0.2.6/geomux/utils.py
+-rw-r--r--   0        0        0      555 2023-07-06 16:28:36.932248 geomux-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3943 1970-01-01 00:00:00.000000 geomux-0.2.6/PKG-INFO
```

### Comparing `geomux-0.2.5/PKG-INFO` & `geomux-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: geomux
-Version: 0.2.5
-Summary: a tool to assign an identity to a table of barcode guides
-Home-page: https://github.com/noamteyssier/geomux
-Author: Noam Teysser
-Author-email: Noam.Teyssier@ucsf.edu
-Description-Content-Type: text/markdown
-
 # geomux
 
 A tool that assigns guides to cell barcodes. 
 
 Uses a hypergeometric distribution to calculate the pvalue of observing the
 specific count of a guide for each guide in each barcode.
 This can be used to calculate the MOI of the cell and assigned guides for each cell.
```

### Comparing `geomux-0.2.5/README.md` & `geomux-0.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: geomux
+Version: 0.2.6
+Summary: A tool to assign identifiers to cell barcodes
+License: MIT
+Author: Noam Teyssier
+Requires-Python: >=3.9,<3.13
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: adjustpy (>=0.1.1,<0.2.0)
+Requires-Dist: anndata (>=0.9.1,<0.10.0)
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: scipy (>=1.11.1,<2.0.0)
+Description-Content-Type: text/markdown
+
 # geomux
 
 A tool that assigns guides to cell barcodes. 
 
 Uses a hypergeometric distribution to calculate the pvalue of observing the
 specific count of a guide for each guide in each barcode.
 This can be used to calculate the MOI of the cell and assigned guides for each cell.
@@ -107,7 +126,8 @@
     - The number of UMIs observed in the cell.
 - p_value
     - The adjusted p-value of the hypergeometric test for that cell/guide test.
 - log_odds
     - The log odds of observing the highest scoring guide compared to the second highest.
 - tested
     - A bool flag representing whether the cell was included in the test (or `False` if it was filtered for low UMI counts)
+
```

### Comparing `geomux-0.2.5/geomux/__main__.py` & `geomux-0.2.6/geomux/__main__.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.5/geomux/geomux.py` & `geomux-0.2.6/geomux/geomux.py`

 * *Files identical despite different names*

### Comparing `geomux-0.2.5/geomux/utils.py` & `geomux-0.2.6/geomux/utils.py`

 * *Files identical despite different names*

