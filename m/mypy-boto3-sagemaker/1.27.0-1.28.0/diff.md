# Comparing `tmp/mypy-boto3-sagemaker-1.27.0.tar.gz` & `tmp/mypy-boto3-sagemaker-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-1.27.0.tar", last modified: Mon Jul  3 19:51:24 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-1.28.0.tar", last modified: Thu Jul  6 21:00:33 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-1.27.0.tar` & `mypy-boto3-sagemaker-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.539947 mypy-boto3-sagemaker-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-03 19:51:24.527947 mypy-boto3-sagemaker-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    79242 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.527947 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   262100 2023-07-03 19:47:07.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   261710 2023-07-03 19:47:06.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57365 2023-07-03 19:47:09.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    57363 2023-07-03 19:47:08.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    97555 2023-07-03 19:47:08.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    97484 2023-07-03 19:47:07.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   495915 2023-07-03 19:47:23.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   495286 2023-07-03 19:47:16.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:05.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-03 19:47:08.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-03 19:47:08.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:24.527947 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:51:24.000000 mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:24.539947 mypy-boto3-sagemaker-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:47:04.000000 mypy-boto3-sagemaker-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    79242 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.038422 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18512 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262100 2023-07-06 20:54:24.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   261710 2023-07-06 20:54:23.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57365 2023-07-06 20:54:27.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57363 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    97555 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97484 2023-07-06 20:54:25.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   495915 2023-07-06 20:54:47.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   495286 2023-07-06 20:54:37.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:18.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-06 20:54:26.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    80735 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:33.054422 mypy-boto3-sagemaker-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:54:17.000000 mypy-boto3-sagemaker-1.28.0/setup.py
```

### Comparing `mypy-boto3-sagemaker-1.27.0/LICENSE` & `mypy-boto3-sagemaker-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/PKG-INFO` & `mypy-boto3-sagemaker-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.27.0
-Summary: Type annotations for boto3.SageMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sagemaker-1.27.0/README.md` & `mypy-boto3-sagemaker-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__init__.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__init__.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/__main__.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMaker 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.SageMaker 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.27.0")
+    print("1.28.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/client.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/client.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/literals.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/literals.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/paginator.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/paginator.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/type_defs.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/type_defs.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/waiter.py` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker/waiter.pyi` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker
-Version: 1.27.0
-Summary: Type annotations for boto3.SageMaker 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMaker 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[boto3.SageMaker 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sagemaker-1.27.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-1.28.0/mypy_boto3_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-1.27.0/setup.py` & `mypy-boto3-sagemaker-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMaker 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.SageMaker 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

