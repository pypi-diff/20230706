# Comparing `tmp/mypy-boto3-kms-1.27.1.tar.gz` & `tmp/mypy-boto3-kms-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.27.1.tar", last modified: Wed Jul  5 19:47:56 2023, max compression
+gzip compressed data, was "mypy-boto3-kms-1.28.0.tar", last modified: Thu Jul  6 20:59:57 2023, max compression
```

## Comparing `mypy-boto3-kms-1.27.1.tar` & `mypy-boto3-kms-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-05 19:47:21.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-05 19:47:21.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-07-05 19:47:23.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40953 2023-07-05 19:47:22.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 19:47:56.000000 mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 19:47:56.824989 mypy-boto3-kms-1.27.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-05 19:47:20.000000 mypy-boto3-kms-1.27.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.230349 mypy-boto3-kms-1.28.0/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41185 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-07-06 20:45:00.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-07-06 20:45:02.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40953 2023-07-06 20:45:01.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17791 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:57.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:56.000000 mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:57.238349 mypy-boto3-kms-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:44:59.000000 mypy-boto3-kms-1.28.0/setup.py
```

### Comparing `mypy-boto3-kms-1.27.1/LICENSE` & `mypy-boto3-kms-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/PKG-INFO` & `mypy-boto3-kms-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.27.1
-Summary: Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.1/README.md` & `mypy-boto3-kms-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__init__.pyi` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/__main__.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.27.1\nVersion:         1.27.1\nBuilder version:"
+        "Type annotations for boto3.KMS 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.27.1")
+    print("1.28.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/client.pyi` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/literals.pyi` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/paginator.pyi` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.py` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms/type_defs.pyi` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.27.1
-Summary: Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kms?color=blue)](https://pypistats.org/packages/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.27.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-kms-1.27.1/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy-boto3-kms-1.28.0/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.27.1/setup.py` & `mypy-boto3-kms-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.27.1",
+    version="1.28.0",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KMS 1.27.1 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.KMS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

