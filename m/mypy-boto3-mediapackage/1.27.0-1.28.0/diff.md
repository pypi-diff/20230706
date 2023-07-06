# Comparing `tmp/mypy-boto3-mediapackage-1.27.0.tar.gz` & `tmp/mypy-boto3-mediapackage-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediapackage-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
+gzip compressed data, was "mypy-boto3-mediapackage-1.28.0.tar", last modified: Thu Jul  6 21:00:05 2023, max compression
```

## Comparing `mypy-boto3-mediapackage-1.27.0.tar` & `mypy-boto3-mediapackage-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.251644 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-07-03 19:42:05.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:06.000000 mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.255644 mypy-boto3-mediapackage-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:42:04.000000 mypy-boto3-mediapackage-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.742366 mypy-boto3-mediapackage-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-06 21:00:05.738366 mypy-boto3-mediapackage-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.718366 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-06 20:47:16.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-07-06 20:47:17.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25742 2023-07-06 20:47:17.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:14.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.738366 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15826 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:05.000000 mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:05.742366 mypy-boto3-mediapackage-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:47:13.000000 mypy-boto3-mediapackage-1.28.0/setup.py
```

### Comparing `mypy-boto3-mediapackage-1.27.0/LICENSE` & `mypy-boto3-mediapackage-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/PKG-INFO` & `mypy-boto3-mediapackage-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediapackage-1.27.0/README.md` & `mypy-boto3-mediapackage-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__init__.pyi` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/__main__.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaPackage 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.MediaPackage 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage\nOther"
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

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/client.pyi` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/literals.pyi` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/paginator.pyi` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.py` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage/type_defs.pyi` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/PKG-INFO` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediapackage
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediapackage.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediapackage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediapackage/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediapackage?color=blue)](https://pypistats.org/packages/mypy-boto3-mediapackage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaPackage 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
+[boto3.MediaPackage 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediapackage-1.27.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt` & `mypy-boto3-mediapackage-1.28.0/mypy_boto3_mediapackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediapackage-1.27.0/setup.py` & `mypy-boto3-mediapackage-1.28.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediapackage",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_mediapackage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaPackage 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaPackage 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

