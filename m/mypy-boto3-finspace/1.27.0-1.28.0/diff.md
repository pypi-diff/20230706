# Comparing `tmp/mypy-boto3-finspace-1.27.0.tar.gz` & `tmp/mypy-boto3-finspace-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.27.0.tar", last modified: Mon Jul  3 19:50:46 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.28.0.tar", last modified: Thu Jul  6 20:59:35 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.27.0.tar` & `mypy-boto3-finspace-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-03 19:37:44.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:50:46.000000 mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:46.279247 mypy-boto3-finspace-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-03 19:37:43.000000 mypy-boto3-finspace-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.070302 mypy-boto3-finspace-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 20:59:35.066302 mypy-boto3-finspace-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.054302 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9692 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-06 20:40:58.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34927 2023-07-06 20:40:59.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34889 2023-07-06 20:40:59.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:35.066302 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 20:59:34.000000 mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:35.070302 mypy-boto3-finspace-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-06 20:40:56.000000 mypy-boto3-finspace-1.28.0/setup.py
```

### Comparing `mypy-boto3-finspace-1.27.0/LICENSE` & `mypy-boto3-finspace-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/PKG-INFO` & `mypy-boto3-finspace-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.27.0
-Summary: Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-finspace-1.27.0/README.md` & `mypy-boto3-finspace-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.finspace 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.27.0
-Summary: Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-finspace?color=blue)](https://pypistats.org/packages/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-finspace-1.27.0/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.28.0/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.27.0/setup.py` & `mypy-boto3-finspace-1.28.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.finspace 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

