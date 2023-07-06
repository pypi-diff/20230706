# Comparing `tmp/mypy-boto3-neptune-1.27.0.tar.gz` & `tmp/mypy-boto3-neptune-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-neptune-1.27.0.tar", last modified: Mon Jul  3 19:51:10 2023, max compression
+gzip compressed data, was "mypy-boto3-neptune-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
```

## Comparing `mypy-boto3-neptune-1.27.0.tar` & `mypy-boto3-neptune-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.675726 mypy-boto3-neptune-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-03 19:51:10.671726 mypy-boto3-neptune-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.663725 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84576 2023-07-03 19:42:41.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84499 2023-07-03 19:42:40.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-03 19:42:38.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:10.671726 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:10.000000 mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:10.675726 mypy-boto3-neptune-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:42:37.000000 mypy-boto3-neptune-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67621 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67527 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-07-06 20:48:06.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-06 20:48:06.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84576 2023-07-06 20:48:08.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84499 2023-07-06 20:48:07.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-06 20:48:05.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25543 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:11.000000 mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.866379 mypy-boto3-neptune-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:48:04.000000 mypy-boto3-neptune-1.28.0/setup.py
```

### Comparing `mypy-boto3-neptune-1.27.0/LICENSE` & `mypy-boto3-neptune-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/PKG-INFO` & `mypy-boto3-neptune-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.27.0
-Summary: Type annotations for boto3.Neptune 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-neptune-1.27.0/README.md` & `mypy-boto3-neptune-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__init__.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__init__.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/__main__.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Neptune 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Neptune 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/client.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/client.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/literals.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/literals.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/paginator.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/paginator.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/type_defs.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/type_defs.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/waiter.py` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune/waiter.pyi` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/PKG-INFO` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-neptune
-Version: 1.27.0
-Summary: Type annotations for boto3.Neptune 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-neptune.svg?color=blue)](https://pypi.org/project/mypy-boto3-neptune)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_neptune/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-neptune?color=blue)](https://pypistats.org/packages/mypy-boto3-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Neptune 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
+[boto3.Neptune 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-neptune-1.27.0/mypy_boto3_neptune.egg-info/SOURCES.txt` & `mypy-boto3-neptune-1.28.0/mypy_boto3_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-neptune-1.27.0/setup.py` & `mypy-boto3-neptune-1.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-neptune",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Neptune 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Neptune 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

