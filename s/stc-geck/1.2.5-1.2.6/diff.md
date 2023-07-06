# Comparing `tmp/stc-geck-1.2.5.tar.gz` & `tmp/stc-geck-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stc-geck-1.2.5.tar", last modified: Wed Jul  5 19:35:12 2023, max compression
+gzip compressed data, was "stc-geck-1.2.6.tar", last modified: Thu Jul  6 10:23:33 2023, max compression
```

## Comparing `stc-geck-1.2.5.tar` & `stc-geck-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.061931 stc-geck-1.2.5/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.5/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:35:12.061662 stc-geck-1.2.5/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.5/README.md
--rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-05 19:34:52.000000 stc-geck-1.2.5/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.2.5/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-05 19:35:12.062031 stc-geck-1.2.5/setup.cfg
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.059336 stc-geck-1.2.5/stc_geck/
--rw-r--r--   0 pasha      (501) staff       (20)      891 2023-07-05 08:35:32.000000 stc-geck-1.2.5/stc_geck/advices.py
--rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.2.5/stc_geck/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5949 2023-07-05 19:34:46.000000 stc-geck-1.2.5/stc_geck/client.py
--rw-r--r--   0 pasha      (501) staff       (20)     1641 2023-06-19 18:59:24.000000 stc-geck-1.2.5/stc_geck/utils.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-05 19:35:12.061118 stc-geck-1.2.5/stc_geck.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-05 19:35:12.000000 stc-geck-1.2.5/stc_geck.egg-info/top_level.txt
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:23:33.084645 stc-geck-1.2.6/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 stc-geck-1.2.6/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:23:33.084041 stc-geck-1.2.6/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      398 2023-07-03 19:45:17.000000 stc-geck-1.2.6/README.md
+-rw-r--r--   0 pasha      (501) staff       (20)      600 2023-07-06 10:23:10.000000 stc-geck-1.2.6/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)       96 2023-07-05 16:20:57.000000 stc-geck-1.2.6/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 10:23:33.084951 stc-geck-1.2.6/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:23:33.077143 stc-geck-1.2.6/stc_geck/
+-rw-r--r--   0 pasha      (501) staff       (20)      805 2023-07-06 10:23:10.000000 stc-geck-1.2.6/stc_geck/advices.py
+-rw-r--r--   0 pasha      (501) staff       (20)     6136 2023-07-05 16:12:35.000000 stc-geck-1.2.6/stc_geck/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5950 2023-07-05 19:36:58.000000 stc-geck-1.2.6/stc_geck/client.py
+-rw-r--r--   0 pasha      (501) staff       (20)     1640 2023-07-05 19:36:42.000000 stc-geck-1.2.6/stc_geck/utils.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 10:23:33.082980 stc-geck-1.2.6/stc_geck.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)      743 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      320 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       97 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        9 2023-07-06 10:23:33.000000 stc-geck-1.2.6/stc_geck.egg-info/top_level.txt
```

### Comparing `stc-geck-1.2.5/PKG-INFO` & `stc-geck-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.5
+Version: 1.2.6
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `stc-geck-1.2.5/pyproject.toml` & `stc-geck-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stc-geck"
-version = "1.2.5"
+version = "1.2.6"
 authors = [{ name = "Interdimensional Walker" }]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

### Comparing `stc-geck-1.2.5/stc_geck/advices.py` & `stc-geck-1.2.6/stc_geck/advices.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from aiosumma import SummaClient
 
-SHOULD = 0
-MUST = 1
-MUST_NOT = 2
-
 
 PR_TEMPORAL_RANKING_FORMULA = "original_score * fastsigm(abs(now - issued_at) / (86400 * 3) + 5, -1) * 1.96 * " \
                               "fastsigm(iqpr(quantized_page_rank), 0.15)"
 
 
 async def get_documents_on_topic(summa_client: SummaClient, topic: str, documents: int = 20):
     return await summa_client.search_documents([{
         "index_alias": "nexus_science",
-        "query": {"query": {"boolean": {"subqueries": [
-            {"occur": SHOULD, "query": {
-                "query": {"match": {"value": topic, "default_fields": ["title", "abstract"], "field_boosts": {}}}}},
-        ]}}},
-        "collectors": [{"collector": {"top_docs": {"limit": documents, "scorer": {"scorer": {
+        "query": {"boolean": {"subqueries": [
+            {"occur": "should", "query": {"match": {"value": topic, "default_fields": ["title", "abstract"], "field_boosts": {}}}},
+        ]}},
+        "collectors": [{"top_docs": {"limit": documents, "scorer": {"scorer": {
             "eval_expr": PR_TEMPORAL_RANKING_FORMULA,
-        }}}}}],
+        }}}}],
         "is_fieldnorms_scoring_enabled": False,
     }])
```

### Comparing `stc-geck-1.2.5/stc_geck/cli.py` & `stc-geck-1.2.6/stc_geck/cli.py`

 * *Files identical despite different names*

### Comparing `stc-geck-1.2.5/stc_geck/client.py` & `stc-geck-1.2.6/stc_geck/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,8 @@
             )
         else:
             return await create_car(
                 output_car,
                 load_document(self.summa_client.documents(index_name)),
                 limit=limit,
                 name_template=name_template,
-            )
+            )
```

### Comparing `stc-geck-1.2.5/stc_geck/utils.py` & `stc-geck-1.2.6/stc_geck/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import os
 import re
 import tempfile
 from urllib.parse import quote
 
 import ipfs_hamt_directory_py
 
-
 NON_ALNUMWHITESPACE_REGEX = re.compile(r'([^\s\w])+')
 MULTIWHITESPACE_REGEX = re.compile(r"\s+")
 
 
 def cast_string_to_single_string(s):
     processed = MULTIWHITESPACE_REGEX.sub(' ', NON_ALNUMWHITESPACE_REGEX.sub(' ', s))
     processed = processed.strip().replace(' ', '-')
```

### Comparing `stc-geck-1.2.5/stc_geck.egg-info/PKG-INFO` & `stc-geck-1.2.6/stc_geck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stc-geck
-Version: 1.2.5
+Version: 1.2.6
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

