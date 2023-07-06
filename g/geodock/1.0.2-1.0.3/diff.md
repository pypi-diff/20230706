# Comparing `tmp/geodock-1.0.2.tar.gz` & `tmp/geodock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/scratch4/jgray21/lchu11/GeoDock/dist/.tmp-yt6dcdhr/geodock-1.0.2.tar", last modified: Wed Jul  5 20:59:29 2023, max compression
+gzip compressed data, was "/scratch4/jgray21/lchu11/GeoDock/dist/.tmp-4mzbkt3g/geodock-1.0.3.tar", last modified: Thu Jul  6 02:28:34 2023, max compression
```

## Comparing `geodock-1.0.2.tar` & `geodock-1.0.3.tar`

### file list

```diff
@@ -1,43 +1,51 @@
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1065 2023-06-30 18:18:41.000000 geodock-1.0.2/LICENSE.md
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)       19 2023-07-05 19:31:03.000000 geodock-1.0.2/MANIFEST.in
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:59:29.000000 geodock-1.0.2/PKG-INFO
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      905 2023-07-04 02:59:52.000000 geodock-1.0.2/README.md
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2494 2023-07-05 17:00:05.000000 geodock-1.0.2/geodock/GeoDockRunner.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:34.000000 geodock-1.0.2/geodock/__init__.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/model/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5221 2023-06-01 18:47:22.000000 geodock-1.0.2/geodock/model/GeoDock.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:17.000000 geodock-1.0.2/geodock/model/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      486 2023-05-17 20:56:02.000000 geodock-1.0.2/geodock/model/interface.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/model/modules/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 17:15:41.000000 geodock-1.0.2/geodock/model/modules/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7909 2023-06-09 18:56:03.000000 geodock-1.0.2/geodock/model/modules/graph_module.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7183 2023-07-04 03:51:21.000000 geodock-1.0.2/geodock/model/modules/iterative_transformer.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9365 2023-07-04 03:50:32.000000 geodock-1.0.2/geodock/model/modules/structure_module.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/refine/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:58:25.000000 geodock-1.0.2/geodock/refine/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1654 2023-07-02 04:02:12.000000 geodock-1.0.2/geodock/refine/openmm_ref.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3243 2023-06-30 21:10:35.000000 geodock-1.0.2/geodock/refine/pyrosetta_ref.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/trainer/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-18 19:22:41.000000 geodock-1.0.2/geodock/trainer/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1013 2023-05-18 19:28:10.000000 geodock-1.0.2/geodock/trainer/run.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3252 2023-05-18 19:29:30.000000 geodock-1.0.2/geodock/trainer/train.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5198 2023-05-18 19:22:42.000000 geodock-1.0.2/geodock/trainer/utils.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock/utils/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:58:12.000000 geodock-1.0.2/geodock/utils/__init__.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2685 2023-05-17 17:15:41.000000 geodock-1.0.2/geodock/utils/coords6d.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3368 2023-07-05 16:57:57.000000 geodock-1.0.2/geodock/utils/docking.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3960 2023-05-19 18:37:10.000000 geodock-1.0.2/geodock/utils/embed.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9640 2023-05-18 14:01:10.000000 geodock-1.0.2/geodock/utils/loss.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     4966 2023-06-12 20:54:16.000000 geodock-1.0.2/geodock/utils/metrics.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3686 2023-06-30 21:06:20.000000 geodock-1.0.2/geodock/utils/pdb.py
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)    18138 2023-07-04 03:50:03.000000 geodock-1.0.2/geodock/utils/transforms.py
-drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/PKG-INFO
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      880 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/SOURCES.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        1 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/dependency_links.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)       84 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/requires.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)        8 2023-07-05 20:59:29.000000 geodock-1.0.2/geodock.egg-info/top_level.txt
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)       81 2023-07-05 18:52:34.000000 geodock-1.0.2/pyproject.toml
--rw-r--r--   0 lchu11    (1163) jgray21   (1016)      434 2023-07-05 20:59:29.000000 geodock-1.0.2/setup.cfg
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1065 2023-06-30 18:18:41.000000 geodock-1.0.3/LICENSE.md
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       19 2023-07-05 19:31:03.000000 geodock-1.0.3/MANIFEST.in
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-06 02:28:34.000000 geodock-1.0.3/PKG-INFO
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      905 2023-07-04 02:59:52.000000 geodock-1.0.3/README.md
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2494 2023-07-05 17:00:05.000000 geodock-1.0.3/geodock/GeoDockRunner.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:34.000000 geodock-1.0.3/geodock/__init__.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/datasets/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     6101 2023-06-23 22:36:15.000000 geodock-1.0.3/geodock/datasets/RepD2_dataset.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:25:07.000000 geodock-1.0.3/geodock/datasets/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5558 2023-06-15 14:52:21.000000 geodock-1.0.3/geodock/datasets/bound_dataset.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9696 2023-06-23 16:05:15.000000 geodock-1.0.3/geodock/datasets/gen_dataset.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2109 2023-06-06 17:44:13.000000 geodock-1.0.3/geodock/datasets/geodock_datamodule.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)    20058 2023-07-04 03:46:53.000000 geodock-1.0.3/geodock/datasets/geodock_dataset.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3242 2023-06-23 14:50:34.000000 geodock-1.0.3/geodock/datasets/unbound_dataset.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/model/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5221 2023-06-01 18:47:22.000000 geodock-1.0.3/geodock/model/GeoDock.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 18:03:17.000000 geodock-1.0.3/geodock/model/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      486 2023-05-17 20:56:02.000000 geodock-1.0.3/geodock/model/interface.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/model/modules/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-17 17:15:41.000000 geodock-1.0.3/geodock/model/modules/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7909 2023-06-09 18:56:03.000000 geodock-1.0.3/geodock/model/modules/graph_module.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     7183 2023-07-04 03:51:21.000000 geodock-1.0.3/geodock/model/modules/iterative_transformer.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9365 2023-07-04 03:50:32.000000 geodock-1.0.3/geodock/model/modules/structure_module.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/refine/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:58:25.000000 geodock-1.0.3/geodock/refine/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1654 2023-07-02 04:02:12.000000 geodock-1.0.3/geodock/refine/openmm_ref.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3243 2023-06-30 21:10:35.000000 geodock-1.0.3/geodock/refine/pyrosetta_ref.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/trainer/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-05-18 19:22:41.000000 geodock-1.0.3/geodock/trainer/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1013 2023-05-18 19:28:10.000000 geodock-1.0.3/geodock/trainer/run.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3252 2023-05-18 19:29:30.000000 geodock-1.0.3/geodock/trainer/train.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     5198 2023-05-18 19:22:42.000000 geodock-1.0.3/geodock/trainer/utils.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock/utils/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        0 2023-07-05 20:58:12.000000 geodock-1.0.3/geodock/utils/__init__.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     2685 2023-05-17 17:15:41.000000 geodock-1.0.3/geodock/utils/coords6d.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3368 2023-07-05 16:57:57.000000 geodock-1.0.3/geodock/utils/docking.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3960 2023-05-19 18:37:10.000000 geodock-1.0.3/geodock/utils/embed.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     9640 2023-05-18 14:01:10.000000 geodock-1.0.3/geodock/utils/loss.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     4966 2023-06-12 20:54:16.000000 geodock-1.0.3/geodock/utils/metrics.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     3686 2023-06-30 21:06:20.000000 geodock-1.0.3/geodock/utils/pdb.py
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)    18138 2023-07-04 03:50:03.000000 geodock-1.0.3/geodock/utils/transforms.py
+drwxr-xr-x   0 lchu11    (1163) jgray21   (1016)        0 2023-07-06 02:28:34.000000 geodock-1.0.3/geodock.egg-info/
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1079 2023-07-06 02:28:33.000000 geodock-1.0.3/geodock.egg-info/PKG-INFO
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)     1120 2023-07-06 02:28:33.000000 geodock-1.0.3/geodock.egg-info/SOURCES.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        1 2023-07-06 02:28:33.000000 geodock-1.0.3/geodock.egg-info/dependency_links.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       84 2023-07-06 02:28:33.000000 geodock-1.0.3/geodock.egg-info/requires.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)        8 2023-07-06 02:28:33.000000 geodock-1.0.3/geodock.egg-info/top_level.txt
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)       81 2023-07-05 18:52:34.000000 geodock-1.0.3/pyproject.toml
+-rw-r--r--   0 lchu11    (1163) jgray21   (1016)      466 2023-07-06 02:28:34.000000 geodock-1.0.3/setup.cfg
```

### Comparing `geodock-1.0.2/LICENSE.md` & `geodock-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/PKG-INFO` & `geodock-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodock
-Version: 1.0.2
+Version: 1.0.3
 Author: Lee-Shin Chu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GeoDock
