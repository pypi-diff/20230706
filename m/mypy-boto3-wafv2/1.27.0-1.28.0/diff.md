# Comparing `tmp/mypy-boto3-wafv2-1.27.0.tar.gz` & `tmp/mypy-boto3-wafv2-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.28.0.tar", last modified: Thu Jul  6 21:00:50 2023, max compression
```

## Comparing `mypy-boto3-wafv2-1.27.0.tar` & `mypy-boto3-wafv2-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.880138 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-07-03 19:49:38.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68292 2023-07-03 19:49:37.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:36.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 19:51:35.000000 mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.892138 mypy-boto3-wafv2-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:49:35.000000 mypy-boto3-wafv2-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.482457 mypy-boto3-wafv2-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-06 21:00:50.478457 mypy-boto3-wafv2-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.462457 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36893 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36834 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-06 20:57:56.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-07-06 20:57:58.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68292 2023-07-06 20:57:57.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.478457 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19830 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:50.000000 mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:50.482457 mypy-boto3-wafv2-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:57:55.000000 mypy-boto3-wafv2-1.28.0/setup.py
```

### Comparing `mypy-boto3-wafv2-1.27.0/LICENSE` & `mypy-boto3-wafv2-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/PKG-INFO` & `mypy-boto3-wafv2-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.27.0
-Summary: Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.27.0/README.md` & `mypy-boto3-wafv2-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.WAFV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\nOther"
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

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1259,22 +1259,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
```

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1228,22 +1228,22 @@
     },
     total=False,
 )
 
 NotStatementTypeDef = TypedDict(
     "NotStatementTypeDef",
     {
-        "Statement": Dict[str, Any],
+        "Statement": "StatementTypeDef",
     },
 )
 
 OrStatementTypeDef = TypedDict(
     "OrStatementTypeDef",
     {
-        "Statements": Sequence["StatementTypeDef"],
+        "Statements": Sequence[Dict[str, Any]],
     },
 )
 
 PhoneNumberFieldTypeDef = TypedDict(
     "PhoneNumberFieldTypeDef",
     {
         "Identifier": str,
```

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.27.0
-Summary: Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wafv2?color=blue)](https://pypistats.org/packages/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.27.0/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.28.0/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.27.0/setup.py` & `mypy-boto3-wafv2-1.28.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFV2 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WAFV2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```
