# Comparing `tmp/mlserver-alibi-explain-1.4.0.dev2.tar.gz` & `tmp/mlserver_alibi_explain-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-alibi-explain-1.4.0.dev2.tar", last modified: Thu May  4 09:30:33 2023, max compression
+gzip compressed data, was "mlserver_alibi_explain-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-alibi-explain-1.4.0.dev2.tar` & `mlserver_alibi_explain-1.4.0.dev3.tar`

### file list

```diff
@@ -1,24 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.207432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/alibi_dependency_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/black_box_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/white_box_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:33.207432 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-04 09:30:33.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 09:30:32.000000 mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:33.211432 mlserver-alibi-explain-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-04 09:29:57.000000 mlserver-alibi-explain-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0      233 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       76 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/__init__.py
+-rw-r--r--   0        0        0     2778 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/alibi_dependency_reference.py
+-rw-r--r--   0        0        0     5296 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/common.py
+-rw-r--r--   0        0        0      462 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/errors.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/__init__.py
+-rw-r--r--   0        0        0     4277 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/black_box_runtime.py
+-rw-r--r--   0        0        0     1010 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/integrated_gradients.py
+-rw-r--r--   0        0        0     1745 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/white_box_runtime.py
+-rw-r--r--   0        0        0     5934 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/runtime.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/version.py
+-rw-r--r--   0        0        0      654 2023-07-05 11:14:01.021094 mlserver_alibi_explain-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 mlserver_alibi_explain-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-alibi-explain-1.4.0.dev2/LICENSE` & `mlserver_alibi_explain-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/alibi_dependency_reference.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/alibi_dependency_reference.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/common.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/common.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/black_box_runtime.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/black_box_runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/integrated_gradients.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/explainers/white_box_runtime.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/explainers/white_box_runtime.py`

 * *Files identical despite different names*

### Comparing `mlserver-alibi-explain-1.4.0.dev2/mlserver_alibi_explain/runtime.py` & `mlserver_alibi_explain-1.4.0.dev3/mlserver_alibi_explain/runtime.py`

 * *Files identical despite different names*

