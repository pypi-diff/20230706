# Comparing `tmp/arcee-align-0.0.5.tar.gz` & `tmp/arcee-align-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcee-align-0.0.5.tar", last modified: Thu Jul  6 20:11:27 2023, max compression
+gzip compressed data, was "arcee-align-0.0.6.tar", last modified: Thu Jul  6 20:13:56 2023, max compression
```

## Comparing `arcee-align-0.0.5.tar` & `arcee-align-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:11:27.914717 arcee-align-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 20:11:27.914717 arcee-align-0.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1216 2023-06-26 14:33:57.000000 arcee-align-0.0.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:11:27.910717 arcee-align-0.0.5/arcee/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-07-06 20:11:23.000000 arcee-align-0.0.5/arcee/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:11:27.910717 arcee-align-0.0.5/arcee/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.5/arcee/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.5/arcee/data/generate.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2250 2023-07-06 17:31:19.000000 arcee-align-0.0.5/arcee/data/instruction_set.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:11:27.910717 arcee-align-0.0.5/arcee/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.5/arcee/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3498 2023-07-06 18:13:47.000000 arcee-align-0.0.5/arcee/models/lm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:11:27.914717 arcee-align-0.0.5/arcee_align.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 20:11:27.000000 arcee-align-0.0.5/arcee_align.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-07-06 20:11:27.000000 arcee-align-0.0.5/arcee_align.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-06 20:11:27.000000 arcee-align-0.0.5/arcee_align.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      148 2023-07-06 20:11:27.000000 arcee-align-0.0.5/arcee_align.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-06 20:11:27.000000 arcee-align-0.0.5/arcee_align.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-06 20:11:27.914717 arcee-align-0.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2023-07-06 20:11:16.000000 arcee-align-0.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:13:56.766761 arcee-align-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 20:13:56.766761 arcee-align-0.0.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1216 2023-06-26 14:33:57.000000 arcee-align-0.0.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:13:56.766761 arcee-align-0.0.6/arcee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-07-06 20:13:53.000000 arcee-align-0.0.6/arcee/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:13:56.766761 arcee-align-0.0.6/arcee/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      115 2023-06-25 23:31:22.000000 arcee-align-0.0.6/arcee/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5076 2023-06-25 23:39:47.000000 arcee-align-0.0.6/arcee/data/generate.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2250 2023-07-06 17:31:19.000000 arcee-align-0.0.6/arcee/data/instruction_set.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:13:56.766761 arcee-align-0.0.6/arcee/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       31 2023-06-22 05:12:31.000000 arcee-align-0.0.6/arcee/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3498 2023-07-06 18:13:47.000000 arcee-align-0.0.6/arcee/models/lm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-06 20:13:56.766761 arcee-align-0.0.6/arcee_align.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2168 2023-07-06 20:13:56.000000 arcee-align-0.0.6/arcee_align.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-07-06 20:13:56.000000 arcee-align-0.0.6/arcee_align.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-06 20:13:56.000000 arcee-align-0.0.6/arcee_align.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2023-07-06 20:13:56.000000 arcee-align-0.0.6/arcee_align.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-06 20:13:56.000000 arcee-align-0.0.6/arcee_align.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-06 20:13:56.766761 arcee-align-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1137 2023-07-06 20:11:16.000000 arcee-align-0.0.6/setup.py
```

### Comparing `arcee-align-0.0.5/PKG-INFO` & `arcee-align-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.5
+Version: 0.0.6
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
```

### Comparing `arcee-align-0.0.5/README.md` & `arcee-align-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.5/arcee/data/generate.py` & `arcee-align-0.0.6/arcee/data/generate.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.5/arcee/data/instruction_set.py` & `arcee-align-0.0.6/arcee/data/instruction_set.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.5/arcee/models/lm.py` & `arcee-align-0.0.6/arcee/models/lm.py`

 * *Files identical despite different names*

### Comparing `arcee-align-0.0.5/arcee_align.egg-info/PKG-INFO` & `arcee-align-0.0.6/arcee_align.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcee-align
-Version: 0.0.5
+Version: 0.0.6
 Summary: The open source toolkit for finetuning and deploying LLMs
 Home-page: https://arcee.ai/
 Author: Arcee
 Author-email: jacob@arcee.ai
 License: UNKNOWN
 Description: # Arcee
```

### Comparing `arcee-align-0.0.5/setup.py` & `arcee-align-0.0.6/setup.py`

 * *Files identical despite different names*

