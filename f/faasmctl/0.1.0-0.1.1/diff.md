# Comparing `tmp/faasmctl-0.1.0.tar.gz` & `tmp/faasmctl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.1.0.tar", last modified: Fri Jun 30 17:20:06 2023, max compression
+gzip compressed data, was "faasmctl-0.1.1.tar", last modified: Thu Jul  6 16:40:22 2023, max compression
```

## Comparing `faasmctl-0.1.0.tar` & `faasmctl-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:20:06.428774 faasmctl-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:19:57.000000 faasmctl-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 17:20:06.428774 faasmctl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-30 17:19:57.000000 faasmctl-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:20:06.428774 faasmctl-0.1.0/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:20:06.428774 faasmctl-0.1.0/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/tasks/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:20:06.428774 faasmctl-0.1.0/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-30 17:19:57.000000 faasmctl-0.1.0/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:20:06.428774 faasmctl-0.1.0/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-30 17:20:06.000000 faasmctl-0.1.0/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-30 17:19:57.000000 faasmctl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:20:06.428774 faasmctl-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 16:40:11.000000 faasmctl-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 16:40:22.349045 faasmctl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 16:40:11.000000 faasmctl-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/tasks/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 16:40:11.000000 faasmctl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:40:22.349045 faasmctl-0.1.1/setup.cfg
```

### Comparing `faasmctl-0.1.0/LICENSE.md` & `faasmctl-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.1.0/PKG-INFO` & `faasmctl-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.0
+pip install faasmctl==0.1.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.0/README.md` & `faasmctl-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.0
+pip install faasmctl==0.1.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.0/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.1.1/faasmctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small example package
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.0
+pip install faasmctl==0.1.1
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.0/pyproject.toml` & `faasmctl-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

