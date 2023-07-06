# Comparing `tmp/topometry-0.2.0.9.1.tar.gz` & `tmp/topometry-0.2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topometry-0.2.0.9.1.tar", last modified: Fri Jun 16 00:34:54 2023, max compression
+gzip compressed data, was "topometry-0.2.1.0.tar", last modified: Thu Jul  6 00:21:49 2023, max compression
```

## Comparing `topometry-0.2.0.9.1.tar` & `topometry-0.2.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/
--rwxrwxr-x   0 root         (0) root         (0)     1101 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     4250 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/README.md
--rwxrwxr-x   0 root         (0) root         (0)      104 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/pyproject.toml
--rwxrwxr-x   0 root         (0) root         (0)      738 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       91 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.119910 topometry-0.2.0.9.1/topo/
--rwxrwxr-x   0 root         (0) root         (0)      897 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/base/
--rwxrwxr-x   0 root         (0) root         (0)      179 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/base/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    47503 2023-06-14 23:37:47.000000 topometry-0.2.0.9.1/topo/base/ann.py
--rwxrwxr-x   0 root         (0) root         (0)    45718 2023-06-14 22:51:02.000000 topometry-0.2.0.9.1/topo/base/dists.py
--rwxrwxr-x   0 root         (0) root         (0)    16721 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/base/sparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/eval/
--rwxrwxr-x   0 root         (0) root         (0)      219 2023-06-14 21:27:15.000000 topometry-0.2.0.9.1/topo/eval/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2309 2023-06-16 00:25:03.000000 topometry-0.2.0.9.1/topo/eval/global_scores.py
--rwxrwxr-x   0 root         (0) root         (0)    12721 2023-06-15 11:44:37.000000 topometry-0.2.0.9.1/topo/eval/local_scores.py
--rwxrwxr-x   0 root         (0) root         (0)     6058 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/eval/rmetric.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/layouts/
--rwxrwxr-x   0 root         (0) root         (0)      120 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/layouts/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    13879 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/layouts/graph_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     3366 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/layouts/isomap.py
--rwxrwxr-x   0 root         (0) root         (0)     9251 2023-06-14 21:31:28.000000 topometry-0.2.0.9.1/topo/layouts/map.py
--rwxrwxr-x   0 root         (0) root         (0)    36168 2023-06-16 00:13:54.000000 topometry-0.2.0.9.1/topo/layouts/projector.py
--rwxrwxr-x   0 root         (0) root         (0)    20101 2023-06-16 00:34:12.000000 topometry-0.2.0.9.1/topo/pipes.py
--rwxrwxr-x   0 root         (0) root         (0)    22966 2023-06-14 22:04:50.000000 topometry-0.2.0.9.1/topo/plot.py
--rwxrwxr-x   0 root         (0) root         (0)    21289 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/single_cell.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/spectral/
--rwxrwxr-x   0 root         (0) root         (0)      265 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/spectral/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    23612 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/spectral/_spectral.py
--rwxrwxr-x   0 root         (0) root         (0)    26918 2023-06-14 21:28:18.000000 topometry-0.2.0.9.1/topo/spectral/eigen.py
--rw-rw-r--   0 root         (0) root         (0)      855 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/spectral/locally.py
--rwxrwxr-x   0 root         (0) root         (0)    30671 2023-06-14 23:34:47.000000 topometry-0.2.0.9.1/topo/spectral/umap_layouts.py
--rwxrwxr-x   0 root         (0) root         (0)    76137 2023-06-16 00:12:47.000000 topometry-0.2.0.9.1/topo/topograph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/tpgraph/
--rwxrwxr-x   0 root         (0) root         (0)      225 2023-06-14 21:28:40.000000 topometry-0.2.0.9.1/topo/tpgraph/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5110 2023-06-14 23:33:52.000000 topometry-0.2.0.9.1/topo/tpgraph/cknn.py
--rwxrwxr-x   0 root         (0) root         (0)    15089 2023-06-14 23:36:03.000000 topometry-0.2.0.9.1/topo/tpgraph/fuzzy.py
--rw-rw-r--   0 root         (0) root         (0)    14221 2023-06-14 21:29:14.000000 topometry-0.2.0.9.1/topo/tpgraph/intrinsic_dim.py
--rwxrwxr-x   0 root         (0) root         (0)    48044 2023-06-14 21:21:07.000000 topometry-0.2.0.9.1/topo/tpgraph/kernels.py
--rwxrwxr-x   0 root         (0) root         (0)    32597 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/tpgraph/procrustes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topo/utils/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/utils/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     5710 2023-06-14 21:31:28.000000 topometry-0.2.0.9.1/topo/utils/_utils.py
--rwxrwxr-x   0 root         (0) root         (0)     8583 2023-06-14 21:18:44.000000 topometry-0.2.0.9.1/topo/utils/umap_utils.py
--rwxrwxr-x   0 root         (0) root         (0)       26 2023-06-16 00:34:28.000000 topometry-0.2.0.9.1/topo/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 00:34:54.123910 topometry-0.2.0.9.1/topometry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-16 00:34:54.000000 topometry-0.2.0.9.1/topometry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-16 00:34:54.000000 topometry-0.2.0.9.1/topometry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 00:34:54.000000 topometry-0.2.0.9.1/topometry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-16 00:34:54.000000 topometry-0.2.0.9.1/topometry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-16 00:34:54.000000 topometry-0.2.0.9.1/topometry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/
+-rwxrwxr-x   0 root         (0) root         (0)     1101 2023-07-01 15:04:44.000000 topometry-0.2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-07-06 00:21:49.572824 topometry-0.2.1.0/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     4250 2023-07-01 15:04:44.000000 topometry-0.2.1.0/README.md
+-rwxrwxr-x   0 root         (0) root         (0)      104 2023-07-01 15:04:45.000000 topometry-0.2.1.0/pyproject.toml
+-rwxrwxr-x   0 root         (0) root         (0)      736 2023-07-06 00:21:49.572824 topometry-0.2.1.0/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)       91 2023-07-01 15:04:45.000000 topometry-0.2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/
+-rwxrwxr-x   0 root         (0) root         (0)      897 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/base/
+-rwxrwxr-x   0 root         (0) root         (0)      179 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    47503 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/ann.py
+-rwxrwxr-x   0 root         (0) root         (0)    45718 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/dists.py
+-rwxrwxr-x   0 root         (0) root         (0)    16721 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/base/sparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/eval/
+-rwxrwxr-x   0 root         (0) root         (0)      219 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/eval/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2105 2023-07-05 22:40:24.000000 topometry-0.2.1.0/topo/eval/global_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     9753 2023-07-05 22:31:43.000000 topometry-0.2.1.0/topo/eval/local_scores.py
+-rwxrwxr-x   0 root         (0) root         (0)     6058 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/eval/rmetric.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/layouts/
+-rwxrwxr-x   0 root         (0) root         (0)      120 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    13879 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/graph_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     3366 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/isomap.py
+-rwxrwxr-x   0 root         (0) root         (0)     9251 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/map.py
+-rwxrwxr-x   0 root         (0) root         (0)    36168 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/layouts/projector.py
+-rwxrwxr-x   0 root         (0) root         (0)    19431 2023-07-05 23:50:27.000000 topometry-0.2.1.0/topo/pipes.py
+-rwxrwxr-x   0 root         (0) root         (0)    22958 2023-07-01 23:20:56.000000 topometry-0.2.1.0/topo/plot.py
+-rwxrwxr-x   0 root         (0) root         (0)    21289 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/single_cell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.568824 topometry-0.2.1.0/topo/spectral/
+-rwxrwxr-x   0 root         (0) root         (0)      265 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)    23612 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/_spectral.py
+-rwxrwxr-x   0 root         (0) root         (0)    27148 2023-07-05 22:46:48.000000 topometry-0.2.1.0/topo/spectral/eigen.py
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/locally.py
+-rwxrwxr-x   0 root         (0) root         (0)    30671 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/spectral/umap_layouts.py
+-rwxrwxr-x   0 root         (0) root         (0)    76295 2023-07-05 22:48:42.000000 topometry-0.2.1.0/topo/topograph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topo/tpgraph/
+-rwxrwxr-x   0 root         (0) root         (0)      225 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5110 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/cknn.py
+-rwxrwxr-x   0 root         (0) root         (0)    15089 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/fuzzy.py
+-rw-rw-r--   0 root         (0) root         (0)    14221 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/intrinsic_dim.py
+-rwxrwxr-x   0 root         (0) root         (0)    48044 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/kernels.py
+-rwxrwxr-x   0 root         (0) root         (0)    32597 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/tpgraph/procrustes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topo/utils/
+-rwxrwxr-x   0 root         (0) root         (0)       22 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     5710 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     8583 2023-07-01 15:04:45.000000 topometry-0.2.1.0/topo/utils/umap_utils.py
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-07-06 00:16:34.000000 topometry-0.2.1.0/topo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 00:21:49.572824 topometry-0.2.1.0/topometry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4870 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      958 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-06 00:21:49.000000 topometry-0.2.1.0/topometry.egg-info/top_level.txt
```

### Comparing `topometry-0.2.0.9.1/LICENSE` & `topometry-0.2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/PKG-INFO` & `topometry-0.2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.9.1
+Version: 0.2.1.0
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.9.1/README.md` & `topometry-0.2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/setup.cfg` & `topometry-0.2.1.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = topometry
-version = 0.2.0.9.1
+version = 0.2.1.0
 author = Davi Sidarta-Oliveira
 author_email = davi.oliveira@dpag.ox.ac.uk
 description = A comprehensive dimensional reduction framework to recover latent information from data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/davisidarta/topometry
 project_urls =
