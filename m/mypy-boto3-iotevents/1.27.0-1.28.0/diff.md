# Comparing `tmp/mypy-boto3-iotevents-1.27.0.tar.gz` & `tmp/mypy-boto3-iotevents-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.28.0.tar", last modified: Thu Jul  6 20:59:48 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.27.0.tar` & `mypy-boto3-iotevents-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.771436 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-07-03 19:39:39.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-03 19:50:54.000000 mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.787437 mypy-boto3-iotevents-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 19:39:38.000000 mypy-boto3-iotevents-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.146330 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-07-06 20:43:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-07-06 20:43:45.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/setup.py
```

### Comparing `mypy-boto3-iotevents-1.27.0/LICENSE` & `mypy-boto3-iotevents-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/PKG-INFO` & `mypy-boto3-iotevents-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.27.0
-Summary: Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IoTEvents 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotevents-1.27.0/README.md` & `mypy-boto3-iotevents-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/__main__.py` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEvents 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.IoTEvents 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents/type_defs.pyi` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/PKG-INFO` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.27.0
-Summary: Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IoTEvents 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotevents-1.27.0/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.27.0/setup.py` & `mypy-boto3-iotevents-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEvents 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.IoTEvents 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

