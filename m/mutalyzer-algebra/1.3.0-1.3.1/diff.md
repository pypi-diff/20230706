# Comparing `tmp/mutalyzer-algebra-1.3.0.tar.gz` & `tmp/mutalyzer-algebra-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutalyzer-algebra-1.3.0.tar", last modified: Thu Jul  6 12:09:28 2023, max compression
+gzip compressed data, was "mutalyzer-algebra-1.3.1.tar", last modified: Thu Jul  6 20:48:22 2023, max compression
```

## Comparing `mutalyzer-algebra-1.3.0.tar` & `mutalyzer-algebra-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     2835 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     2086 2023-07-06 12:06:33.000000 mutalyzer-algebra-1.3.0/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/
--rw-rw-r--   0 mark      (1000) mark      (1000)      373 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2022-07-28 12:46:24.000000 mutalyzer-algebra-1.3.0/algebra/__main__.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/extractor/
--rw-rw-r--   0 mark      (1000) mark      (1000)      209 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/extractor/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7787 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/extractor/extractor.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      575 2023-01-31 11:04:22.000000 mutalyzer-algebra-1.3.0/algebra/extractor/vis.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/lcs/
--rw-rw-r--   0 mark      (1000) mark      (1000)      237 2022-07-26 07:21:12.000000 mutalyzer-algebra-1.3.0/algebra/lcs/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9329 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/lcs/all_lcs.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/algebra/lcs/distance_only.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/relations/
--rw-rw-r--   0 mark      (1000) mark      (1000)      698 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.0/algebra/relations/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      242 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/relations/relation.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/relations/sequence_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     5466 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/relations/supremal_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1603 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/relations/variant_based.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4193 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/utils.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/algebra/variants/
--rw-rw-r--   0 mark      (1000) mark      (1000)      328 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.0/algebra/variants/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8743 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.0/algebra/variants/parser.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.0/algebra/variants/variant.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2835 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      772 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       51 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/entry_points.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       30 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       14 2023-07-06 12:09:28.000000 mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/top_level.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      895 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)       39 2022-05-10 19:50:59.000000 mutalyzer-algebra-1.3.0/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 12:09:28.692618 mutalyzer-algebra-1.3.0/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.0/tests/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1089 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.1/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2829 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2080 2023-07-06 20:45:22.000000 mutalyzer-algebra-1.3.1/README.md
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.488012 mutalyzer-algebra-1.3.1/algebra/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      373 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.1/algebra/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8607 2022-07-28 12:46:24.000000 mutalyzer-algebra-1.3.1/algebra/__main__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.488012 mutalyzer-algebra-1.3.1/algebra/extractor/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      209 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.1/algebra/extractor/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7771 2023-07-06 20:45:22.000000 mutalyzer-algebra-1.3.1/algebra/extractor/extractor.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      575 2023-01-31 11:04:22.000000 mutalyzer-algebra-1.3.1/algebra/extractor/vis.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.488012 mutalyzer-algebra-1.3.1/algebra/lcs/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      237 2022-07-26 07:21:12.000000 mutalyzer-algebra-1.3.1/algebra/lcs/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     9319 2023-07-06 20:45:22.000000 mutalyzer-algebra-1.3.1/algebra/lcs/all_lcs.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1502 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.1/algebra/lcs/distance_only.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.488012 mutalyzer-algebra-1.3.1/algebra/relations/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      698 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.1/algebra/relations/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      242 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.1/algebra/relations/relation.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3330 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.1/algebra/relations/sequence_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5466 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.1/algebra/relations/supremal_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1603 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.1/algebra/relations/variant_based.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3881 2023-07-06 12:19:45.000000 mutalyzer-algebra-1.3.1/algebra/utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/algebra/variants/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      328 2023-07-06 12:08:33.000000 mutalyzer-algebra-1.3.1/algebra/variants/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8743 2023-07-05 13:59:59.000000 mutalyzer-algebra-1.3.1/algebra/variants/parser.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     8654 2022-08-24 06:47:14.000000 mutalyzer-algebra-1.3.1/algebra/variants/variant.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2829 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      772 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       51 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/entry_points.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       30 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       14 2023-07-06 20:48:22.000000 mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      895 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)       39 2022-05-10 19:50:59.000000 mutalyzer-algebra-1.3.1/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-07-06 20:48:22.492012 mutalyzer-algebra-1.3.1/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2022-05-10 11:52:12.000000 mutalyzer-algebra-1.3.1/tests/__init__.py
```

### Comparing `mutalyzer-algebra-1.3.0/LICENSE` & `mutalyzer-algebra-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/PKG-INFO` & `mutalyzer-algebra-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
 Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs,extractor
 Platform: UNKNOWN
