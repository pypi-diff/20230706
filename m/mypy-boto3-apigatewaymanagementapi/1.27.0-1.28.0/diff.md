# Comparing `tmp/mypy-boto3-apigatewaymanagementapi-1.27.0.tar.gz` & `tmp/mypy-boto3-apigatewaymanagementapi-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.27.0.tar", last modified: Mon Jul  3 19:50:20 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
```

## Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0.tar` & `mypy-boto3-apigatewaymanagementapi-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.342781 mypy-boto3-apigatewaymanagementapi-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-03 19:50:20.342781 mypy-boto3-apigatewaymanagementapi-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.342781 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:20.342781 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 19:50:20.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:20.342781 mypy-boto3-apigatewaymanagementapi-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-03 19:32:18.000000 mypy-boto3-apigatewaymanagementapi-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.414214 mypy-boto3-apigatewaymanagementapi-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-06 20:58:55.410214 mypy-boto3-apigatewaymanagementapi-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.402214 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-06 20:33:01.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.410214 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 20:58:55.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.414214 mypy-boto3-apigatewaymanagementapi-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-06 20:33:00.000000 mypy-boto3-apigatewaymanagementapi-1.28.0/setup.py
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/LICENSE` & `mypy-boto3-apigatewaymanagementapi-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.27.0
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/README.md` & `mypy-boto3-apigatewaymanagementapi-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/__main__.py` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.27.0\nVersion:        "
-        " 1.27.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.0\nVersion:        "
+        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi\nOther"
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

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/client.py` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/client.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/literals.py` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/literals.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/type_defs.py` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi/type_defs.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.27.0
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt` & `mypy-boto3-apigatewaymanagementapi-1.28.0/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.27.0/setup.py` & `mypy-boto3-apigatewaymanagementapi-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewaymanagementapi",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_apigatewaymanagementapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.27.0 service generated with"
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

