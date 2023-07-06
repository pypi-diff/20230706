# Comparing `tmp/motion_python-0.1.71.tar.gz` & `tmp/motion_python-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.71.tar", max compression
+gzip compressed data, was "motion_python-0.1.72.tar", max compression
```

## Comparing `motion_python-0.1.71.tar` & `motion_python-0.1.72.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3344 2023-07-06 18:29:22.418477 motion_python-0.1.71/README.md
--rw-r--r--   0        0        0      338 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/cli.py
--rw-r--r--   0        0        0    22752 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/component.py
--rw-r--r--   0        0        0    17241 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/execute.py
--rw-r--r--   0        0        0    13742 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/instance.py
--rw-r--r--   0        0        0     4889 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1125 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/route.py
--rw-r--r--   0        0        0     5890 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/server/fit_task.py
--rw-r--r--   0        0        0     9333 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-06 18:29:45.570838 motion_python-0.1.71/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.71/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-06 18:38:18.732894 motion_python-0.1.72/README.md
+-rw-r--r--   0        0        0      338 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/cli.py
+-rw-r--r--   0        0        0    22752 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/component.py
+-rw-r--r--   0        0        0    17241 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/execute.py
+-rw-r--r--   0        0        0    13742 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/instance.py
+-rw-r--r--   0        0        0     4889 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1125 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/route.py
+-rw-r--r--   0        0        0     5890 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/server/fit_task.py
+-rw-r--r--   0        0        0     9333 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-06 18:38:38.128875 motion_python-0.1.72/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.72/PKG-INFO
```

### Comparing `motion_python-0.1.71/README.md` & `motion_python-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/cli.py` & `motion_python-0.1.72/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/component.py` & `motion_python-0.1.72/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/execute.py` & `motion_python-0.1.72/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/instance.py` & `motion_python-0.1.72/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/migrate.py` & `motion_python-0.1.72/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.72/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/route.py` & `motion_python-0.1.72/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/server/fit_task.py` & `motion_python-0.1.72/motion/server/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/motion/utils.py` & `motion_python-0.1.72/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.71/pyproject.toml` & `motion_python-0.1.72/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.71"
+version = "0.1.72"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.71/PKG-INFO` & `motion_python-0.1.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.71
+Version: 0.1.72
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

