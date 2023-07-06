# Comparing `tmp/pmotif_lib-1.0.0.tar.gz` & `tmp/pmotif_lib-1.0.1.tar.gz`

## Comparing `pmotif_lib-1.0.0.tar` & `pmotif_lib-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/requirements.txt
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/config.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/graphlet_occurence.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/graphlet_representation.py
--rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_motif_graph.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/randomization.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/result_transformer.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/__init__.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/graph_io.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/parsing.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/__init__.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/metric_consolidation.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/metric_processing.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/p_anchor_node_distance.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/p_degree.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/p_graph_module_participation.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/p_metric.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pmotif_lib/p_metric/p_metric_result.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/.showcase_env
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/graphlet_detection.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/motif_detection.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/pgraphlet_detection.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/pmotif_detection.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/showcase/artifacts/karate_club.edgelist
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/LICENSE
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/README.md
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pmotif_lib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/config.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/graphlet_occurence.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/graphlet_representation.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_motif_graph.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/randomization.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/result_transformer.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/__init__.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/graph_io.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/parsing.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/__init__.py
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_consolidation.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_processing.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_anchor_node_distance.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_degree.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_graph_module_participation.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric_result.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/.showcase_env
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/graphlet_detection.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/motif_detection.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/pgraphlet_detection.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/pmotif_detection.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/showcase/artifacts/karate_club.edgelist
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 pmotif_lib-1.0.1/PKG-INFO
```

### Comparing `pmotif_lib-1.0.0/pmotif_lib/graphlet_occurence.py` & `pmotif_lib-1.0.1/pmotif_lib/graphlet_occurence.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/graphlet_representation.py` & `pmotif_lib-1.0.1/pmotif_lib/graphlet_representation.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_motif_graph.py` & `pmotif_lib-1.0.1/pmotif_lib/p_motif_graph.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/randomization.py` & `pmotif_lib-1.0.1/pmotif_lib/randomization.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/result_transformer.py` & `pmotif_lib-1.0.1/pmotif_lib/result_transformer.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/graph_io.py` & `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/graph_io.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/parsing.py` & `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/parsing.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/gtrieScanner/wrapper.py` & `pmotif_lib-1.0.1/pmotif_lib/gtrieScanner/wrapper.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/metric_consolidation.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_consolidation.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,31 +17,46 @@
 
 
 def max_normalized_anchor_hop_distances(
     raw_metric: RawMetric, pre_compute: PreComputation
 ) -> float:
     """Consolidate PAnchorNodeDistance. Normalize the distances by closeness centrality
     and return the highest distance."""
-    return max(_get_normalized_anchor_hop_distances(raw_metric, pre_compute))
+    distances = _get_normalized_anchor_hop_distances(raw_metric, pre_compute)
+    if len(distances) == 0:
+        return -1
+    if len(distances) == 1:
+        return distances[0]
+    return max(distances)
 
 
 def min_normalized_anchor_hop_distances(
     raw_metric: RawMetric, pre_compute: PreComputation
 ) -> float:
     """Consolidate PAnchorNodeDistance. Normalize the distances by closeness centrality
     and return the lowest distance."""
-    return min(_get_normalized_anchor_hop_distances(raw_metric, pre_compute))
+    distances = _get_normalized_anchor_hop_distances(raw_metric, pre_compute)
+    if len(distances) == 0:
+        return -1
+    if len(distances) == 1:
+        return distances[0]
+    return min(distances)
 
 
 def mean_normalized_anchor_hop_distances(
     raw_metric: RawMetric, pre_compute: PreComputation
 ) -> float:
     """Consolidate PAnchorNodeDistance. Normalize the distances by closeness centrality
     and return the mean distance."""
-    return mean(_get_normalized_anchor_hop_distances(raw_metric, pre_compute))
+    distances = _get_normalized_anchor_hop_distances(raw_metric, pre_compute)
+    if len(distances) == 0:
+        return -1
+    if len(distances) == 1:
+        return distances[0]
+    return mean(distances)
 
 
 def _get_normalized_anchor_hop_distances(
     raw_metric: RawMetric, pre_compute: PreComputation
 ) -> List[float]:
     """Normalize the distances by closeness centrality of the anchor nodes.
     Some nodes are more central than others, making such normalization necessary to make
```

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/metric_processing.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/metric_processing.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/p_anchor_node_distance.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_anchor_node_distance.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/p_degree.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_degree.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/p_graph_module_participation.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_graph_module_participation.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/p_metric.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pmotif_lib/p_metric/p_metric_result.py` & `pmotif_lib-1.0.1/pmotif_lib/p_metric/p_metric_result.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/showcase/graphlet_detection.py` & `pmotif_lib-1.0.1/showcase/graphlet_detection.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/showcase/motif_detection.py` & `pmotif_lib-1.0.1/showcase/motif_detection.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/showcase/pgraphlet_detection.py` & `pmotif_lib-1.0.1/showcase/pgraphlet_detection.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/showcase/pmotif_detection.py` & `pmotif_lib-1.0.1/showcase/pmotif_detection.py`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/showcase/artifacts/karate_club.edgelist` & `pmotif_lib-1.0.1/showcase/artifacts/karate_club.edgelist`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/LICENSE` & `pmotif_lib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/README.md` & `pmotif_lib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pmotif_lib-1.0.0/pyproject.toml` & `pmotif_lib-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pmotif_lib"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Tim Garrels", email="tim.garrels@protonmail.com" },
 ]
 description = "Perform motif detection, either with traditional frequency, or with positional metrics for each graphlet occurrence."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pmotif_lib-1.0.0/PKG-INFO` & `pmotif_lib-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmotif_lib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Perform motif detection, either with traditional frequency, or with positional metrics for each graphlet occurrence.
 Project-URL: Homepage, https://github.com/timgarrels/pmotif_lib
 Project-URL: documentation, https://github.com/timgarrels/pmotif_lib/wiki
 Project-URL: Bug Tracker, https://github.com/timgarrels/pmotif_lib/issues
 Project-URL: Repository, https://github.com/timgarrels/pmotif_lib
 Author-email: Tim Garrels <tim.garrels@protonmail.com>
 License-File: LICENSE
```