```

### Comparing `topometry-0.2.0.9.1/topo/__init__.py` & `topometry-0.2.1.0/topo/__init__.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/base/ann.py` & `topometry-0.2.1.0/topo/base/ann.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/base/dists.py` & `topometry-0.2.1.0/topo/base/dists.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/base/sparse.py` & `topometry-0.2.1.0/topo/base/sparse.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/eval/global_scores.py` & `topometry-0.2.1.0/topo/eval/global_scores.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,37 +7,31 @@
     X = X - np.mean(X, axis=0)
     Y = Y - np.mean(Y, axis=0)
     A = X.T @ (Y @ np.linalg.inv(Y.T @ Y))
     GL = np.mean(np.power(X.T - A @ Y.T, 2))
     return GL
 
 
-def global_score_pca(X, Y, X_is_pca=False):
+def global_score_pca(X, Y, Y_pca=None):
     """
     Global score
     Input
     ------
     X: Instance matrix
     Y: Embedding
     """
-    if X_is_pca:
-        Y_pca = X
-    else:
+    if Y_pca is None:
+        n_dims = Y.shape[1]
         if issparse(X) == True:
             if isinstance(X, np.ndarray):
                 X = csr_matrix(X)
-        if issparse(X) == False:
-            if isinstance(X, np.ndarray):
-                X = csr_matrix(X)
-            else:
-                import pandas as pd
-                if isinstance(X, pd.DataFrame):
-                    X = csr_matrix(X.values.T)
-        n_dims = Y.shape[1]
-        Y_pca = TruncatedSVD(n_components=n_dims).fit_transform(X)
+            Y_pca = TruncatedSVD(n_components=n_dims).fit_transform(X)
+        else:
+            Y_pca = PCA(n_components=n_dims).fit_transform(X)
+
     gs_pca = global_loss_(X, Y_pca)
     gs_emb = global_loss_(X, Y)
     GSP = np.exp(-(gs_emb - gs_pca) / gs_pca)
     if GSP > 1.0:
         GSP = 1.0
     return GSP
