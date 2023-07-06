# Comparing `tmp/mypy-boto3-iam-1.27.0.tar.gz` & `tmp/mypy-boto3-iam-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iam-1.27.0.tar", last modified: Mon Jul  3 19:50:51 2023, max compression
+gzip compressed data, was "mypy-boto3-iam-1.28.0.tar", last modified: Thu Jul  6 20:59:43 2023, max compression
```

## Comparing `mypy-boto3-iam-1.27.0.tar` & `mypy-boto3-iam-1.28.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.491378 mypy-boto3-iam-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-03 19:50:51.487378 mypy-boto3-iam-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.471378 mypy-boto3-iam-1.27.0/mypy_boto3_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-03 19:38:58.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-03 19:38:58.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-03 19:38:58.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-03 19:38:57.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   141689 2023-07-03 19:38:57.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   141336 2023-07-03 19:38:56.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   146128 2023-07-03 19:39:02.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   145913 2023-07-03 19:38:59.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:55.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-03 19:38:58.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-03 19:38:58.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:51.487378 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:51.000000 mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:51.491378 mypy-boto3-iam-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:38:54.000000 mypy-boto3-iam-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/mypy_boto3_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-06 20:42:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-06 20:42:41.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-06 20:42:45.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-06 20:42:45.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   141689 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141336 2023-07-06 20:42:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   146128 2023-07-06 20:42:50.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145913 2023-07-06 20:42:48.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-06 20:42:44.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:43.000000 mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:43.474321 mypy-boto3-iam-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:42:40.000000 mypy-boto3-iam-1.28.0/setup.py
```

### Comparing `mypy-boto3-iam-1.27.0/LICENSE` & `mypy-boto3-iam-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/PKG-INFO` & `mypy-boto3-iam-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.27.0
-Summary: Type annotations for boto3.IAM 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iam-1.27.0/README.md` & `mypy-boto3-iam-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/__init__.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/__init__.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/__main__.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.IAM 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
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

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/client.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/client.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/literals.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/literals.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/paginator.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/paginator.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/service_resource.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/service_resource.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/type_defs.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/type_defs.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/waiter.py` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam/waiter.pyi` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/PKG-INFO` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.27.0
-Summary: Type annotations for boto3.IAM 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iam.svg?color=blue)](https://pypi.org/project/mypy-boto3-iam)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iam?color=blue)](https://pypistats.org/packages/mypy-boto3-iam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IAM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
+[boto3.IAM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iam-1.27.0/mypy_boto3_iam.egg-info/SOURCES.txt` & `mypy-boto3-iam-1.28.0/mypy_boto3_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.27.0/setup.py` & `mypy-boto3-iam-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iam",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IAM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

