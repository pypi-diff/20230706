# Comparing `tmp/rsxml-0.0.1.tar.gz` & `tmp/rsxml-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsxml-0.0.1.tar", last modified: Tue May 23 14:32:36 2023, max compression
+gzip compressed data, was "rsxml-0.0.1a0.tar", last modified: Tue May 23 14:37:02 2023, max compression
```

## Comparing `rsxml-0.0.1.tar` & `rsxml-0.0.1a0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.350793 rsxml-0.0.1/
--rw-r--r--   0 matt       (501) staff       (20)      476 2023-05-23 14:32:36.350880 rsxml-0.0.1/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       39 2023-05-23 14:16:11.000000 rsxml-0.0.1/README.md
--rw-r--r--   0 matt       (501) staff       (20)      550 2023-05-23 14:30:46.000000 rsxml-0.0.1/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)       79 2023-05-23 14:32:36.351170 rsxml-0.0.1/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1197 2023-05-23 14:24:16.000000 rsxml-0.0.1/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.343659 rsxml-0.0.1/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.345246 rsxml-0.0.1/src/debug/
--rw-r--r--   0 matt       (501) staff       (20)      102 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/debug/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     7971 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/debug/debug_proc.py
--rw-r--r--   0 matt       (501) staff       (20)     3118 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/debug/loop_timer.py
--rw-r--r--   0 matt       (501) staff       (20)     1904 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/debug/timer.py
--rw-r--r--   0 matt       (501) staff       (20)     8508 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/debug/timer_buckets.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.345726 rsxml-0.0.1/src/logging/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/logging/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     8209 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/logging/logger.py
--rw-r--r--   0 matt       (501) staff       (20)     3712 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/logging/progress_bar.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.348012 rsxml-0.0.1/src/rsxml/
--rw-r--r--   0 matt       (501) staff       (20)     2768 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/Analysis.py
--rw-r--r--   0 matt       (501) staff       (20)     7517 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/Dataset.py
--rw-r--r--   0 matt       (501) staff       (20)     2214 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/MetaData.py
--rw-r--r--   0 matt       (501) staff       (20)     5713 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/Project.py
--rw-r--r--   0 matt       (501) staff       (20)     2611 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/ProjectBounds.py
--rw-r--r--   0 matt       (501) staff       (20)     3128 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/QAQCEvent.py
--rw-r--r--   0 matt       (501) staff       (20)     2984 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/RSObj.py
--rw-r--r--   0 matt       (501) staff       (20)     2461 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/Realization.py
--rw-r--r--   0 matt       (501) staff       (20)      236 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      428 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/rsxml/common.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.348968 rsxml-0.0.1/src/rsxml.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)      476 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      824 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       24 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       26 2023-05-23 14:32:36.000000 rsxml-0.0.1/src/rsxml.egg-info/top_level.txt
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:32:36.350620 rsxml-0.0.1/src/tests/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     2320 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_dotenv.py
--rw-r--r--   0 matt       (501) staff       (20)     1127 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_etags.py
--rw-r--r--   0 matt       (501) staff       (20)     1325 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_paths.py
--rw-r--r--   0 matt       (501) staff       (20)     6908 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_project_xml.py
--rw-r--r--   0 matt       (501) staff       (20)     7499 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_timers.py
--rw-r--r--   0 matt       (501) staff       (20)     3202 2023-05-23 14:16:11.000000 rsxml-0.0.1/src/tests/test_util.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.650679 rsxml-0.0.1a0/
+-rw-r--r--   0 matt       (501) staff       (20)      478 2023-05-23 14:37:02.650772 rsxml-0.0.1a0/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)       39 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/README.md
+-rw-r--r--   0 matt       (501) staff       (20)      550 2023-05-23 14:30:46.000000 rsxml-0.0.1a0/pyproject.toml
+-rw-r--r--   0 matt       (501) staff       (20)       79 2023-05-23 14:37:02.651038 rsxml-0.0.1a0/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1197 2023-05-23 14:24:16.000000 rsxml-0.0.1a0/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.642647 rsxml-0.0.1a0/src/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.644759 rsxml-0.0.1a0/src/debug/
+-rw-r--r--   0 matt       (501) staff       (20)      102 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     7971 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/debug_proc.py
+-rw-r--r--   0 matt       (501) staff       (20)     3118 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/loop_timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     1904 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/timer.py
+-rw-r--r--   0 matt       (501) staff       (20)     8508 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/debug/timer_buckets.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.645199 rsxml-0.0.1a0/src/logging/
+-rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     8209 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/logger.py
+-rw-r--r--   0 matt       (501) staff       (20)     3712 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/logging/progress_bar.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.647792 rsxml-0.0.1a0/src/rsxml/
+-rw-r--r--   0 matt       (501) staff       (20)     2768 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Analysis.py
+-rw-r--r--   0 matt       (501) staff       (20)     7517 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Dataset.py
+-rw-r--r--   0 matt       (501) staff       (20)     2214 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/MetaData.py
+-rw-r--r--   0 matt       (501) staff       (20)     5713 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Project.py
+-rw-r--r--   0 matt       (501) staff       (20)     2611 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/ProjectBounds.py
+-rw-r--r--   0 matt       (501) staff       (20)     3128 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/QAQCEvent.py
+-rw-r--r--   0 matt       (501) staff       (20)     2984 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/RSObj.py
+-rw-r--r--   0 matt       (501) staff       (20)     2461 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/Realization.py
+-rw-r--r--   0 matt       (501) staff       (20)      236 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      428 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/rsxml/common.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.648821 rsxml-0.0.1a0/src/rsxml.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)      478 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      824 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-05-23 14:32:36.000000 rsxml-0.0.1a0/src/rsxml.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)       24 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)       26 2023-05-23 14:37:02.000000 rsxml-0.0.1a0/src/rsxml.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-05-23 14:37:02.650431 rsxml-0.0.1a0/src/tests/
+-rw-r--r--   0 matt       (501) staff       (20)        0 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     2320 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_dotenv.py
+-rw-r--r--   0 matt       (501) staff       (20)     1127 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_etags.py
+-rw-r--r--   0 matt       (501) staff       (20)     1325 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_paths.py
+-rw-r--r--   0 matt       (501) staff       (20)     6908 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_project_xml.py
+-rw-r--r--   0 matt       (501) staff       (20)     7499 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_timers.py
+-rw-r--r--   0 matt       (501) staff       (20)     3202 2023-05-23 14:16:11.000000 rsxml-0.0.1a0/src/tests/test_util.py
```

### Comparing `rsxml-0.0.1/pyproject.toml` & `rsxml-0.0.1a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/setup.py` & `rsxml-0.0.1a0/setup.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/debug/debug_proc.py` & `rsxml-0.0.1a0/src/debug/debug_proc.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/debug/loop_timer.py` & `rsxml-0.0.1a0/src/debug/loop_timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/debug/timer.py` & `rsxml-0.0.1a0/src/debug/timer.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/debug/timer_buckets.py` & `rsxml-0.0.1a0/src/debug/timer_buckets.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/logging/logger.py` & `rsxml-0.0.1a0/src/logging/logger.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/logging/progress_bar.py` & `rsxml-0.0.1a0/src/logging/progress_bar.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/Analysis.py` & `rsxml-0.0.1a0/src/rsxml/Analysis.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/Dataset.py` & `rsxml-0.0.1a0/src/rsxml/Dataset.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/MetaData.py` & `rsxml-0.0.1a0/src/rsxml/MetaData.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/Project.py` & `rsxml-0.0.1a0/src/rsxml/Project.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/ProjectBounds.py` & `rsxml-0.0.1a0/src/rsxml/ProjectBounds.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/QAQCEvent.py` & `rsxml-0.0.1a0/src/rsxml/QAQCEvent.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/RSObj.py` & `rsxml-0.0.1a0/src/rsxml/RSObj.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml/Realization.py` & `rsxml-0.0.1a0/src/rsxml/Realization.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/rsxml.egg-info/SOURCES.txt` & `rsxml-0.0.1a0/src/rsxml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_dotenv.py` & `rsxml-0.0.1a0/src/tests/test_dotenv.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_etags.py` & `rsxml-0.0.1a0/src/tests/test_etags.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_paths.py` & `rsxml-0.0.1a0/src/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_project_xml.py` & `rsxml-0.0.1a0/src/tests/test_project_xml.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_timers.py` & `rsxml-0.0.1a0/src/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `rsxml-0.0.1/src/tests/test_util.py` & `rsxml-0.0.1a0/src/tests/test_util.py`

 * *Files identical despite different names*

