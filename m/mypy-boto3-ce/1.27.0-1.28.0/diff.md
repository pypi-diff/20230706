# Comparing `tmp/mypy-boto3-ce-1.27.0.tar.gz` & `tmp/mypy-boto3-ce-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.27.0.tar", last modified: Mon Jul  3 19:50:27 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
```

## Comparing `mypy-boto3-ce-1.27.0.tar` & `mypy-boto3-ce-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31896 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-07-03 19:33:15.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-03 19:33:15.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63440 2023-07-03 19:33:17.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63371 2023-07-03 19:33:16.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 19:50:26.000000 mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:27.130903 mypy-boto3-ce-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-03 19:33:14.000000 mypy-boto3-ce-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17305 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.594235 mypy-boto3-ce-1.28.0/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31940 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31896 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-07-06 20:34:26.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-07-06 20:34:26.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63440 2023-07-06 20:34:29.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63371 2023-07-06 20:34:28.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18780 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 20:59:05.000000 mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.602235 mypy-boto3-ce-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:34:25.000000 mypy-boto3-ce-1.28.0/setup.py
```

### Comparing `mypy-boto3-ce-1.27.0/LICENSE` & `mypy-boto3-ce-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/PKG-INFO` & `mypy-boto3-ce-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.27.0
-Summary: Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.27.0/README.md` & `mypy-boto3-ce-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.CostExplorer 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.27.0
-Summary: Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.27.0/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.0/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.27.0/setup.py` & `mypy-boto3-ce-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.CostExplorer 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

