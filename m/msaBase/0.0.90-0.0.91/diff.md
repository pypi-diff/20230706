# Comparing `tmp/msaBase-0.0.90.tar.gz` & `tmp/msaBase-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msaBase-0.0.90.tar", last modified: Wed Jul  5 17:52:11 2023, max compression
+gzip compressed data, was "msaBase-0.0.91.tar", last modified: Wed Jul  5 19:00:40 2023, max compression
```

## Comparing `msaBase-0.0.90.tar` & `msaBase-0.0.91.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 17:52:11.784714 msaBase-0.0.90/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     1094 2023-03-17 10:16:02.000000 msaBase-0.0.90/LICENCE
--rw-rw-r--   0 eduard    (1000) eduard    (1000)       58 2023-03-17 10:16:02.000000 msaBase-0.0.90/MANIFEST.in
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     4135 2023-07-05 17:52:11.780714 msaBase-0.0.90/PKG-INFO
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2689 2023-03-17 10:16:02.000000 msaBase-0.0.90/README.md
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 17:52:11.776714 msaBase-0.0.90/msaBase/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      472 2023-07-05 17:48:43.000000 msaBase-0.0.90/msaBase/__init__.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     8143 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/config.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)    37124 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/configurate.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2116 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/errorhandling.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2930 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/helpers.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     3720 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/logger.py
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 17:52:11.780714 msaBase-0.0.90/msaBase/models/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      211 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/models/__init__.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      948 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/models/functionality.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     1414 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/models/middlewares.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      381 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/models/settings.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)    14964 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/models/sysinfo.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     4785 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/profiler.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)    14841 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/sysinfo.py
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 17:52:11.780714 msaBase-0.0.90/msaBase/utils/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        0 2023-03-17 10:16:02.000000 msaBase-0.0.90/msaBase/utils/__init__.py
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      487 2023-06-22 08:27:08.000000 msaBase-0.0.90/msaBase/utils/constants.py
-drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 17:52:11.776714 msaBase-0.0.90/msaBase.egg-info/
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     4135 2023-07-05 17:52:11.000000 msaBase-0.0.90/msaBase.egg-info/PKG-INFO
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      592 2023-07-05 17:52:11.000000 msaBase-0.0.90/msaBase.egg-info/SOURCES.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-07-05 17:52:11.000000 msaBase-0.0.90/msaBase.egg-info/dependency_links.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)      808 2023-07-05 17:52:11.000000 msaBase-0.0.90/msaBase.egg-info/requires.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        8 2023-07-05 17:52:11.000000 msaBase-0.0.90/msaBase.egg-info/top_level.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-06-22 08:41:45.000000 msaBase-0.0.90/msaBase.egg-info/zip-safe
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     3878 2023-07-05 17:48:17.000000 msaBase-0.0.90/requirements.txt
--rw-rw-r--   0 eduard    (1000) eduard    (1000)       38 2023-07-05 17:52:11.784714 msaBase-0.0.90/setup.cfg
--rw-rw-r--   0 eduard    (1000) eduard    (1000)     2312 2023-03-17 10:16:02.000000 msaBase-0.0.90/setup.py
+drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 19:00:40.123278 msaBase-0.0.91/
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     1094 2023-03-17 10:16:02.000000 msaBase-0.0.91/LICENCE
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)       58 2023-03-17 10:16:02.000000 msaBase-0.0.91/MANIFEST.in
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     4135 2023-07-05 19:00:40.123278 msaBase-0.0.91/PKG-INFO
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     2689 2023-03-17 10:16:02.000000 msaBase-0.0.91/README.md
+drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 19:00:40.123278 msaBase-0.0.91/msaBase/
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      472 2023-07-05 18:55:16.000000 msaBase-0.0.91/msaBase/__init__.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     8143 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/config.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)    37124 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/configurate.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     2116 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/errorhandling.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     2930 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/helpers.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     3720 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/logger.py
+drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 19:00:40.123278 msaBase-0.0.91/msaBase/models/
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      211 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/models/__init__.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      948 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/models/functionality.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     1414 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/models/middlewares.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      381 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/models/settings.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)    14964 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/models/sysinfo.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     4785 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/profiler.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)    14841 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/sysinfo.py
+drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 19:00:40.123278 msaBase-0.0.91/msaBase/utils/
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)        0 2023-03-17 10:16:02.000000 msaBase-0.0.91/msaBase/utils/__init__.py
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      487 2023-06-22 08:27:08.000000 msaBase-0.0.91/msaBase/utils/constants.py
+drwxrwxr-x   0 eduard    (1000) eduard    (1000)        0 2023-07-05 19:00:40.123278 msaBase-0.0.91/msaBase.egg-info/
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     4135 2023-07-05 19:00:40.000000 msaBase-0.0.91/msaBase.egg-info/PKG-INFO
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      592 2023-07-05 19:00:40.000000 msaBase-0.0.91/msaBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-07-05 19:00:40.000000 msaBase-0.0.91/msaBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)      808 2023-07-05 19:00:40.000000 msaBase-0.0.91/msaBase.egg-info/requires.txt
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)        8 2023-07-05 19:00:40.000000 msaBase-0.0.91/msaBase.egg-info/top_level.txt
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)        1 2023-06-22 08:41:45.000000 msaBase-0.0.91/msaBase.egg-info/zip-safe
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     3878 2023-07-05 18:55:19.000000 msaBase-0.0.91/requirements.txt
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)       38 2023-07-05 19:00:40.123278 msaBase-0.0.91/setup.cfg
+-rw-rw-r--   0 eduard    (1000) eduard    (1000)     2312 2023-03-17 10:16:02.000000 msaBase-0.0.91/setup.py
```

### Comparing `msaBase-0.0.90/LICENCE` & `msaBase-0.0.91/LICENCE`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/PKG-INFO` & `msaBase-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaBase
-Version: 0.0.90
+Version: 0.0.91
 Summary: msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, Healtcheck, Error Handling etc.
 Home-page: https://github.com/u2d-ai/msaBase
 Download-URL: http://pypi.python.org/pypi/msaBase
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaBase.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaBase Version: 0.0.90 Summary: msaBase - General
+Metadata-Version: 2.1 Name: msaBase Version: 0.0.91 Summary: msaBase - General
 package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo,
 Healtcheck, Error Handling etc. Home-page: https://github.com/u2d-ai/msaBase
 Download-URL: http://pypi.python.org/pypi/msaBase Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaBase.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/msaBase Project-
 URL: Tracker, https://github.com/u2d-ai/msaBase/issues Classifier: Development
 Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier: Intended
```

