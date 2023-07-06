# Comparing `tmp/mlserver-sklearn-1.4.0.dev2.tar.gz` & `tmp/mlserver_sklearn-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-sklearn-1.4.0.dev2.tar", last modified: Thu May  4 09:30:47 2023, max compression
+gzip compressed data, was "mlserver_sklearn-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-sklearn-1.4.0.dev2.tar` & `mlserver_sklearn-1.4.0.dev3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:47.090384 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:47.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 09:30:46.000000 mlserver-sklearn-1.4.0.dev2/mlserver_sklearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:47.094384 mlserver-sklearn-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 09:30:02.000000 mlserver-sklearn-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0     2371 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       62 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/mlserver_sklearn/__init__.py
+-rw-r--r--   0        0        0     4491 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/mlserver_sklearn/sklearn.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/mlserver_sklearn/version.py
+-rw-r--r--   0        0        0      524 2023-07-05 11:14:10.829734 mlserver_sklearn-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 mlserver_sklearn-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-sklearn-1.4.0.dev2/LICENSE` & `mlserver_sklearn-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-sklearn-1.4.0.dev2/mlserver_sklearn/sklearn.py` & `mlserver_sklearn-1.4.0.dev3/mlserver_sklearn/sklearn.py`

 * *Files identical despite different names*

