# Comparing `tmp/golfy-1.3.4.tar.gz` & `tmp/golfy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-1.3.4.tar", last modified: Wed Jul  5 20:24:09 2023, max compression
+gzip compressed data, was "golfy-1.4.0.tar", last modified: Thu Jul  6 20:44:31 2023, max compression
```

## Comparing `golfy-1.3.4.tar` & `golfy-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-05 20:24:09.107637 golfy-1.3.4/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.3.4/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     1194 2023-07-05 20:24:09.107519 golfy-1.3.4/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      468 2023-07-03 19:41:44.000000 golfy-1.3.4/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-05 20:24:09.106315 golfy-1.3.4/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      289 2023-07-04 03:33:07.000000 golfy-1.3.4/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     6396 2023-07-03 19:39:52.000000 golfy-1.3.4/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     8467 2023-07-04 04:26:02.000000 golfy-1.3.4/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     2908 2023-07-03 19:47:51.000000 golfy-1.3.4/golfy/solution.py
--rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.3.4/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)      335 2023-07-03 19:34:38.000000 golfy-1.3.4/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.3.4/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-05 20:24:09.106734 golfy-1.3.4/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     1194 2023-07-05 20:24:09.000000 golfy-1.3.4/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      319 2023-07-05 20:24:09.000000 golfy-1.3.4/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-05 20:24:09.000000 golfy-1.3.4/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-05 20:24:09.000000 golfy-1.3.4/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      734 2023-07-05 20:21:27.000000 golfy-1.3.4/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-05 20:24:09.107673 golfy-1.3.4/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-05 20:24:09.107090 golfy-1.3.4/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      234 2023-07-03 19:40:32.000000 golfy-1.3.4/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.3.4/tests/test_optimize.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997751 golfy-1.4.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-1.4.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     1872 2023-07-06 20:44:31.997600 golfy-1.4.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     1146 2023-07-06 20:37:45.000000 golfy-1.4.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.996271 golfy-1.4.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      289 2023-07-04 03:33:07.000000 golfy-1.4.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5494 2023-07-06 20:32:53.000000 golfy-1.4.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6396 2023-07-03 19:39:52.000000 golfy-1.4.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     8453 2023-07-06 20:20:26.000000 golfy-1.4.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3163 2023-07-06 20:21:28.000000 golfy-1.4.0/golfy/solution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      270 2023-07-03 19:32:27.000000 golfy-1.4.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)      335 2023-07-03 19:34:38.000000 golfy-1.4.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3632 2023-07-03 19:39:30.000000 golfy-1.4.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997064 golfy-1.4.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     1872 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      370 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-06 20:44:31.000000 golfy-1.4.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      734 2023-07-06 20:42:37.000000 golfy-1.4.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-06 20:44:31.997792 golfy-1.4.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-06 20:44:31.997416 golfy-1.4.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      884 2023-07-06 20:33:42.000000 golfy-1.4.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      234 2023-07-03 19:40:32.000000 golfy-1.4.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      203 2023-07-03 19:41:20.000000 golfy-1.4.0/tests/test_optimize.py
```

### Comparing `golfy-1.3.4/LICENSE` & `golfy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-1.3.4/golfy/initialization.py` & `golfy-1.4.0/golfy/initialization.py`

 * *Files identical despite different names*

### Comparing `golfy-1.3.4/golfy/optimization.py` & `golfy-1.4.0/golfy/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,20 +210,21 @@
 
         if num_iters_without_improvement >= 3 and add_pool_if_stuck:
             replicates_in_need = [
                 r for (r, v) in replicate_to_violation_count.items() if v > 0
             ]
             assert len(replicates_in_need) > 0
             replicate_idx = min(replicates_in_need)
-            replicate = s.assignments[replicate_idx]
-            num_pools = len(replicate)
-            replicate[num_pools] = np.array([])
+            s.add_empty_pool(replicate_idx)
             num_iters_without_improvement = 0
             if verbose:
-                print("Adding pool %d to replicate %d" % (num_pools, replicate_idx + 1))
+                print(
+                    "Adding pool %d to replicate %d"
+                    % (len(s.assignments[replicate_idx]), replicate_idx + 1)
+                )
 
     result = old_num_violations == 0
 
     # just in case we ended up with any empty pools, remove them from the solution
     s.remove_empty_pools()
 
     if return_history:
```

### Comparing `golfy-1.3.4/golfy/solution.py` & `golfy-1.4.0/golfy/solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,22 @@
         pool_to_peptides[pool_idx_a] = np.array(
             [i for i in pool_a if i != peptide_a] + [peptide_b]
         )
         pool_to_peptides[pool_idx_b] = np.array(
             [i for i in pool_b if i != peptide_b] + [peptide_a]
         )
 
+    def add_empty_pool(self, replicate_idx: int):
+        """
+        Add an empty pool to the given replicate
+        """
+        replicate = self.assignments[replicate_idx]
+        num_pools = len(replicate)
+        replicate[num_pools] = np.array([])
+
     def remove_empty_pools(self):
         """
         Delete any empty pools and renumber the pools to be contiguous
         """
         for replicate_idx, pool_to_peptides in self.assignments.items():
             to_delete = [
                 pool_idx
```

### Comparing `golfy-1.3.4/golfy/validity.py` & `golfy-1.4.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-1.3.4/pyproject.toml` & `golfy-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'Environment :: Console',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: Apache Software License',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 readme = "README.md"
-version = "1.3.4"  
+version = "1.4.0"  
 
 [tool.setuptools]
 packages = ["golfy"]
 
 [project.urls]
 "Homepage" = "https://github.com/pirl-unc/golfy"
 "Bug Tracker" = "https://github.com/pirl-unc/golfy"
```

