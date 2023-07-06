# Comparing `tmp/catwalk_common-0.0.5.tar.gz` & `tmp/catwalk_common-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catwalk_common-0.0.5.tar", last modified: Mon Jun 12 14:15:52 2023, max compression
+gzip compressed data, was "catwalk_common-0.0.6.tar", last modified: Thu Jul  6 14:12:54 2023, max compression
```

## Comparing `catwalk_common-0.0.5.tar` & `catwalk_common-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-06-12 07:47:42.000000 catwalk_common-0.0.5/README.md
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/catwalk_common/
--rw-rw-r--   0 marek     (1000) marek     (1000)      127 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1698 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/_ccf_dataframe.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2942 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/_common_case_format.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     2236 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/catwalk_common/plugins.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/catwalk_common.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      337 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       30 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-06-12 14:15:52.000000 catwalk_common-0.0.5/catwalk_common.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)      622 2023-06-12 13:38:38.000000 catwalk_common-0.0.5/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-06-12 14:15:52.837417 catwalk_common-0.0.5/setup.cfg
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-07-06 14:12:54.472206 catwalk_common-0.0.6/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-07-06 14:12:54.472206 catwalk_common-0.0.6/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)       49 2023-07-03 08:15:33.000000 catwalk_common-0.0.6/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-07-06 14:12:54.472206 catwalk_common-0.0.6/catwalk_common/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      127 2023-07-06 07:36:28.000000 catwalk_common-0.0.6/catwalk_common/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1698 2023-07-06 07:29:21.000000 catwalk_common-0.0.6/catwalk_common/_ccf_dataframe.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2942 2023-07-06 14:11:21.000000 catwalk_common-0.0.6/catwalk_common/_common_case_format.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     2236 2023-07-06 07:29:21.000000 catwalk_common-0.0.6/catwalk_common/plugins.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2023-07-06 14:12:54.472206 catwalk_common-0.0.6/catwalk_common.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      578 2023-07-06 14:12:54.000000 catwalk_common-0.0.6/catwalk_common.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      337 2023-07-06 14:12:54.000000 catwalk_common-0.0.6/catwalk_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2023-07-06 14:12:54.000000 catwalk_common-0.0.6/catwalk_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       28 2023-07-06 14:12:54.000000 catwalk_common-0.0.6/catwalk_common.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       15 2023-07-06 14:12:54.000000 catwalk_common-0.0.6/catwalk_common.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)      620 2023-07-06 14:11:21.000000 catwalk_common-0.0.6/pyproject.toml
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2023-07-06 14:12:54.472206 catwalk_common-0.0.6/setup.cfg
```

### Comparing `catwalk_common-0.0.5/PKG-INFO` & `catwalk_common-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk_common
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `catwalk_common-0.0.5/catwalk_common/_ccf_dataframe.py` & `catwalk_common-0.0.6/catwalk_common/_ccf_dataframe.py`

 * *Files identical despite different names*

### Comparing `catwalk_common-0.0.5/catwalk_common/_common_case_format.py` & `catwalk_common-0.0.6/catwalk_common/_common_case_format.py`

 * *Files identical despite different names*

### Comparing `catwalk_common-0.0.5/catwalk_common/plugins.py` & `catwalk_common-0.0.6/catwalk_common/plugins.py`

 * *Files identical despite different names*

### Comparing `catwalk_common-0.0.5/catwalk_common.egg-info/PKG-INFO` & `catwalk_common-0.0.6/catwalk_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catwalk-common
-Version: 0.0.5
+Version: 0.0.6
 Author-email: Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Marek Połom <marek.polom@deepsense.ai>
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `catwalk_common-0.0.5/pyproject.toml` & `catwalk_common-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "catwalk_common"
-version = "0.0.5"
+version = "0.0.6"
 license = { text = "GPLv3+" }
 authors = [
     { name = "Mateusz Hordyński", email = "mateusz.hordynski@deepsense.ai" },
     { name = "Marek Połom", email = "marek.polom@deepsense.ai" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
 ]
 requires-python = ">=3.8.0"
-dependencies = ["pydantic >= 1.8.2", "pandas >= 2.0.0"]
+dependencies = ["pydantic >= 1.8.2", "pandas >= 1.5"]
 readme = "README.md"
```

