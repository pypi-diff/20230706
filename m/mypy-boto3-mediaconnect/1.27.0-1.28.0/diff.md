# Comparing `tmp/mypy-boto3-mediaconnect-1.27.0.tar.gz` & `tmp/mypy-boto3-mediaconnect-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconnect-1.27.0.tar", last modified: Mon Jul  3 19:51:05 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconnect-1.28.0.tar", last modified: Thu Jul  6 21:00:04 2023, max compression
```

## Comparing `mypy-boto3-mediaconnect-1.27.0.tar` & `mypy-boto3-mediaconnect-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.967639 mypy-boto3-mediaconnect-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-03 19:51:05.963639 mypy-boto3-mediaconnect-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20551 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.955639 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:40.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65058 2023-07-03 19:41:42.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64967 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-03 19:41:41.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:05.963639 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:05.000000 mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:05.967639 mypy-boto3-mediaconnect-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:41:39.000000 mypy-boto3-mediaconnect-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20551 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.706364 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40299 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65058 2023-07-06 20:46:45.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64967 2023-07-06 20:46:42.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-06 20:46:41.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:04.000000 mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:04.714364 mypy-boto3-mediaconnect-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:46:40.000000 mypy-boto3-mediaconnect-1.28.0/setup.py
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/LICENSE` & `mypy-boto3-mediaconnect-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/README.md` & `mypy-boto3-mediaconnect-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__init__.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/__main__.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConnect 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.MediaConnect 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
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

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/client.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlgorithmType",
     "BridgePlacementType",
     "BridgeStateType",
     "ColorimetryType",
     "ConnectionStatusType",
     "DesiredStateType",
@@ -61,15 +60,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
 BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
 BridgeStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETED",
     "DELETING",
@@ -511,20 +509,22 @@
     "list_gateway_instances",
     "list_gateways",
     "list_offerings",
     "list_reservations",
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/literals.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AlgorithmType",
     "BridgePlacementType",
     "BridgeStateType",
     "ColorimetryType",
     "ConnectionStatusType",
     "DesiredStateType",
@@ -60,14 +61,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
 BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
 BridgeStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETED",
     "DELETING",
@@ -509,20 +511,22 @@
     "list_gateway_instances",
     "list_gateways",
     "list_offerings",
     "list_reservations",
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/paginator.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/type_defs.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.py` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect/waiter.pyi` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconnect
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconnect/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconnect?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConnect 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[boto3.MediaConnect 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconnect-1.27.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt` & `mypy-boto3-mediaconnect-1.28.0/mypy_boto3_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconnect-1.27.0/setup.py` & `mypy-boto3-mediaconnect-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconnect",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConnect 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaConnect 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

