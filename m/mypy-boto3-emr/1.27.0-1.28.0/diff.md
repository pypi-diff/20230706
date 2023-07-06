# Comparing `tmp/mypy-boto3-emr-1.27.0.tar.gz` & `tmp/mypy-boto3-emr-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.27.0.tar", last modified: Mon Jul  3 19:50:45 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.28.0.tar", last modified: Thu Jul  6 20:59:33 2023, max compression
```

## Comparing `mypy-boto3-emr-1.27.0.tar` & `mypy-boto3-emr-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-03 19:37:27.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79659 2023-07-03 19:37:29.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79553 2023-07-03 19:37:29.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-03 19:37:28.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:45.000000 mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:45.539234 mypy-boto3-emr-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:37:26.000000 mypy-boto3-emr-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22388 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.470299 mypy-boto3-emr-1.28.0/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-06 20:40:35.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79659 2023-07-06 20:40:38.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79553 2023-07-06 20:40:36.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-06 20:40:34.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:33.470299 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23857 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:33.000000 mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:33.474299 mypy-boto3-emr-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:40:33.000000 mypy-boto3-emr-1.28.0/setup.py
```

### Comparing `mypy-boto3-emr-1.27.0/LICENSE` & `mypy-boto3-emr-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/PKG-INFO` & `mypy-boto3-emr-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.27.0
-Summary: Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-1.27.0/README.md` & `mypy-boto3-emr-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.EMR 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.27.0
-Summary: Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-emr?color=blue)](https://pypistats.org/packages/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-emr-1.27.0/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.28.0/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.27.0/setup.py` & `mypy-boto3-emr-1.28.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.EMR 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

