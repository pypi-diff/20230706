# Comparing `tmp/mypy-boto3-sdb-1.27.0.tar.gz` & `tmp/mypy-boto3-sdb-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sdb-1.27.0.tar", last modified: Mon Jul  3 19:51:25 2023, max compression
+gzip compressed data, was "mypy-boto3-sdb-1.28.0.tar", last modified: Thu Jul  6 21:00:35 2023, max compression
```

## Comparing `mypy-boto3-sdb-1.27.0.tar` & `mypy-boto3-sdb-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.783969 mypy-boto3-sdb-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 19:47:35.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:25.775969 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:51:25.000000 mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:25.783969 mypy-boto3-sdb-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-03 19:47:34.000000 mypy-boto3-sdb-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.338426 mypy-boto3-sdb-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 21:00:35.330426 mypy-boto3-sdb-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.318426 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10495 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-06 20:55:01.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:35.330426 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:35.000000 mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:35.338426 mypy-boto3-sdb-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-06 20:55:00.000000 mypy-boto3-sdb-1.28.0/setup.py
```

### Comparing `mypy-boto3-sdb-1.27.0/LICENSE` & `mypy-boto3-sdb-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/PKG-INFO` & `mypy-boto3-sdb-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.27.0
-Summary: Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sdb-1.27.0/README.md` & `mypy-boto3-sdb-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__init__.pyi` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/__main__.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SimpleDB 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.SimpleDB 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB\nOther"
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

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/client.pyi` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/literals.pyi` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/paginator.pyi` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.py` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb/type_defs.pyi` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/PKG-INFO` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sdb
-Version: 1.27.0
-Summary: Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sdb.svg?color=blue)](https://pypi.org/project/mypy-boto3-sdb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sdb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sdb?color=blue)](https://pypistats.org/packages/mypy-boto3-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimpleDB 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
+[boto3.SimpleDB 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-sdb-1.27.0/mypy_boto3_sdb.egg-info/SOURCES.txt` & `mypy-boto3-sdb-1.28.0/mypy_boto3_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sdb-1.27.0/setup.py` & `mypy-boto3-sdb-1.28.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sdb",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimpleDB 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.SimpleDB 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

