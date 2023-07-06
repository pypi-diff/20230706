# Comparing `tmp/mutalyzer-algebra-1.2.1.tar.gz` & `tmp/mutalyzer-algebra-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutalyzer-algebra-1.2.1.tar", last modified: Mon Jun  5 08:45:02 2023, max compression
+gzip compressed data, was "mutalyzer-algebra-1.3.0.tar", last modified: Thu Jul  6 12:09:28 2023, max compression
```

## Comparing `mutalyzer-algebra-1.2.1.tar` & `mutalyzer-algebra-1.3.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     2602 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     1863 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.824218 mutalyzer-algebra-1.2.1/algebra/
--rw-rw-r--   0 mark      (1000) mark      (1000)      373 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/__main__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.824218 mutalyzer-algebra-1.2.1/algebra/lcs/
--rw-rw-r--   0 mark      (1000) mark      (1000)      237 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9631 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/all_lcs.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/lcs/distance_only.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/algebra/relations/
--rw-rw-r--   0 mark      (1000) mark      (1000)      698 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/relation.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/sequence_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4998 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/supremal_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1595 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/relations/variant_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3747 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/utils.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/algebra/variants/
--rw-rw-r--   0 mark      (1000) mark      (1000)      304 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8743 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/parser.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/algebra/variants/variant.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2602 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      686 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       51 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       30 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2023-06-05 08:45:02.000000 mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      884 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)       39 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-06-05 08:45:02.828218 mutalyzer-algebra-1.2.1/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2023-05-31 11:17:37.000000 mutalyzer-algebra-1.2.1/tests/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2835 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2086 2023-07-06 12:06:33.000000 mutalyzer-algebra-1.3.0/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      373 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2022-07-28 12:46:24.000000 mutalyzer-algebra-1.3.0/algebra/__main__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/extractor/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      209 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/extractor/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7787 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/extractor/extractor.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      575 2023-01-31 11:04:22.000000 mutalyzer-algebra-1.3.0/algebra/extractor/vis.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/lcs/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      237 2022-07-26 07:21:12.000000 mutalyzer-algebra-1.3.0/algebra/lcs/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     9329 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/lcs/all_lcs.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/algebra/lcs/distance_only.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/relations/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      698 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.0/algebra/relations/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/relations/relation.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/relations/sequence_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5466 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/relations/supremal_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1603 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/relations/variant_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4193 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/variants/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      328 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/variants/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8743 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.0/algebra/variants/parser.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/variants/variant.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2835 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      772 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       51 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       30 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      895 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)       39 2022-05-10 19:50:59.000000 mutalyzer-algebra-1.3.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/tests/__init__.py
```

### Comparing `mutalyzer-algebra-1.2.1/LICENSE` & `mutalyzer-algebra-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/PKG-INFO` & `mutalyzer-algebra-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
-Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs
+Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs,extractor
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
@@ -84,14 +84,26 @@
 lhs = parse_hgvs("2_7AT[4]")  # observed: CATATATATC
 rhs = parse_hgvs("5_6insT")   # observed: CATATTATC
 
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
+Extracting variants from sequences.
+
+```python
+from algebra.extractor import extract, to_hgvs
+
+reference = "CATATATC"
+observed = "CATATATATC"
+
+# returns: 2_7AT[4]
+to_hgvs(list(extract(reference, observed)), reference)
+```
+
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.1/README.md` & `mutalyzer-algebra-1.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -65,13 +65,25 @@
 lhs = parse_hgvs("2_7AT[4]")  # observed: CATATATATC
 rhs = parse_hgvs("5_6insT")   # observed: CATATTATC
 
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
+Extracting variants from sequences.
+
+```python
+from algebra.extractor import extract, to_hgvs
+
+reference = "CATATATC"
+observed = "CATATATATC"
+
+# returns: 2_7AT[4]
+to_hgvs(list(extract(reference, observed)), reference)
+```
+
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.1/algebra/__main__.py` & `mutalyzer-algebra-1.3.0/algebra/__main__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/algebra/lcs/all_lcs.py` & `mutalyzer-algebra-1.3.0/algebra/lcs/all_lcs.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
     def __init__(self, row, col, length=0):
         self.row = row
         self.col = col
         self.length = length
 
         self.edges = []