@@ -93,15 +93,15 @@
 ```python
 from algebra.extractor import extract, to_hgvs
 
 reference = "CATATATC"
 observed = "CATATATATC"
 
 # returns: 2_7AT[4]
-to_hgvs(list(extract(reference, observed)), reference)
+to_hgvs(extract(reference, observed), reference)
 ```
 
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
```

### Comparing `mutalyzer-algebra-1.3.0/README.md` & `mutalyzer-algebra-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 ```python
 from algebra.extractor import extract, to_hgvs
 
 reference = "CATATATC"
 observed = "CATATATATC"
 
 # returns: 2_7AT[4]
-to_hgvs(list(extract(reference, observed)), reference)
+to_hgvs(extract(reference, observed), reference)
 ```
 
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
```

### Comparing `mutalyzer-algebra-1.3.0/algebra/__main__.py` & `mutalyzer-algebra-1.3.1/algebra/__main__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/extractor/extractor.py` & `mutalyzer-algebra-1.3.1/algebra/extractor/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
             n_a, e_a, _ = visited[n_a]
 
     queue = deque([(root, None, None, 0)])
 
     visited = {}
 
     while queue:
-
         node, parent, edge, distance = queue.popleft()
 
         if not node.edges:
             sink = node
 
         if node in visited:
             other_parent, other_edge, other_distance = visited[node]
@@ -65,41 +64,39 @@
             start = min(edge_a.start, edge_b.start)
             start_offset = start - lca.row
 
             if other_parent != parent and parent.row == other_parent.row and parent.col == other_parent.col:
                 end = max(parent.row - 1, visited[parent][1].end, visited[other_parent][1].end)
                 end_offset = end - parent.row
 
-                delins = Variant(start, end, observed[lca.col + start_offset : parent.col + end_offset])
+                delins = Variant(start, end, observed[lca.col + start_offset:parent.col + end_offset])
 
                 visited[other_parent] = (lca, delins, distance - 1)
                 # does not seem to be required to: visited[parent] = (lca, delins, distance - 1)
-
             else:
                 end = max(node.row - 1, edge.end, other_edge.end)
                 end_offset = end - node.row
 
-                delins = Variant(start, end, observed[lca.col + start_offset : node.col + end_offset])
+                delins = Variant(start, end, observed[lca.col + start_offset:node.col + end_offset])
 
                 visited[node] = (lca, delins, distance)
 
-
         else:
             visited[node] = (parent, edge, distance)
 
             for succ_node, succ_edge in node.edges:
                 queue.append((succ_node, node, succ_edge, distance + 1))
 
     variants = []
     while sink:
         sink, variant, _ = visited[sink]
         if variant:
-            variants.append(variant)
+            variants.insert(0, variant)
 
-    return reversed(variants)
+    return variants
 
 
 def extract(reference, observed):
     """Extract the canonical variant representation (allele) for a
     reference and observed sequence."""
     _, lcs_nodes = edit(reference, observed)
     root, _ = lcs_graph(reference, observed, lcs_nodes)
@@ -182,15 +179,15 @@
             return f"{to_hgvs_position(variant.start, variant.end - deleted_remainder)}{inserted_unit}[{inserted_number}]"
 
         # Prefix and suffix trimming
         start, end = trim(deleted, variant.sequence)
         trimmed = Variant(variant.start + start, variant.end - end, variant.sequence[start:len(variant.sequence) - end])
 
         # Inversion
-        if len(trimmed.sequence) > 1 and trimmed.sequence == reverse_complement(reference[trimmed.start : trimmed.end]):
+        if len(trimmed.sequence) > 1 and trimmed.sequence == reverse_complement(reference[trimmed.start:trimmed.end]):
             return f"{to_hgvs_position(trimmed.start, trimmed.end)}inv"
 
         # Deletion/insertion with repeated insertion
         inserted_unit, inserted_number, inserted_remainder = repeats(trimmed.sequence)
         if inserted_number > 1:
             suffix = f"{inserted_unit}[{inserted_number}]"
             if inserted_remainder:
