# Comparing `tmp/mypy-boto3-mwaa-1.27.0.tar.gz` & `tmp/mypy-boto3-mwaa-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
```

## Comparing `mypy-boto3-mwaa-1.27.0.tar` & `mypy-boto3-mwaa-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.475722 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-03 19:42:36.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 19:51:10.000000 mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.479722 mypy-boto3-mwaa-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 19:42:35.000000 mypy-boto3-mwaa-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.610378 mypy-boto3-mwaa-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-06 21:00:11.606378 mypy-boto3-mwaa-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.602378 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-07-06 20:48:01.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-07-06 20:48:01.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.606378 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:00:11.000000 mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.610378 mypy-boto3-mwaa-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 20:48:00.000000 mypy-boto3-mwaa-1.28.0/setup.py
```

### Comparing `mypy-boto3-mwaa-1.27.0/LICENSE` & `mypy-boto3-mwaa-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/PKG-INFO` & `mypy-boto3-mwaa-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.27.0
-Summary: Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MWAA 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mwaa-1.27.0/README.md` & `mypy-boto3-mwaa-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/__main__.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MWAA 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.MWAA 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.27.0
-Summary: Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MWAA 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mwaa?color=blue)](https://pypistats.org/packages/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mwaa-1.27.0/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.28.0/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.27.0/setup.py` & `mypy-boto3-mwaa-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MWAA 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MWAA 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

