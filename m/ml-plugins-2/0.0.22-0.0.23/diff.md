# Comparing `tmp/ml_plugins_2-0.0.22.tar.gz` & `tmp/ml_plugins_2-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_plugins_2-0.0.22.tar", last modified: Wed Jun 28 03:20:36 2023, max compression
+gzip compressed data, was "ml_plugins_2-0.0.23.tar", last modified: Thu Jul  6 02:00:12 2023, max compression
```

## Comparing `ml_plugins_2-0.0.22.tar` & `ml_plugins_2-0.0.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.468722 ml_plugins_2-0.0.22/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)       57 2023-06-28 03:20:36.468523 ml_plugins_2-0.0.22/PKG-INFO
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.464932 ml_plugins_2-0.0.22/examples/
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.465678 ml_plugins_2-0.0.22/examples/pip/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1751 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.22/examples/pip/extras_flow.py
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1975 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.22/examples/pip/pip_flow.py
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.465923 ml_plugins_2-0.0.22/examples/poetry/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1901 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.22/examples/poetry/poetry_flow.py
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     3857 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.22/examples/reference.py
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.466967 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)       57 2023-06-28 03:20:36.000000 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/PKG-INFO
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)      417 2023-06-28 03:20:36.000000 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/SOURCES.txt
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)        1 2023-06-28 03:20:36.000000 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/dependency_links.txt
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)       23 2023-06-28 03:20:36.000000 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/requires.txt
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)       22 2023-06-28 03:20:36.000000 ml_plugins_2-0.0.22/ml_plugins_2.egg-info/top_level.txt
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.467157 ml_plugins_2-0.0.22/plugins/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.22/plugins/__init__.py
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.467427 ml_plugins_2-0.0.22/plugins/pip/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.22/plugins/pip/__init__.py
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1390 2023-06-27 01:59:00.000000 ml_plugins_2-0.0.22/plugins/pip/plugin.py
-drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-06-28 03:20:36.467981 ml_plugins_2-0.0.22/plugins/poetry/
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.22/plugins/poetry/__init__.py
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1583 2023-06-28 03:16:38.000000 ml_plugins_2-0.0.22/plugins/poetry/plugin.py
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)      284 2023-06-28 03:20:27.000000 ml_plugins_2-0.0.22/pyproject.toml
--rw-r--r--   0 rikish.kamboj   (503) staff       (20)       38 2023-06-28 03:20:36.468774 ml_plugins_2-0.0.22/setup.cfg
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.948244 ml_plugins_2-0.0.23/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)       57 2023-07-06 02:00:12.948037 ml_plugins_2-0.0.23/PKG-INFO
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.944451 ml_plugins_2-0.0.23/examples/
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.945241 ml_plugins_2-0.0.23/examples/pip/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1751 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.23/examples/pip/extras_flow.py
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1975 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.23/examples/pip/pip_flow.py
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.945487 ml_plugins_2-0.0.23/examples/poetry/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1901 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.23/examples/poetry/poetry_flow.py
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     3857 2023-06-15 05:26:48.000000 ml_plugins_2-0.0.23/examples/reference.py
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.946406 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)       57 2023-07-06 02:00:12.000000 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/PKG-INFO
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)      417 2023-07-06 02:00:12.000000 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/SOURCES.txt
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)        1 2023-07-06 02:00:12.000000 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/dependency_links.txt
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)       23 2023-07-06 02:00:12.000000 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/requires.txt
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)       22 2023-07-06 02:00:12.000000 ml_plugins_2-0.0.23/ml_plugins_2.egg-info/top_level.txt
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.946547 ml_plugins_2-0.0.23/plugins/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.23/plugins/__init__.py
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.946862 ml_plugins_2-0.0.23/plugins/pip/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.23/plugins/pip/__init__.py
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1390 2023-06-27 01:59:00.000000 ml_plugins_2-0.0.23/plugins/pip/plugin.py
+drwxr-xr-x   0 rikish.kamboj   (503) staff       (20)        0 2023-07-06 02:00:12.947522 ml_plugins_2-0.0.23/plugins/poetry/
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)        0 2023-06-07 05:31:29.000000 ml_plugins_2-0.0.23/plugins/poetry/__init__.py
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)     1583 2023-06-28 03:16:38.000000 ml_plugins_2-0.0.23/plugins/poetry/plugin.py
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)      284 2023-07-06 01:59:44.000000 ml_plugins_2-0.0.23/pyproject.toml
+-rw-r--r--   0 rikish.kamboj   (503) staff       (20)       38 2023-07-06 02:00:12.948305 ml_plugins_2-0.0.23/setup.cfg
```

### Comparing `ml_plugins_2-0.0.22/examples/pip/extras_flow.py` & `ml_plugins_2-0.0.23/examples/pip/extras_flow.py`

 * *Files identical despite different names*

### Comparing `ml_plugins_2-0.0.22/examples/pip/pip_flow.py` & `ml_plugins_2-0.0.23/examples/pip/pip_flow.py`

 * *Files identical despite different names*

### Comparing `ml_plugins_2-0.0.22/examples/poetry/poetry_flow.py` & `ml_plugins_2-0.0.23/examples/poetry/poetry_flow.py`

 * *Files identical despite different names*

### Comparing `ml_plugins_2-0.0.22/examples/reference.py` & `ml_plugins_2-0.0.23/examples/reference.py`

 * *Files identical despite different names*

### Comparing `ml_plugins_2-0.0.22/plugins/pip/plugin.py` & `ml_plugins_2-0.0.23/plugins/pip/plugin.py`

 * *Files identical despite different names*

### Comparing `ml_plugins_2-0.0.22/plugins/poetry/plugin.py` & `ml_plugins_2-0.0.23/plugins/poetry/plugin.py`

 * *Files identical despite different names*

