# Comparing `tmp/lodkit-0.1.0.tar.gz` & `tmp/lodkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodkit-0.1.0.tar", max compression
+gzip compressed data, was "lodkit-0.1.1.tar", max compression
```

## Comparing `lodkit-0.1.0.tar` & `lodkit-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-06-05 13:34:34.817840 lodkit-0.1.0/LICENSE
--rw-r--r--   0        0        0     2877 2023-06-22 11:30:45.314872 lodkit-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-05 13:34:34.821173 lodkit-0.1.0/lodkit/__init__.py
--rw-r--r--   0        0        0     3138 2023-06-21 10:05:33.409340 lodkit-0.1.0/lodkit/connections.py
--rw-r--r--   0        0        0     1322 2023-06-20 10:13:37.139309 lodkit-0.1.0/lodkit/graph.py
--rw-r--r--   0        0        0     1274 2023-06-06 08:39:54.017219 lodkit-0.1.0/lodkit/importer.py
--rw-r--r--   0        0        0     2907 2023-06-20 10:13:37.139309 lodkit-0.1.0/lodkit/reasoners.py
--rw-r--r--   0        0        0      397 2023-06-20 10:13:37.142642 lodkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 lodkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-05 13:34:34.817840 lodkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2877 2023-07-06 06:20:51.465671 lodkit-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-05 13:34:34.821173 lodkit-0.1.1/lodkit/__init__.py
+-rw-r--r--   0        0        0     3138 2023-07-06 06:20:51.465671 lodkit-0.1.1/lodkit/connections.py
+-rw-r--r--   0        0        0     1335 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/graph.py
+-rw-r--r--   0        0        0     1274 2023-06-06 08:39:54.017219 lodkit-0.1.1/lodkit/importer.py
+-rw-r--r--   0        0        0     2914 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/reasoners.py
+-rw-r--r--   0        0        0      280 2023-07-06 06:20:59.159038 lodkit-0.1.1/lodkit/types.py
+-rw-r--r--   0        0        0      397 2023-07-06 06:22:18.586045 lodkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 lodkit-0.1.1/PKG-INFO
```

### Comparing `lodkit-0.1.0/LICENSE` & `lodkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.0/README.md` & `lodkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.0/lodkit/connections.py` & `lodkit-0.1.1/lodkit/connections.py`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.0/lodkit/graph.py` & `lodkit-0.1.1/lodkit/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """An rdflib.Graph subclass with plugin-based inferencing capability."""
 
 from typing import Optional
 import rdflib
-import reasoners
+
+from lodkit import reasoners
 
 
 _Reasoner = reasoners.Reasoner
 _ReasonerReference = _Reasoner | str
 
 
 class Graph(rdflib.Graph):
```

### Comparing `lodkit-0.1.0/lodkit/importer.py` & `lodkit-0.1.1/lodkit/importer.py`

 * *Files identical despite different names*

### Comparing `lodkit-0.1.0/lodkit/reasoners.py` & `lodkit-0.1.1/lodkit/reasoners.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import reasonable
 
 from franz.openrdf.rio.rdfformat import RDFFormat
 from rdflib import Graph
 from owlrl import DeductiveClosure, RDFS_OWLRL_Semantics, RDFS_Semantics
 
-from connections import AllegroConnection
+from lodkit.connections import AllegroConnection
 
 
 @runtime_checkable
 class Reasoner(Protocol):
     """Protocol class for lodkit.Graph reasoners."""
 
     def inference(self, graph: Graph) -> Graph:
```

### Comparing `lodkit-0.1.0/PKG-INFO` & `lodkit-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Lukas Plank
 Author-email: lupl@tuta.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agraph-python (>=102.0.0,<103.0.0)
```

