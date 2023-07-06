# Comparing `tmp/mypy-boto3-dynamodb-1.27.0.tar.gz` & `tmp/mypy-boto3-dynamodb-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodb-1.27.0.tar", last modified: Mon Jul  3 19:50:41 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodb-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
```

## Comparing `mypy-boto3-dynamodb-1.27.0.tar` & `mypy-boto3-dynamodb-1.28.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.075153 mypy-boto3-dynamodb-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-03 19:50:41.071153 mypy-boto3-dynamodb-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.067153 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   152926 2023-07-03 19:36:04.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152773 2023-07-03 19:36:02.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-03 19:36:00.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:41.067153 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:40.000000 mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:41.075153 mypy-boto3-dynamodb-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:35:59.000000 mypy-boto3-dynamodb-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26772 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54381 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54314 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27454 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-07-06 20:38:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   152926 2023-07-06 20:38:33.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152773 2023-07-06 20:38:31.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-06 20:38:27.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:26.000000 mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.886284 mypy-boto3-dynamodb-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:38:25.000000 mypy-boto3-dynamodb-1.28.0/setup.py
```

### Comparing `mypy-boto3-dynamodb-1.27.0/LICENSE` & `mypy-boto3-dynamodb-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/PKG-INFO` & `mypy-boto3-dynamodb-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.27.0
-Summary: Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dynamodb-1.27.0/README.md` & `mypy-boto3-dynamodb-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__init__.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/__main__.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDB 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.DynamoDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
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

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/client.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/literals.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/paginator.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/service_resource.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/type_defs.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.py` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb/waiter.pyi` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/PKG-INFO` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodb
-Version: 1.27.0
-Summary: Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodb.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dynamodb?color=blue)](https://pypistats.org/packages/mypy-boto3-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[boto3.DynamoDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dynamodb-1.27.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt` & `mypy-boto3-dynamodb-1.28.0/mypy_boto3_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodb-1.27.0/setup.py` & `mypy-boto3-dynamodb-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodb",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDB 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.DynamoDB 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

