# Comparing `tmp/mypy-boto3-license-manager-1.27.0.tar.gz` & `tmp/mypy-boto3-license-manager-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.27.0.tar", last modified: Mon Jul  3 19:51:01 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.28.0.tar", last modified: Thu Jul  6 20:59:59 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.27.0.tar` & `mypy-boto3-license-manager-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.771562 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-03 19:41:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55080 2023-07-03 19:41:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 19:51:01.000000 mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:01.783563 mypy-boto3-license-manager-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-03 19:41:00.000000 mypy-boto3-license-manager-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.986353 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-06 20:45:42.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-06 20:45:45.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55080 2023-07-06 20:45:44.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/setup.py
```

### Comparing `mypy-boto3-license-manager-1.27.0/LICENSE` & `mypy-boto3-license-manager-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/PKG-INFO` & `mypy-boto3-license-manager-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.27.0
-Summary: Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-license-manager-1.27.0/README.md` & `mypy-boto3-license-manager-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.27.0
-Summary: Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-license-manager-1.27.0/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.27.0/setup.py` & `mypy-boto3-license-manager-1.28.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManager 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