```

### Comparing `topometry-0.2.0.9.1/topo/eval/local_scores.py` & `topometry-0.2.1.0/topo/eval/local_scores.py`

 * *Files 16% similar despite different names*

```diff
@@ -231,79 +231,7 @@
         if verbose:
             print('Computing Kendall Tau for eigenbasis...')
         results = kendalltau(
             base_geodesics, embedding_geodesics).correlation
     if return_graphs:
         return results, data_graph, emb_graph
     return results
-
-def trustworthiness(X, X_embedded, n_neighbors=3, metric='euclidean', X_is_distance=False, n_jobs=-1, backend='hnswlib', **kwargs):
-    """
-    Expresses to what extent the local structure is retained.
-    Adapted from scikit-learn for increased computational efficiency.
-
-
-    Parameters
-    ----------
-    X : ndarray of shape (n_samples, n_features) or (n_samples, n_samples)
-        If the metric is 'precomputed' X must be a square distance
-        matrix. Otherwise it contains a sample per row.
-
-    X_embedded : ndarray of shape (n_samples, n_components)
-        Embedding of the training data in low-dimensional space.
-
-    n_neighbors : int, default=5
-        Number of neighbors k that will be considered.
-
-    X_is_distance : bool, default=False
-        Whether X is a distance matrix. If metric is 'precomputed', X may be a
-        distance matrix, in which case X_is_distance must be True.
-
-    metric : str or callable, default='euclidean'
-        Which metric to use for computing pairwise distances between samples
-        from the original input space. 
-
-
-        
-    Returns
-    -------
-    trustworthiness : float
-        Trustworthiness of the low-dimensional embedding.
-    """
-
-    dist_X = pairwise_distances(X, metric=metric, n_jobs=n_jobs)
-    if X_is_distance:
-        dist_X = dist_X.copy()
-    # we set the diagonal to np.inf to exclude the points themselves from
-    # their own neighborhood
-    np.fill_diagonal(dist_X, np.inf)
-    ind_X = np.argsort(dist_X, axis=1)
-    # `ind_X[i]` is the index of sorted distances between i and other samples
-    
-    if backend == 'sklearn':
-        ind_X_embedded = NearestNeighbors(metric=metric, n_neighbors=n_neighbors, n_jobs=n_jobs).fit(
-                X_embedded).kneighbors(return_distance=False)
-
-    if backend == 'hnswlib':
-        from topo.base.ann import HNSWlibTransformer
-        nbrs_transformer = HNSWlibTransformer(metric=metric,
-                                               n_neighbors=n_neighbors,
-                                                 n_jobs=n_jobs, **kwargs).fit(X_embedded)
-        ind_X_embedded, _ = nbrs_transformer.p.knn_query(X_embedded, k=n_neighbors+1)
-        ind_X_embedded = ind_X_embedded[:, 1:]
-
-    # We build an inverted index of neighbors in the input space: For sample i,
-    # we define `inverted_index[i]` as the inverted index of sorted distances:
-    # inverted_index[i][ind_X[i]] = np.arange(1, n_sample + 1)
-    n_samples = X.shape[0]
-    inverted_index = np.zeros((n_samples, n_samples), dtype=int)
-    ordered_indices = np.arange(n_samples + 1)
-    inverted_index[ordered_indices[:-1, np.newaxis],
-                   ind_X] = ordered_indices[1:]
-    ranks = inverted_index[ordered_indices[:-1, np.newaxis],
-                           ind_X_embedded] - n_neighbors
-    t = np.sum(ranks[ranks > 0])
-    t = 1.0 - t * (2.0 / (n_samples * n_neighbors *
-                          (2.0 * n_samples - 3.0 * n_neighbors - 1.0)))
-    return t
-
-
```

### Comparing `topometry-0.2.0.9.1/topo/eval/rmetric.py` & `topometry-0.2.1.0/topo/eval/rmetric.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/layouts/graph_utils.py` & `topometry-0.2.1.0/topo/layouts/graph_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/layouts/isomap.py` & `topometry-0.2.1.0/topo/layouts/isomap.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/layouts/map.py` & `topometry-0.2.1.0/topo/layouts/map.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/layouts/projector.py` & `topometry-0.2.1.0/topo/layouts/projector.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/pipes.py` & `topometry-0.2.1.0/topo/pipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import numpy as np
 from scipy.sparse import issparse, csr_matrix