### Comparing `msaBase-0.0.90/README.md` & `msaBase-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/config.py` & `msaBase-0.0.91/msaBase/config.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/configurate.py` & `msaBase-0.0.91/msaBase/configurate.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/errorhandling.py` & `msaBase-0.0.91/msaBase/errorhandling.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/helpers.py` & `msaBase-0.0.91/msaBase/helpers.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/logger.py` & `msaBase-0.0.91/msaBase/logger.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/models/functionality.py` & `msaBase-0.0.91/msaBase/models/functionality.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/models/middlewares.py` & `msaBase-0.0.91/msaBase/models/middlewares.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/models/sysinfo.py` & `msaBase-0.0.91/msaBase/models/sysinfo.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/profiler.py` & `msaBase-0.0.91/msaBase/profiler.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase/sysinfo.py` & `msaBase-0.0.91/msaBase/sysinfo.py`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase.egg-info/PKG-INFO` & `msaBase-0.0.91/msaBase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msaBase
-Version: 0.0.90
+Version: 0.0.91
 Summary: msaBase - General package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo, Healtcheck, Error Handling etc.
 Home-page: https://github.com/u2d-ai/msaBase
 Download-URL: http://pypi.python.org/pypi/msaBase
 Author: Stefan Welcker
 Author-email: stefan@u2d.ai
 License: MIT
 Project-URL: Documentation, http://msaBase.u2d.ai/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: msaBase Version: 0.0.90 Summary: msaBase - General
+Metadata-Version: 2.1 Name: msaBase Version: 0.0.91 Summary: msaBase - General
 package for Microservices based on FastAPI like Profiler, Scheduler, Sysinfo,
 Healtcheck, Error Handling etc. Home-page: https://github.com/u2d-ai/msaBase
 Download-URL: http://pypi.python.org/pypi/msaBase Author: Stefan Welcker
 Author-email: stefan@u2d.ai License: MIT Project-URL: Documentation, http://
 msaBase.u2d.ai/ Project-URL: Source, https://github.com/u2d-ai/msaBase Project-
 URL: Tracker, https://github.com/u2d-ai/msaBase/issues Classifier: Development
 Status :: 4 - Beta Classifier: Framework :: FastAPI Classifier: Intended
```

### Comparing `msaBase-0.0.90/msaBase.egg-info/SOURCES.txt` & `msaBase-0.0.91/msaBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msaBase-0.0.90/msaBase.egg-info/requires.txt` & `msaBase-0.0.91/msaBase.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 msaFileSystem==0.0.3
-msaDocModels==0.0.81
+msaDocModels==0.0.82
 fastapi[all]==0.86.0
 fastapi_utils==0.2.1
 pydantic[dotenv,email]==1.9.2
 pyinstrument==4.4.0
 autoflake==2.0.1
 black==22.6.0
 pyproject-flake8==6.0.0
```

### Comparing `msaBase-0.0.90/requirements.txt` & `msaBase-0.0.91/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MSA Dependencies
 msaFileSystem==0.0.3 # Agnostic Abstract Filesystem API which allows to use S3, GCS, Azure Datalake, your local FS, Youtube etc Optimized for use with FastAPI/Pydantic.
-msaDocModels==0.0.81 # MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
+msaDocModels==0.0.82 # MSA Document Pydantic Models and Schemas, used to store Parser, NLP, NLU and AI results for processed documents
 
 # FastAPI related Dependencies
 fastapi[all]==0.86.0 # FastAPI framework, high performance, easy to learn, fast to code, ready for production
 fastapi_utils==0.2.1 # Reusable utilities for FastAPI, Repeated Tasks, APIModel, APISettings
 pydantic[email,dotenv]==1.9.2 # Data validation and settings management using python type hints
 pyinstrument==4.4.0 # pyinstrument to check service performance.
```

### Comparing `msaBase-0.0.90/setup.py` & `msaBase-0.0.91/setup.py`

 * *Files identical despite different names*

