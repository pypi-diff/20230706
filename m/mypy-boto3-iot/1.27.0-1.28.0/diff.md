# Comparing `tmp/mypy-boto3-iot-1.27.0.tar.gz` & `tmp/mypy-boto3-iot-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.27.0.tar", last modified: Mon Jul  3 19:50:54 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-1.28.0.tar", last modified: Thu Jul  6 20:59:47 2023, max compression
```

## Comparing `mypy-boto3-iot-1.27.0.tar` & `mypy-boto3-iot-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.043424 mypy-boto3-iot-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-03 19:50:54.043424 mypy-boto3-iot-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    52856 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.035423 mypy-boto3-iot-1.27.0/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-03 19:39:19.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-03 19:39:19.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-07-03 19:39:21.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    24957 2023-07-03 19:39:21.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    69164 2023-07-03 19:39:21.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    69103 2023-07-03 19:39:21.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   257086 2023-07-03 19:39:28.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   256759 2023-07-03 19:39:24.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:54.043424 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:53.000000 mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:54.043424 mypy-boto3-iot-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:39:18.000000 mypy-boto3-iot-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    52856 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.302328 mypy-boto3-iot-1.28.0/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-06 20:43:16.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24959 2023-07-06 20:43:18.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24957 2023-07-06 20:43:18.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    69164 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69103 2023-07-06 20:43:17.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   257086 2023-07-06 20:43:27.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   256759 2023-07-06 20:43:23.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54325 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:47.000000 mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:47.306328 mypy-boto3-iot-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:43:13.000000 mypy-boto3-iot-1.28.0/setup.py
```

### Comparing `mypy-boto3-iot-1.27.0/LICENSE` & `mypy-boto3-iot-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/PKG-INFO` & `mypy-boto3-iot-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.27.0
-Summary: Type annotations for boto3.IoT 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iot-1.27.0/README.md` & `mypy-boto3-iot-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.IoT 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.27.0
-Summary: Type annotations for boto3.IoT 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iot?color=blue)](https://pypistats.org/packages/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iot-1.27.0/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.28.0/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.27.0/setup.py` & `mypy-boto3-iot-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.IoT 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