-from scipy.stats import spearmanr, kendalltau
+from scipy.stats import spearmanr
 from scipy.spatial.distance import squareform
+from sklearn.metrics import pairwise_distances
+from sklearn.manifold import trustworthiness
 from topo.utils._utils import get_landmark_indices
 from topo.base.ann import kNN
 from topo.topograph import TopOGraph
 from topo.eval.global_scores import global_score_pca
-from topo.eval.local_scores import geodesic_distance, geodesic_correlation, trustworthiness
+from topo.eval.local_scores import geodesic_distance, geodesic_correlation
 
 
 
-def global_score(data, emb, X_is_pca=False):
-    global_scores_pca = global_score_pca(data, emb, X_is_pca=X_is_pca)
+def global_score(data, emb, Y_pca=False):
+    global_scores_pca = global_score_pca(data, emb, Y_pca=Y_pca)
     return global_scores_pca
 
 def eval_models_layouts(TopOGraph, X,
                         methods=['tw', 'gc', 'gs'],
                         kernels=['cknn', 'bw_adaptive'],
                         eigenmap_methods=['DM', 'LE'],
                         projections=['MAP'],
                         additional_eigenbases=None,
                         additional_projections=None,
                         n_neighbors=5, n_jobs=-1,
                         landmark_method='kmeans',
                         metric='euclidean',
                         n_pcs=30,
-                        cor_method='spearman',
                         landmarks=None,
+                        run_uncomputed_models=True,
                           **kwargs):
     """
     Evaluates all orthogonal bases, topological graphs and layouts in the TopOGraph object.
     
     Currently uses three different quality metrics: trustworthiness (https://scikit-learn.org/stable/modules/generated/sklearn.manifold.trustworthiness.html),
     geodesic correlation (defined in the TopOMetry manuscript as the Spearman R correlation between high- and low-dimensional geodesic distances),
     and global score (defined in the TriMAP paper as the MRE normalized by PCA's MRE).
@@ -109,15 +111,16 @@
 
     """
 
     import gc
     # Run models
     if TopOGraph.verbosity > 0:
         print('Running specified models...')