```

### Comparing `mutalyzer-algebra-1.3.0/algebra/extractor/vis.py` & `mutalyzer-algebra-1.3.1/algebra/extractor/vis.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/lcs/all_lcs.py` & `mutalyzer-algebra-1.3.1/algebra/lcs/all_lcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,22 +154,21 @@
     See Also
     --------
     `edit` : Calculates the LCS nodes.
     `traversal` : Traverses the LS graph.
     `algebra.utils.to_dot` : Graphviz DOT format.
     """
 
-
     edges = []
 
     if not lcs_nodes or lcs_nodes == [[]]:
-        source = _Node(0, 0, 0)
+        source = _Node(0, 0)
         if not reference and not observed:
             return source, edges
-        sink = _Node(len(reference) + 1, len(observed) + 1, 0)
+        sink = _Node(len(reference) + 1, len(observed) + 1)
         variant = Variant(0, len(reference), observed)
         edges.append(variant)
         source.edges = [(sink, variant)]
         return source, edges
 
     if lcs_nodes[-1][-1].row + lcs_nodes[-1][-1].length == len(reference) + 1 and lcs_nodes[-1][-1].col + lcs_nodes[-1][-1].length == len(observed) + 1:
         sink = lcs_nodes[-1][-1]
@@ -187,30 +186,28 @@
                 variant = Variant(pred.row + pred.length - 1, sink.row + sink.length - 2, observed[pred.col + pred.length - 1:sink.col + sink.length - 2])
                 pred.edges.append((sink, variant))
                 edges.append(variant)
 
     lcs_pos = len(lcs_nodes) - 1
 
     while lcs_pos > 0:
-
         nodes = lcs_nodes[lcs_pos]
 
-        idx_split = [False for e in lcs_nodes[lcs_pos - 1]]
+        idx_split = [False for _ in lcs_nodes[lcs_pos - 1]]
 
         while nodes:
             node = nodes.pop(0)
 
             if not node.edges and node != sink:
                 continue
 
             idx_pred = -1
             edge_added = False
 
             for i, pred in enumerate(lcs_nodes[lcs_pos - 1]):
-
                 if pred.row + pred.length - 1 < node.row + node.length - 1 and pred.col + pred.length - 1 < node.col + node.length - 1:
                     variant = Variant(pred.row + pred.length - 1, node.row + node.length - 2, observed[pred.col + pred.length - 1:node.col + node.length - 2])
                     edges.append(variant)
 
                     if pred.incoming == lcs_pos:
                         idx_split[i] = False
                         upper_node = _Node(pred.row, pred.col, pred.length)
@@ -246,15 +243,14 @@
             variant = Variant(source.row + source.length - 1, succ.row + succ.length - 2, observed[source.col + source.length - 1:succ.col + succ.length - 2])
             source.edges.append((succ, variant))
             edges.append(variant)
 
     return source, edges
 
 
-
 def traversal(root, atomics=False):
     """Traverse the LCS graph.
 
     Parameters
     ----------
     atomics : bool, optional
         If set to `True` the variants are represented using separate
```

### Comparing `mutalyzer-algebra-1.3.0/algebra/lcs/distance_only.py` & `mutalyzer-algebra-1.3.1/algebra/lcs/distance_only.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/relations/__init__.py` & `mutalyzer-algebra-1.3.1/algebra/relations/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/relations/sequence_based.py` & `mutalyzer-algebra-1.3.1/algebra/relations/sequence_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/relations/supremal_based.py` & `mutalyzer-algebra-1.3.1/algebra/relations/supremal_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/relations/variant_based.py` & `mutalyzer-algebra-1.3.1/algebra/relations/variant_based.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/utils.py` & `mutalyzer-algebra-1.3.1/algebra/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 """Utility functions for sequences and variants."""
 
 
 from collections import deque
-from itertools import chain
 import random
 from . import Variant
-from .variants import DNA_NUCLEOTIDES, to_hgvs
-
-
-def canonical(variants, max_distance=40):
-    """Pick a canonical representation from all minimal variant
-    representations."""
-    first = next(variants)
-    if sum(map(len, first)) > max_distance:
-        return first
-
-    return min(chain([first], variants), key=len)
+from .variants import DNA_NUCLEOTIDES
 
 
 def fasta_sequence(lines):
     """Create a single sequence from (FASTA) lines."""
     return "".join([line.strip() if not line.startswith(">") else "" for line in lines])
```

### Comparing `mutalyzer-algebra-1.3.0/algebra/variants/parser.py` & `mutalyzer-algebra-1.3.1/algebra/variants/parser.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/algebra/variants/variant.py` & `mutalyzer-algebra-1.3.1/algebra/variants/variant.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/PKG-INFO` & `mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer-algebra
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Boolean Algebra for Genetic Variants
 Home-page: https://github.com/mutalyzer/algebra
 Author: Mark A. Santcroos, Jonathan K. Vis
 Author-email: m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 License: MIT
 Keywords: algebra,genomics,graph,string,genetics,edit-distance,alignment,compare,sequence,variants,lcs,relations,hgvs,extractor
 Platform: UNKNOWN
@@ -93,15 +93,15 @@
 ```python
 from algebra.extractor import extract, to_hgvs
 
 reference = "CATATATC"
 observed = "CATATATATC"
 
 # returns: 2_7AT[4]
-to_hgvs(list(extract(reference, observed)), reference)
+to_hgvs(extract(reference, observed), reference)
 ```
 
 See Also
 --------
 
 A web interface with integration with [Mutalyzer](https://github.com/mutalyzer): [Mutalyzer Algebra](https://mutalyzer.nl/algebra)
```

### Comparing `mutalyzer-algebra-1.3.0/mutalyzer_algebra.egg-info/SOURCES.txt` & `mutalyzer-algebra-1.3.1/mutalyzer_algebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutalyzer-algebra-1.3.0/setup.cfg` & `mutalyzer-algebra-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer-algebra
-version = 1.3.0
+version = 1.3.1
 description = A Boolean Algebra for Genetic Variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mark A. Santcroos, Jonathan K. Vis
 author_email = m.a.santcroos@lumc.nl, j.k.vis@lumc.nl
 url = https://github.com/mutalyzer/algebra
 keywords = algebra, genomics, graph, string, genetics, edit-distance, alignment, compare, sequence, variants, lcs, relations, hgvs, extractor
```