```

### Comparing `geodock-1.0.2/README.md` & `geodock-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/GeoDockRunner.py` & `geodock-1.0.3/geodock/GeoDockRunner.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/model/GeoDock.py` & `geodock-1.0.3/geodock/model/GeoDock.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/model/modules/graph_module.py` & `geodock-1.0.3/geodock/model/modules/graph_module.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/model/modules/iterative_transformer.py` & `geodock-1.0.3/geodock/model/modules/iterative_transformer.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/model/modules/structure_module.py` & `geodock-1.0.3/geodock/model/modules/structure_module.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/refine/openmm_ref.py` & `geodock-1.0.3/geodock/refine/openmm_ref.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/refine/pyrosetta_ref.py` & `geodock-1.0.3/geodock/refine/pyrosetta_ref.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/trainer/run.py` & `geodock-1.0.3/geodock/trainer/run.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/trainer/train.py` & `geodock-1.0.3/geodock/trainer/train.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/trainer/utils.py` & `geodock-1.0.3/geodock/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/coords6d.py` & `geodock-1.0.3/geodock/utils/coords6d.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/docking.py` & `geodock-1.0.3/geodock/utils/docking.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/embed.py` & `geodock-1.0.3/geodock/utils/embed.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/loss.py` & `geodock-1.0.3/geodock/utils/loss.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/metrics.py` & `geodock-1.0.3/geodock/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/pdb.py` & `geodock-1.0.3/geodock/utils/pdb.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock/utils/transforms.py` & `geodock-1.0.3/geodock/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `geodock-1.0.2/geodock.egg-info/PKG-INFO` & `geodock-1.0.3/geodock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geodock
-Version: 1.0.2
+Version: 1.0.3
 Author: Lee-Shin Chu
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # GeoDock
```

### Comparing `geodock-1.0.2/geodock.egg-info/SOURCES.txt` & `geodock-1.0.3/geodock.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 geodock/GeoDockRunner.py
 geodock/__init__.py
 geodock.egg-info/PKG-INFO
 geodock.egg-info/SOURCES.txt
 geodock.egg-info/dependency_links.txt
 geodock.egg-info/requires.txt
 geodock.egg-info/top_level.txt
+geodock/datasets/RepD2_dataset.py
+geodock/datasets/__init__.py
+geodock/datasets/bound_dataset.py
+geodock/datasets/gen_dataset.py
+geodock/datasets/geodock_datamodule.py
+geodock/datasets/geodock_dataset.py
+geodock/datasets/unbound_dataset.py
 geodock/model/GeoDock.py
 geodock/model/__init__.py
 geodock/model/interface.py
 geodock/model/modules/__init__.py
 geodock/model/modules/graph_module.py
 geodock/model/modules/iterative_transformer.py
 geodock/model/modules/structure_module.py
```