-    TopOGraph.run_models(X, kernels, eigenmap_methods, projections)
+    if run_uncomputed_models:
+        TopOGraph.run_models(X, kernels, eigenmap_methods, projections)
     # Define landmarks if applicable
     if landmarks is not None:
         if landmark_method == 'random':
             if isinstance(landmarks, int):
                 landmark_indices = get_landmark_indices(
                     TopOGraph.base_knn_graph, n_landmarks=landmarks, method=landmark_method, random_state=TopOGraph.random_state)
                 if landmark_indices.shape[0] == TopOGraph.base_knn_graph.shape[0]:
@@ -175,21 +178,19 @@
     EigenbasisGCResults = {}
     EigenbasisGSResults = {}
 
     if TopOGraph.verbosity > 0:
         print('Assessing base graph...')
     if 'gc' in methods:
         base_geodesics = squareform(geodesic_distance(base_graph, directed=False, n_jobs=n_jobs))
-        #base_geodesics = squareform(geodesic_distance(base_graph, directed=False, n_jobs=n_jobs))
     if 'tw' in methods:
-        from sklearn.metrics import pairwise_distances
         if isinstance(X, csr_matrix):
-            data_pdist = pairwise_distances(X.toarray(), metric=metric, n_jobs=n_jobs)
+            data_pdist = pairwise_distances(X.toarray(), metric=TopOGraph.base_metric, n_jobs=n_jobs)
         else:
-            data_pdist = pairwise_distances(X, metric=metric, n_jobs=n_jobs)
+            data_pdist = pairwise_distances(X, metric=TopOGraph.base_metric, n_jobs=n_jobs)
     gc.collect()
     for key in TopOGraph.EigenbasisDict.keys():
         if 'gc' in methods:
             if TopOGraph.verbosity > 0:
                 print('Computing geodesics for eigenbasis \'{}...\''.format(key))
             emb_graph = kNN(TopOGraph.EigenbasisDict[key].results(), n_neighbors=n_neighbors,
                             metric=metric,
@@ -206,22 +207,21 @@
             if TopOGraph.verbosity > 0:
                 print('Computing geodesic correlation for eigenbasis \'{}...\''.format(key))
             EigenbasisGCResults[key], _ = spearmanr(
                 base_geodesics, embedding_geodesics)
             gc.collect()
         if 'gs' in methods:
             EigenbasisGSResults[key] = global_score(
-                pca_emb, TopOGraph.EigenbasisDict[key].results(), X_is_pca=True)
+                X, TopOGraph.EigenbasisDict[key].results(), Y_pca=pca_emb)
             if TopOGraph.verbosity > 0:
                 print('Computed global score for eigenbasis {}'.format(key))
             gc.collect()
         if 'tw' in methods:
             EigenbasisTWResults[key] = trustworthiness(data_pdist,
-                                                        TopOGraph.EigenbasisDict[key].results(), n_neighbors=n_neighbors,
-                                                        n_jobs=n_jobs, X_is_distance=True, metric=metric)
+                                                        TopOGraph.EigenbasisDict[key].results(), metric='precomputed')
             if TopOGraph.verbosity > 0:
                 print('Computed trustworthiness for projection {}'.format(key))
             gc.collect()
 
     ProjectionTWResults = {}
     ProjectionGCResults = {}
     ProjectionGSResults = {}
