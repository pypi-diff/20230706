# Comparing `tmp/mypy-boto3-application-autoscaling-1.27.0.tar.gz` & `tmp/mypy-boto3-application-autoscaling-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-autoscaling-1.27.0.tar", last modified: Mon Jul  3 19:50:22 2023, max compression
+gzip compressed data, was "mypy-boto3-application-autoscaling-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
```

## Comparing `mypy-boto3-application-autoscaling-1.27.0.tar` & `mypy-boto3-application-autoscaling-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-03 19:50:22.000000 mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:22.522822 mypy-boto3-application-autoscaling-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-03 19:32:31.000000 mypy-boto3-application-autoscaling-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.762221 mypy-boto3-application-autoscaling-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-06 20:58:58.754221 mypy-boto3-application-autoscaling-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.746221 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16364 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11797 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22741 2023-07-06 20:33:22.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22698 2023-07-06 20:33:21.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.754221 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 20:58:58.000000 mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.762221 mypy-boto3-application-autoscaling-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-06 20:33:20.000000 mypy-boto3-application-autoscaling-1.28.0/setup.py
```

### Comparing `mypy-boto3-application-autoscaling-1.27.0/LICENSE` & `mypy-boto3-application-autoscaling-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.27.0
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-application-autoscaling-1.27.0/README.md` & `mypy-boto3-application-autoscaling-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__init__.pyi` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/__main__.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationAutoScaling 1.27.0\nVersion:         1.27.0\nBuilder"
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.0\nVersion:         1.28.0\nBuilder"
         " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/client.pyi` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/literals.pyi` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/paginator.pyi` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.py` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling/type_defs.pyi` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-autoscaling
-Version: 1.27.0
-Summary: Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.ApplicationAutoScaling 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-autoscaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_autoscaling/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-autoscaling?color=blue)](https://pypistats.org/packages/mypy-boto3-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationAutoScaling 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
+[boto3.ApplicationAutoScaling 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-application-autoscaling-1.27.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt` & `mypy-boto3-application-autoscaling-1.28.0/mypy_boto3_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-autoscaling-1.27.0/setup.py` & `mypy-boto3-application-autoscaling-1.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-autoscaling",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationAutoScaling 1.27.0 service generated with"
+        "Type annotations for boto3.ApplicationAutoScaling 1.28.0 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

