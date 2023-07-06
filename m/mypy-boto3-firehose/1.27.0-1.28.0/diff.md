# Comparing `tmp/mypy-boto3-firehose-1.27.0.tar.gz` & `tmp/mypy-boto3-firehose-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-firehose-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
+gzip compressed data, was "mypy-boto3-firehose-1.28.0.tar", last modified: Thu Jul  6 20:59:36 2023, max compression
```

## Comparing `mypy-boto3-firehose-1.27.0.tar` & `mypy-boto3-firehose-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.023261 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45008 2023-07-03 19:37:48.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44959 2023-07-03 19:37:48.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:46.000000 mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.027261 mypy-boto3-firehose-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:37:47.000000 mypy-boto3-firehose-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.686306 mypy-boto3-firehose-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-06 20:59:36.682306 mypy-boto3-firehose-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.670306 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45008 2023-07-06 20:41:06.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44959 2023-07-06 20:41:06.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:05.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:36.682306 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16218 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:36.000000 mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:36.686306 mypy-boto3-firehose-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:41:03.000000 mypy-boto3-firehose-1.28.0/setup.py
```

### Comparing `mypy-boto3-firehose-1.27.0/LICENSE` & `mypy-boto3-firehose-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/PKG-INFO` & `mypy-boto3-firehose-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.27.0
-Summary: Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-firehose-1.27.0/README.md` & `mypy-boto3-firehose-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/__main__.py` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Firehose 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Firehose 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose\nOther"
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

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.py` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/client.pyi` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.py` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/literals.pyi` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.py` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose/type_defs.pyi` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/PKG-INFO` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-firehose
-Version: 1.27.0
-Summary: Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-firehose.svg?color=blue)](https://pypi.org/project/mypy-boto3-firehose)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_firehose/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-firehose?color=blue)](https://pypistats.org/packages/mypy-boto3-firehose)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Firehose 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
+[boto3.Firehose 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-firehose-1.27.0/mypy_boto3_firehose.egg-info/SOURCES.txt` & `mypy-boto3-firehose-1.28.0/mypy_boto3_firehose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-firehose-1.27.0/setup.py` & `mypy-boto3-firehose-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-firehose",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_firehose"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Firehose 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Firehose 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

