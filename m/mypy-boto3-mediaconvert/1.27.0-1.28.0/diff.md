# Comparing `tmp/mypy-boto3-mediaconvert-1.27.0.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.27.0.tar", last modified: Mon Jul  3 19:51:06 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.28.0.tar", last modified: Thu Jul  6 21:00:05 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.27.0.tar` & `mypy-boto3-mediaconvert-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55528 2023-07-03 19:41:51.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-03 19:41:50.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103367 2023-07-03 19:41:53.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103342 2023-07-03 19:41:52.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:05.000000 mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:06.015640 mypy-boto3-mediaconvert-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-03 19:41:49.000000 mypy-boto3-mediaconvert-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.042365 mypy-boto3-mediaconvert-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-06 21:00:05.038365 mypy-boto3-mediaconvert-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.026365 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55528 2023-07-06 20:46:55.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-06 20:46:55.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103367 2023-07-06 20:47:00.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103342 2023-07-06 20:46:59.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.038365 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:05.042365 mypy-boto3-mediaconvert-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:46:53.000000 mypy-boto3-mediaconvert-1.28.0/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.27.0/LICENSE` & `mypy-boto3-mediaconvert-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconvert-1.27.0/README.md` & `mypy-boto3-mediaconvert-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.MediaConvert 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
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

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.27.0
-Summary: Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-mediaconvert-1.27.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.27.0/setup.py` & `mypy-boto3-mediaconvert-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

