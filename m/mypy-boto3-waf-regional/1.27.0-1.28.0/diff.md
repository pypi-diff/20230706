# Comparing `tmp/mypy-boto3-waf-regional-1.27.0.tar.gz` & `tmp/mypy-boto3-waf-regional-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-waf-regional-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
+gzip compressed data, was "mypy-boto3-waf-regional-1.28.0.tar", last modified: Thu Jul  6 21:00:50 2023, max compression
```

## Comparing `mypy-boto3-waf-regional-1.27.0.tar` & `mypy-boto3-waf-regional-1.28.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.728135 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55486 2023-07-03 19:49:30.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55439 2023-07-03 19:49:29.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 19:51:35.000000 mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.732135 mypy-boto3-waf-regional-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-03 19:49:28.000000 mypy-boto3-waf-regional-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46208 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46120 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-06 20:57:46.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-07-06 20:57:46.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55486 2023-07-06 20:57:47.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55439 2023-07-06 20:57:47.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20419 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:50.000000 mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:50.446457 mypy-boto3-waf-regional-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:57:45.000000 mypy-boto3-waf-regional-1.28.0/setup.py
```

### Comparing `mypy-boto3-waf-regional-1.27.0/LICENSE` & `mypy-boto3-waf-regional-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/PKG-INFO` & `mypy-boto3-waf-regional-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.27.0
-Summary: Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-waf-regional-1.27.0/README.md` & `mypy-boto3-waf-regional-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/__main__.py` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFRegional 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.WAFRegional 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional\nOther"
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

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.py` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/client.pyi` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.py` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/literals.pyi` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.py` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional/type_defs.pyi` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/PKG-INFO` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-waf-regional
-Version: 1.27.0
-Summary: Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-waf-regional.svg?color=blue)](https://pypi.org/project/mypy-boto3-waf-regional)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_waf_regional/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-waf-regional?color=blue)](https://pypistats.org/packages/mypy-boto3-waf-regional)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFRegional 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
+[boto3.WAFRegional 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#WAFRegional)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-waf-regional-1.27.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt` & `mypy-boto3-waf-regional-1.28.0/mypy_boto3_waf_regional.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-waf-regional-1.27.0/setup.py` & `mypy-boto3-waf-regional-1.28.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-waf-regional",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_waf_regional"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WAFRegional 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.WAFRegional 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

