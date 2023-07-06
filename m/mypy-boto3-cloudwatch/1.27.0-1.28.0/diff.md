# Comparing `tmp/mypy-boto3-cloudwatch-1.27.0.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.27.0.tar", last modified: Mon Jul  3 19:50:31 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.27.0.tar` & `mypy-boto3-cloudwatch-1.28.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.522980 mypy-boto3-cloudwatch-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-07-03 19:34:05.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-07-03 19:34:04.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-03 19:34:03.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:31.518980 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:50:31.000000 mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:31.522980 mypy-boto3-cloudwatch-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:34:02.000000 mypy-boto3-cloudwatch-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.394250 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32826 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32773 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-07-06 20:35:38.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-07-06 20:35:37.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23124 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23079 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    42495 2023-07-06 20:35:39.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-07-06 20:35:38.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-06 20:35:36.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20798 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:12.000000 mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.402250 mypy-boto3-cloudwatch-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:35.000000 mypy-boto3-cloudwatch-1.28.0/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.27.0/LICENSE` & `mypy-boto3-cloudwatch-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.27.0
-Summary: Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.27.0/README.md` & `mypy-boto3-cloudwatch-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.CloudWatch 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.27.0
-Summary: Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudwatch?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.27.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.28.0/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.27.0/setup.py` & `mypy-boto3-cloudwatch-1.28.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatch 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.CloudWatch 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

