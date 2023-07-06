# Comparing `tmp/mypy-boto3-transfer-1.27.0.tar.gz` & `tmp/mypy-boto3-transfer-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transfer-1.27.0.tar", last modified: Mon Jul  3 19:51:34 2023, max compression
+gzip compressed data, was "mypy-boto3-transfer-1.28.0.tar", last modified: Thu Jul  6 21:00:48 2023, max compression
```

## Comparing `mypy-boto3-transfer-1.27.0.tar` & `mypy-boto3-transfer-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.376112 mypy-boto3-transfer-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-03 19:51:34.376112 mypy-boto3-transfer-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.376112 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46221 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46143 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-07-03 19:49:15.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59129 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-03 19:49:14.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:34.376112 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:34.000000 mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:34.376112 mypy-boto3-transfer-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:49:13.000000 mypy-boto3-transfer-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.794454 mypy-boto3-transfer-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20154 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46221 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46143 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-07-06 20:57:22.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-07-06 20:57:27.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59129 2023-07-06 20:57:26.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-06 20:57:21.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:48.790454 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21643 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:48.000000 mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:48.794454 mypy-boto3-transfer-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:57:20.000000 mypy-boto3-transfer-1.28.0/setup.py
```

### Comparing `mypy-boto3-transfer-1.27.0/LICENSE` & `mypy-boto3-transfer-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/PKG-INFO` & `mypy-boto3-transfer-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.27.0
-Summary: Type annotations for boto3.Transfer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.27.0/README.md` & `mypy-boto3-transfer-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__init__.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__init__.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/__main__.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Transfer 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/client.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/client.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/literals.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/literals.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/paginator.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/paginator.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/type_defs.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/type_defs.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/waiter.py` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer/waiter.pyi` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.27.0
-Summary: Type annotations for boto3.Transfer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transfer?color=blue)](https://pypistats.org/packages/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-transfer-1.27.0/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy-boto3-transfer-1.28.0/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transfer-1.27.0/setup.py` & `mypy-boto3-transfer-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Transfer 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Transfer 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