@@ -246,22 +246,21 @@
             if TopOGraph.verbosity > 0:
                 print('Computing Sgeodesic correlation for projection \'{}...\''.format(key))
             ProjectionGCResults[key], _ = spearmanr(
                 base_geodesics, embedding_geodesics)
             gc.collect()
         if 'gs' in methods:
             ProjectionGSResults[key] = global_score(
-                pca_emb, TopOGraph.ProjectionDict[key], X_is_pca=True)
+                X, TopOGraph.ProjectionDict[key], Y_pca=pca_emb)
             if TopOGraph.verbosity > 0:
                 print('Computed global score for projection {}'.format(key))
             gc.collect()
         if 'tw' in methods:
             ProjectionTWResults[key] = trustworthiness(data_pdist,
-                                                        TopOGraph.ProjectionDict[key], n_neighbors=n_neighbors, 
-                                                        n_jobs=n_jobs, X_is_distance=True, metric=metric)
+                                                        TopOGraph.ProjectionDict[key], metric='precomputed')
             if TopOGraph.verbosity > 0:
                 print('Computed trustworthiness for projection {}'.format(key))
             gc.collect()
 
     gc.collect()
     if 'gc' in methods:
         if TopOGraph.verbosity > 0:
@@ -282,17 +281,15 @@
         if TopOGraph.verbosity > 0:
             print('Computing Spearman R for PCA...')
         EigenbasisGCResults['PCA'], _ = spearmanr(
             base_geodesics, embedding_geodesics)
         gc.collect()
     if 'tw' in methods:
         EigenbasisTWResults['PCA'] = trustworthiness(data_pdist,
-                                                pca_emb,
-                                                n_neighbors=TopOGraph.base_knn,
-                                                n_jobs=n_jobs, X_is_distance=True, metric=metric)
+                                                pca_emb, metric='precomputed')
         if TopOGraph.verbosity > 0:
             print('Computed trustworthiness for projection {}'.format(key))
         gc.collect()
     if additional_eigenbases is not None:
         for key in additional_eigenbases.keys():
             if 'gc' in methods:
                 if TopOGraph.verbosity > 0:
@@ -313,22 +310,21 @@
                 if TopOGraph.verbosity > 0:
                     print('Computing Spearman R for eigenbasis \'{}...\''.format(key))
                 EigenbasisGCResults[key], _ = spearmanr(
                     base_geodesics, embedding_geodesics)
                 gc.collect()
             if 'gs' in methods:
                 EigenbasisGSResults[key] = global_score(
-                    pca_emb, additional_eigenbases[key], X_is_pca=True)
+                    X, additional_eigenbases[key], Y_pca=pca_emb)
                 if TopOGraph.verbosity > 0:
                     print('Computed global score for eigenbasis {}'.format(key))
                 gc.collect()
             if 'tw' in methods:
                 EigenbasisTWResults[key] = trustworthiness(data_pdist,
-                                                            additional_eigenbases[key], n_neighbors=TopOGraph.base_knn,
-                                                            n_jobs=n_jobs, X_is_distance=True, metric=metric)
+                                                            additional_eigenbases[key], metric='precomputed')
                 if TopOGraph.verbosity > 0:
                     print('Computed trustworthiness for eigenbasis {}'.format(key))
                 gc.collect()
     if additional_projections is not None:
         for key in additional_projections.keys():
             if 'gc' in methods:
                 if TopOGraph.verbosity > 0:
