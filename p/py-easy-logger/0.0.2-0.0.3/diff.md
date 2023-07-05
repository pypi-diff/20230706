# Comparing `tmp/py-easy-logger-0.0.2.tar.gz` & `tmp/py-easy-logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-easy-logger-0.0.2.tar", last modified: Tue Jul  4 18:47:23 2023, max compression
+gzip compressed data, was "py-easy-logger-0.0.3.tar", last modified: Wed Jul  5 22:34:57 2023, max compression
```

## Comparing `py-easy-logger-0.0.2.tar` & `py-easy-logger-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-04 18:47:23.579299 py-easy-logger-0.0.2/
--rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/LICENSE
--rw-r--r--   0 adamt      (501) staff       (20)    41163 2023-07-04 18:47:23.578503 py-easy-logger-0.0.2/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)      154 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-04 18:47:23.573244 py-easy-logger-0.0.2/py_easy_logger.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)    41163 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      409 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       49 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/top_level.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-04 18:47:23.000000 py-easy-logger-0.0.2/py_easy_logger.egg-info/zip-safe
--rw-rw-r--   0 adamt      (501) staff       (20)     1078 2023-07-04 18:47:09.000000 py-easy-logger-0.0.2/pyproject.toml
--rw-rw-r--   0 adamt      (501) staff       (20)       48 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/requirements.txt
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-07-04 18:47:23.579549 py-easy-logger-0.0.2/setup.cfg
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-04 18:47:23.567487 py-easy-logger-0.0.2/src/
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-04 18:47:23.577176 py-easy-logger-0.0.2/src/easy_logger/
--rw-rw-r--   0 adamt      (501) staff       (20)      129 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/src/easy_logger/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       47 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/src/easy_logger/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     5906 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/src/easy_logger/log_config.py
--rw-rw-r--   0 adamt      (501) staff       (20)      192 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/src/easy_logger/statics.py
--rw-rw-r--   0 adamt      (501) staff       (20)      712 2023-07-04 18:35:48.000000 py-easy-logger-0.0.2/src/easy_logger/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-05 22:34:57.608709 py-easy-logger-0.0.3/
+-rw-rw-r--   0 adamt      (501) staff       (20)    35129 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/LICENSE
+-rw-r--r--   0 adamt      (501) staff       (20)    41272 2023-07-05 22:34:57.607890 py-easy-logger-0.0.3/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)      270 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-05 22:34:57.601326 py-easy-logger-0.0.3/py_easy_logger.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    41272 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      439 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       49 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/top_level.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-05 22:34:57.000000 py-easy-logger-0.0.3/py_easy_logger.egg-info/zip-safe
+-rw-rw-r--   0 adamt      (501) staff       (20)     1070 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       48 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/requirements.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-07-05 22:34:57.608942 py-easy-logger-0.0.3/setup.cfg
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-05 22:34:57.595562 py-easy-logger-0.0.3/src/
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-05 22:34:57.606297 py-easy-logger-0.0.3/src/easy_logger/
+-rw-rw-r--   0 adamt      (501) staff       (20)      199 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       48 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     5907 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/log_config.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1213 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/log_format.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      192 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/statics.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      712 2023-07-05 22:15:03.000000 py-easy-logger-0.0.3/src/easy_logger/utils.py
```

### Comparing `py-easy-logger-0.0.2/LICENSE` & `py-easy-logger-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-easy-logger-0.0.2/PKG-INFO` & `py-easy-logger-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-easy-logger
-Version: 0.0.2
-Summary: Python Easy Logger
+Version: 0.0.3
+Summary: Easy Logger
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -686,7 +686,14 @@
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # easy-logger
 
 Simple Easy baseline Logger. Creates a color stream logger or a basic rotating logger that can be used and called on throughout a project.
+
+## Versions
+
+### v0.0.3
+
+* Added Splunk basic string log out format.
+* Added Splunk HEC JSON format for messaging.
```

### Comparing `py-easy-logger-0.0.2/py_easy_logger.egg-info/PKG-INFO` & `py-easy-logger-0.0.3/py_easy_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-easy-logger
-Version: 0.0.2
-Summary: Python Easy Logger
+Version: 0.0.3
+Summary: Easy Logger
 Author-email: atav928 <dev@tavnets.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -686,7 +686,14 @@
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # easy-logger
 
 Simple Easy baseline Logger. Creates a color stream logger or a basic rotating logger that can be used and called on throughout a project.
+
+## Versions
+
+### v0.0.3
+
+* Added Splunk basic string log out format.
+* Added Splunk HEC JSON format for messaging.
```

### Comparing `py-easy-logger-0.0.2/pyproject.toml` & `py-easy-logger-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 
 [project]
 name = "py-easy-logger"
 authors = [
     {name = "atav928", email = "dev@tavnets.com"}
 ]
-description = "Python Easy Logger"
+description = "Easy Logger"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE", content-type = "text"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -38,8 +38,8 @@
 #include = ["easy_logger"]
 #namespaces = true
 
 [tool.coverage.run]
 source = ["src"]
 
 [tool.pylint]
-max-line-length = 101
+max-line-length = 101
```

### Comparing `py-easy-logger-0.0.2/src/easy_logger/log_config.py` & `py-easy-logger-0.0.3/src/easy_logger/log_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 
 def with_suffix(logName) -> str:
     """Add suffix to logname."""
 
     return str(Path(logName).with_suffix('.log'))
 
+
 class RotatingLog:
     """Customized RotatigLogger.
 
     :return: _description_
     :rtype: _type_
     """
```

### Comparing `py-easy-logger-0.0.2/src/easy_logger/utils.py` & `py-easy-logger-0.0.3/src/easy_logger/utils.py`

 * *Files identical despite different names*

