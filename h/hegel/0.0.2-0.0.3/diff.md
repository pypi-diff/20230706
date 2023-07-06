# Comparing `tmp/hegel-0.0.2.tar.gz` & `tmp/hegel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hegel-0.0.2.tar", last modified: Thu Jul  6 15:23:00 2023, max compression
+gzip compressed data, was "hegel-0.0.3.tar", last modified: Thu Jul  6 15:46:48 2023, max compression
```

## Comparing `hegel-0.0.2.tar` & `hegel-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.496710 hegel-0.0.2/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:52:07.000000 hegel-0.0.2/LICENSE
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:23:00.496337 hegel-0.0.2/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2288 2023-07-05 23:53:02.000000 hegel-0.0.2/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.494056 hegel-0.0.2/hegel/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 00:08:03.000000 hegel-0.0.2/hegel/__init__.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     9418 2023-07-05 23:53:02.000000 hegel-0.0.2/hegel/scribe.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      796 2023-07-05 23:53:02.000000 hegel-0.0.2/hegel/utils.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel/version.py
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.495869 hegel-0.0.2/hegel.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      308 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-05 21:38:27.000000 hegel-0.0.2/hegel.egg-info/not-zip-safe
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       22 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/requires.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        6 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      684 2023-07-06 15:22:37.000000 hegel-0.0.2/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       13 2023-07-05 21:37:08.000000 hegel-0.0.2/requirements.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 15:23:00.496807 hegel-0.0.2/setup.cfg
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3635 2023-07-05 21:38:08.000000 hegel-0.0.2/setup.py
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 00:10:46.000000 hegel-0.0.2/version.txt
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:46:48.532959 hegel-0.0.3/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:52:07.000000 hegel-0.0.3/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:46:48.532641 hegel-0.0.3/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2288 2023-07-05 23:53:02.000000 hegel-0.0.3/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:46:48.530194 hegel-0.0.3/hegel/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 00:08:03.000000 hegel-0.0.3/hegel/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     9424 2023-07-06 15:40:31.000000 hegel-0.0.3/hegel/scribe.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      796 2023-07-05 23:53:02.000000 hegel-0.0.3/hegel/utils.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel/version.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:46:48.532259 hegel-0.0.3/hegel.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      308 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-05 21:38:27.000000 hegel-0.0.3/hegel.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       14 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        6 2023-07-06 15:46:48.000000 hegel-0.0.3/hegel.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      669 2023-07-06 15:38:40.000000 hegel-0.0.3/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       13 2023-07-05 21:37:08.000000 hegel-0.0.3/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 15:46:48.533040 hegel-0.0.3/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3635 2023-07-05 21:38:08.000000 hegel-0.0.3/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 15:38:48.000000 hegel-0.0.3/version.txt
```

### Comparing `hegel-0.0.2/LICENSE` & `hegel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hegel-0.0.2/PKG-INFO` & `hegel-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hegel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Supercharge your LLM with a frictionless wrapper
 Home-page: https://github.com/hegelai/hegel
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/hegel
 Project-URL: Bug Tracker, https://github.com/hegelai/hegel
```

### Comparing `hegel-0.0.2/README.md` & `hegel-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hegel-0.0.2/hegel/scribe.py` & `hegel-0.0.3/hegel/scribe.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Callable, Optional, Dict
 from time import perf_counter
 import requests
 import uuid
 from enum import Enum
 from dotenv import load_dotenv
 import logging
-from utils import set_environment, get_current_time_millis, get_present_date
+from hegel.utils import set_environment, get_current_time_millis, get_present_date
 
 # Load environmental variables from `.env` file
 load_dotenv()
 set_environment()
 
 
 class TaskTypes(Enum):
```

### Comparing `hegel-0.0.2/hegel/utils.py` & `hegel-0.0.3/hegel/utils.py`

 * *Files identical despite different names*

### Comparing `hegel-0.0.2/hegel.egg-info/PKG-INFO` & `hegel-0.0.3/hegel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hegel
-Version: 0.0.2
+Version: 0.0.3
 Summary: Supercharge your LLM with a frictionless wrapper
 Home-page: https://github.com/hegelai/hegel
 Author: Hegel AI
 Author-email: Hegel AI <team@hegel-ai.com>
 License: Proprietary
 Project-URL: Homepage, https://github.com/hegelai/hegel
 Project-URL: Bug Tracker, https://github.com/hegelai/hegel
```

### Comparing `hegel-0.0.2/pyproject.toml` & `hegel-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hegel"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Hegel AI", email="team@hegel-ai.com" },
 ]
 description = "Supercharge your LLM with a frictionless wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,8 +20,8 @@
 dynamic = ["dependencies"]
 
 [project.urls]
 "Homepage" = "https://github.com/hegelai/hegel"
 "Bug Tracker" = "https://github.com/hegelai/hegel"
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt", "version.txt"]}
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `hegel-0.0.2/setup.py` & `hegel-0.0.3/setup.py`

 * *Files identical despite different names*