-        self.pre_edges = []
         self.incoming = 0
 
     def __eq__(self, other):
         return (self.row == other.row and self.col == other.col and
                 self.length == other.length)
 
     def __hash__(self):
@@ -155,114 +154,107 @@
     See Also
     --------
     `edit` : Calculates the LCS nodes.
     `traversal` : Traverses the LS graph.
     `algebra.utils.to_dot` : Graphviz DOT format.
     """
 
-    sink = _Node(len(reference) + 1, len(observed) + 1)
-    source = _Node(0, 0)
 
-    if reference == observed:
-        source.edges = [(sink, [])]
-        return source, []
+    edges = []
 
     if not lcs_nodes or lcs_nodes == [[]]:
+        source = _Node(0, 0, 0)
+        if not reference and not observed:
+            return source, edges
+        sink = _Node(len(reference) + 1, len(observed) + 1, 0)
         variant = Variant(0, len(reference), observed)
-        source.edges = [(sink, [variant])]
-        return source, [variant]
+        edges.append(variant)
+        source.edges = [(sink, variant)]
+        return source, edges
+
+    if lcs_nodes[-1][-1].row + lcs_nodes[-1][-1].length == len(reference) + 1 and lcs_nodes[-1][-1].col + lcs_nodes[-1][-1].length == len(observed) + 1:
+        sink = lcs_nodes[-1][-1]
+        sink.length += 1
+        for pred in lcs_nodes[-1][:-1]:
+            if pred.row + pred.length - 1 < sink.row + sink.length - 1 and pred.col + pred.length - 1 < sink.col + sink.length - 1:
+                variant = Variant(pred.row + pred.length - 1, sink.row + sink.length - 2, observed[pred.col + pred.length - 1:sink.col + sink.length - 2])
+                pred.edges.append((sink, variant))
+                edges.append(variant)
+        sink.length -= 1
+    else:
+        sink = _Node(len(reference) + 1, len(observed) + 1, 1)
+        for pred in lcs_nodes[-1]:
+            if pred.row + pred.length - 1 < sink.row + sink.length - 1 and pred.col + pred.length - 1 < sink.col + sink.length - 1:
+                variant = Variant(pred.row + pred.length - 1, sink.row + sink.length - 2, observed[pred.col + pred.length - 1:sink.col + sink.length - 2])
+                pred.edges.append((sink, variant))
+                edges.append(variant)
 
-    edges = []
-    for node in lcs_nodes[-1]:
-        offset = node.length
-        variant = Variant(node.row + offset - 1, len(reference), observed[node.col + offset - 1:])
-        if variant:
-            node.edges = [(sink, [variant])]
-            edges.append(variant)
-        else:
-            node.edges = [(sink, [])]
+    lcs_pos = len(lcs_nodes) - 1
+
+    while lcs_pos > 0:
+
+        nodes = lcs_nodes[lcs_pos]
 
-    for idx, nodes in enumerate(lcs_nodes[:0:-1]):
-        lcs_pos = len(lcs_nodes) - idx - 1
+        idx_split = [False for e in lcs_nodes[lcs_pos - 1]]
 
         while nodes:
             node = nodes.pop(0)
-            if not node.edges and not node.pre_edges:
+
+            if not node.edges and node != sink:
                 continue
 
-            offset = node.length - 1
-            for pred in nodes:
-                if pred.length <= 1:
-                    continue
-
-                pred_offset = pred.length - 1
-                if node.row + offset >= pred.row + pred_offset and node.col + offset >= pred.col + pred_offset:
-                    if node.pre_edges:
-                        split = _Node(node.row, node.col, node.length - 1)
-                        split.edges = node.pre_edges + [(node, [])]
-                        node.row += offset
-                        node.col += offset
-                        node.length = 1
-                        node.pre_edges = []
-                        offset = 0
-                        lcs_nodes[lcs_pos - 1].append(split)
+            idx_pred = -1
+            edge_added = False
 
-                    variant = Variant(pred.row + pred_offset - 1, node.row + offset - 1, observed[pred.col + pred_offset - 1:node.col + offset - 1])
-                    pred.pre_edges.append((node, [variant]))
-                    edges.append(variant)
-                    node.incoming = lcs_pos
+            for i, pred in enumerate(lcs_nodes[lcs_pos - 1]):
 
-            for pred_idx, pred in enumerate(lcs_nodes[lcs_pos - 1]):
-                pred_offset = pred.length
-                if node.row + offset >= pred.row + pred_offset and node.col + offset >= pred.col + pred_offset:
-                    if node.row + offset == pred.row + pred_offset and node.col + offset == pred.col + pred_offset:
-                        continue
+                if pred.row + pred.length - 1 < node.row + node.length - 1 and pred.col + pred.length - 1 < node.col + node.length - 1:
+                    variant = Variant(pred.row + pred.length - 1, node.row + node.length - 2, observed[pred.col + pred.length - 1:node.col + node.length - 2])
+                    edges.append(variant)
 
                     if pred.incoming == lcs_pos:
-                        split = _Node(pred.row, pred.col, pred.length)
-                        pred.row += pred_offset
-                        pred.col += pred_offset
-                        pred.length = 1
-                        split.edges = [(pred, [])]
-                        lcs_nodes[lcs_pos - 1][pred_idx] = split
-                        pred = split
-                    elif node.pre_edges:
-                        split = _Node(node.row, node.col, node.length - 1)
-                        split.edges = node.pre_edges + [(node, [])]
-                        node.row += offset
-                        node.col += offset
-                        node.length = 1
-                        node.pre_edges = []
-                        offset = 0
-                        lcs_nodes[lcs_pos - 1].append(split)
+                        idx_split[i] = False
+                        upper_node = _Node(pred.row, pred.col, pred.length)
+                        upper_node.edges = pred.edges + [(node, variant)]
+                        pred.length += 1
+                        lcs_nodes[lcs_pos - 1][i] = upper_node
+                    else:
+                        pred.edges.append((node, variant))
 
-                    variant = Variant(pred.row + pred_offset - 1, node.row + offset - 1, observed[pred.col + pred_offset - 1:node.col + offset - 1])
-                    pred.edges.append((node, [variant]))
-                    edges.append(variant)
                     node.incoming = lcs_pos
-
-            node.edges += node.pre_edges
-            node.pre_edges = []
+                    edge_added = True
+                    idx_pred = i
 
             if node.length > 1:
+                idx_insert = idx_pred + 1
                 node.length -= 1
-                lcs_nodes[lcs_pos - 1].append(node)
+                lcs_nodes[lcs_pos - 1].insert(idx_insert, node)
+                idx_split.insert(idx_insert, edge_added)
 
-    for node in lcs_nodes[0]:
-        if node.edges:
-            variant = Variant(0, node.row - 1, observed[:node.col - 1])
-            if variant:
-                source.edges.append((node, [variant]))
-                edges.append(variant)
-            else:
-                source.edges.append((node, []))
+        lcs_pos -= 1
+
+    if lcs_nodes[0][0].row == 1 == lcs_nodes[0][0].col:
+        source = lcs_nodes[0][0]
+        source.row -= 1
+        source.col -= 1
+        successors = lcs_nodes[0][1:]
+    else:
+        source = _Node(0, 0, 1)
+        successors = lcs_nodes[0]
+
+    for succ in successors:
+        if source.row + source.length - 1 < sink.row + sink.length - 1 and source.col + source.length - 1 < sink.col + sink.length - 1 and (succ == sink or succ.edges):
+            variant = Variant(source.row + source.length - 1, succ.row + succ.length - 2, observed[source.col + source.length - 1:succ.col + succ.length - 2])
+            source.edges.append((succ, variant))
+            edges.append(variant)
 
     return source, edges
 
 
+
 def traversal(root, atomics=False):
     """Traverse the LCS graph.
 
     Parameters
     ----------
     atomics : bool, optional
         If set to `True` the variants are represented using separate
