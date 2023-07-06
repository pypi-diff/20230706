# Comparing `tmp/bootstrapping_tools-2.0.0.tar.gz` & `tmp/bootstrapping_tools-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapping_tools-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bootstrapping_tools-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bootstrapping_tools-2.0.0.tar` & `bootstrapping_tools-3.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      200 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/README.md
--rw-r--r--   0        0        0      185 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/__init__.py
--rw-r--r--   0        0        0    11721 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/bootstrapping.py
--rw-r--r--   0        0        0      293 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/n0_and_lambdas_intervals.py
--rw-r--r--   0        0        0      859 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/bootstrapping_tools/resample_by_blocks.py
--rw-r--r--   0        0        0      516 2023-07-04 19:18:05.867960 bootstrapping_tools-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/README.md
+-rw-r--r--   0        0        0      185 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/bootstrapping_tools/__init__.py
+-rw-r--r--   0        0        0    11721 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/bootstrapping_tools/bootstrapping.py
+-rw-r--r--   0        0        0      293 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/bootstrapping_tools/n0_and_lambdas_intervals.py
+-rw-r--r--   0        0        0      877 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/bootstrapping_tools/resample_by_blocks.py
+-rw-r--r--   0        0        0      516 2023-07-06 16:55:37.684380 bootstrapping_tools-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-3.0.0/PKG-INFO
```

### Comparing `bootstrapping_tools-2.0.0/bootstrapping_tools/bootstrapping.py` & `bootstrapping_tools-3.0.0/bootstrapping_tools/bootstrapping.py`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-2.0.0/pyproject.toml` & `bootstrapping_tools-3.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-2.0.0/PKG-INFO` & `bootstrapping_tools-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapping_tools
-Version: 2.0.0
+Version: 3.0.0
 Summary: GECI Tools for bootstrapping
 Home-page: https://github.com/IslasGECI/bootstrapping_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bootstrapping_tools Version: 2.0.0 Summary: GECI
+Metadata-Version: 2.1 Name: bootstrapping_tools Version: 3.0.0 Summary: GECI
 Tools for bootstrapping Home-page: https://github.com/IslasGECI/
 bootstrapping_tools Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Requires-Dist: numpy Requires-Dist: pandas-stubs Requires-
 Dist: pandas Requires-Dist: scipy Requires-Dist: tqdm [https://
 www.islas.org.mx/img/logo.svg] # Bootstrapping tools GECI tools to perform
```