@@ -349,22 +345,21 @@
                 if TopOGraph.verbosity > 0:
                     print('Computing Spearman R for projection \'{}...\''.format(key))
                 ProjectionGCResults[key], _ = spearmanr(
                     base_geodesics, embedding_geodesics)
                 gc.collect()
             if 'gs' in methods:
                 ProjectionGSResults[key] = global_score(
-                    pca_emb, additional_projections[key], X_is_pca=True)
+                    X, additional_projections[key], Y_pca=pca_emb)
                 if TopOGraph.verbosity > 0:
                     print('Computed global score for projection {}'.format(key))
                 gc.collect()
             if 'tw' in methods:
                 ProjectionTWResults[key] = trustworthiness(data_pdist,
-                                                            additional_projections[key], n_neighbors=TopOGraph.base_knn,
-                                                            n_jobs=n_jobs, X_is_distance=True, metric=metric)
+                                                            additional_projections[key], metric='precomputed')
                 if TopOGraph.verbosity > 0:
                     print('Computed trustworthiness for projection {}'.format(key))
                 gc.collect()
 
     res_dict = {'Eigenbasis - Trustworthiness' : EigenbasisTWResults,
                 'Eigenbasis - Geodesic correlation' : EigenbasisGCResults,
                 'Eigenbasis - Global score' : EigenbasisGSResults,
```

### Comparing `topometry-0.2.0.9.1/topo/plot.py` & `topometry-0.2.1.0/topo/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
     width, height = 2 * nstd * np.sqrt(np.absolute(vals))
     ellip = Ellipse(pos, width=width, height=height, angle=theta, **kwargs)
     ax.add_artist(ellip)
     return ellip
 
 
 
-def plot_riemann_metric(emb, laplacian, H_emb=None, ax=None, n_plot=50, std=1, alpha=0.1, title='Riemannian metric', title_fontsize=10,
+def plot_riemann_metric(emb, L, H_emb=None, ax=None, n_plot=50, std=1, alpha=0.1, title='Riemannian metric', title_fontsize=10,
                         labels=None, pt_size=1, cmap='Spectral',  figsize=(8,8), random_state=None, **kwargs):
     """
     Plot Riemannian metric using ellipses. Adapted from Megaman (https://github.com/mmp2/megaman).
 
     Parameters
     ----------
```

### Comparing `topometry-0.2.0.9.1/topo/single_cell.py` & `topometry-0.2.1.0/topo/single_cell.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/spectral/_spectral.py` & `topometry-0.2.1.0/topo/spectral/_spectral.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/spectral/eigen.py` & `topometry-0.2.1.0/topo/spectral/eigen.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
                  weight=True,
                  laplacian_type='random_walk',
                  anisotropy=1,
                  t=1,
                  random_state=None,
                  return_evals=False,
                  estimate_eigengap=True,
+                 enforce_min_eigs=True,
                  verbose=False):
         self.n_components = n_components
         self.method = method
         self.eigensolver = eigensolver
         self.eigen_tol = eigen_tol
         self.drop_first = drop_first
         self.laplacian_type = laplacian_type
@@ -220,14 +221,15 @@
         self.embedding = None
         self.powered_operator = None
         self.N = None
         self.D_inv_sqrt_ = None
         self.return_evals = return_evals
         self.estimate_eigengap = estimate_eigengap
         self.eigengap = None
+        self.enforce_min_eigs = enforce_min_eigs
 
     def __repr__(self):
         if self.eigenvectors is not None:
             if (self.N is not None):
                 msg = "EigenDecomposition() estimator fitted with %i samples" % (
                     self.N)
             else:
@@ -326,21 +328,23 @@
         evals, evecs = eigendecompose(target, eigensolver=self.eigensolver, n_components=self.n_components,
                                       largest=largest, eigen_tol=self.eigen_tol, random_state=self.random_state, verbose=self.verbose)
         if self.drop_first:
             evals = evals[1:]
             evecs = evecs[:, 1:]
         if self.estimate_eigengap:
             max_eigs = int(np.sum(evals > 0, axis=0))
-            first_diff = np.diff(evals)
-            eg = np.argmax(first_diff) + 1
-            if max_eigs == len(evals):
-                self.eigengap = max_eigs
+            if self.method not in ['LE', 'top', 'bottom']:
+                first_diff = np.diff(evals)
+                eg = np.argmax(first_diff) + 1
+                if max_eigs == len(evals):
+                    self.eigengap = max_eigs
+                else:
+                    self.eigengap = eg
             else:
-                self.eigengap = eg
-
+                self.eigengap = max_eigs
         if self.method in ['DM', 'msDM']:
             if symmetric:
                 evecs = self.D_inv_sqrt_.dot(evecs)
             for i in range(evecs.shape[1]):
                 evecs[:, i] = evecs[:, i] / np.linalg.norm(evecs[:, i])
             if self.method == 'DM':
                 self.embedding = evecs * evals
```

### Comparing `topometry-0.2.0.9.1/topo/spectral/locally.py` & `topometry-0.2.1.0/topo/spectral/locally.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/spectral/umap_layouts.py` & `topometry-0.2.1.0/topo/spectral/umap_layouts.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/topograph.py` & `topometry-0.2.1.0/topo/topograph.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,17 @@
 
     base_kernel : topo.tpgraph.Kernel (optional, default None).
         An optional Kernel object already fitted with the data. If available, the original input data X is not required.
 
     eigenmap_method : str (optional, default 'DM').
         Which eigenmap method to use. Defaults to 'DM', which is the diffusion maps method and will use the diffusion
         operator learned from the used kernel. Options include:
-        * 'DM' - uses the diffusion operator learned from the used kernel (TopOGraph.kernel.P). By default, uses
-        the multiscale Diffusion Maps version, which accounts for all possible diffusion timescales. Finds top eigenpairs (with highest eigenvalues).
+        * 'msDM' - uses the diffusion operator learned from the used kernel (TopOGraph.base_kernel.P) using the multiscale version of Diffusion Maps version,
+          which accounts for all possible diffusion timescales. Finds top eigenpairs (with highest eigenvalues).
+        * 'DM' - uses the diffusion operator learned from the used kernel (TopOGraph.base_kernel.P). Finds top eigenpairs (with highest eigenvalues).
         * 'LE' - uses the graph Laplacian learned from the used kernel (TopOGraph.kernel.L). Finds bottom eigenpairs (with lowest eigenvalues).
         * 'top' - uses the kernel matrix (TopOGraph.kernel.K) as the affinity matrix. Finds top eigenpairs (with highest eigenvalues).
         * 'bottom' - uses the kernel matrix (TopOGraph.kernel.K) as the affinity matrix. Finds bottom eigenpairs (with lowest eigenvalues).
 
     alpha : int or float (optional, default 1).
          Anisotropy. Alpha in the diffusion maps literature. Controls how much the results are biased by data distribution.
          Defaults to 1, which unbiases results from data underlying sampling distribution.
```

### Comparing `topometry-0.2.0.9.1/topo/tpgraph/cknn.py` & `topometry-0.2.1.0/topo/tpgraph/cknn.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/tpgraph/fuzzy.py` & `topometry-0.2.1.0/topo/tpgraph/fuzzy.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/tpgraph/intrinsic_dim.py` & `topometry-0.2.1.0/topo/tpgraph/intrinsic_dim.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/tpgraph/kernels.py` & `topometry-0.2.1.0/topo/tpgraph/kernels.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/tpgraph/procrustes.py` & `topometry-0.2.1.0/topo/tpgraph/procrustes.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/utils/_utils.py` & `topometry-0.2.1.0/topo/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topo/utils/umap_utils.py` & `topometry-0.2.1.0/topo/utils/umap_utils.py`

 * *Files identical despite different names*

### Comparing `topometry-0.2.0.9.1/topometry.egg-info/PKG-INFO` & `topometry-0.2.1.0/topometry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topometry
-Version: 0.2.0.9.1
+Version: 0.2.1.0
 Summary: A comprehensive dimensional reduction framework to recover latent information from data.
 Home-page: https://github.com/davisidarta/topometry
 Author: Davi Sidarta-Oliveira
 Author-email: davi.oliveira@dpag.ox.ac.uk
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/davisidarta/topometry/issues
 Platform: UNKNOWN
```

### Comparing `topometry-0.2.0.9.1/topometry.egg-info/SOURCES.txt` & `topometry-0.2.1.0/topometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

