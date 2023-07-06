# Comparing `tmp/mypy-boto3-kendra-1.27.0.tar.gz` & `tmp/mypy-boto3-kendra-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kendra-1.27.0.tar", last modified: Mon Jul  3 19:50:57 2023, max compression
+gzip compressed data, was "mypy-boto3-kendra-1.28.0.tar", last modified: Thu Jul  6 20:59:52 2023, max compression
```

## Comparing `mypy-boto3-kendra-1.27.0.tar` & `mypy-boto3-kendra-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.415484 mypy-boto3-kendra-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-03 19:50:57.411484 mypy-boto3-kendra-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.407483 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-03 19:40:13.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   110862 2023-07-03 19:40:15.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   110709 2023-07-03 19:40:14.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:57.411484 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:57.000000 mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:57.415484 mypy-boto3-kendra-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:40:11.000000 mypy-boto3-kendra-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.298339 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47945 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47873 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-06 20:44:34.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-07-06 20:44:34.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   110862 2023-07-06 20:44:37.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110709 2023-07-06 20:44:35.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23685 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:52.000000 mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:52.310339 mypy-boto3-kendra-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:44:33.000000 mypy-boto3-kendra-1.28.0/setup.py
```

### Comparing `mypy-boto3-kendra-1.27.0/LICENSE` & `mypy-boto3-kendra-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/PKG-INFO` & `mypy-boto3-kendra-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.27.0
-Summary: Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.kendra 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kendra-1.27.0/README.md` & `mypy-boto3-kendra-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/__main__.py` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.kendra 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.kendra 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra\nOther"
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

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.py` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/client.pyi` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.py` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/literals.pyi` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.py` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra/type_defs.pyi` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/PKG-INFO` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kendra
-Version: 1.27.0
-Summary: Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.kendra 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kendra.svg?color=blue)](https://pypi.org/project/mypy-boto3-kendra)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kendra/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kendra?color=blue)](https://pypistats.org/packages/mypy-boto3-kendra)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.kendra 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
+[boto3.kendra 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kendra-1.27.0/mypy_boto3_kendra.egg-info/SOURCES.txt` & `mypy-boto3-kendra-1.28.0/mypy_boto3_kendra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kendra-1.27.0/setup.py` & `mypy-boto3-kendra-1.28.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kendra",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_kendra"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.kendra 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.kendra 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

