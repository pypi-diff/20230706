# Comparing `tmp/cybrex-1.0.4.tar.gz` & `tmp/cybrex-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.0.4.tar", last modified: Thu Jul  6 09:55:58 2023, max compression
+gzip compressed data, was "cybrex-1.0.5.tar", last modified: Thu Jul  6 09:59:08 2023, max compression
```

## Comparing `cybrex-1.0.4.tar` & `cybrex-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.437226 cybrex-1.0.4/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.4/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:55:58.436953 cybrex-1.0.4/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.4/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.433940 cybrex-1.0.4/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)     1298 2023-07-06 09:55:22.000000 cybrex-1.0.4/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)     5805 2023-07-06 09:55:22.000000 cybrex-1.0.4/cybrex/cybrex_ai.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:55:58.436432 cybrex-1.0.4/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-06 09:55:58.000000 cybrex-1.0.4/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-06 09:55:12.000000 cybrex-1.0.4/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:35:09.000000 cybrex-1.0.4/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 09:55:58.437347 cybrex-1.0.4/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.525329 cybrex-1.0.5/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.0.5/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:59:08.525057 cybrex-1.0.5/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      943 2023-07-05 20:42:40.000000 cybrex-1.0.5/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.522411 cybrex-1.0.5/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)     1300 2023-07-06 09:58:52.000000 cybrex-1.0.5/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5805 2023-07-06 09:55:22.000000 cybrex-1.0.5/cybrex/cybrex_ai.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-07-06 09:59:08.524502 cybrex-1.0.5/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)     1219 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      269 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      172 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-07-06 09:59:08.000000 cybrex-1.0.5/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-07-06 09:58:58.000000 cybrex-1.0.5/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      171 2023-07-05 19:35:09.000000 cybrex-1.0.5/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-07-06 09:59:08.525436 cybrex-1.0.5/setup.cfg
```

### Comparing `cybrex-1.0.4/PKG-INFO` & `cybrex-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.4
+Version: 1.0.5
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.4/README.md` & `cybrex-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.0.4/cybrex/cli.py` & `cybrex-1.0.5/cybrex/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import fire
-from cybrex_ai import CybrexAI
 from termcolor import colored
 
+from .cybrex_ai import CybrexAI
+
 
 class CybrexCli:
     def __init__(self):
         self.cybrex = CybrexAI()
 
     async def chat_doc(self, doi: str, question: str):
         """
```

### Comparing `cybrex-1.0.4/cybrex/cybrex_ai.py` & `cybrex-1.0.5/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.0.4/cybrex.egg-info/PKG-INFO` & `cybrex-1.0.5/cybrex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.0.4
+Version: 1.0.5
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.0.4/pyproject.toml` & `cybrex-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.0.4"
+version = "1.0.5"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```

