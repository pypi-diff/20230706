# Comparing `tmp/mypy-boto3-personalize-runtime-1.27.0.tar.gz` & `tmp/mypy-boto3-personalize-runtime-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-runtime-1.27.0.tar", last modified: Mon Jul  3 19:51:14 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-runtime-1.28.0.tar", last modified: Thu Jul  6 21:00:18 2023, max compression
```

## Comparing `mypy-boto3-personalize-runtime-1.27.0.tar` & `mypy-boto3-personalize-runtime-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.951799 mypy-boto3-personalize-runtime-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-03 19:51:14.951799 mypy-boto3-personalize-runtime-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.947799 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-03 19:43:26.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-03 19:43:26.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:14.951799 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-03 19:51:14.000000 mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:14.951799 mypy-boto3-personalize-runtime-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-03 19:43:24.000000 mypy-boto3-personalize-runtime-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11134 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:18.000000 mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:18.510392 mypy-boto3-personalize-runtime-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:49:13.000000 mypy-boto3-personalize-runtime-1.28.0/setup.py
```

### Comparing `mypy-boto3-personalize-runtime-1.27.0/LICENSE` & `mypy-boto3-personalize-runtime-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/PKG-INFO` & `mypy-boto3-personalize-runtime-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.27.0
-Summary: Type annotations for boto3.PersonalizeRuntime 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-personalize-runtime-1.27.0/README.md` & `mypy-boto3-personalize-runtime-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/__main__.py` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PersonalizeRuntime 1.27.0\nVersion:         1.27.0\nBuilder"
+        "Type annotations for boto3.PersonalizeRuntime 1.28.0\nVersion:         1.28.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime\nOther"
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

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/client.py` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/client.pyi` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/literals.py` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/literals.pyi` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/type_defs.py` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime/type_defs.pyi` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-runtime
-Version: 1.27.0
-Summary: Type annotations for boto3.PersonalizeRuntime 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_runtime/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-runtime?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeRuntime 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
+[boto3.PersonalizeRuntime 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-personalize-runtime-1.27.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt` & `mypy-boto3-personalize-runtime-1.28.0/mypy_boto3_personalize_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-runtime-1.27.0/setup.py` & `mypy-boto3-personalize-runtime-1.28.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-runtime",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_personalize_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PersonalizeRuntime 1.27.0 service generated with"
+        "Type annotations for boto3.PersonalizeRuntime 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

