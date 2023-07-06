# Comparing `tmp/SHACL2SPARQLpy-1.1.1.tar.gz` & `tmp/SHACL2SPARQLpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SHACL2SPARQLpy-1.1.1.tar", last modified: Tue Aug  2 09:35:36 2022, max compression
+gzip compressed data, was "SHACL2SPARQLpy-1.2.0.tar", last modified: Thu Jul  6 08:09:53 2023, max compression
```

## Comparing `SHACL2SPARQLpy-1.1.1.tar` & `SHACL2SPARQLpy-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/DependencyGraphImpl.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/Eval.py
--rw-r--r--   0 runner    (1001) docker     (121)    22086 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/RuleBasedValidation.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/SchemaImpl.py
--rw-r--r--   0 runner    (1001) docker     (121)     5731 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/Shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/ShapeNetwork.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/Literal.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/Query.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/RuleMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/
--rw-r--r--   0 runner    (1001) docker     (121)     6952 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/RuleBasedValidStats.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/fileManagement.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2022-08-02 09:35:36.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-08-02 09:35:36.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-02 09:35:36.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-02 09:35:36.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-02 09:35:36.000000 SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-08-02 09:35:36.297941 SHACL2SPARQLpy-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-02 09:35:23.000000 SHACL2SPARQLpy-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.462941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/DependencyGraphImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22086 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/RuleBasedValidation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/SchemaImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RuleMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/fileManagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:09:53.462941 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 08:09:53.000000 SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-06 08:09:53.466941 SHACL2SPARQLpy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-06 08:09:39.000000 SHACL2SPARQLpy-1.2.0/setup.py
```

### Comparing `SHACL2SPARQLpy-1.1.1/LICENSE` & `SHACL2SPARQLpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/PKG-INFO` & `SHACL2SPARQLpy-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: SHACL2SPARQLpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python reference implementation of SHACL2SPARQL
 Home-page: https://github.com/SDM-TIB/SHACL2SPARQLpy
 Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Latest Release](http://img.shields.io/github/release/SDM-TIB/SHACL2SPARQLpy.svg?logo=github)](https://github.com/SDM-TIB/SHACL2SPARQLpy/releases)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/SHACL2SPARQLpy)](https://pypi.org/project/SHACL2SPARQLpy)
```

### Comparing `SHACL2SPARQLpy-1.1.1/README.md` & `SHACL2SPARQLpy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/DependencyGraphImpl.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/DependencyGraphImpl.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/RuleBasedValidation.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/RuleBasedValidation.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/Shape.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/Shape.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/ShapeNetwork.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/ShapeNetwork.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/VariableGenerator.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/Constraint.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MaxOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MinMaxConstraint.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/constraints/MinOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/Literal.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/Literal.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/RuleMap.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RuleMap.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/core/RulePattern.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/QueryGenerator.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/QueryGenerator.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy/utils/RuleBasedValidStats.py` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy/utils/RuleBasedValidStats.py`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/PKG-INFO` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: SHACL2SPARQLpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python reference implementation of SHACL2SPARQL
 Home-page: https://github.com/SDM-TIB/SHACL2SPARQLpy
 Download-URL: https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Latest Release](http://img.shields.io/github/release/SDM-TIB/SHACL2SPARQLpy.svg?logo=github)](https://github.com/SDM-TIB/SHACL2SPARQLpy/releases)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/SHACL2SPARQLpy)](https://pypi.org/project/SHACL2SPARQLpy)
```

### Comparing `SHACL2SPARQLpy-1.1.1/SHACL2SPARQLpy.egg-info/SOURCES.txt` & `SHACL2SPARQLpy-1.2.0/SHACL2SPARQLpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SHACL2SPARQLpy-1.1.1/setup.py` & `SHACL2SPARQLpy-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SHACL2SPARQLpy',
-    version='1.1.1',
+    version='1.2.0',
     packages=['SHACL2SPARQLpy', 'SHACL2SPARQLpy.constraints', 'SHACL2SPARQLpy.core', 'SHACL2SPARQLpy.sparql', 'SHACL2SPARQLpy.utils'],
     license='MIT',
     author='Mónica Figuera, Philipp D. Rohde',
     author_email='philipp.rohde@tib.eu',
     url='https://github.com/SDM-TIB/SHACL2SPARQLpy',
     download_url='https://github.com/SDM-TIB/SHACL2SPARQLpy/archive/refs/tags/v1.1.0.tar.gz',
     description='Python reference implementation of SHACL2SPARQL',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['SPARQLWrapper>=1.8.5'],
-    python_requires='>=3.6',
+    install_requires=['SPARQLWrapper>=1.8.5', 'rdflib>=6.0.0'],
+    python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Science/Research'
       ]
 )
```

