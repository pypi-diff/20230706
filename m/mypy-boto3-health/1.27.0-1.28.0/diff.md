# Comparing `tmp/mypy-boto3-health-1.27.0.tar.gz` & `tmp/mypy-boto3-health-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-health-1.27.0.tar", last modified: Mon Jul  3 19:50:50 2023, max compression
+gzip compressed data, was "mypy-boto3-health-1.28.0.tar", last modified: Thu Jul  6 20:59:42 2023, max compression
```

## Comparing `mypy-boto3-health-1.27.0.tar` & `mypy-boto3-health-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.303355 mypy-boto3-health-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/mypy_boto3_health/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-07-03 19:38:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-07-03 19:38:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/mypy_boto3_health/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:50.295355 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 19:50:50.000000 mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:50.303355 mypy-boto3-health-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-03 19:38:49.000000 mypy-boto3-health-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.034317 mypy-boto3-health-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:42:32.000000 mypy-boto3-health-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-06 20:59:42.022317 mypy-boto3-health-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-07-06 20:42:32.000000 mypy-boto3-health-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.022317 mypy-boto3-health-1.28.0/mypy_boto3_health/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9824 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:42:34.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21653 2023-07-06 20:42:35.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21628 2023-07-06 20:42:35.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:42:32.000000 mypy-boto3-health-1.28.0/mypy_boto3_health/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:42.022317 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:41.000000 mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:42.034317 mypy-boto3-health-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:42:32.000000 mypy-boto3-health-1.28.0/setup.py
```

### Comparing `mypy-boto3-health-1.27.0/LICENSE` & `mypy-boto3-health-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/PKG-INFO` & `mypy-boto3-health-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.27.0
-Summary: Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Health 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.27.0/README.md` & `mypy-boto3-health-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/__init__.pyi` & `mypy-boto3-health-1.28.0/mypy_boto3_health/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/__main__.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Health 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.Health 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health\nOther"
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

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/client.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/client.pyi` & `mypy-boto3-health-1.28.0/mypy_boto3_health/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/literals.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/literals.pyi` & `mypy-boto3-health-1.28.0/mypy_boto3_health/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/paginator.pyi` & `mypy-boto3-health-1.28.0/mypy_boto3_health/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.py` & `mypy-boto3-health-1.28.0/mypy_boto3_health/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health/type_defs.pyi` & `mypy-boto3-health-1.28.0/mypy_boto3_health/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/PKG-INFO` & `mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-health
-Version: 1.27.0
-Summary: Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.Health 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-health.svg?color=blue)](https://pypi.org/project/mypy-boto3-health)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_health/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-health?color=blue)](https://pypistats.org/packages/mypy-boto3-health)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Health 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
+[boto3.Health 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-health-1.27.0/mypy_boto3_health.egg-info/SOURCES.txt` & `mypy-boto3-health-1.28.0/mypy_boto3_health.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-health-1.27.0/setup.py` & `mypy-boto3-health-1.28.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-health",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_health"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Health 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Health 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

