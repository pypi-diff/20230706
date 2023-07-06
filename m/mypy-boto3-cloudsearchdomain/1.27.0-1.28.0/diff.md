# Comparing `tmp/mypy-boto3-cloudsearchdomain-1.27.0.tar.gz` & `tmp/mypy-boto3-cloudsearchdomain-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.27.0.tar", last modified: Mon Jul  3 19:50:30 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudsearchdomain-1.28.0.tar", last modified: Thu Jul  6 20:59:11 2023, max compression
```

## Comparing `mypy-boto3-cloudsearchdomain-1.27.0.tar` & `mypy-boto3-cloudsearchdomain-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:30.434961 mypy-boto3-cloudsearchdomain-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-03 19:50:30.434961 mypy-boto3-cloudsearchdomain-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:30.434961 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:30.434961 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-03 19:50:30.000000 mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:30.434961 mypy-boto3-cloudsearchdomain-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-03 19:33:58.000000 mypy-boto3-cloudsearchdomain-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.146247 mypy-boto3-cloudsearchdomain-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-06 20:59:11.142248 mypy-boto3-cloudsearchdomain-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.126248 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-06 20:35:30.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:11.142248 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:10.000000 mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:11.146247 mypy-boto3-cloudsearchdomain-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-06 20:35:29.000000 mypy-boto3-cloudsearchdomain-1.28.0/setup.py
```

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/LICENSE` & `mypy-boto3-cloudsearchdomain-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.27.0
-Summary: Type annotations for boto3.CloudSearchDomain 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/README.md` & `mypy-boto3-cloudsearchdomain-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/__main__.py` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudSearchDomain 1.27.0\nVersion:         1.27.0\nBuilder"
+        "Type annotations for boto3.CloudSearchDomain 1.28.0\nVersion:         1.28.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/client.py` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/client.pyi` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/literals.py` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/literals.pyi` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/type_defs.py` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain/type_defs.pyi` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudsearchdomain
-Version: 1.27.0
-Summary: Type annotations for boto3.CloudSearchDomain 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudsearchdomain/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudsearchdomain?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudSearchDomain 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[boto3.CloudSearchDomain 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt` & `mypy-boto3-cloudsearchdomain-1.28.0/mypy_boto3_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudsearchdomain-1.27.0/setup.py` & `mypy-boto3-cloudsearchdomain-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudsearchdomain",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudSearchDomain 1.27.0 service generated with"
+        "Type annotations for boto3.CloudSearchDomain 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

