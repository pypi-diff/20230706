# Comparing `tmp/faasmctl-0.1.1.tar.gz` & `tmp/faasmctl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.1.1.tar", last modified: Thu Jul  6 16:40:22 2023, max compression
+gzip compressed data, was "faasmctl-0.1.2.tar", last modified: Thu Jul  6 17:00:35 2023, max compression
```

## Comparing `faasmctl-0.1.1.tar` & `faasmctl-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 16:40:11.000000 faasmctl-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 16:40:22.349045 faasmctl-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 16:40:11.000000 faasmctl-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/tasks/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 16:40:11.000000 faasmctl-0.1.1/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:40:22.349045 faasmctl-0.1.1/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 16:40:22.000000 faasmctl-0.1.1/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 16:40:11.000000 faasmctl-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:40:22.349045 faasmctl-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-06 17:00:26.000000 faasmctl-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 17:00:35.455517 faasmctl-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 17:00:26.000000 faasmctl-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.451517 faasmctl-0.1.2/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/tasks/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 17:00:26.000000 faasmctl-0.1.2/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:00:35.455517 faasmctl-0.1.2/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 17:00:35.000000 faasmctl-0.1.2/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 17:00:26.000000 faasmctl-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:00:35.455517 faasmctl-0.1.2/setup.cfg
```

### Comparing `faasmctl-0.1.1/LICENSE.md` & `faasmctl-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.1.1/PKG-INFO` & `faasmctl-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.1
-Summary: A small example package
+Version: 0.1.2
+Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.1
+pip install faasmctl==0.1.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.1/README.md` & `faasmctl-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.1
+pip install faasmctl==0.1.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.1/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.1.2/faasmctl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.1.1
-Summary: A small example package
+Version: 0.1.2
+Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.1.1
+pip install faasmctl==0.1.2
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.1.1/pyproject.toml` & `faasmctl-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
-description = "A small example package"
+description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

