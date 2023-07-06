# Comparing `tmp/mypy-boto3-dlm-1.27.0.tar.gz` & `tmp/mypy-boto3-dlm-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dlm-1.27.0.tar", last modified: Mon Jul  3 19:50:40 2023, max compression
+gzip compressed data, was "mypy-boto3-dlm-1.28.0.tar", last modified: Thu Jul  6 20:59:26 2023, max compression
```

## Comparing `mypy-boto3-dlm-1.27.0.tar` & `mypy-boto3-dlm-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.203137 mypy-boto3-dlm-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-03 19:35:39.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:40.199137 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:40.000000 mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:40.203137 mypy-boto3-dlm-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:35:38.000000 mypy-boto3-dlm-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.066282 mypy-boto3-dlm-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-06 20:59:26.066282 mypy-boto3-dlm-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.062282 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-06 20:37:57.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-06 20:37:57.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-06 20:37:57.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:26.066282 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:25.000000 mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:26.066282 mypy-boto3-dlm-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:37:56.000000 mypy-boto3-dlm-1.28.0/setup.py
```

### Comparing `mypy-boto3-dlm-1.27.0/LICENSE` & `mypy-boto3-dlm-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/PKG-INFO` & `mypy-boto3-dlm-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.27.0
-Summary: Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DLM 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dlm-1.27.0/README.md` & `mypy-boto3-dlm-1.28.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/__main__.py` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DLM 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.DLM 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.py` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/client.pyi` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.py` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/literals.pyi` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.py` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm/type_defs.pyi` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/PKG-INFO` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.27.0
-Summary: Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.DLM 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dlm?color=blue)](https://pypistats.org/packages/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-dlm-1.27.0/mypy_boto3_dlm.egg-info/SOURCES.txt` & `mypy-boto3-dlm-1.28.0/mypy_boto3_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.27.0/setup.py` & `mypy-boto3-dlm-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dlm",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DLM 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.DLM 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

