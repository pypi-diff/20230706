# Comparing `tmp/mypy-boto3-s3outposts-1.27.0.tar.gz` & `tmp/mypy-boto3-s3outposts-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3outposts-1.27.0.tar", last modified: Mon Jul  3 19:51:23 2023, max compression
+gzip compressed data, was "mypy-boto3-s3outposts-1.28.0.tar", last modified: Thu Jul  6 21:00:31 2023, max compression
```

## Comparing `mypy-boto3-s3outposts-1.27.0.tar` & `mypy-boto3-s3outposts-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.227924 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-03 19:51:23.000000 mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:23.235924 mypy-boto3-s3outposts-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:46:58.000000 mypy-boto3-s3outposts-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:31.000000 mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:31.766419 mypy-boto3-s3outposts-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:54:09.000000 mypy-boto3-s3outposts-1.28.0/setup.py
```

### Comparing `mypy-boto3-s3outposts-1.27.0/LICENSE` & `mypy-boto3-s3outposts-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/PKG-INFO` & `mypy-boto3-s3outposts-1.28.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3outposts
-Version: 1.27.0
-Summary: Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3outposts-1.27.0/README.md` & `mypy-boto3-s3outposts-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__init__.pyi` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/__main__.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Outposts 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.S3Outposts 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts\nOther"
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

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/client.pyi` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/literals.pyi` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/paginator.pyi` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.py` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts/type_defs.pyi` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/PKG-INFO` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3outposts
-Version: 1.27.0
-Summary: Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3outposts.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3outposts)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3outposts/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3outposts?color=blue)](https://pypistats.org/packages/mypy-boto3-s3outposts)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Outposts 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
+[boto3.S3Outposts 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-s3outposts-1.27.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt` & `mypy-boto3-s3outposts-1.28.0/mypy_boto3_s3outposts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3outposts-1.27.0/setup.py` & `mypy-boto3-s3outposts-1.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3outposts",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_s3outposts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Outposts 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.S3Outposts 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

