# Comparing `tmp/mypy-boto3-schemas-1.27.0.tar.gz` & `tmp/mypy-boto3-schemas-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-schemas-1.27.0.tar", last modified: Mon Jul  3 19:51:25 2023, max compression
+gzip compressed data, was "mypy-boto3-schemas-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
```

## Comparing `mypy-boto3-schemas-1.27.0.tar` & `mypy-boto3-schemas-1.28.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-07-03 19:47:34.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-03 19:47:34.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 19:47:33.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 19:51:25.000000 mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:25.423962 mypy-boto3-schemas-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 19:47:30.000000 mypy-boto3-schemas-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.038426 mypy-boto3-schemas-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:35.030426 mypy-boto3-schemas-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15184 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.026426 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23385 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23341 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26173 2023-07-06 20:55:00.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-06 20:54:59.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.030426 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 21:00:34.000000 mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.038426 mypy-boto3-schemas-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:54:58.000000 mypy-boto3-schemas-1.28.0/setup.py
```

### Comparing `mypy-boto3-schemas-1.27.0/LICENSE` & `mypy-boto3-schemas-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/PKG-INFO` & `mypy-boto3-schemas-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.27.0
-Summary: Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-schemas-1.27.0/README.md` & `mypy-boto3-schemas-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__init__.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/__main__.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Schemas 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Schemas 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/client.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/literals.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/paginator.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/type_defs.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.py` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas/waiter.pyi` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/PKG-INFO` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-schemas
-Version: 1.27.0
-Summary: Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-schemas.svg?color=blue)](https://pypi.org/project/mypy-boto3-schemas)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_schemas/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-schemas?color=blue)](https://pypistats.org/packages/mypy-boto3-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Schemas 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[boto3.Schemas 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-schemas-1.27.0/mypy_boto3_schemas.egg-info/SOURCES.txt` & `mypy-boto3-schemas-1.28.0/mypy_boto3_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-schemas-1.27.0/setup.py` & `mypy-boto3-schemas-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-schemas",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Schemas 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Schemas 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

