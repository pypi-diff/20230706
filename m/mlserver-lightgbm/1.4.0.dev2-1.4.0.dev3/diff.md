# Comparing `tmp/mlserver-lightgbm-1.4.0.dev2.tar.gz` & `tmp/mlserver_lightgbm-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-lightgbm-1.4.0.dev2.tar", last modified: Thu May  4 09:30:40 2023, max compression
+gzip compressed data, was "mlserver_lightgbm-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-lightgbm-1.4.0.dev2.tar` & `mlserver_lightgbm-1.4.0.dev3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.241904 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 09:30:40.000000 mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:30:40.245904 mlserver-lightgbm-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-04 09:30:00.000000 mlserver-lightgbm-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0      752 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0       65 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/mlserver_lightgbm/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/mlserver_lightgbm/lightgbm.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/mlserver_lightgbm/version.py
+-rw-r--r--   0        0        0      518 2023-07-05 11:14:04.248400 mlserver_lightgbm-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     1346 1970-01-01 00:00:00.000000 mlserver_lightgbm-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-lightgbm-1.4.0.dev2/LICENSE` & `mlserver_lightgbm-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.4.0.dev2/README.md` & `mlserver_lightgbm-1.4.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-lightgbm-1.4.0.dev2/mlserver_lightgbm/lightgbm.py` & `mlserver_lightgbm-1.4.0.dev3/mlserver_lightgbm/lightgbm.py`

 * *Files identical despite different names*

