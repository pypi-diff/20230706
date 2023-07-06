# Comparing `tmp/boto3-stubs-1.27.1.tar.gz` & `tmp/boto3-stubs-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-1.27.1.tar", last modified: Wed Jul  5 19:47:58 2023, max compression
+gzip compressed data, was "boto3-stubs-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
```

## Comparing `boto3-stubs-1.27.1.tar` & `boto3-stubs-1.28.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 19:46:53.000000 boto3-stubs-1.27.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    64299 2023-07-05 19:46:53.000000 boto3-stubs-1.27.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.740987 boto3-stubs-1.27.1/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)   188206 2023-07-05 19:47:02.000000 boto3-stubs-1.27.1/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.740987 boto3-stubs-1.27.1/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.740987 boto3-stubs-1.27.1/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.740987 boto3-stubs-1.27.1/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:02.000000 boto3-stubs-1.27.1/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   213622 2023-07-05 19:46:58.000000 boto3-stubs-1.27.1/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/boto3_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-05 19:47:58.000000 boto3-stubs-1.27.1/boto3_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:47:58.744987 boto3-stubs-1.27.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    46039 2023-07-05 19:46:52.000000 boto3-stubs-1.27.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.606220 boto3-stubs-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:13.000000 boto3-stubs-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-06 20:58:58.602220 boto3-stubs-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    64299 2023-07-06 20:32:13.000000 boto3-stubs-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.570220 boto3-stubs-1.28.0/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)   188206 2023-07-06 20:32:17.000000 boto3-stubs-1.28.0/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.578220 boto3-stubs-1.28.0/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.582220 boto3-stubs-1.28.0/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.582220 boto3-stubs-1.28.0/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:13.000000 boto3-stubs-1.28.0/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.598220 boto3-stubs-1.28.0/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.602220 boto3-stubs-1.28.0/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   213622 2023-07-06 20:32:23.000000 boto3-stubs-1.28.0/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-06 20:32:11.000000 boto3-stubs-1.28.0/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.602220 boto3-stubs-1.28.0/boto3_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    75725 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 20:58:58.000000 boto3-stubs-1.28.0/boto3_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.606220 boto3-stubs-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    46039 2023-07-06 20:32:12.000000 boto3-stubs-1.28.0/setup.py
```

### Comparing `boto3-stubs-1.27.1/LICENSE` & `boto3-stubs-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/PKG-INFO` & `boto3-stubs-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.27.1
-Summary: Type annotations for boto3 1.27.1 generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3 1.28.0 generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -391,15 +391,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/1.27.1/index.html)
+[boto3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/1.28.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-1.27.1/README.md` & `boto3-stubs-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/1.27.1/index.html)
+[boto3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/1.28.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-1.27.1/boto3-stubs/__init__.pyi` & `boto3-stubs-1.28.0/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/docs/utils.pyi` & `boto3-stubs-1.28.0/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/dynamodb/conditions.pyi` & `boto3-stubs-1.28.0/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/dynamodb/table.pyi` & `boto3-stubs-1.28.0/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/dynamodb/transform.pyi` & `boto3-stubs-1.28.0/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/dynamodb/types.pyi` & `boto3-stubs-1.28.0/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/exceptions.pyi` & `boto3-stubs-1.28.0/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/action.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/base.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/collection.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/model.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/params.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/resources/response.pyi` & `boto3-stubs-1.28.0/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/s3/inject.pyi` & `boto3-stubs-1.28.0/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/s3/transfer.pyi` & `boto3-stubs-1.28.0/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/session.pyi` & `boto3-stubs-1.28.0/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3-stubs/utils.pyi` & `boto3-stubs-1.28.0/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3_stubs.egg-info/PKG-INFO` & `boto3-stubs-1.28.0/boto3_stubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs
-Version: 1.27.1
-Summary: Type annotations for boto3 1.27.1 generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3 1.28.0 generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -391,15 +391,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/boto3-stubs.svg?color=blue)](https://pypi.org/project/boto3-stubs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/boto3-stubs?color=blue)](https://pypistats.org/packages/boto3-stubs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/1.27.1/index.html)
+[boto3 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/1.28.0/index.html)
 compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `boto3-stubs-1.27.1/boto3_stubs.egg-info/SOURCES.txt` & `boto3-stubs-1.28.0/boto3_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-1.27.1/boto3_stubs.egg-info/requires.txt` & `boto3-stubs-1.28.0/boto3_stubs.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,1420 +1,1420 @@
 botocore-stubs
 types-s3transfer
 
 [:python_version < "3.9"]
 typing-extensions>=4.1.0
 
 [accessanalyzer]
-mypy-boto3-accessanalyzer<1.28.0,>=1.27.0
+mypy-boto3-accessanalyzer<1.29.0,>=1.28.0
 
 [account]
-mypy-boto3-account<1.28.0,>=1.27.0
+mypy-boto3-account<1.29.0,>=1.28.0
 
 [acm]
-mypy-boto3-acm<1.28.0,>=1.27.0
+mypy-boto3-acm<1.29.0,>=1.28.0
 
 [acm-pca]
-mypy-boto3-acm-pca<1.28.0,>=1.27.0
+mypy-boto3-acm-pca<1.29.0,>=1.28.0
 
 [alexaforbusiness]
-mypy-boto3-alexaforbusiness<1.28.0,>=1.27.0
+mypy-boto3-alexaforbusiness<1.29.0,>=1.28.0
 
 [all]
-mypy-boto3-accessanalyzer<1.28.0,>=1.27.0
-mypy-boto3-account<1.28.0,>=1.27.0
-mypy-boto3-acm<1.28.0,>=1.27.0
-mypy-boto3-acm-pca<1.28.0,>=1.27.0
-mypy-boto3-alexaforbusiness<1.28.0,>=1.27.0
-mypy-boto3-amp<1.28.0,>=1.27.0
-mypy-boto3-amplify<1.28.0,>=1.27.0
-mypy-boto3-amplifybackend<1.28.0,>=1.27.0
-mypy-boto3-amplifyuibuilder<1.28.0,>=1.27.0
-mypy-boto3-apigateway<1.28.0,>=1.27.0
-mypy-boto3-apigatewaymanagementapi<1.28.0,>=1.27.0
-mypy-boto3-apigatewayv2<1.28.0,>=1.27.0
-mypy-boto3-appconfig<1.28.0,>=1.27.0
-mypy-boto3-appconfigdata<1.28.0,>=1.27.0
-mypy-boto3-appfabric<1.28.0,>=1.27.0
-mypy-boto3-appflow<1.28.0,>=1.27.0
-mypy-boto3-appintegrations<1.28.0,>=1.27.0
-mypy-boto3-application-autoscaling<1.28.0,>=1.27.0
-mypy-boto3-application-insights<1.28.0,>=1.27.0
-mypy-boto3-applicationcostprofiler<1.28.0,>=1.27.0
-mypy-boto3-appmesh<1.28.0,>=1.27.0
-mypy-boto3-apprunner<1.28.0,>=1.27.0
-mypy-boto3-appstream<1.28.0,>=1.27.0
-mypy-boto3-appsync<1.28.0,>=1.27.0
-mypy-boto3-arc-zonal-shift<1.28.0,>=1.27.0
-mypy-boto3-athena<1.28.0,>=1.27.0
-mypy-boto3-auditmanager<1.28.0,>=1.27.0
-mypy-boto3-autoscaling<1.28.0,>=1.27.0
-mypy-boto3-autoscaling-plans<1.28.0,>=1.27.0
-mypy-boto3-backup<1.28.0,>=1.27.0
-mypy-boto3-backup-gateway<1.28.0,>=1.27.0
-mypy-boto3-backupstorage<1.28.0,>=1.27.0
-mypy-boto3-batch<1.28.0,>=1.27.0
-mypy-boto3-billingconductor<1.28.0,>=1.27.0
-mypy-boto3-braket<1.28.0,>=1.27.0
-mypy-boto3-budgets<1.28.0,>=1.27.0
-mypy-boto3-ce<1.28.0,>=1.27.0
-mypy-boto3-chime<1.28.0,>=1.27.0
-mypy-boto3-chime-sdk-identity<1.28.0,>=1.27.0
-mypy-boto3-chime-sdk-media-pipelines<1.28.0,>=1.27.0
-mypy-boto3-chime-sdk-meetings<1.28.0,>=1.27.0
-mypy-boto3-chime-sdk-messaging<1.28.0,>=1.27.0
-mypy-boto3-chime-sdk-voice<1.28.0,>=1.27.0
-mypy-boto3-cleanrooms<1.28.0,>=1.27.0
-mypy-boto3-cloud9<1.28.0,>=1.27.0
-mypy-boto3-cloudcontrol<1.28.0,>=1.27.0
-mypy-boto3-clouddirectory<1.28.0,>=1.27.0
-mypy-boto3-cloudformation<1.28.0,>=1.27.0
-mypy-boto3-cloudfront<1.28.0,>=1.27.0
-mypy-boto3-cloudhsm<1.28.0,>=1.27.0
-mypy-boto3-cloudhsmv2<1.28.0,>=1.27.0
-mypy-boto3-cloudsearch<1.28.0,>=1.27.0
-mypy-boto3-cloudsearchdomain<1.28.0,>=1.27.0
-mypy-boto3-cloudtrail<1.28.0,>=1.27.0
-mypy-boto3-cloudtrail-data<1.28.0,>=1.27.0
-mypy-boto3-cloudwatch<1.28.0,>=1.27.0
-mypy-boto3-codeartifact<1.28.0,>=1.27.0
-mypy-boto3-codebuild<1.28.0,>=1.27.0
-mypy-boto3-codecatalyst<1.28.0,>=1.27.0
-mypy-boto3-codecommit<1.28.0,>=1.27.0
-mypy-boto3-codedeploy<1.28.0,>=1.27.0
-mypy-boto3-codeguru-reviewer<1.28.0,>=1.27.0
-mypy-boto3-codeguru-security<1.28.0,>=1.27.0
-mypy-boto3-codeguruprofiler<1.28.0,>=1.27.0
-mypy-boto3-codepipeline<1.28.0,>=1.27.0
-mypy-boto3-codestar<1.28.0,>=1.27.0
-mypy-boto3-codestar-connections<1.28.0,>=1.27.0
-mypy-boto3-codestar-notifications<1.28.0,>=1.27.0
-mypy-boto3-cognito-identity<1.28.0,>=1.27.0
-mypy-boto3-cognito-idp<1.28.0,>=1.27.0
-mypy-boto3-cognito-sync<1.28.0,>=1.27.0
-mypy-boto3-comprehend<1.28.0,>=1.27.0
-mypy-boto3-comprehendmedical<1.28.0,>=1.27.0
-mypy-boto3-compute-optimizer<1.28.0,>=1.27.0
-mypy-boto3-config<1.28.0,>=1.27.0
-mypy-boto3-connect<1.28.0,>=1.27.0
-mypy-boto3-connect-contact-lens<1.28.0,>=1.27.0
-mypy-boto3-connectcampaigns<1.28.0,>=1.27.0
-mypy-boto3-connectcases<1.28.0,>=1.27.0
-mypy-boto3-connectparticipant<1.28.0,>=1.27.0
-mypy-boto3-controltower<1.28.0,>=1.27.0
-mypy-boto3-cur<1.28.0,>=1.27.0
-mypy-boto3-customer-profiles<1.28.0,>=1.27.0
-mypy-boto3-databrew<1.28.0,>=1.27.0
-mypy-boto3-dataexchange<1.28.0,>=1.27.0
-mypy-boto3-datapipeline<1.28.0,>=1.27.0
-mypy-boto3-datasync<1.28.0,>=1.27.0
-mypy-boto3-dax<1.28.0,>=1.27.0
-mypy-boto3-detective<1.28.0,>=1.27.0
-mypy-boto3-devicefarm<1.28.0,>=1.27.0
-mypy-boto3-devops-guru<1.28.0,>=1.27.0
-mypy-boto3-directconnect<1.28.0,>=1.27.0
-mypy-boto3-discovery<1.28.0,>=1.27.0
-mypy-boto3-dlm<1.28.0,>=1.27.0
-mypy-boto3-dms<1.28.0,>=1.27.0
-mypy-boto3-docdb<1.28.0,>=1.27.0
-mypy-boto3-docdb-elastic<1.28.0,>=1.27.0
-mypy-boto3-drs<1.28.0,>=1.27.0
-mypy-boto3-ds<1.28.0,>=1.27.0
-mypy-boto3-dynamodb<1.28.0,>=1.27.0
-mypy-boto3-dynamodbstreams<1.28.0,>=1.27.0
-mypy-boto3-ebs<1.28.0,>=1.27.0
-mypy-boto3-ec2<1.28.0,>=1.27.0
-mypy-boto3-ec2-instance-connect<1.28.0,>=1.27.0
-mypy-boto3-ecr<1.28.0,>=1.27.0
-mypy-boto3-ecr-public<1.28.0,>=1.27.0
-mypy-boto3-ecs<1.28.0,>=1.27.0
-mypy-boto3-efs<1.28.0,>=1.27.0
-mypy-boto3-eks<1.28.0,>=1.27.0
-mypy-boto3-elastic-inference<1.28.0,>=1.27.0
-mypy-boto3-elasticache<1.28.0,>=1.27.0
-mypy-boto3-elasticbeanstalk<1.28.0,>=1.27.0
-mypy-boto3-elastictranscoder<1.28.0,>=1.27.0
-mypy-boto3-elb<1.28.0,>=1.27.0
-mypy-boto3-elbv2<1.28.0,>=1.27.0
-mypy-boto3-emr<1.28.0,>=1.27.0
-mypy-boto3-emr-containers<1.28.0,>=1.27.0
-mypy-boto3-emr-serverless<1.28.0,>=1.27.0
-mypy-boto3-es<1.28.0,>=1.27.0
-mypy-boto3-events<1.28.0,>=1.27.0
-mypy-boto3-evidently<1.28.0,>=1.27.0
-mypy-boto3-finspace<1.28.0,>=1.27.0
-mypy-boto3-finspace-data<1.28.0,>=1.27.0
-mypy-boto3-firehose<1.28.0,>=1.27.0
-mypy-boto3-fis<1.28.0,>=1.27.0
-mypy-boto3-fms<1.28.0,>=1.27.0
-mypy-boto3-forecast<1.28.0,>=1.27.0
-mypy-boto3-forecastquery<1.28.0,>=1.27.0
-mypy-boto3-frauddetector<1.28.0,>=1.27.0
-mypy-boto3-fsx<1.28.0,>=1.27.0
-mypy-boto3-gamelift<1.28.0,>=1.27.0
-mypy-boto3-gamesparks<1.28.0,>=1.27.0
-mypy-boto3-glacier<1.28.0,>=1.27.0
-mypy-boto3-globalaccelerator<1.28.0,>=1.27.0
-mypy-boto3-glue<1.28.0,>=1.27.0
-mypy-boto3-grafana<1.28.0,>=1.27.0
-mypy-boto3-greengrass<1.28.0,>=1.27.0
-mypy-boto3-greengrassv2<1.28.0,>=1.27.0
-mypy-boto3-groundstation<1.28.0,>=1.27.0
-mypy-boto3-guardduty<1.28.0,>=1.27.0
-mypy-boto3-health<1.28.0,>=1.27.0
-mypy-boto3-healthlake<1.28.0,>=1.27.0
-mypy-boto3-honeycode<1.28.0,>=1.27.0
-mypy-boto3-iam<1.28.0,>=1.27.0
-mypy-boto3-identitystore<1.28.0,>=1.27.0
-mypy-boto3-imagebuilder<1.28.0,>=1.27.0
-mypy-boto3-importexport<1.28.0,>=1.27.0
-mypy-boto3-inspector<1.28.0,>=1.27.0
-mypy-boto3-inspector2<1.28.0,>=1.27.0
-mypy-boto3-internetmonitor<1.28.0,>=1.27.0
-mypy-boto3-iot<1.28.0,>=1.27.0
-mypy-boto3-iot-data<1.28.0,>=1.27.0
-mypy-boto3-iot-jobs-data<1.28.0,>=1.27.0
-mypy-boto3-iot-roborunner<1.28.0,>=1.27.0
-mypy-boto3-iot1click-devices<1.28.0,>=1.27.0
-mypy-boto3-iot1click-projects<1.28.0,>=1.27.0
-mypy-boto3-iotanalytics<1.28.0,>=1.27.0
-mypy-boto3-iotdeviceadvisor<1.28.0,>=1.27.0
-mypy-boto3-iotevents<1.28.0,>=1.27.0
-mypy-boto3-iotevents-data<1.28.0,>=1.27.0
-mypy-boto3-iotfleethub<1.28.0,>=1.27.0
-mypy-boto3-iotfleetwise<1.28.0,>=1.27.0
-mypy-boto3-iotsecuretunneling<1.28.0,>=1.27.0
-mypy-boto3-iotsitewise<1.28.0,>=1.27.0
-mypy-boto3-iotthingsgraph<1.28.0,>=1.27.0
-mypy-boto3-iottwinmaker<1.28.0,>=1.27.0
-mypy-boto3-iotwireless<1.28.0,>=1.27.0
-mypy-boto3-ivs<1.28.0,>=1.27.0
-mypy-boto3-ivs-realtime<1.28.0,>=1.27.0
-mypy-boto3-ivschat<1.28.0,>=1.27.0
-mypy-boto3-kafka<1.28.0,>=1.27.0
-mypy-boto3-kafkaconnect<1.28.0,>=1.27.0
-mypy-boto3-kendra<1.28.0,>=1.27.0
-mypy-boto3-kendra-ranking<1.28.0,>=1.27.0
-mypy-boto3-keyspaces<1.28.0,>=1.27.0
-mypy-boto3-kinesis<1.28.0,>=1.27.0
-mypy-boto3-kinesis-video-archived-media<1.28.0,>=1.27.0
-mypy-boto3-kinesis-video-media<1.28.0,>=1.27.0
-mypy-boto3-kinesis-video-signaling<1.28.0,>=1.27.0
-mypy-boto3-kinesis-video-webrtc-storage<1.28.0,>=1.27.0
-mypy-boto3-kinesisanalytics<1.28.0,>=1.27.0
-mypy-boto3-kinesisanalyticsv2<1.28.0,>=1.27.0
-mypy-boto3-kinesisvideo<1.28.0,>=1.27.0
-mypy-boto3-kms<1.28.0,>=1.27.0
-mypy-boto3-lakeformation<1.28.0,>=1.27.0
-mypy-boto3-lambda<1.28.0,>=1.27.0
-mypy-boto3-lex-models<1.28.0,>=1.27.0
-mypy-boto3-lex-runtime<1.28.0,>=1.27.0
-mypy-boto3-lexv2-models<1.28.0,>=1.27.0
-mypy-boto3-lexv2-runtime<1.28.0,>=1.27.0
-mypy-boto3-license-manager<1.28.0,>=1.27.0
-mypy-boto3-license-manager-linux-subscriptions<1.28.0,>=1.27.0
-mypy-boto3-license-manager-user-subscriptions<1.28.0,>=1.27.0
-mypy-boto3-lightsail<1.28.0,>=1.27.0
-mypy-boto3-location<1.28.0,>=1.27.0
-mypy-boto3-logs<1.28.0,>=1.27.0
-mypy-boto3-lookoutequipment<1.28.0,>=1.27.0
-mypy-boto3-lookoutmetrics<1.28.0,>=1.27.0
-mypy-boto3-lookoutvision<1.28.0,>=1.27.0
-mypy-boto3-m2<1.28.0,>=1.27.0
-mypy-boto3-machinelearning<1.28.0,>=1.27.0
-mypy-boto3-macie<1.28.0,>=1.27.0
-mypy-boto3-macie2<1.28.0,>=1.27.0
-mypy-boto3-managedblockchain<1.28.0,>=1.27.0
-mypy-boto3-marketplace-catalog<1.28.0,>=1.27.0
-mypy-boto3-marketplace-entitlement<1.28.0,>=1.27.0
-mypy-boto3-marketplacecommerceanalytics<1.28.0,>=1.27.0
-mypy-boto3-mediaconnect<1.28.0,>=1.27.0
-mypy-boto3-mediaconvert<1.28.0,>=1.27.0
-mypy-boto3-medialive<1.28.0,>=1.27.0
-mypy-boto3-mediapackage<1.28.0,>=1.27.0
-mypy-boto3-mediapackage-vod<1.28.0,>=1.27.0
-mypy-boto3-mediapackagev2<1.28.0,>=1.27.0
-mypy-boto3-mediastore<1.28.0,>=1.27.0
-mypy-boto3-mediastore-data<1.28.0,>=1.27.0
-mypy-boto3-mediatailor<1.28.0,>=1.27.0
-mypy-boto3-memorydb<1.28.0,>=1.27.0
-mypy-boto3-meteringmarketplace<1.28.0,>=1.27.0
-mypy-boto3-mgh<1.28.0,>=1.27.0
-mypy-boto3-mgn<1.28.0,>=1.27.0
-mypy-boto3-migration-hub-refactor-spaces<1.28.0,>=1.27.0
-mypy-boto3-migrationhub-config<1.28.0,>=1.27.0
-mypy-boto3-migrationhuborchestrator<1.28.0,>=1.27.0
-mypy-boto3-migrationhubstrategy<1.28.0,>=1.27.0
-mypy-boto3-mobile<1.28.0,>=1.27.0
-mypy-boto3-mq<1.28.0,>=1.27.0
-mypy-boto3-mturk<1.28.0,>=1.27.0
-mypy-boto3-mwaa<1.28.0,>=1.27.0
-mypy-boto3-neptune<1.28.0,>=1.27.0
-mypy-boto3-network-firewall<1.28.0,>=1.27.0
-mypy-boto3-networkmanager<1.28.0,>=1.27.0
-mypy-boto3-nimble<1.28.0,>=1.27.0
-mypy-boto3-oam<1.28.0,>=1.27.0
-mypy-boto3-omics<1.28.0,>=1.27.0
-mypy-boto3-opensearch<1.28.0,>=1.27.0
-mypy-boto3-opensearchserverless<1.28.0,>=1.27.0
-mypy-boto3-opsworks<1.28.0,>=1.27.0
-mypy-boto3-opsworkscm<1.28.0,>=1.27.0
-mypy-boto3-organizations<1.28.0,>=1.27.0
-mypy-boto3-osis<1.28.0,>=1.27.0
-mypy-boto3-outposts<1.28.0,>=1.27.0
-mypy-boto3-panorama<1.28.0,>=1.27.0
-mypy-boto3-payment-cryptography<1.28.0,>=1.27.0
-mypy-boto3-payment-cryptography-data<1.28.0,>=1.27.0
-mypy-boto3-personalize<1.28.0,>=1.27.0
-mypy-boto3-personalize-events<1.28.0,>=1.27.0
-mypy-boto3-personalize-runtime<1.28.0,>=1.27.0
-mypy-boto3-pi<1.28.0,>=1.27.0
-mypy-boto3-pinpoint<1.28.0,>=1.27.0
-mypy-boto3-pinpoint-email<1.28.0,>=1.27.0
-mypy-boto3-pinpoint-sms-voice<1.28.0,>=1.27.0
-mypy-boto3-pinpoint-sms-voice-v2<1.28.0,>=1.27.0
-mypy-boto3-pipes<1.28.0,>=1.27.0
-mypy-boto3-polly<1.28.0,>=1.27.0
-mypy-boto3-pricing<1.28.0,>=1.27.0
-mypy-boto3-privatenetworks<1.28.0,>=1.27.0
-mypy-boto3-proton<1.28.0,>=1.27.0
-mypy-boto3-qldb<1.28.0,>=1.27.0
-mypy-boto3-qldb-session<1.28.0,>=1.27.0
-mypy-boto3-quicksight<1.28.0,>=1.27.0
-mypy-boto3-ram<1.28.0,>=1.27.0
-mypy-boto3-rbin<1.28.0,>=1.27.0
-mypy-boto3-rds<1.28.0,>=1.27.0
-mypy-boto3-rds-data<1.28.0,>=1.27.0
-mypy-boto3-redshift<1.28.0,>=1.27.0
-mypy-boto3-redshift-data<1.28.0,>=1.27.0
-mypy-boto3-redshift-serverless<1.28.0,>=1.27.0
-mypy-boto3-rekognition<1.28.0,>=1.27.0
-mypy-boto3-resiliencehub<1.28.0,>=1.27.0
-mypy-boto3-resource-explorer-2<1.28.0,>=1.27.0
-mypy-boto3-resource-groups<1.28.0,>=1.27.0
-mypy-boto3-resourcegroupstaggingapi<1.28.0,>=1.27.0
-mypy-boto3-robomaker<1.28.0,>=1.27.0
-mypy-boto3-rolesanywhere<1.28.0,>=1.27.0
-mypy-boto3-route53<1.28.0,>=1.27.0
-mypy-boto3-route53-recovery-cluster<1.28.0,>=1.27.0
-mypy-boto3-route53-recovery-control-config<1.28.0,>=1.27.0
-mypy-boto3-route53-recovery-readiness<1.28.0,>=1.27.0
-mypy-boto3-route53domains<1.28.0,>=1.27.0
-mypy-boto3-route53resolver<1.28.0,>=1.27.0
-mypy-boto3-rum<1.28.0,>=1.27.0
-mypy-boto3-s3<1.28.0,>=1.27.0
-mypy-boto3-s3control<1.28.0,>=1.27.0
-mypy-boto3-s3outposts<1.28.0,>=1.27.0
-mypy-boto3-sagemaker<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-a2i-runtime<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-edge<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-featurestore-runtime<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-geospatial<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-metrics<1.28.0,>=1.27.0
-mypy-boto3-sagemaker-runtime<1.28.0,>=1.27.0
-mypy-boto3-savingsplans<1.28.0,>=1.27.0
-mypy-boto3-scheduler<1.28.0,>=1.27.0
-mypy-boto3-schemas<1.28.0,>=1.27.0
-mypy-boto3-sdb<1.28.0,>=1.27.0
-mypy-boto3-secretsmanager<1.28.0,>=1.27.0
-mypy-boto3-securityhub<1.28.0,>=1.27.0
-mypy-boto3-securitylake<1.28.0,>=1.27.0
-mypy-boto3-serverlessrepo<1.28.0,>=1.27.0
-mypy-boto3-service-quotas<1.28.0,>=1.27.0
-mypy-boto3-servicecatalog<1.28.0,>=1.27.0
-mypy-boto3-servicecatalog-appregistry<1.28.0,>=1.27.0
-mypy-boto3-servicediscovery<1.28.0,>=1.27.0
-mypy-boto3-ses<1.28.0,>=1.27.0
-mypy-boto3-sesv2<1.28.0,>=1.27.0
-mypy-boto3-shield<1.28.0,>=1.27.0
-mypy-boto3-signer<1.28.0,>=1.27.0
-mypy-boto3-simspaceweaver<1.28.0,>=1.27.0
-mypy-boto3-sms<1.28.0,>=1.27.0
-mypy-boto3-sms-voice<1.28.0,>=1.27.0
-mypy-boto3-snow-device-management<1.28.0,>=1.27.0
-mypy-boto3-snowball<1.28.0,>=1.27.0
-mypy-boto3-sns<1.28.0,>=1.27.0
-mypy-boto3-sqs<1.28.0,>=1.27.0
-mypy-boto3-ssm<1.28.0,>=1.27.0
-mypy-boto3-ssm-contacts<1.28.0,>=1.27.0
-mypy-boto3-ssm-incidents<1.28.0,>=1.27.0
-mypy-boto3-ssm-sap<1.28.0,>=1.27.0
-mypy-boto3-sso<1.28.0,>=1.27.0
-mypy-boto3-sso-admin<1.28.0,>=1.27.0
-mypy-boto3-sso-oidc<1.28.0,>=1.27.0
-mypy-boto3-stepfunctions<1.28.0,>=1.27.0
-mypy-boto3-storagegateway<1.28.0,>=1.27.0
-mypy-boto3-sts<1.28.0,>=1.27.0
-mypy-boto3-support<1.28.0,>=1.27.0
-mypy-boto3-support-app<1.28.0,>=1.27.0
-mypy-boto3-swf<1.28.0,>=1.27.0
-mypy-boto3-synthetics<1.28.0,>=1.27.0
-mypy-boto3-textract<1.28.0,>=1.27.0
-mypy-boto3-timestream-query<1.28.0,>=1.27.0
-mypy-boto3-timestream-write<1.28.0,>=1.27.0
-mypy-boto3-tnb<1.28.0,>=1.27.0
-mypy-boto3-transcribe<1.28.0,>=1.27.0
-mypy-boto3-transfer<1.28.0,>=1.27.0
-mypy-boto3-translate<1.28.0,>=1.27.0
-mypy-boto3-verifiedpermissions<1.28.0,>=1.27.0
-mypy-boto3-voice-id<1.28.0,>=1.27.0
-mypy-boto3-vpc-lattice<1.28.0,>=1.27.0
-mypy-boto3-waf<1.28.0,>=1.27.0
-mypy-boto3-waf-regional<1.28.0,>=1.27.0
-mypy-boto3-wafv2<1.28.0,>=1.27.0
-mypy-boto3-wellarchitected<1.28.0,>=1.27.0
-mypy-boto3-wisdom<1.28.0,>=1.27.0
-mypy-boto3-workdocs<1.28.0,>=1.27.0
-mypy-boto3-worklink<1.28.0,>=1.27.0
-mypy-boto3-workmail<1.28.0,>=1.27.0
-mypy-boto3-workmailmessageflow<1.28.0,>=1.27.0
-mypy-boto3-workspaces<1.28.0,>=1.27.0
-mypy-boto3-workspaces-web<1.28.0,>=1.27.0
-mypy-boto3-xray<1.28.0,>=1.27.0
+mypy-boto3-accessanalyzer<1.29.0,>=1.28.0
+mypy-boto3-account<1.29.0,>=1.28.0
+mypy-boto3-acm<1.29.0,>=1.28.0
+mypy-boto3-acm-pca<1.29.0,>=1.28.0
+mypy-boto3-alexaforbusiness<1.29.0,>=1.28.0
+mypy-boto3-amp<1.29.0,>=1.28.0
+mypy-boto3-amplify<1.29.0,>=1.28.0
+mypy-boto3-amplifybackend<1.29.0,>=1.28.0
+mypy-boto3-amplifyuibuilder<1.29.0,>=1.28.0
+mypy-boto3-apigateway<1.29.0,>=1.28.0
+mypy-boto3-apigatewaymanagementapi<1.29.0,>=1.28.0
+mypy-boto3-apigatewayv2<1.29.0,>=1.28.0
+mypy-boto3-appconfig<1.29.0,>=1.28.0
+mypy-boto3-appconfigdata<1.29.0,>=1.28.0
+mypy-boto3-appfabric<1.29.0,>=1.28.0
+mypy-boto3-appflow<1.29.0,>=1.28.0
+mypy-boto3-appintegrations<1.29.0,>=1.28.0
+mypy-boto3-application-autoscaling<1.29.0,>=1.28.0
+mypy-boto3-application-insights<1.29.0,>=1.28.0
+mypy-boto3-applicationcostprofiler<1.29.0,>=1.28.0
+mypy-boto3-appmesh<1.29.0,>=1.28.0
+mypy-boto3-apprunner<1.29.0,>=1.28.0
+mypy-boto3-appstream<1.29.0,>=1.28.0
+mypy-boto3-appsync<1.29.0,>=1.28.0
+mypy-boto3-arc-zonal-shift<1.29.0,>=1.28.0
+mypy-boto3-athena<1.29.0,>=1.28.0
+mypy-boto3-auditmanager<1.29.0,>=1.28.0
+mypy-boto3-autoscaling<1.29.0,>=1.28.0
+mypy-boto3-autoscaling-plans<1.29.0,>=1.28.0
+mypy-boto3-backup<1.29.0,>=1.28.0
+mypy-boto3-backup-gateway<1.29.0,>=1.28.0
+mypy-boto3-backupstorage<1.29.0,>=1.28.0
+mypy-boto3-batch<1.29.0,>=1.28.0
+mypy-boto3-billingconductor<1.29.0,>=1.28.0
+mypy-boto3-braket<1.29.0,>=1.28.0
+mypy-boto3-budgets<1.29.0,>=1.28.0
+mypy-boto3-ce<1.29.0,>=1.28.0
+mypy-boto3-chime<1.29.0,>=1.28.0
+mypy-boto3-chime-sdk-identity<1.29.0,>=1.28.0
+mypy-boto3-chime-sdk-media-pipelines<1.29.0,>=1.28.0
+mypy-boto3-chime-sdk-meetings<1.29.0,>=1.28.0
+mypy-boto3-chime-sdk-messaging<1.29.0,>=1.28.0
+mypy-boto3-chime-sdk-voice<1.29.0,>=1.28.0
+mypy-boto3-cleanrooms<1.29.0,>=1.28.0
+mypy-boto3-cloud9<1.29.0,>=1.28.0
+mypy-boto3-cloudcontrol<1.29.0,>=1.28.0
+mypy-boto3-clouddirectory<1.29.0,>=1.28.0
+mypy-boto3-cloudformation<1.29.0,>=1.28.0
+mypy-boto3-cloudfront<1.29.0,>=1.28.0
+mypy-boto3-cloudhsm<1.29.0,>=1.28.0
+mypy-boto3-cloudhsmv2<1.29.0,>=1.28.0
+mypy-boto3-cloudsearch<1.29.0,>=1.28.0
+mypy-boto3-cloudsearchdomain<1.29.0,>=1.28.0
+mypy-boto3-cloudtrail<1.29.0,>=1.28.0
+mypy-boto3-cloudtrail-data<1.29.0,>=1.28.0
+mypy-boto3-cloudwatch<1.29.0,>=1.28.0
+mypy-boto3-codeartifact<1.29.0,>=1.28.0
+mypy-boto3-codebuild<1.29.0,>=1.28.0
+mypy-boto3-codecatalyst<1.29.0,>=1.28.0
+mypy-boto3-codecommit<1.29.0,>=1.28.0
+mypy-boto3-codedeploy<1.29.0,>=1.28.0
+mypy-boto3-codeguru-reviewer<1.29.0,>=1.28.0
+mypy-boto3-codeguru-security<1.29.0,>=1.28.0
+mypy-boto3-codeguruprofiler<1.29.0,>=1.28.0
+mypy-boto3-codepipeline<1.29.0,>=1.28.0
+mypy-boto3-codestar<1.29.0,>=1.28.0
+mypy-boto3-codestar-connections<1.29.0,>=1.28.0
+mypy-boto3-codestar-notifications<1.29.0,>=1.28.0
+mypy-boto3-cognito-identity<1.29.0,>=1.28.0
+mypy-boto3-cognito-idp<1.29.0,>=1.28.0
+mypy-boto3-cognito-sync<1.29.0,>=1.28.0
+mypy-boto3-comprehend<1.29.0,>=1.28.0
+mypy-boto3-comprehendmedical<1.29.0,>=1.28.0
+mypy-boto3-compute-optimizer<1.29.0,>=1.28.0
+mypy-boto3-config<1.29.0,>=1.28.0
+mypy-boto3-connect<1.29.0,>=1.28.0
+mypy-boto3-connect-contact-lens<1.29.0,>=1.28.0
+mypy-boto3-connectcampaigns<1.29.0,>=1.28.0
+mypy-boto3-connectcases<1.29.0,>=1.28.0
+mypy-boto3-connectparticipant<1.29.0,>=1.28.0
+mypy-boto3-controltower<1.29.0,>=1.28.0
+mypy-boto3-cur<1.29.0,>=1.28.0
+mypy-boto3-customer-profiles<1.29.0,>=1.28.0
+mypy-boto3-databrew<1.29.0,>=1.28.0
+mypy-boto3-dataexchange<1.29.0,>=1.28.0
+mypy-boto3-datapipeline<1.29.0,>=1.28.0
+mypy-boto3-datasync<1.29.0,>=1.28.0
+mypy-boto3-dax<1.29.0,>=1.28.0
+mypy-boto3-detective<1.29.0,>=1.28.0
+mypy-boto3-devicefarm<1.29.0,>=1.28.0
+mypy-boto3-devops-guru<1.29.0,>=1.28.0
+mypy-boto3-directconnect<1.29.0,>=1.28.0
+mypy-boto3-discovery<1.29.0,>=1.28.0
+mypy-boto3-dlm<1.29.0,>=1.28.0
+mypy-boto3-dms<1.29.0,>=1.28.0
+mypy-boto3-docdb<1.29.0,>=1.28.0
+mypy-boto3-docdb-elastic<1.29.0,>=1.28.0
+mypy-boto3-drs<1.29.0,>=1.28.0
+mypy-boto3-ds<1.29.0,>=1.28.0
+mypy-boto3-dynamodb<1.29.0,>=1.28.0
+mypy-boto3-dynamodbstreams<1.29.0,>=1.28.0
+mypy-boto3-ebs<1.29.0,>=1.28.0
+mypy-boto3-ec2<1.29.0,>=1.28.0
+mypy-boto3-ec2-instance-connect<1.29.0,>=1.28.0
+mypy-boto3-ecr<1.29.0,>=1.28.0
+mypy-boto3-ecr-public<1.29.0,>=1.28.0
+mypy-boto3-ecs<1.29.0,>=1.28.0
+mypy-boto3-efs<1.29.0,>=1.28.0
+mypy-boto3-eks<1.29.0,>=1.28.0
+mypy-boto3-elastic-inference<1.29.0,>=1.28.0
+mypy-boto3-elasticache<1.29.0,>=1.28.0
+mypy-boto3-elasticbeanstalk<1.29.0,>=1.28.0
+mypy-boto3-elastictranscoder<1.29.0,>=1.28.0
+mypy-boto3-elb<1.29.0,>=1.28.0
+mypy-boto3-elbv2<1.29.0,>=1.28.0
+mypy-boto3-emr<1.29.0,>=1.28.0
+mypy-boto3-emr-containers<1.29.0,>=1.28.0
+mypy-boto3-emr-serverless<1.29.0,>=1.28.0
+mypy-boto3-es<1.29.0,>=1.28.0
+mypy-boto3-events<1.29.0,>=1.28.0
+mypy-boto3-evidently<1.29.0,>=1.28.0
+mypy-boto3-finspace<1.29.0,>=1.28.0
+mypy-boto3-finspace-data<1.29.0,>=1.28.0
+mypy-boto3-firehose<1.29.0,>=1.28.0
+mypy-boto3-fis<1.29.0,>=1.28.0
+mypy-boto3-fms<1.29.0,>=1.28.0
+mypy-boto3-forecast<1.29.0,>=1.28.0
+mypy-boto3-forecastquery<1.29.0,>=1.28.0
+mypy-boto3-frauddetector<1.29.0,>=1.28.0
+mypy-boto3-fsx<1.29.0,>=1.28.0
+mypy-boto3-gamelift<1.29.0,>=1.28.0
+mypy-boto3-gamesparks<1.29.0,>=1.28.0
+mypy-boto3-glacier<1.29.0,>=1.28.0
+mypy-boto3-globalaccelerator<1.29.0,>=1.28.0
+mypy-boto3-glue<1.29.0,>=1.28.0
+mypy-boto3-grafana<1.29.0,>=1.28.0
+mypy-boto3-greengrass<1.29.0,>=1.28.0
+mypy-boto3-greengrassv2<1.29.0,>=1.28.0
+mypy-boto3-groundstation<1.29.0,>=1.28.0
+mypy-boto3-guardduty<1.29.0,>=1.28.0
+mypy-boto3-health<1.29.0,>=1.28.0
+mypy-boto3-healthlake<1.29.0,>=1.28.0
+mypy-boto3-honeycode<1.29.0,>=1.28.0
+mypy-boto3-iam<1.29.0,>=1.28.0
+mypy-boto3-identitystore<1.29.0,>=1.28.0
+mypy-boto3-imagebuilder<1.29.0,>=1.28.0
+mypy-boto3-importexport<1.29.0,>=1.28.0
+mypy-boto3-inspector<1.29.0,>=1.28.0
+mypy-boto3-inspector2<1.29.0,>=1.28.0
+mypy-boto3-internetmonitor<1.29.0,>=1.28.0
+mypy-boto3-iot<1.29.0,>=1.28.0
+mypy-boto3-iot-data<1.29.0,>=1.28.0
+mypy-boto3-iot-jobs-data<1.29.0,>=1.28.0
+mypy-boto3-iot-roborunner<1.29.0,>=1.28.0
+mypy-boto3-iot1click-devices<1.29.0,>=1.28.0
+mypy-boto3-iot1click-projects<1.29.0,>=1.28.0
+mypy-boto3-iotanalytics<1.29.0,>=1.28.0
+mypy-boto3-iotdeviceadvisor<1.29.0,>=1.28.0
+mypy-boto3-iotevents<1.29.0,>=1.28.0
+mypy-boto3-iotevents-data<1.29.0,>=1.28.0
+mypy-boto3-iotfleethub<1.29.0,>=1.28.0
+mypy-boto3-iotfleetwise<1.29.0,>=1.28.0
+mypy-boto3-iotsecuretunneling<1.29.0,>=1.28.0
+mypy-boto3-iotsitewise<1.29.0,>=1.28.0
+mypy-boto3-iotthingsgraph<1.29.0,>=1.28.0
+mypy-boto3-iottwinmaker<1.29.0,>=1.28.0
+mypy-boto3-iotwireless<1.29.0,>=1.28.0
+mypy-boto3-ivs<1.29.0,>=1.28.0
+mypy-boto3-ivs-realtime<1.29.0,>=1.28.0
+mypy-boto3-ivschat<1.29.0,>=1.28.0
+mypy-boto3-kafka<1.29.0,>=1.28.0
+mypy-boto3-kafkaconnect<1.29.0,>=1.28.0
+mypy-boto3-kendra<1.29.0,>=1.28.0
+mypy-boto3-kendra-ranking<1.29.0,>=1.28.0
+mypy-boto3-keyspaces<1.29.0,>=1.28.0
+mypy-boto3-kinesis<1.29.0,>=1.28.0
+mypy-boto3-kinesis-video-archived-media<1.29.0,>=1.28.0
+mypy-boto3-kinesis-video-media<1.29.0,>=1.28.0
+mypy-boto3-kinesis-video-signaling<1.29.0,>=1.28.0
+mypy-boto3-kinesis-video-webrtc-storage<1.29.0,>=1.28.0
+mypy-boto3-kinesisanalytics<1.29.0,>=1.28.0
+mypy-boto3-kinesisanalyticsv2<1.29.0,>=1.28.0
+mypy-boto3-kinesisvideo<1.29.0,>=1.28.0
+mypy-boto3-kms<1.29.0,>=1.28.0
+mypy-boto3-lakeformation<1.29.0,>=1.28.0
+mypy-boto3-lambda<1.29.0,>=1.28.0
+mypy-boto3-lex-models<1.29.0,>=1.28.0
+mypy-boto3-lex-runtime<1.29.0,>=1.28.0
+mypy-boto3-lexv2-models<1.29.0,>=1.28.0
+mypy-boto3-lexv2-runtime<1.29.0,>=1.28.0
+mypy-boto3-license-manager<1.29.0,>=1.28.0
+mypy-boto3-license-manager-linux-subscriptions<1.29.0,>=1.28.0
+mypy-boto3-license-manager-user-subscriptions<1.29.0,>=1.28.0
+mypy-boto3-lightsail<1.29.0,>=1.28.0
+mypy-boto3-location<1.29.0,>=1.28.0
+mypy-boto3-logs<1.29.0,>=1.28.0
+mypy-boto3-lookoutequipment<1.29.0,>=1.28.0
+mypy-boto3-lookoutmetrics<1.29.0,>=1.28.0
+mypy-boto3-lookoutvision<1.29.0,>=1.28.0
+mypy-boto3-m2<1.29.0,>=1.28.0
+mypy-boto3-machinelearning<1.29.0,>=1.28.0
+mypy-boto3-macie<1.29.0,>=1.28.0
+mypy-boto3-macie2<1.29.0,>=1.28.0
+mypy-boto3-managedblockchain<1.29.0,>=1.28.0
+mypy-boto3-marketplace-catalog<1.29.0,>=1.28.0
+mypy-boto3-marketplace-entitlement<1.29.0,>=1.28.0
+mypy-boto3-marketplacecommerceanalytics<1.29.0,>=1.28.0
+mypy-boto3-mediaconnect<1.29.0,>=1.28.0
+mypy-boto3-mediaconvert<1.29.0,>=1.28.0
+mypy-boto3-medialive<1.29.0,>=1.28.0
+mypy-boto3-mediapackage<1.29.0,>=1.28.0
+mypy-boto3-mediapackage-vod<1.29.0,>=1.28.0
+mypy-boto3-mediapackagev2<1.29.0,>=1.28.0
+mypy-boto3-mediastore<1.29.0,>=1.28.0
+mypy-boto3-mediastore-data<1.29.0,>=1.28.0
+mypy-boto3-mediatailor<1.29.0,>=1.28.0
+mypy-boto3-memorydb<1.29.0,>=1.28.0
+mypy-boto3-meteringmarketplace<1.29.0,>=1.28.0
+mypy-boto3-mgh<1.29.0,>=1.28.0
+mypy-boto3-mgn<1.29.0,>=1.28.0
+mypy-boto3-migration-hub-refactor-spaces<1.29.0,>=1.28.0
+mypy-boto3-migrationhub-config<1.29.0,>=1.28.0
+mypy-boto3-migrationhuborchestrator<1.29.0,>=1.28.0
+mypy-boto3-migrationhubstrategy<1.29.0,>=1.28.0
+mypy-boto3-mobile<1.29.0,>=1.28.0
+mypy-boto3-mq<1.29.0,>=1.28.0
+mypy-boto3-mturk<1.29.0,>=1.28.0
+mypy-boto3-mwaa<1.29.0,>=1.28.0
+mypy-boto3-neptune<1.29.0,>=1.28.0
+mypy-boto3-network-firewall<1.29.0,>=1.28.0
+mypy-boto3-networkmanager<1.29.0,>=1.28.0
+mypy-boto3-nimble<1.29.0,>=1.28.0
+mypy-boto3-oam<1.29.0,>=1.28.0
+mypy-boto3-omics<1.29.0,>=1.28.0
+mypy-boto3-opensearch<1.29.0,>=1.28.0
+mypy-boto3-opensearchserverless<1.29.0,>=1.28.0
+mypy-boto3-opsworks<1.29.0,>=1.28.0
+mypy-boto3-opsworkscm<1.29.0,>=1.28.0
+mypy-boto3-organizations<1.29.0,>=1.28.0
+mypy-boto3-osis<1.29.0,>=1.28.0
+mypy-boto3-outposts<1.29.0,>=1.28.0
+mypy-boto3-panorama<1.29.0,>=1.28.0
+mypy-boto3-payment-cryptography<1.29.0,>=1.28.0
+mypy-boto3-payment-cryptography-data<1.29.0,>=1.28.0
+mypy-boto3-personalize<1.29.0,>=1.28.0
+mypy-boto3-personalize-events<1.29.0,>=1.28.0
+mypy-boto3-personalize-runtime<1.29.0,>=1.28.0
+mypy-boto3-pi<1.29.0,>=1.28.0
+mypy-boto3-pinpoint<1.29.0,>=1.28.0
+mypy-boto3-pinpoint-email<1.29.0,>=1.28.0
+mypy-boto3-pinpoint-sms-voice<1.29.0,>=1.28.0
+mypy-boto3-pinpoint-sms-voice-v2<1.29.0,>=1.28.0
+mypy-boto3-pipes<1.29.0,>=1.28.0
+mypy-boto3-polly<1.29.0,>=1.28.0
+mypy-boto3-pricing<1.29.0,>=1.28.0
+mypy-boto3-privatenetworks<1.29.0,>=1.28.0
+mypy-boto3-proton<1.29.0,>=1.28.0
+mypy-boto3-qldb<1.29.0,>=1.28.0
+mypy-boto3-qldb-session<1.29.0,>=1.28.0
+mypy-boto3-quicksight<1.29.0,>=1.28.0
+mypy-boto3-ram<1.29.0,>=1.28.0
+mypy-boto3-rbin<1.29.0,>=1.28.0
+mypy-boto3-rds<1.29.0,>=1.28.0
+mypy-boto3-rds-data<1.29.0,>=1.28.0
+mypy-boto3-redshift<1.29.0,>=1.28.0
+mypy-boto3-redshift-data<1.29.0,>=1.28.0
+mypy-boto3-redshift-serverless<1.29.0,>=1.28.0
+mypy-boto3-rekognition<1.29.0,>=1.28.0
+mypy-boto3-resiliencehub<1.29.0,>=1.28.0
+mypy-boto3-resource-explorer-2<1.29.0,>=1.28.0
+mypy-boto3-resource-groups<1.29.0,>=1.28.0
+mypy-boto3-resourcegroupstaggingapi<1.29.0,>=1.28.0
+mypy-boto3-robomaker<1.29.0,>=1.28.0
+mypy-boto3-rolesanywhere<1.29.0,>=1.28.0
+mypy-boto3-route53<1.29.0,>=1.28.0
+mypy-boto3-route53-recovery-cluster<1.29.0,>=1.28.0
+mypy-boto3-route53-recovery-control-config<1.29.0,>=1.28.0
+mypy-boto3-route53-recovery-readiness<1.29.0,>=1.28.0
+mypy-boto3-route53domains<1.29.0,>=1.28.0
+mypy-boto3-route53resolver<1.29.0,>=1.28.0
+mypy-boto3-rum<1.29.0,>=1.28.0
+mypy-boto3-s3<1.29.0,>=1.28.0
+mypy-boto3-s3control<1.29.0,>=1.28.0
+mypy-boto3-s3outposts<1.29.0,>=1.28.0
+mypy-boto3-sagemaker<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-a2i-runtime<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-edge<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-featurestore-runtime<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-geospatial<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-metrics<1.29.0,>=1.28.0
+mypy-boto3-sagemaker-runtime<1.29.0,>=1.28.0
+mypy-boto3-savingsplans<1.29.0,>=1.28.0
+mypy-boto3-scheduler<1.29.0,>=1.28.0
+mypy-boto3-schemas<1.29.0,>=1.28.0
+mypy-boto3-sdb<1.29.0,>=1.28.0
+mypy-boto3-secretsmanager<1.29.0,>=1.28.0
+mypy-boto3-securityhub<1.29.0,>=1.28.0
+mypy-boto3-securitylake<1.29.0,>=1.28.0
+mypy-boto3-serverlessrepo<1.29.0,>=1.28.0
+mypy-boto3-service-quotas<1.29.0,>=1.28.0
+mypy-boto3-servicecatalog<1.29.0,>=1.28.0
+mypy-boto3-servicecatalog-appregistry<1.29.0,>=1.28.0
+mypy-boto3-servicediscovery<1.29.0,>=1.28.0
+mypy-boto3-ses<1.29.0,>=1.28.0
+mypy-boto3-sesv2<1.29.0,>=1.28.0
+mypy-boto3-shield<1.29.0,>=1.28.0
+mypy-boto3-signer<1.29.0,>=1.28.0
+mypy-boto3-simspaceweaver<1.29.0,>=1.28.0
+mypy-boto3-sms<1.29.0,>=1.28.0
+mypy-boto3-sms-voice<1.29.0,>=1.28.0
+mypy-boto3-snow-device-management<1.29.0,>=1.28.0
+mypy-boto3-snowball<1.29.0,>=1.28.0
+mypy-boto3-sns<1.29.0,>=1.28.0
+mypy-boto3-sqs<1.29.0,>=1.28.0
+mypy-boto3-ssm<1.29.0,>=1.28.0
+mypy-boto3-ssm-contacts<1.29.0,>=1.28.0
+mypy-boto3-ssm-incidents<1.29.0,>=1.28.0
+mypy-boto3-ssm-sap<1.29.0,>=1.28.0
+mypy-boto3-sso<1.29.0,>=1.28.0
+mypy-boto3-sso-admin<1.29.0,>=1.28.0
+mypy-boto3-sso-oidc<1.29.0,>=1.28.0
+mypy-boto3-stepfunctions<1.29.0,>=1.28.0
+mypy-boto3-storagegateway<1.29.0,>=1.28.0
+mypy-boto3-sts<1.29.0,>=1.28.0
+mypy-boto3-support<1.29.0,>=1.28.0
+mypy-boto3-support-app<1.29.0,>=1.28.0
+mypy-boto3-swf<1.29.0,>=1.28.0
+mypy-boto3-synthetics<1.29.0,>=1.28.0
+mypy-boto3-textract<1.29.0,>=1.28.0
+mypy-boto3-timestream-query<1.29.0,>=1.28.0
+mypy-boto3-timestream-write<1.29.0,>=1.28.0
+mypy-boto3-tnb<1.29.0,>=1.28.0
+mypy-boto3-transcribe<1.29.0,>=1.28.0
+mypy-boto3-transfer<1.29.0,>=1.28.0
+mypy-boto3-translate<1.29.0,>=1.28.0
+mypy-boto3-verifiedpermissions<1.29.0,>=1.28.0
+mypy-boto3-voice-id<1.29.0,>=1.28.0
+mypy-boto3-vpc-lattice<1.29.0,>=1.28.0
+mypy-boto3-waf<1.29.0,>=1.28.0
+mypy-boto3-waf-regional<1.29.0,>=1.28.0
+mypy-boto3-wafv2<1.29.0,>=1.28.0
+mypy-boto3-wellarchitected<1.29.0,>=1.28.0
+mypy-boto3-wisdom<1.29.0,>=1.28.0
+mypy-boto3-workdocs<1.29.0,>=1.28.0
+mypy-boto3-worklink<1.29.0,>=1.28.0
+mypy-boto3-workmail<1.29.0,>=1.28.0
+mypy-boto3-workmailmessageflow<1.29.0,>=1.28.0
+mypy-boto3-workspaces<1.29.0,>=1.28.0
+mypy-boto3-workspaces-web<1.29.0,>=1.28.0
+mypy-boto3-xray<1.29.0,>=1.28.0
 
 [amp]
-mypy-boto3-amp<1.28.0,>=1.27.0
+mypy-boto3-amp<1.29.0,>=1.28.0
 
 [amplify]
-mypy-boto3-amplify<1.28.0,>=1.27.0
+mypy-boto3-amplify<1.29.0,>=1.28.0
 
 [amplifybackend]
-mypy-boto3-amplifybackend<1.28.0,>=1.27.0
+mypy-boto3-amplifybackend<1.29.0,>=1.28.0
 
 [amplifyuibuilder]
-mypy-boto3-amplifyuibuilder<1.28.0,>=1.27.0
+mypy-boto3-amplifyuibuilder<1.29.0,>=1.28.0
 
 [apigateway]
-mypy-boto3-apigateway<1.28.0,>=1.27.0
+mypy-boto3-apigateway<1.29.0,>=1.28.0
 
 [apigatewaymanagementapi]
-mypy-boto3-apigatewaymanagementapi<1.28.0,>=1.27.0
+mypy-boto3-apigatewaymanagementapi<1.29.0,>=1.28.0
 
 [apigatewayv2]
-mypy-boto3-apigatewayv2<1.28.0,>=1.27.0
+mypy-boto3-apigatewayv2<1.29.0,>=1.28.0
 
 [appconfig]
-mypy-boto3-appconfig<1.28.0,>=1.27.0
+mypy-boto3-appconfig<1.29.0,>=1.28.0
 
 [appconfigdata]
-mypy-boto3-appconfigdata<1.28.0,>=1.27.0
+mypy-boto3-appconfigdata<1.29.0,>=1.28.0
 
 [appfabric]
-mypy-boto3-appfabric<1.28.0,>=1.27.0
+mypy-boto3-appfabric<1.29.0,>=1.28.0
 
 [appflow]
-mypy-boto3-appflow<1.28.0,>=1.27.0
+mypy-boto3-appflow<1.29.0,>=1.28.0
 
 [appintegrations]
-mypy-boto3-appintegrations<1.28.0,>=1.27.0
+mypy-boto3-appintegrations<1.29.0,>=1.28.0
 
 [application-autoscaling]
-mypy-boto3-application-autoscaling<1.28.0,>=1.27.0
+mypy-boto3-application-autoscaling<1.29.0,>=1.28.0
 
 [application-insights]
-mypy-boto3-application-insights<1.28.0,>=1.27.0
+mypy-boto3-application-insights<1.29.0,>=1.28.0
 
 [applicationcostprofiler]
-mypy-boto3-applicationcostprofiler<1.28.0,>=1.27.0
+mypy-boto3-applicationcostprofiler<1.29.0,>=1.28.0
 
 [appmesh]
-mypy-boto3-appmesh<1.28.0,>=1.27.0
+mypy-boto3-appmesh<1.29.0,>=1.28.0
 
 [apprunner]
-mypy-boto3-apprunner<1.28.0,>=1.27.0
+mypy-boto3-apprunner<1.29.0,>=1.28.0
 
 [appstream]
-mypy-boto3-appstream<1.28.0,>=1.27.0
+mypy-boto3-appstream<1.29.0,>=1.28.0
 
 [appsync]
-mypy-boto3-appsync<1.28.0,>=1.27.0
+mypy-boto3-appsync<1.29.0,>=1.28.0
 
 [arc-zonal-shift]
-mypy-boto3-arc-zonal-shift<1.28.0,>=1.27.0
+mypy-boto3-arc-zonal-shift<1.29.0,>=1.28.0
 
 [athena]
-mypy-boto3-athena<1.28.0,>=1.27.0
+mypy-boto3-athena<1.29.0,>=1.28.0
 
 [auditmanager]
-mypy-boto3-auditmanager<1.28.0,>=1.27.0
+mypy-boto3-auditmanager<1.29.0,>=1.28.0
 
 [autoscaling]
-mypy-boto3-autoscaling<1.28.0,>=1.27.0
+mypy-boto3-autoscaling<1.29.0,>=1.28.0
 
 [autoscaling-plans]
-mypy-boto3-autoscaling-plans<1.28.0,>=1.27.0
+mypy-boto3-autoscaling-plans<1.29.0,>=1.28.0
 
 [backup]
-mypy-boto3-backup<1.28.0,>=1.27.0
+mypy-boto3-backup<1.29.0,>=1.28.0
 
 [backup-gateway]
-mypy-boto3-backup-gateway<1.28.0,>=1.27.0
+mypy-boto3-backup-gateway<1.29.0,>=1.28.0
 
 [backupstorage]
-mypy-boto3-backupstorage<1.28.0,>=1.27.0
+mypy-boto3-backupstorage<1.29.0,>=1.28.0
 
 [batch]
-mypy-boto3-batch<1.28.0,>=1.27.0
+mypy-boto3-batch<1.29.0,>=1.28.0
 
 [billingconductor]
-mypy-boto3-billingconductor<1.28.0,>=1.27.0
+mypy-boto3-billingconductor<1.29.0,>=1.28.0
 
 [boto3]
-boto3==1.27.1
-botocore==1.30.1
+boto3==1.28.0
+botocore==1.31.0
 
 [braket]
-mypy-boto3-braket<1.28.0,>=1.27.0
+mypy-boto3-braket<1.29.0,>=1.28.0
 
 [budgets]
-mypy-boto3-budgets<1.28.0,>=1.27.0
+mypy-boto3-budgets<1.29.0,>=1.28.0
 
 [ce]
-mypy-boto3-ce<1.28.0,>=1.27.0
+mypy-boto3-ce<1.29.0,>=1.28.0
 
 [chime]
-mypy-boto3-chime<1.28.0,>=1.27.0
+mypy-boto3-chime<1.29.0,>=1.28.0
 
 [chime-sdk-identity]
-mypy-boto3-chime-sdk-identity<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-identity<1.29.0,>=1.28.0
 
 [chime-sdk-media-pipelines]
-mypy-boto3-chime-sdk-media-pipelines<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-media-pipelines<1.29.0,>=1.28.0
 
 [chime-sdk-meetings]
-mypy-boto3-chime-sdk-meetings<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-meetings<1.29.0,>=1.28.0
 
 [chime-sdk-messaging]
-mypy-boto3-chime-sdk-messaging<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-messaging<1.29.0,>=1.28.0
 
 [chime-sdk-voice]
-mypy-boto3-chime-sdk-voice<1.28.0,>=1.27.0
+mypy-boto3-chime-sdk-voice<1.29.0,>=1.28.0
 
 [cleanrooms]
-mypy-boto3-cleanrooms<1.28.0,>=1.27.0
+mypy-boto3-cleanrooms<1.29.0,>=1.28.0
 
 [cloud9]
-mypy-boto3-cloud9<1.28.0,>=1.27.0
+mypy-boto3-cloud9<1.29.0,>=1.28.0
 
 [cloudcontrol]
-mypy-boto3-cloudcontrol<1.28.0,>=1.27.0
+mypy-boto3-cloudcontrol<1.29.0,>=1.28.0
 
 [clouddirectory]
-mypy-boto3-clouddirectory<1.28.0,>=1.27.0
+mypy-boto3-clouddirectory<1.29.0,>=1.28.0
 
 [cloudformation]
-mypy-boto3-cloudformation<1.28.0,>=1.27.0
+mypy-boto3-cloudformation<1.29.0,>=1.28.0
 
 [cloudfront]
-mypy-boto3-cloudfront<1.28.0,>=1.27.0
+mypy-boto3-cloudfront<1.29.0,>=1.28.0
 
 [cloudhsm]
-mypy-boto3-cloudhsm<1.28.0,>=1.27.0
+mypy-boto3-cloudhsm<1.29.0,>=1.28.0
 
 [cloudhsmv2]
-mypy-boto3-cloudhsmv2<1.28.0,>=1.27.0
+mypy-boto3-cloudhsmv2<1.29.0,>=1.28.0
 
 [cloudsearch]
-mypy-boto3-cloudsearch<1.28.0,>=1.27.0
+mypy-boto3-cloudsearch<1.29.0,>=1.28.0
 
 [cloudsearchdomain]
-mypy-boto3-cloudsearchdomain<1.28.0,>=1.27.0
+mypy-boto3-cloudsearchdomain<1.29.0,>=1.28.0
 
 [cloudtrail]
-mypy-boto3-cloudtrail<1.28.0,>=1.27.0
+mypy-boto3-cloudtrail<1.29.0,>=1.28.0
 
 [cloudtrail-data]
-mypy-boto3-cloudtrail-data<1.28.0,>=1.27.0
+mypy-boto3-cloudtrail-data<1.29.0,>=1.28.0
 
 [cloudwatch]
-mypy-boto3-cloudwatch<1.28.0,>=1.27.0
+mypy-boto3-cloudwatch<1.29.0,>=1.28.0
 
 [codeartifact]
-mypy-boto3-codeartifact<1.28.0,>=1.27.0
+mypy-boto3-codeartifact<1.29.0,>=1.28.0
 
 [codebuild]
-mypy-boto3-codebuild<1.28.0,>=1.27.0
+mypy-boto3-codebuild<1.29.0,>=1.28.0
 
 [codecatalyst]
-mypy-boto3-codecatalyst<1.28.0,>=1.27.0
+mypy-boto3-codecatalyst<1.29.0,>=1.28.0
 
 [codecommit]
-mypy-boto3-codecommit<1.28.0,>=1.27.0
+mypy-boto3-codecommit<1.29.0,>=1.28.0
 
 [codedeploy]
-mypy-boto3-codedeploy<1.28.0,>=1.27.0
+mypy-boto3-codedeploy<1.29.0,>=1.28.0
 
 [codeguru-reviewer]
-mypy-boto3-codeguru-reviewer<1.28.0,>=1.27.0
+mypy-boto3-codeguru-reviewer<1.29.0,>=1.28.0
 
 [codeguru-security]
-mypy-boto3-codeguru-security<1.28.0,>=1.27.0
+mypy-boto3-codeguru-security<1.29.0,>=1.28.0
 
 [codeguruprofiler]
-mypy-boto3-codeguruprofiler<1.28.0,>=1.27.0
+mypy-boto3-codeguruprofiler<1.29.0,>=1.28.0
 
 [codepipeline]
-mypy-boto3-codepipeline<1.28.0,>=1.27.0
+mypy-boto3-codepipeline<1.29.0,>=1.28.0
 
 [codestar]
-mypy-boto3-codestar<1.28.0,>=1.27.0
+mypy-boto3-codestar<1.29.0,>=1.28.0
 
 [codestar-connections]
-mypy-boto3-codestar-connections<1.28.0,>=1.27.0
+mypy-boto3-codestar-connections<1.29.0,>=1.28.0
 
 [codestar-notifications]
-mypy-boto3-codestar-notifications<1.28.0,>=1.27.0
+mypy-boto3-codestar-notifications<1.29.0,>=1.28.0
 
 [cognito-identity]
-mypy-boto3-cognito-identity<1.28.0,>=1.27.0
+mypy-boto3-cognito-identity<1.29.0,>=1.28.0
 
 [cognito-idp]
-mypy-boto3-cognito-idp<1.28.0,>=1.27.0
+mypy-boto3-cognito-idp<1.29.0,>=1.28.0
 
 [cognito-sync]
-mypy-boto3-cognito-sync<1.28.0,>=1.27.0
+mypy-boto3-cognito-sync<1.29.0,>=1.28.0
 
 [comprehend]
-mypy-boto3-comprehend<1.28.0,>=1.27.0
+mypy-boto3-comprehend<1.29.0,>=1.28.0
 
 [comprehendmedical]
-mypy-boto3-comprehendmedical<1.28.0,>=1.27.0
+mypy-boto3-comprehendmedical<1.29.0,>=1.28.0
 
 [compute-optimizer]
-mypy-boto3-compute-optimizer<1.28.0,>=1.27.0
+mypy-boto3-compute-optimizer<1.29.0,>=1.28.0
 
 [config]
-mypy-boto3-config<1.28.0,>=1.27.0
+mypy-boto3-config<1.29.0,>=1.28.0
 
 [connect]
-mypy-boto3-connect<1.28.0,>=1.27.0
+mypy-boto3-connect<1.29.0,>=1.28.0
 
 [connect-contact-lens]
-mypy-boto3-connect-contact-lens<1.28.0,>=1.27.0
+mypy-boto3-connect-contact-lens<1.29.0,>=1.28.0
 
 [connectcampaigns]
-mypy-boto3-connectcampaigns<1.28.0,>=1.27.0
+mypy-boto3-connectcampaigns<1.29.0,>=1.28.0
 
 [connectcases]
-mypy-boto3-connectcases<1.28.0,>=1.27.0
+mypy-boto3-connectcases<1.29.0,>=1.28.0
 
 [connectparticipant]
-mypy-boto3-connectparticipant<1.28.0,>=1.27.0
+mypy-boto3-connectparticipant<1.29.0,>=1.28.0
 
 [controltower]
-mypy-boto3-controltower<1.28.0,>=1.27.0
+mypy-boto3-controltower<1.29.0,>=1.28.0
 
 [cur]
-mypy-boto3-cur<1.28.0,>=1.27.0
+mypy-boto3-cur<1.29.0,>=1.28.0
 
 [customer-profiles]
-mypy-boto3-customer-profiles<1.28.0,>=1.27.0
+mypy-boto3-customer-profiles<1.29.0,>=1.28.0
 
 [databrew]
-mypy-boto3-databrew<1.28.0,>=1.27.0
+mypy-boto3-databrew<1.29.0,>=1.28.0
 
 [dataexchange]
-mypy-boto3-dataexchange<1.28.0,>=1.27.0
+mypy-boto3-dataexchange<1.29.0,>=1.28.0
 
 [datapipeline]
-mypy-boto3-datapipeline<1.28.0,>=1.27.0
+mypy-boto3-datapipeline<1.29.0,>=1.28.0
 
 [datasync]
-mypy-boto3-datasync<1.28.0,>=1.27.0
+mypy-boto3-datasync<1.29.0,>=1.28.0
 
 [dax]
-mypy-boto3-dax<1.28.0,>=1.27.0
+mypy-boto3-dax<1.29.0,>=1.28.0
 
 [detective]
-mypy-boto3-detective<1.28.0,>=1.27.0
+mypy-boto3-detective<1.29.0,>=1.28.0
 
 [devicefarm]
-mypy-boto3-devicefarm<1.28.0,>=1.27.0
+mypy-boto3-devicefarm<1.29.0,>=1.28.0
 
 [devops-guru]
-mypy-boto3-devops-guru<1.28.0,>=1.27.0
+mypy-boto3-devops-guru<1.29.0,>=1.28.0
 
 [directconnect]
-mypy-boto3-directconnect<1.28.0,>=1.27.0
+mypy-boto3-directconnect<1.29.0,>=1.28.0
 
 [discovery]
-mypy-boto3-discovery<1.28.0,>=1.27.0
+mypy-boto3-discovery<1.29.0,>=1.28.0
 
 [dlm]
-mypy-boto3-dlm<1.28.0,>=1.27.0
+mypy-boto3-dlm<1.29.0,>=1.28.0
 
 [dms]
-mypy-boto3-dms<1.28.0,>=1.27.0
+mypy-boto3-dms<1.29.0,>=1.28.0
 
 [docdb]
-mypy-boto3-docdb<1.28.0,>=1.27.0
+mypy-boto3-docdb<1.29.0,>=1.28.0
 
 [docdb-elastic]
-mypy-boto3-docdb-elastic<1.28.0,>=1.27.0
+mypy-boto3-docdb-elastic<1.29.0,>=1.28.0
 
 [drs]
-mypy-boto3-drs<1.28.0,>=1.27.0
+mypy-boto3-drs<1.29.0,>=1.28.0
 
 [ds]
-mypy-boto3-ds<1.28.0,>=1.27.0
+mypy-boto3-ds<1.29.0,>=1.28.0
 
 [dynamodb]
-mypy-boto3-dynamodb<1.28.0,>=1.27.0
+mypy-boto3-dynamodb<1.29.0,>=1.28.0
 
 [dynamodbstreams]
-mypy-boto3-dynamodbstreams<1.28.0,>=1.27.0
+mypy-boto3-dynamodbstreams<1.29.0,>=1.28.0
 
 [ebs]
-mypy-boto3-ebs<1.28.0,>=1.27.0
+mypy-boto3-ebs<1.29.0,>=1.28.0
 
 [ec2]
-mypy-boto3-ec2<1.28.0,>=1.27.0
+mypy-boto3-ec2<1.29.0,>=1.28.0
 
 [ec2-instance-connect]
-mypy-boto3-ec2-instance-connect<1.28.0,>=1.27.0
+mypy-boto3-ec2-instance-connect<1.29.0,>=1.28.0
 
 [ecr]
-mypy-boto3-ecr<1.28.0,>=1.27.0
+mypy-boto3-ecr<1.29.0,>=1.28.0
 
 [ecr-public]
-mypy-boto3-ecr-public<1.28.0,>=1.27.0
+mypy-boto3-ecr-public<1.29.0,>=1.28.0
 
 [ecs]
-mypy-boto3-ecs<1.28.0,>=1.27.0
+mypy-boto3-ecs<1.29.0,>=1.28.0
 
 [efs]
-mypy-boto3-efs<1.28.0,>=1.27.0
+mypy-boto3-efs<1.29.0,>=1.28.0
 
 [eks]
-mypy-boto3-eks<1.28.0,>=1.27.0
+mypy-boto3-eks<1.29.0,>=1.28.0
 
 [elastic-inference]
-mypy-boto3-elastic-inference<1.28.0,>=1.27.0
+mypy-boto3-elastic-inference<1.29.0,>=1.28.0
 
 [elasticache]
-mypy-boto3-elasticache<1.28.0,>=1.27.0
+mypy-boto3-elasticache<1.29.0,>=1.28.0
 
 [elasticbeanstalk]
-mypy-boto3-elasticbeanstalk<1.28.0,>=1.27.0
+mypy-boto3-elasticbeanstalk<1.29.0,>=1.28.0
 
 [elastictranscoder]
-mypy-boto3-elastictranscoder<1.28.0,>=1.27.0
+mypy-boto3-elastictranscoder<1.29.0,>=1.28.0
 
 [elb]
-mypy-boto3-elb<1.28.0,>=1.27.0
+mypy-boto3-elb<1.29.0,>=1.28.0
 
 [elbv2]
-mypy-boto3-elbv2<1.28.0,>=1.27.0
+mypy-boto3-elbv2<1.29.0,>=1.28.0
 
 [emr]
-mypy-boto3-emr<1.28.0,>=1.27.0
+mypy-boto3-emr<1.29.0,>=1.28.0
 
 [emr-containers]
-mypy-boto3-emr-containers<1.28.0,>=1.27.0
+mypy-boto3-emr-containers<1.29.0,>=1.28.0
 
 [emr-serverless]
-mypy-boto3-emr-serverless<1.28.0,>=1.27.0
+mypy-boto3-emr-serverless<1.29.0,>=1.28.0
 
 [es]
-mypy-boto3-es<1.28.0,>=1.27.0
+mypy-boto3-es<1.29.0,>=1.28.0
 
 [essential]
-mypy-boto3-cloudformation<1.28.0,>=1.27.0
-mypy-boto3-dynamodb<1.28.0,>=1.27.0
-mypy-boto3-ec2<1.28.0,>=1.27.0
-mypy-boto3-lambda<1.28.0,>=1.27.0
-mypy-boto3-rds<1.28.0,>=1.27.0
-mypy-boto3-s3<1.28.0,>=1.27.0
-mypy-boto3-sqs<1.28.0,>=1.27.0
+mypy-boto3-cloudformation<1.29.0,>=1.28.0
+mypy-boto3-dynamodb<1.29.0,>=1.28.0
+mypy-boto3-ec2<1.29.0,>=1.28.0
+mypy-boto3-lambda<1.29.0,>=1.28.0
+mypy-boto3-rds<1.29.0,>=1.28.0
+mypy-boto3-s3<1.29.0,>=1.28.0
+mypy-boto3-sqs<1.29.0,>=1.28.0
 
 [events]
-mypy-boto3-events<1.28.0,>=1.27.0
+mypy-boto3-events<1.29.0,>=1.28.0
 
 [evidently]
-mypy-boto3-evidently<1.28.0,>=1.27.0
+mypy-boto3-evidently<1.29.0,>=1.28.0
 
 [finspace]
-mypy-boto3-finspace<1.28.0,>=1.27.0
+mypy-boto3-finspace<1.29.0,>=1.28.0
 
 [finspace-data]
-mypy-boto3-finspace-data<1.28.0,>=1.27.0
+mypy-boto3-finspace-data<1.29.0,>=1.28.0
 
 [firehose]
-mypy-boto3-firehose<1.28.0,>=1.27.0
+mypy-boto3-firehose<1.29.0,>=1.28.0
 
 [fis]
-mypy-boto3-fis<1.28.0,>=1.27.0
+mypy-boto3-fis<1.29.0,>=1.28.0
 
 [fms]
-mypy-boto3-fms<1.28.0,>=1.27.0
+mypy-boto3-fms<1.29.0,>=1.28.0
 
 [forecast]
-mypy-boto3-forecast<1.28.0,>=1.27.0
+mypy-boto3-forecast<1.29.0,>=1.28.0
 
 [forecastquery]
-mypy-boto3-forecastquery<1.28.0,>=1.27.0
+mypy-boto3-forecastquery<1.29.0,>=1.28.0
 
 [frauddetector]
-mypy-boto3-frauddetector<1.28.0,>=1.27.0
+mypy-boto3-frauddetector<1.29.0,>=1.28.0
 
 [fsx]
-mypy-boto3-fsx<1.28.0,>=1.27.0
+mypy-boto3-fsx<1.29.0,>=1.28.0
 
 [gamelift]
-mypy-boto3-gamelift<1.28.0,>=1.27.0
+mypy-boto3-gamelift<1.29.0,>=1.28.0
 
 [gamesparks]
-mypy-boto3-gamesparks<1.28.0,>=1.27.0
+mypy-boto3-gamesparks<1.29.0,>=1.28.0
 
 [glacier]
-mypy-boto3-glacier<1.28.0,>=1.27.0
+mypy-boto3-glacier<1.29.0,>=1.28.0
 
 [globalaccelerator]
-mypy-boto3-globalaccelerator<1.28.0,>=1.27.0
+mypy-boto3-globalaccelerator<1.29.0,>=1.28.0
 
 [glue]
-mypy-boto3-glue<1.28.0,>=1.27.0
+mypy-boto3-glue<1.29.0,>=1.28.0
 
 [grafana]
-mypy-boto3-grafana<1.28.0,>=1.27.0
+mypy-boto3-grafana<1.29.0,>=1.28.0
 
 [greengrass]
-mypy-boto3-greengrass<1.28.0,>=1.27.0
+mypy-boto3-greengrass<1.29.0,>=1.28.0
 
 [greengrassv2]
-mypy-boto3-greengrassv2<1.28.0,>=1.27.0
+mypy-boto3-greengrassv2<1.29.0,>=1.28.0
 
 [groundstation]
-mypy-boto3-groundstation<1.28.0,>=1.27.0
+mypy-boto3-groundstation<1.29.0,>=1.28.0
 
 [guardduty]
-mypy-boto3-guardduty<1.28.0,>=1.27.0
+mypy-boto3-guardduty<1.29.0,>=1.28.0
 
 [health]
-mypy-boto3-health<1.28.0,>=1.27.0
+mypy-boto3-health<1.29.0,>=1.28.0
 
 [healthlake]
-mypy-boto3-healthlake<1.28.0,>=1.27.0
+mypy-boto3-healthlake<1.29.0,>=1.28.0
 
 [honeycode]
-mypy-boto3-honeycode<1.28.0,>=1.27.0
+mypy-boto3-honeycode<1.29.0,>=1.28.0
 
 [iam]
-mypy-boto3-iam<1.28.0,>=1.27.0
+mypy-boto3-iam<1.29.0,>=1.28.0
 
 [identitystore]
-mypy-boto3-identitystore<1.28.0,>=1.27.0
+mypy-boto3-identitystore<1.29.0,>=1.28.0
 
 [imagebuilder]
-mypy-boto3-imagebuilder<1.28.0,>=1.27.0
+mypy-boto3-imagebuilder<1.29.0,>=1.28.0
 
 [importexport]
-mypy-boto3-importexport<1.28.0,>=1.27.0
+mypy-boto3-importexport<1.29.0,>=1.28.0
 
 [inspector]
-mypy-boto3-inspector<1.28.0,>=1.27.0
+mypy-boto3-inspector<1.29.0,>=1.28.0
 
 [inspector2]
-mypy-boto3-inspector2<1.28.0,>=1.27.0
+mypy-boto3-inspector2<1.29.0,>=1.28.0
 
 [internetmonitor]
-mypy-boto3-internetmonitor<1.28.0,>=1.27.0
+mypy-boto3-internetmonitor<1.29.0,>=1.28.0
 
 [iot]
-mypy-boto3-iot<1.28.0,>=1.27.0
+mypy-boto3-iot<1.29.0,>=1.28.0
 
 [iot-data]
-mypy-boto3-iot-data<1.28.0,>=1.27.0
+mypy-boto3-iot-data<1.29.0,>=1.28.0
 
 [iot-jobs-data]
-mypy-boto3-iot-jobs-data<1.28.0,>=1.27.0
+mypy-boto3-iot-jobs-data<1.29.0,>=1.28.0
 
 [iot-roborunner]
-mypy-boto3-iot-roborunner<1.28.0,>=1.27.0
+mypy-boto3-iot-roborunner<1.29.0,>=1.28.0
 
 [iot1click-devices]
-mypy-boto3-iot1click-devices<1.28.0,>=1.27.0
+mypy-boto3-iot1click-devices<1.29.0,>=1.28.0
 
 [iot1click-projects]
-mypy-boto3-iot1click-projects<1.28.0,>=1.27.0
+mypy-boto3-iot1click-projects<1.29.0,>=1.28.0
 
 [iotanalytics]
-mypy-boto3-iotanalytics<1.28.0,>=1.27.0
+mypy-boto3-iotanalytics<1.29.0,>=1.28.0
 
 [iotdeviceadvisor]
-mypy-boto3-iotdeviceadvisor<1.28.0,>=1.27.0
+mypy-boto3-iotdeviceadvisor<1.29.0,>=1.28.0
 
 [iotevents]
-mypy-boto3-iotevents<1.28.0,>=1.27.0
+mypy-boto3-iotevents<1.29.0,>=1.28.0
 
 [iotevents-data]
-mypy-boto3-iotevents-data<1.28.0,>=1.27.0
+mypy-boto3-iotevents-data<1.29.0,>=1.28.0
 
 [iotfleethub]
-mypy-boto3-iotfleethub<1.28.0,>=1.27.0
+mypy-boto3-iotfleethub<1.29.0,>=1.28.0
 
 [iotfleetwise]
-mypy-boto3-iotfleetwise<1.28.0,>=1.27.0
+mypy-boto3-iotfleetwise<1.29.0,>=1.28.0
 
 [iotsecuretunneling]
-mypy-boto3-iotsecuretunneling<1.28.0,>=1.27.0
+mypy-boto3-iotsecuretunneling<1.29.0,>=1.28.0
 
 [iotsitewise]
-mypy-boto3-iotsitewise<1.28.0,>=1.27.0
+mypy-boto3-iotsitewise<1.29.0,>=1.28.0
 
 [iotthingsgraph]
-mypy-boto3-iotthingsgraph<1.28.0,>=1.27.0
+mypy-boto3-iotthingsgraph<1.29.0,>=1.28.0
 
 [iottwinmaker]
-mypy-boto3-iottwinmaker<1.28.0,>=1.27.0
+mypy-boto3-iottwinmaker<1.29.0,>=1.28.0
 
 [iotwireless]
-mypy-boto3-iotwireless<1.28.0,>=1.27.0
+mypy-boto3-iotwireless<1.29.0,>=1.28.0
 
 [ivs]
-mypy-boto3-ivs<1.28.0,>=1.27.0
+mypy-boto3-ivs<1.29.0,>=1.28.0
 
 [ivs-realtime]
-mypy-boto3-ivs-realtime<1.28.0,>=1.27.0
+mypy-boto3-ivs-realtime<1.29.0,>=1.28.0
 
 [ivschat]
-mypy-boto3-ivschat<1.28.0,>=1.27.0
+mypy-boto3-ivschat<1.29.0,>=1.28.0
 
 [kafka]
-mypy-boto3-kafka<1.28.0,>=1.27.0
+mypy-boto3-kafka<1.29.0,>=1.28.0
 
 [kafkaconnect]
-mypy-boto3-kafkaconnect<1.28.0,>=1.27.0
+mypy-boto3-kafkaconnect<1.29.0,>=1.28.0
 
 [kendra]
-mypy-boto3-kendra<1.28.0,>=1.27.0
+mypy-boto3-kendra<1.29.0,>=1.28.0
 
 [kendra-ranking]
-mypy-boto3-kendra-ranking<1.28.0,>=1.27.0
+mypy-boto3-kendra-ranking<1.29.0,>=1.28.0
 
 [keyspaces]
-mypy-boto3-keyspaces<1.28.0,>=1.27.0
+mypy-boto3-keyspaces<1.29.0,>=1.28.0
 
 [kinesis]
-mypy-boto3-kinesis<1.28.0,>=1.27.0
+mypy-boto3-kinesis<1.29.0,>=1.28.0
 
 [kinesis-video-archived-media]
-mypy-boto3-kinesis-video-archived-media<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-archived-media<1.29.0,>=1.28.0
 
 [kinesis-video-media]
-mypy-boto3-kinesis-video-media<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-media<1.29.0,>=1.28.0
 
 [kinesis-video-signaling]
-mypy-boto3-kinesis-video-signaling<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-signaling<1.29.0,>=1.28.0
 
 [kinesis-video-webrtc-storage]
-mypy-boto3-kinesis-video-webrtc-storage<1.28.0,>=1.27.0
+mypy-boto3-kinesis-video-webrtc-storage<1.29.0,>=1.28.0
 
 [kinesisanalytics]
-mypy-boto3-kinesisanalytics<1.28.0,>=1.27.0
+mypy-boto3-kinesisanalytics<1.29.0,>=1.28.0
 
 [kinesisanalyticsv2]
-mypy-boto3-kinesisanalyticsv2<1.28.0,>=1.27.0
+mypy-boto3-kinesisanalyticsv2<1.29.0,>=1.28.0
 
 [kinesisvideo]
-mypy-boto3-kinesisvideo<1.28.0,>=1.27.0
+mypy-boto3-kinesisvideo<1.29.0,>=1.28.0
 
 [kms]
-mypy-boto3-kms<1.28.0,>=1.27.0
+mypy-boto3-kms<1.29.0,>=1.28.0
 
 [lakeformation]
-mypy-boto3-lakeformation<1.28.0,>=1.27.0
+mypy-boto3-lakeformation<1.29.0,>=1.28.0
 
 [lambda]
-mypy-boto3-lambda<1.28.0,>=1.27.0
+mypy-boto3-lambda<1.29.0,>=1.28.0
 
 [lex-models]
-mypy-boto3-lex-models<1.28.0,>=1.27.0
+mypy-boto3-lex-models<1.29.0,>=1.28.0
 
 [lex-runtime]
-mypy-boto3-lex-runtime<1.28.0,>=1.27.0
+mypy-boto3-lex-runtime<1.29.0,>=1.28.0
 
 [lexv2-models]
-mypy-boto3-lexv2-models<1.28.0,>=1.27.0
+mypy-boto3-lexv2-models<1.29.0,>=1.28.0
 
 [lexv2-runtime]
-mypy-boto3-lexv2-runtime<1.28.0,>=1.27.0
+mypy-boto3-lexv2-runtime<1.29.0,>=1.28.0
 
 [license-manager]
-mypy-boto3-license-manager<1.28.0,>=1.27.0
+mypy-boto3-license-manager<1.29.0,>=1.28.0
 
 [license-manager-linux-subscriptions]
-mypy-boto3-license-manager-linux-subscriptions<1.28.0,>=1.27.0
+mypy-boto3-license-manager-linux-subscriptions<1.29.0,>=1.28.0
 
 [license-manager-user-subscriptions]
-mypy-boto3-license-manager-user-subscriptions<1.28.0,>=1.27.0
+mypy-boto3-license-manager-user-subscriptions<1.29.0,>=1.28.0
 
 [lightsail]
-mypy-boto3-lightsail<1.28.0,>=1.27.0
+mypy-boto3-lightsail<1.29.0,>=1.28.0
 
 [location]
-mypy-boto3-location<1.28.0,>=1.27.0
+mypy-boto3-location<1.29.0,>=1.28.0
 
 [logs]
-mypy-boto3-logs<1.28.0,>=1.27.0
+mypy-boto3-logs<1.29.0,>=1.28.0
 
 [lookoutequipment]
-mypy-boto3-lookoutequipment<1.28.0,>=1.27.0
+mypy-boto3-lookoutequipment<1.29.0,>=1.28.0
 
 [lookoutmetrics]
-mypy-boto3-lookoutmetrics<1.28.0,>=1.27.0
+mypy-boto3-lookoutmetrics<1.29.0,>=1.28.0
 
 [lookoutvision]
-mypy-boto3-lookoutvision<1.28.0,>=1.27.0
+mypy-boto3-lookoutvision<1.29.0,>=1.28.0
 
 [m2]
-mypy-boto3-m2<1.28.0,>=1.27.0
+mypy-boto3-m2<1.29.0,>=1.28.0
 
 [machinelearning]
-mypy-boto3-machinelearning<1.28.0,>=1.27.0
+mypy-boto3-machinelearning<1.29.0,>=1.28.0
 
 [macie]
-mypy-boto3-macie<1.28.0,>=1.27.0
+mypy-boto3-macie<1.29.0,>=1.28.0
 
 [macie2]
-mypy-boto3-macie2<1.28.0,>=1.27.0
+mypy-boto3-macie2<1.29.0,>=1.28.0
 
 [managedblockchain]
-mypy-boto3-managedblockchain<1.28.0,>=1.27.0
+mypy-boto3-managedblockchain<1.29.0,>=1.28.0
 
 [marketplace-catalog]
-mypy-boto3-marketplace-catalog<1.28.0,>=1.27.0
+mypy-boto3-marketplace-catalog<1.29.0,>=1.28.0
 
 [marketplace-entitlement]
-mypy-boto3-marketplace-entitlement<1.28.0,>=1.27.0
+mypy-boto3-marketplace-entitlement<1.29.0,>=1.28.0
 
 [marketplacecommerceanalytics]
-mypy-boto3-marketplacecommerceanalytics<1.28.0,>=1.27.0
+mypy-boto3-marketplacecommerceanalytics<1.29.0,>=1.28.0
 
 [mediaconnect]
-mypy-boto3-mediaconnect<1.28.0,>=1.27.0
+mypy-boto3-mediaconnect<1.29.0,>=1.28.0
 
 [mediaconvert]
-mypy-boto3-mediaconvert<1.28.0,>=1.27.0
+mypy-boto3-mediaconvert<1.29.0,>=1.28.0
 
 [medialive]
-mypy-boto3-medialive<1.28.0,>=1.27.0
+mypy-boto3-medialive<1.29.0,>=1.28.0
 
 [mediapackage]
-mypy-boto3-mediapackage<1.28.0,>=1.27.0
+mypy-boto3-mediapackage<1.29.0,>=1.28.0
 
 [mediapackage-vod]
-mypy-boto3-mediapackage-vod<1.28.0,>=1.27.0
+mypy-boto3-mediapackage-vod<1.29.0,>=1.28.0
 
 [mediapackagev2]
-mypy-boto3-mediapackagev2<1.28.0,>=1.27.0
+mypy-boto3-mediapackagev2<1.29.0,>=1.28.0
 
 [mediastore]
-mypy-boto3-mediastore<1.28.0,>=1.27.0
+mypy-boto3-mediastore<1.29.0,>=1.28.0
 
 [mediastore-data]
-mypy-boto3-mediastore-data<1.28.0,>=1.27.0
+mypy-boto3-mediastore-data<1.29.0,>=1.28.0
 
 [mediatailor]
-mypy-boto3-mediatailor<1.28.0,>=1.27.0
+mypy-boto3-mediatailor<1.29.0,>=1.28.0
 
 [memorydb]
-mypy-boto3-memorydb<1.28.0,>=1.27.0
+mypy-boto3-memorydb<1.29.0,>=1.28.0
 
 [meteringmarketplace]
-mypy-boto3-meteringmarketplace<1.28.0,>=1.27.0
+mypy-boto3-meteringmarketplace<1.29.0,>=1.28.0
 
 [mgh]
-mypy-boto3-mgh<1.28.0,>=1.27.0
+mypy-boto3-mgh<1.29.0,>=1.28.0
 
 [mgn]
-mypy-boto3-mgn<1.28.0,>=1.27.0
+mypy-boto3-mgn<1.29.0,>=1.28.0
 
 [migration-hub-refactor-spaces]
-mypy-boto3-migration-hub-refactor-spaces<1.28.0,>=1.27.0
+mypy-boto3-migration-hub-refactor-spaces<1.29.0,>=1.28.0
 
 [migrationhub-config]
-mypy-boto3-migrationhub-config<1.28.0,>=1.27.0
+mypy-boto3-migrationhub-config<1.29.0,>=1.28.0
 
 [migrationhuborchestrator]
-mypy-boto3-migrationhuborchestrator<1.28.0,>=1.27.0
+mypy-boto3-migrationhuborchestrator<1.29.0,>=1.28.0
 
 [migrationhubstrategy]
-mypy-boto3-migrationhubstrategy<1.28.0,>=1.27.0
+mypy-boto3-migrationhubstrategy<1.29.0,>=1.28.0
 
 [mobile]
-mypy-boto3-mobile<1.28.0,>=1.27.0
+mypy-boto3-mobile<1.29.0,>=1.28.0
 
 [mq]
-mypy-boto3-mq<1.28.0,>=1.27.0
+mypy-boto3-mq<1.29.0,>=1.28.0
 
 [mturk]
-mypy-boto3-mturk<1.28.0,>=1.27.0
+mypy-boto3-mturk<1.29.0,>=1.28.0
 
 [mwaa]
-mypy-boto3-mwaa<1.28.0,>=1.27.0
+mypy-boto3-mwaa<1.29.0,>=1.28.0
 
 [neptune]
-mypy-boto3-neptune<1.28.0,>=1.27.0
+mypy-boto3-neptune<1.29.0,>=1.28.0
 
 [network-firewall]
-mypy-boto3-network-firewall<1.28.0,>=1.27.0
+mypy-boto3-network-firewall<1.29.0,>=1.28.0
 
 [networkmanager]
-mypy-boto3-networkmanager<1.28.0,>=1.27.0
+mypy-boto3-networkmanager<1.29.0,>=1.28.0
 
 [nimble]
-mypy-boto3-nimble<1.28.0,>=1.27.0
+mypy-boto3-nimble<1.29.0,>=1.28.0
 
 [oam]
-mypy-boto3-oam<1.28.0,>=1.27.0
+mypy-boto3-oam<1.29.0,>=1.28.0
 
 [omics]
-mypy-boto3-omics<1.28.0,>=1.27.0
+mypy-boto3-omics<1.29.0,>=1.28.0
 
 [opensearch]
-mypy-boto3-opensearch<1.28.0,>=1.27.0
+mypy-boto3-opensearch<1.29.0,>=1.28.0
 
 [opensearchserverless]
-mypy-boto3-opensearchserverless<1.28.0,>=1.27.0
+mypy-boto3-opensearchserverless<1.29.0,>=1.28.0
 
 [opsworks]
-mypy-boto3-opsworks<1.28.0,>=1.27.0
+mypy-boto3-opsworks<1.29.0,>=1.28.0
 
 [opsworkscm]
-mypy-boto3-opsworkscm<1.28.0,>=1.27.0
+mypy-boto3-opsworkscm<1.29.0,>=1.28.0
 
 [organizations]
-mypy-boto3-organizations<1.28.0,>=1.27.0
+mypy-boto3-organizations<1.29.0,>=1.28.0
 
 [osis]
-mypy-boto3-osis<1.28.0,>=1.27.0
+mypy-boto3-osis<1.29.0,>=1.28.0
 
 [outposts]
-mypy-boto3-outposts<1.28.0,>=1.27.0
+mypy-boto3-outposts<1.29.0,>=1.28.0
 
 [panorama]
-mypy-boto3-panorama<1.28.0,>=1.27.0
+mypy-boto3-panorama<1.29.0,>=1.28.0
 
 [payment-cryptography]
-mypy-boto3-payment-cryptography<1.28.0,>=1.27.0
+mypy-boto3-payment-cryptography<1.29.0,>=1.28.0
 
 [payment-cryptography-data]
-mypy-boto3-payment-cryptography-data<1.28.0,>=1.27.0
+mypy-boto3-payment-cryptography-data<1.29.0,>=1.28.0
 
 [personalize]
-mypy-boto3-personalize<1.28.0,>=1.27.0
+mypy-boto3-personalize<1.29.0,>=1.28.0
 
 [personalize-events]
-mypy-boto3-personalize-events<1.28.0,>=1.27.0
+mypy-boto3-personalize-events<1.29.0,>=1.28.0
 
 [personalize-runtime]
-mypy-boto3-personalize-runtime<1.28.0,>=1.27.0
+mypy-boto3-personalize-runtime<1.29.0,>=1.28.0
 
 [pi]
-mypy-boto3-pi<1.28.0,>=1.27.0
+mypy-boto3-pi<1.29.0,>=1.28.0
 
 [pinpoint]
-mypy-boto3-pinpoint<1.28.0,>=1.27.0
+mypy-boto3-pinpoint<1.29.0,>=1.28.0
 
 [pinpoint-email]
-mypy-boto3-pinpoint-email<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-email<1.29.0,>=1.28.0
 
 [pinpoint-sms-voice]
-mypy-boto3-pinpoint-sms-voice<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-sms-voice<1.29.0,>=1.28.0
 
 [pinpoint-sms-voice-v2]
-mypy-boto3-pinpoint-sms-voice-v2<1.28.0,>=1.27.0
+mypy-boto3-pinpoint-sms-voice-v2<1.29.0,>=1.28.0
 
 [pipes]
-mypy-boto3-pipes<1.28.0,>=1.27.0
+mypy-boto3-pipes<1.29.0,>=1.28.0
 
 [polly]
-mypy-boto3-polly<1.28.0,>=1.27.0
+mypy-boto3-polly<1.29.0,>=1.28.0
 
 [pricing]
-mypy-boto3-pricing<1.28.0,>=1.27.0
+mypy-boto3-pricing<1.29.0,>=1.28.0
 
 [privatenetworks]
-mypy-boto3-privatenetworks<1.28.0,>=1.27.0
+mypy-boto3-privatenetworks<1.29.0,>=1.28.0
 
 [proton]
-mypy-boto3-proton<1.28.0,>=1.27.0
+mypy-boto3-proton<1.29.0,>=1.28.0
 
 [qldb]
-mypy-boto3-qldb<1.28.0,>=1.27.0
+mypy-boto3-qldb<1.29.0,>=1.28.0
 
 [qldb-session]
-mypy-boto3-qldb-session<1.28.0,>=1.27.0
+mypy-boto3-qldb-session<1.29.0,>=1.28.0
 
 [quicksight]
-mypy-boto3-quicksight<1.28.0,>=1.27.0
+mypy-boto3-quicksight<1.29.0,>=1.28.0
 
 [ram]
-mypy-boto3-ram<1.28.0,>=1.27.0
+mypy-boto3-ram<1.29.0,>=1.28.0
 
 [rbin]
-mypy-boto3-rbin<1.28.0,>=1.27.0
+mypy-boto3-rbin<1.29.0,>=1.28.0
 
 [rds]
-mypy-boto3-rds<1.28.0,>=1.27.0
+mypy-boto3-rds<1.29.0,>=1.28.0
 
 [rds-data]
-mypy-boto3-rds-data<1.28.0,>=1.27.0
+mypy-boto3-rds-data<1.29.0,>=1.28.0
 
 [redshift]
-mypy-boto3-redshift<1.28.0,>=1.27.0
+mypy-boto3-redshift<1.29.0,>=1.28.0
 
 [redshift-data]
-mypy-boto3-redshift-data<1.28.0,>=1.27.0
+mypy-boto3-redshift-data<1.29.0,>=1.28.0
 
 [redshift-serverless]
-mypy-boto3-redshift-serverless<1.28.0,>=1.27.0
+mypy-boto3-redshift-serverless<1.29.0,>=1.28.0
 
 [rekognition]
-mypy-boto3-rekognition<1.28.0,>=1.27.0
+mypy-boto3-rekognition<1.29.0,>=1.28.0
 
 [resiliencehub]
-mypy-boto3-resiliencehub<1.28.0,>=1.27.0
+mypy-boto3-resiliencehub<1.29.0,>=1.28.0
 
 [resource-explorer-2]
-mypy-boto3-resource-explorer-2<1.28.0,>=1.27.0
+mypy-boto3-resource-explorer-2<1.29.0,>=1.28.0
 
 [resource-groups]
-mypy-boto3-resource-groups<1.28.0,>=1.27.0
+mypy-boto3-resource-groups<1.29.0,>=1.28.0
 
 [resourcegroupstaggingapi]
-mypy-boto3-resourcegroupstaggingapi<1.28.0,>=1.27.0
+mypy-boto3-resourcegroupstaggingapi<1.29.0,>=1.28.0
 
 [robomaker]
-mypy-boto3-robomaker<1.28.0,>=1.27.0
+mypy-boto3-robomaker<1.29.0,>=1.28.0
 
 [rolesanywhere]
-mypy-boto3-rolesanywhere<1.28.0,>=1.27.0
+mypy-boto3-rolesanywhere<1.29.0,>=1.28.0
 
 [route53]
-mypy-boto3-route53<1.28.0,>=1.27.0
+mypy-boto3-route53<1.29.0,>=1.28.0
 
 [route53-recovery-cluster]
-mypy-boto3-route53-recovery-cluster<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-cluster<1.29.0,>=1.28.0
 
 [route53-recovery-control-config]
-mypy-boto3-route53-recovery-control-config<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-control-config<1.29.0,>=1.28.0
 
 [route53-recovery-readiness]
-mypy-boto3-route53-recovery-readiness<1.28.0,>=1.27.0
+mypy-boto3-route53-recovery-readiness<1.29.0,>=1.28.0
 
 [route53domains]
-mypy-boto3-route53domains<1.28.0,>=1.27.0
+mypy-boto3-route53domains<1.29.0,>=1.28.0
 
 [route53resolver]
-mypy-boto3-route53resolver<1.28.0,>=1.27.0
+mypy-boto3-route53resolver<1.29.0,>=1.28.0
 
 [rum]
-mypy-boto3-rum<1.28.0,>=1.27.0
+mypy-boto3-rum<1.29.0,>=1.28.0
 
 [s3]
-mypy-boto3-s3<1.28.0,>=1.27.0
+mypy-boto3-s3<1.29.0,>=1.28.0
 
 [s3control]
-mypy-boto3-s3control<1.28.0,>=1.27.0
+mypy-boto3-s3control<1.29.0,>=1.28.0
 
 [s3outposts]
-mypy-boto3-s3outposts<1.28.0,>=1.27.0
+mypy-boto3-s3outposts<1.29.0,>=1.28.0
 
 [sagemaker]
-mypy-boto3-sagemaker<1.28.0,>=1.27.0
+mypy-boto3-sagemaker<1.29.0,>=1.28.0
 
 [sagemaker-a2i-runtime]
-mypy-boto3-sagemaker-a2i-runtime<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-a2i-runtime<1.29.0,>=1.28.0
 
 [sagemaker-edge]
-mypy-boto3-sagemaker-edge<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-edge<1.29.0,>=1.28.0
 
 [sagemaker-featurestore-runtime]
-mypy-boto3-sagemaker-featurestore-runtime<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-featurestore-runtime<1.29.0,>=1.28.0
 
 [sagemaker-geospatial]
-mypy-boto3-sagemaker-geospatial<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-geospatial<1.29.0,>=1.28.0
 
 [sagemaker-metrics]
-mypy-boto3-sagemaker-metrics<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-metrics<1.29.0,>=1.28.0
 
 [sagemaker-runtime]
-mypy-boto3-sagemaker-runtime<1.28.0,>=1.27.0
+mypy-boto3-sagemaker-runtime<1.29.0,>=1.28.0
 
 [savingsplans]
-mypy-boto3-savingsplans<1.28.0,>=1.27.0
+mypy-boto3-savingsplans<1.29.0,>=1.28.0
 
 [scheduler]
-mypy-boto3-scheduler<1.28.0,>=1.27.0
+mypy-boto3-scheduler<1.29.0,>=1.28.0
 
 [schemas]
-mypy-boto3-schemas<1.28.0,>=1.27.0
+mypy-boto3-schemas<1.29.0,>=1.28.0
 
 [sdb]
-mypy-boto3-sdb<1.28.0,>=1.27.0
+mypy-boto3-sdb<1.29.0,>=1.28.0
 
 [secretsmanager]
-mypy-boto3-secretsmanager<1.28.0,>=1.27.0
+mypy-boto3-secretsmanager<1.29.0,>=1.28.0
 
 [securityhub]
-mypy-boto3-securityhub<1.28.0,>=1.27.0
+mypy-boto3-securityhub<1.29.0,>=1.28.0
 
 [securitylake]
-mypy-boto3-securitylake<1.28.0,>=1.27.0
+mypy-boto3-securitylake<1.29.0,>=1.28.0
 
 [serverlessrepo]
-mypy-boto3-serverlessrepo<1.28.0,>=1.27.0
+mypy-boto3-serverlessrepo<1.29.0,>=1.28.0
 
 [service-quotas]
-mypy-boto3-service-quotas<1.28.0,>=1.27.0
+mypy-boto3-service-quotas<1.29.0,>=1.28.0
 
 [servicecatalog]
-mypy-boto3-servicecatalog<1.28.0,>=1.27.0
+mypy-boto3-servicecatalog<1.29.0,>=1.28.0
 
 [servicecatalog-appregistry]
-mypy-boto3-servicecatalog-appregistry<1.28.0,>=1.27.0
+mypy-boto3-servicecatalog-appregistry<1.29.0,>=1.28.0
 
 [servicediscovery]
-mypy-boto3-servicediscovery<1.28.0,>=1.27.0
+mypy-boto3-servicediscovery<1.29.0,>=1.28.0
 
 [ses]
-mypy-boto3-ses<1.28.0,>=1.27.0
+mypy-boto3-ses<1.29.0,>=1.28.0
 
 [sesv2]
-mypy-boto3-sesv2<1.28.0,>=1.27.0
+mypy-boto3-sesv2<1.29.0,>=1.28.0
 
 [shield]
-mypy-boto3-shield<1.28.0,>=1.27.0
+mypy-boto3-shield<1.29.0,>=1.28.0
 
 [signer]
-mypy-boto3-signer<1.28.0,>=1.27.0
+mypy-boto3-signer<1.29.0,>=1.28.0
 
 [simspaceweaver]
-mypy-boto3-simspaceweaver<1.28.0,>=1.27.0
+mypy-boto3-simspaceweaver<1.29.0,>=1.28.0
 
 [sms]
-mypy-boto3-sms<1.28.0,>=1.27.0
+mypy-boto3-sms<1.29.0,>=1.28.0
 
 [sms-voice]
-mypy-boto3-sms-voice<1.28.0,>=1.27.0
+mypy-boto3-sms-voice<1.29.0,>=1.28.0
 
 [snow-device-management]
-mypy-boto3-snow-device-management<1.28.0,>=1.27.0
+mypy-boto3-snow-device-management<1.29.0,>=1.28.0
 
 [snowball]
-mypy-boto3-snowball<1.28.0,>=1.27.0
+mypy-boto3-snowball<1.29.0,>=1.28.0
 
 [sns]
-mypy-boto3-sns<1.28.0,>=1.27.0
+mypy-boto3-sns<1.29.0,>=1.28.0
 
 [sqs]
-mypy-boto3-sqs<1.28.0,>=1.27.0
+mypy-boto3-sqs<1.29.0,>=1.28.0
 
 [ssm]
-mypy-boto3-ssm<1.28.0,>=1.27.0
+mypy-boto3-ssm<1.29.0,>=1.28.0
 
 [ssm-contacts]
-mypy-boto3-ssm-contacts<1.28.0,>=1.27.0
+mypy-boto3-ssm-contacts<1.29.0,>=1.28.0
 
 [ssm-incidents]
-mypy-boto3-ssm-incidents<1.28.0,>=1.27.0
+mypy-boto3-ssm-incidents<1.29.0,>=1.28.0
 
 [ssm-sap]
-mypy-boto3-ssm-sap<1.28.0,>=1.27.0
+mypy-boto3-ssm-sap<1.29.0,>=1.28.0
 
 [sso]
-mypy-boto3-sso<1.28.0,>=1.27.0
+mypy-boto3-sso<1.29.0,>=1.28.0
 
 [sso-admin]
-mypy-boto3-sso-admin<1.28.0,>=1.27.0
+mypy-boto3-sso-admin<1.29.0,>=1.28.0
 
 [sso-oidc]
-mypy-boto3-sso-oidc<1.28.0,>=1.27.0
+mypy-boto3-sso-oidc<1.29.0,>=1.28.0
 
 [stepfunctions]
-mypy-boto3-stepfunctions<1.28.0,>=1.27.0
+mypy-boto3-stepfunctions<1.29.0,>=1.28.0
 
 [storagegateway]
-mypy-boto3-storagegateway<1.28.0,>=1.27.0
+mypy-boto3-storagegateway<1.29.0,>=1.28.0
 
 [sts]
-mypy-boto3-sts<1.28.0,>=1.27.0
+mypy-boto3-sts<1.29.0,>=1.28.0
 
 [support]
-mypy-boto3-support<1.28.0,>=1.27.0
+mypy-boto3-support<1.29.0,>=1.28.0
 
 [support-app]
-mypy-boto3-support-app<1.28.0,>=1.27.0
+mypy-boto3-support-app<1.29.0,>=1.28.0
 
 [swf]
-mypy-boto3-swf<1.28.0,>=1.27.0
+mypy-boto3-swf<1.29.0,>=1.28.0
 
 [synthetics]
-mypy-boto3-synthetics<1.28.0,>=1.27.0
+mypy-boto3-synthetics<1.29.0,>=1.28.0
 
 [textract]
-mypy-boto3-textract<1.28.0,>=1.27.0
+mypy-boto3-textract<1.29.0,>=1.28.0
 
 [timestream-query]
-mypy-boto3-timestream-query<1.28.0,>=1.27.0
+mypy-boto3-timestream-query<1.29.0,>=1.28.0
 
 [timestream-write]
-mypy-boto3-timestream-write<1.28.0,>=1.27.0
+mypy-boto3-timestream-write<1.29.0,>=1.28.0
 
 [tnb]
-mypy-boto3-tnb<1.28.0,>=1.27.0
+mypy-boto3-tnb<1.29.0,>=1.28.0
 
 [transcribe]
-mypy-boto3-transcribe<1.28.0,>=1.27.0
+mypy-boto3-transcribe<1.29.0,>=1.28.0
 
 [transfer]
-mypy-boto3-transfer<1.28.0,>=1.27.0
+mypy-boto3-transfer<1.29.0,>=1.28.0
 
 [translate]
-mypy-boto3-translate<1.28.0,>=1.27.0
+mypy-boto3-translate<1.29.0,>=1.28.0
 
 [verifiedpermissions]
-mypy-boto3-verifiedpermissions<1.28.0,>=1.27.0
+mypy-boto3-verifiedpermissions<1.29.0,>=1.28.0
 
 [voice-id]
-mypy-boto3-voice-id<1.28.0,>=1.27.0
+mypy-boto3-voice-id<1.29.0,>=1.28.0
 
 [vpc-lattice]
-mypy-boto3-vpc-lattice<1.28.0,>=1.27.0
+mypy-boto3-vpc-lattice<1.29.0,>=1.28.0
 
 [waf]
-mypy-boto3-waf<1.28.0,>=1.27.0
+mypy-boto3-waf<1.29.0,>=1.28.0
 
 [waf-regional]
-mypy-boto3-waf-regional<1.28.0,>=1.27.0
+mypy-boto3-waf-regional<1.29.0,>=1.28.0
 
 [wafv2]
-mypy-boto3-wafv2<1.28.0,>=1.27.0
+mypy-boto3-wafv2<1.29.0,>=1.28.0
 
 [wellarchitected]
-mypy-boto3-wellarchitected<1.28.0,>=1.27.0
+mypy-boto3-wellarchitected<1.29.0,>=1.28.0
 
 [wisdom]
-mypy-boto3-wisdom<1.28.0,>=1.27.0
+mypy-boto3-wisdom<1.29.0,>=1.28.0
 
 [workdocs]
-mypy-boto3-workdocs<1.28.0,>=1.27.0
+mypy-boto3-workdocs<1.29.0,>=1.28.0
 
 [worklink]
-mypy-boto3-worklink<1.28.0,>=1.27.0
+mypy-boto3-worklink<1.29.0,>=1.28.0
 
 [workmail]
-mypy-boto3-workmail<1.28.0,>=1.27.0
+mypy-boto3-workmail<1.29.0,>=1.28.0
 
 [workmailmessageflow]
-mypy-boto3-workmailmessageflow<1.28.0,>=1.27.0
+mypy-boto3-workmailmessageflow<1.29.0,>=1.28.0
 
 [workspaces]
-mypy-boto3-workspaces<1.28.0,>=1.27.0
+mypy-boto3-workspaces<1.29.0,>=1.28.0
 
 [workspaces-web]
-mypy-boto3-workspaces-web<1.28.0,>=1.27.0
+mypy-boto3-workspaces-web<1.29.0,>=1.28.0
 
 [xray]
-mypy-boto3-xray<1.28.0,>=1.27.0
+mypy-boto3-xray<1.29.0,>=1.28.0
```

