# Comparing `tmp/atomlite-1.3.0.tar.gz` & `tmp/atomlite-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-1.3.0.tar", last modified: Thu Jun 29 14:56:20 2023, max compression
+gzip compressed data, was "atomlite-1.3.1.tar", last modified: Thu Jul  6 10:37:48 2023, max compression
```

## Comparing `atomlite-1.3.0.tar` & `atomlite-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-06-29 14:56:20.944223 atomlite-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1230 2023-06-29 14:56:08.000000 atomlite-1.3.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1156 2023-06-29 14:56:08.000000 atomlite-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:56:20.944223 atomlite-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite/
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite/_internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11418 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/database.py
--rw-r--r--   0 root         (0) root         (0)     5639 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/json.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      375 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)    10139 2023-06-29 14:56:08.000000 atomlite-1.3.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 10:37:05.000000 atomlite-1.3.1/.github/workflows/publish_release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-06 10:37:05.000000 atomlite-1.3.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 10:37:05.000000 atomlite-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 10:37:05.000000 atomlite-1.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-06 10:37:48.787756 atomlite-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 10:37:05.000000 atomlite-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/docker_testing_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 10:37:05.000000 atomlite-1.3.1/docker_testing_environment/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_static/empty
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 10:37:05.000000 atomlite-1.3.1/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-06 10:37:05.000000 atomlite-1.3.1/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-06 10:37:05.000000 atomlite-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:37:48.787756 atomlite-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.783756 atomlite-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/_internal/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:05.000000 atomlite-1.3.1/src/atomlite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/src/atomlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 10:37:48.000000 atomlite-1.3.1/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:37:48.787756 atomlite-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-06 10:37:05.000000 atomlite-1.3.1/tests/test_database.py
```

### Comparing `atomlite-1.3.0/PKG-INFO` & `atomlite-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.0
+Version: 1.3.1
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.0/README.rst` & `atomlite-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.0/pyproject.toml` & `atomlite-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.0/src/atomlite/_internal/database.py` & `atomlite-1.3.1/src/atomlite/_internal/database.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.0/src/atomlite/_internal/json.py` & `atomlite-1.3.1/src/atomlite/_internal/json.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.3.0/src/atomlite.egg-info/PKG-INFO` & `atomlite-1.3.1/src/atomlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.3.0
+Version: 1.3.1
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.3.0/tests/test_database.py` & `atomlite-1.3.1/tests/test_database.py`

 * *Files identical despite different names*

