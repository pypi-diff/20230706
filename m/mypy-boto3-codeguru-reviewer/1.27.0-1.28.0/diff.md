# Comparing `tmp/mypy-boto3-codeguru-reviewer-1.27.0.tar.gz` & `tmp/mypy-boto3-codeguru-reviewer-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.27.0.tar", last modified: Mon Jul  3 19:50:32 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.0.tar", last modified: Thu Jul  6 20:59:14 2023, max compression
```

## Comparing `mypy-boto3-codeguru-reviewer-1.27.0.tar` & `mypy-boto3-codeguru-reviewer-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.122991 mypy-boto3-codeguru-reviewer-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-03 19:34:22.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:32.114991 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:31.000000 mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:32.122991 mypy-boto3-codeguru-reviewer-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-03 19:34:21.000000 mypy-boto3-codeguru-reviewer-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.014254 mypy-boto3-codeguru-reviewer-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-06 20:59:14.010254 mypy-boto3-codeguru-reviewer-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.002254 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.010254 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:14.014254 mypy-boto3-codeguru-reviewer-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/setup.py
```

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/LICENSE` & `mypy-boto3-codeguru-reviewer-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.27.0
-Summary: Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/README.md` & `mypy-boto3-codeguru-reviewer-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/__init__.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/client.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/literals.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/paginator.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/type_defs.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.py` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer/waiter.pyi` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.27.0
-Summary: Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.27.0/setup.py` & `mypy-boto3-codeguru-reviewer-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-reviewer",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruReviewer 1.27.0 service generated with"
+        "Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

