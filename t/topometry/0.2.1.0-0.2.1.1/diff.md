# Comparing `tmp/topometry-0.2.1.0.tar.gz` & `tmp/topometry-0.2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.1.0.tar", last modified: Thu Jul  6 00:21:49 2023, max compression
+gzip compressed data, was "topometry-0.2.1.1.tar", last modified: Thu Jul  6 01:29:28 2023, max compression
```

## Comparing `topometry-0.2.1.0.tar` & `topometry-0.2.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-07-01 15:04:44.000000 topometry-0.2.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4870 2023-07-06 00:21:49.572824 topometry-0.2.1.0/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-07-01 15:04:44.000000 topometry-0.2.1.0/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-07-01 15:04:45.000000 topometry-0.2.1.0/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      736 2023-07-06 00:21:49.572824 topometry-0.2.1.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-07-01 15:04:45.000000 topometry-0.2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45718 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2105 2023-07-05 22:40:24.000000 topometry-0.2.1.0/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     9753 2023-07-05 22:31:43.000000 topometry-0.2.1.0/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36168 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    19431 2023-07-05 23:50:27.000000 topometry-0.2.1.0/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22958 2023-07-01 23:20:56.000000 topometry-0.2.1.0/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    27148 2023-07-05 22:46:48.000000 topometry-0.2.1.0/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76295 2023-07-05 22:48:42.000000 topometry-0.2.1.0/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5110 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       24 2023-07-06 00:16:34.000000 topometry-0.2.1.0/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4870 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.685369 topometry-0.2.1.1/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-07-01 15:04:44.000000 topometry-0.2.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-07-06 01:29:28.685369 topometry-0.2.1.1/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-07-01 15:04:44.000000 topometry-0.2.1.1/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-07-01 15:04:45.000000 topometry-0.2.1.1/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-07-06 01:29:28.685369 topometry-0.2.1.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-07-01 15:04:45.000000 topometry-0.2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2183 2023-07-06 01:14:43.000000 topometry-0.2.1.1/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     9753 2023-07-05 22:31:43.000000 topometry-0.2.1.1/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36168 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19431 2023-07-05 23:50:27.000000 topometry-0.2.1.1/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22958 2023-07-01 23:20:56.000000 topometry-0.2.1.1/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    27148 2023-07-05 22:46:48.000000 topometry-0.2.1.1/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76295 2023-07-05 22:48:42.000000 topometry-0.2.1.1/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.681369 topometry-0.2.1.1/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.685369 topometry-0.2.1.1/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-07-01 15:04:45.000000 topometry-0.2.1.1/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-07-06 01:29:12.000000 topometry-0.2.1.1/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 01:29:28.685369 topometry-0.2.1.1/topometry.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4870 2023-07-06 01:29:28.000000 topometry-0.2.1.1/topometry.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      958 2023-07-06 01:29:28.000000 topometry-0.2.1.1/topometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-06 01:29:28.000000 topometry-0.2.1.1/topometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       60 2023-07-06 01:29:28.000000 topometry-0.2.1.1/topometry.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-07-06 01:29:28.000000 topometry-0.2.1.1/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.1.0/LICENSE` & `topometry-0.2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/PKG-INFO` & `topometry-0.2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.1.0
+Version: 0.2.1.1
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.1.0/README.md` & `topometry-0.2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/setup.cfg` & `topometry-0.2.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.1.0
+version = 0.2.1.1
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.1.0/topo/__init__.py` & `topometry-0.2.1.1/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/base/ann.py` & `topometry-0.2.1.1/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/base/dists.py` & `topometry-0.2.1.1/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/base/sparse.py` & `topometry-0.2.1.1/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/eval/global_scores.py` & `topometry-0.2.1.1/topo/eval/global_scores.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,23 +15,25 @@
     """
     Global score
     Input
     ------
     X: Instance matrix
     Y: Embedding
     """
+    n_dims = Y.shape[1]
     if Y_pca is None:
-        n_dims = Y.shape[1]
         if issparse(X) == True:
             if isinstance(X, np.ndarray):
                 X = csr_matrix(X)
             Y_pca = TruncatedSVD(n_components=n_dims).fit_transform(X)
         else:
             Y_pca = PCA(n_components=n_dims).fit_transform(X)
-
+    else:
+        # select only the first n_dims
+        Y_pca = Y_pca[:, :n_dims]
     gs_pca = global_loss_(X, Y_pca)
     gs_emb = global_loss_(X, Y)
     GSP = np.exp(-(gs_emb - gs_pca) / gs_pca)
     if GSP > 1.0:
         GSP = 1.0
     return GSP
```

### Comparing `topometry-0.2.1.0/topo/eval/local_scores.py` & `topometry-0.2.1.1/topo/eval/local_scores.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/eval/rmetric.py` & `topometry-0.2.1.1/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/layouts/graph_utils.py` & `topometry-0.2.1.1/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/layouts/isomap.py` & `topometry-0.2.1.1/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/layouts/map.py` & `topometry-0.2.1.1/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/layouts/projector.py` & `topometry-0.2.1.1/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/pipes.py` & `topometry-0.2.1.1/topo/pipes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/plot.py` & `topometry-0.2.1.1/topo/plot.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/single_cell.py` & `topometry-0.2.1.1/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/spectral/_spectral.py` & `topometry-0.2.1.1/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/spectral/eigen.py` & `topometry-0.2.1.1/topo/spectral/eigen.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/spectral/locally.py` & `topometry-0.2.1.1/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/spectral/umap_layouts.py` & `topometry-0.2.1.1/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/topograph.py` & `topometry-0.2.1.1/topo/topograph.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/tpgraph/cknn.py` & `topometry-0.2.1.1/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/tpgraph/fuzzy.py` & `topometry-0.2.1.1/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.1.1/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/tpgraph/kernels.py` & `topometry-0.2.1.1/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/tpgraph/procrustes.py` & `topometry-0.2.1.1/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/utils/_utils.py` & `topometry-0.2.1.1/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topo/utils/umap_utils.py` & `topometry-0.2.1.1/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.1.0/topometry.egg-info/PKG-INFO` & `topometry-0.2.1.1/topometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.1.0
+Version: 0.2.1.1
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.1.0/topometry.egg-info/SOURCES.txt` & `topometry-0.2.1.1/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

