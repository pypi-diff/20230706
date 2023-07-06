# Comparing `tmp/robocorp_tasks-2.1.0.tar.gz` & `tmp/robocorp_tasks-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-2.1.0.tar", max compression
+gzip compressed data, was "robocorp_tasks-2.1.1.tar", max compression
```

## Comparing `robocorp_tasks-2.1.0.tar` & `robocorp_tasks-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5432 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/README.md
--rw-r--r--   0        0        0     1234 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1467 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5121 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    10273 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1122 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5080 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2160 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3943 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5489 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     2436 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_toml_settings.py
--rw-r--r--   0        0        0      869 2023-07-06 17:52:11.434171 robocorp_tasks-2.1.0/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-07-06 17:52:11.434171 robocorp_tasks-2.1.0/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     6209 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5432 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/README.md
+-rw-r--r--   0        0        0     1240 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1467 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10273 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5080 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2160 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3943 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     2436 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/_toml_settings.py
+-rw-r--r--   0        0        0      869 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-07-06 18:17:41.660042 robocorp_tasks-2.1.1/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     6211 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.1/PKG-INFO
```

### Comparing `robocorp_tasks-2.1.0/README.md` & `robocorp_tasks-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/pyproject.toml` & `robocorp_tasks-2.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "2.1.0"
+version = "2.1.1"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "^2"
+robocorp-log = ">=2.2,<3"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
```

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/__init__.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 
 from ._protocols import ITask
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_callback.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_commands.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_commands.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_config.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_task.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/_toml_settings.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/_toml_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/src/robocorp/tasks/cli.py` & `robocorp_tasks-2.1.1/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.1.0/PKG-INFO` & `robocorp_tasks-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 2.1.0
+Version: 2.1.1
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (>=2,<3)
+Requires-Dist: robocorp-log (>=2.2,<3)
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
```