@@ -275,20 +267,18 @@
 
     See Also
     --------
     `lcs_graph` : Constructs the LCS graph.
     """
 
     def traverse(node, path):
-        # depth-first traversal
         if not node.edges:
             yield path
-            return
 
         for succ, variant in node.edges:
-            if atomics and variant:
-                for atomic in variant[0].atomics():
+            if atomics:
+                for atomic in variant.atomics():
                     yield from traverse(succ, path + atomic)
             else:
-                yield from traverse(succ, path + variant)
+                yield from traverse(succ, path + [variant])
 
     yield from traverse(root, [])
```

### Comparing `mutalyzer-algebra-1.2.1/algebra/lcs/distance_only.py` & `mutalyzer-algebra-1.3.0/algebra/lcs/distance_only.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/algebra/relations/__init__.py` & `mutalyzer-algebra-1.3.0/algebra/relations/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/algebra/relations/sequence_based.py` & `mutalyzer-algebra-1.3.0/algebra/relations/sequence_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/algebra/relations/supremal_based.py` & `mutalyzer-algebra-1.3.0/algebra/relations/supremal_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Functions to find and compare supremal (minimum spanning) variants."""
+"""Functions to find, compare and construct supremal variants."""
 
 
 from operator import attrgetter
 from .relation import Relation
 from .sequence_based import (are_disjoint as sequence_based_are_disjoint,
                              compare as sequence_based_compare,
                              contains as sequence_based_contains,
@@ -98,47 +98,62 @@
 
     start = min(variants, key=attrgetter("start")).start
     end = max(variants, key=attrgetter("end")).end
     return Variant(start, end, observed[start:len(observed) - (len(reference) - end)])
 
 
 def find_supremal(reference, variant, offset=10):
-    """Iteratively find the supremal variant.
+    """Iteratively find the supremal variant by repeatedly widening a
+    range of influence.
 
     Parameters
     ----------
     reference : str
         The reference sequence.
     variant : `Variant`
         The variant of interest. Allele descriptions should be converted
         to a single (delins type) variant.
 
     Other Parameters
     ----------------
     offset : int, optional
         The minimum offset around the variant.
 
+    Returns
+    -------
+    supremal : `Variant`
+        The supremal variant.
+    root : `_Node`
+        The root of the LCS-graph in which the supremal was determined.
+    start : int
+        The start offset for the given LCS-graph.
+    observed : str
+        The observed sequence for the given LCS-graph.
+
     See Also
     --------
-    `spanning_variant` : The minimum spanning (delins) variant.
+    `spanning_variant` : The minimum spanning (delins) variant for an allele.
     """
 
     offset = max(offset, len(variant) // 2, 1)
 
     while True:
         start = max(0, variant.start - offset)
         end = min(len(reference), variant.end + offset)
 
         observed = reference[start:variant.start] + variant.sequence + reference[variant.end:end]
 
         _, lcs_nodes = edit(reference[start:end], observed)
-        _, edges = lcs_graph(reference[start:end], observed, lcs_nodes)
+        root, edges = lcs_graph(reference[start:end], observed, lcs_nodes)
         supremum = spanning_variant(reference[start:end], observed, edges)
 
+        if not supremum:
+            return supremum, root, start, observed
+
         supremum.start += start
         supremum.end += start
 
         if ((supremum.start > start or supremum.start == 0) and
                 (supremum.end < end or supremum.end == len(reference))):
-            return supremum
+            return supremum, root, start, observed
 
         offset *= 2
```

### Comparing `mutalyzer-algebra-1.2.1/algebra/relations/variant_based.py` & `mutalyzer-algebra-1.3.0/algebra/relations/variant_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,11 +45,11 @@
 
     Returns
     -------
     `Relation`
         The relation between the two variant alleles.
     """
 
-    lhs_sup = find_supremal(reference, spanning_variant(reference, patch(reference, lhs), lhs))
-    rhs_sup = find_supremal(reference, spanning_variant(reference, patch(reference, rhs), rhs))
+    lhs_sup, *_ = find_supremal(reference, spanning_variant(reference, patch(reference, lhs), lhs))
+    rhs_sup, *_ = find_supremal(reference, spanning_variant(reference, patch(reference, rhs), rhs))
 
     return compare_supremal(reference, lhs_sup, rhs_sup)
```

### Comparing `mutalyzer-algebra-1.2.1/algebra/utils.py` & `mutalyzer-algebra-1.3.0/algebra/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Utility functions for sequences and variants."""
 
 
+from collections import deque
 from itertools import chain
 import random
 from . import Variant
 from .variants import DNA_NUCLEOTIDES, to_hgvs
 
 
 def canonical(variants, max_distance=40):
@@ -29,26 +30,42 @@
     return Variant(start, start + len(deleted), inserted)
 
 
 def to_dot(reference, root):
     """The LCS graph in Graphviz DOT format."""
     def traverse():
         # breadth-first traversal
-        visited = {root}
-        queue = [root]
+        node_count = 0
+        visited = {root: node_count}
+        queue = deque([root])
         while queue:
-            node = queue.pop(0)
+            node = queue.popleft()
+
+            if not node.edges:
+                yield f'"s{visited[node]}"' + "[shape=doublecircle]"
+
             for succ, variant in node.edges:
-                yield (f'"{node.row}_{node.col}" -> "{succ.row}_{succ.col}"'
-                       f' [label="{to_hgvs(variant, reference)}"];')
                 if succ not in visited:
-                    visited.add(succ)
+                    node_count += 1
+                    visited[succ] = node_count
                     queue.append(succ)
-
-    return "digraph {\n    " + "\n    ".join(traverse()) + "\n}"
+                yield (
+                    f'"s{visited[node]}" -> "s{visited[succ]}"'
+                    f' [label="{variant.to_hgvs(reference)}"];'
+                )
+
+    return (
+        "digraph {\n"
+        "    rankdir=LR\n"
+        "    edge[fontname=monospace]\n"
+        "    node[shape=circle]\n"
+        "    si[shape=point]\n"
+        "    si->" + f'"s{0}"' + "\n"
+        "    " + "\n    ".join(traverse()) + "\n}"
+    )
 
 
 def random_sequence(max_length, min_length=0, alphabet=DNA_NUCLEOTIDES, weights=None):
     """Create a random sequence.
 
     Parameters
     ----------
```

### Comparing `mutalyzer-algebra-1.2.1/algebra/variants/parser.py` & `mutalyzer-algebra-1.3.0/algebra/variants/parser.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/algebra/variants/variant.py` & `mutalyzer-algebra-1.3.0/algebra/variants/variant.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/PKG-INFO` & `mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
-Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs
+Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs,extractor
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
@@ -84,14 +84,26 @@
 lhs = parse_hgvs("2_7AT[4]")  # observed: CATATATATC
 rhs = parse_hgvs("5_6insT")   # observed: CATATTATC
 
 # returns: Relation.CONTAINS
 compare(reference, lhs, rhs)
 ```
 
+Extracting variants from sequences.
+
+```python
+from algebra.extractor import extract, to_hgvs
+
+reference = "CATATATC"
+observed = "CATATATATC"
+
+# returns: 2_7AT[4]
+to_hgvs(list(extract(reference, observed)), reference)
+```
+
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
 
 [Mutalyzer Algebra on PyPI](https://pypi.org/project/mutalyzer-algebra/)
```

### Comparing `mutalyzer-algebra-1.2.1/mutalyzer_algebra.egg-info/SOURCES.txt` & `mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 algebra/__init__.py
 algebra/__main__.py
 algebra/utils.py
+algebra/extractor/__init__.py
+algebra/extractor/extractor.py
+algebra/extractor/vis.py
 algebra/lcs/__init__.py
 algebra/lcs/all_lcs.py
 algebra/lcs/distance_only.py
 algebra/relations/__init__.py
 algebra/relations/relation.py
 algebra/relations/sequence_based.py
 algebra/relations/supremal_based.py
```

### Comparing `mutalyzer-algebra-1.2.1/setup.cfg` & `mutalyzer-algebra-1.3.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = mutalyzer-algebra
-version = 1.2.1
+version = 1.3.0
 description = A Boolean Algebra for Genetic Variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mark A. Santcroos, Jonathan K. Vis
 author_email = m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 url = https://github.com/mutalyzer/algebra
-keywords = algebra, genomics, graph, string, genetics, edit-distance, alignment, compare, sequence, variants, lcs, relations, hgvs
+keywords = algebra, genomics, graph, string, genetics, edit-distance, alignment, compare, sequence, variants, lcs, relations, hgvs, extractor
 license = MIT
 classifiers = 
 	Intended Audience :: Science/Research
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Bio-Informatics
```

