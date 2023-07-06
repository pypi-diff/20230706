# Comparing `tmp/mypy-boto3-timestream-query-1.27.0.tar.gz` & `tmp/mypy-boto3-timestream-query-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.27.0.tar", last modified: Mon Jul  3 19:51:33 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.28.0.tar", last modified: Thu Jul  6 21:00:47 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.27.0.tar` & `mypy-boto3-timestream-query-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-03 19:49:05.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 19:51:33.000000 mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:33.484097 mypy-boto3-timestream-query-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 19:49:04.000000 mypy-boto3-timestream-query-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.990450 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19457 2023-07-06 20:57:13.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-07-06 20:57:13.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 21:00:46.000000 mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:46.994450 mypy-boto3-timestream-query-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-06 20:57:12.000000 mypy-boto3-timestream-query-1.28.0/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.27.0/LICENSE` & `mypy-boto3-timestream-query-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/PKG-INFO` & `mypy-boto3-timestream-query-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.27.0
-Summary: Type annotations for boto3.TimestreamQuery 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.TimestreamQuery 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-timestream-query-1.27.0/README.md` & `mypy-boto3-timestream-query-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.27.0\nVersion:         1.27.0\nBuilder"
+        "Type annotations for boto3.TimestreamQuery 1.28.0\nVersion:         1.28.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,23 +148,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List["DatumTypeDef"],
+        "Data": List[Dict[str, Any]],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": Dict[str, Any],
+        "Value": "DatumTypeDef",
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
```

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -145,23 +145,23 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
-        "Data": List["DatumTypeDef"],
+        "Data": List[Dict[str, Any]],
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": Dict[str, Any],
+        "Value": "DatumTypeDef",
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
```

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.27.0
-Summary: Type annotations for boto3.TimestreamQuery 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.TimestreamQuery 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-query?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-timestream-query-1.27.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.28.0/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.27.0/setup.py` & `mypy-boto3-timestream-query-1.28.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamQuery 1.27.0 service generated with"
+        "Type annotations for boto3.TimestreamQuery 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

