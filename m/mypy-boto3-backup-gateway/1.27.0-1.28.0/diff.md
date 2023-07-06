# Comparing `tmp/mypy-boto3-backup-gateway-1.27.0.tar.gz` & `tmp/mypy-boto3-backup-gateway-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-gateway-1.27.0.tar", last modified: Mon Jul  3 19:50:24 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-gateway-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
```

## Comparing `mypy-boto3-backup-gateway-1.27.0.tar` & `mypy-boto3-backup-gateway-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.938865 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-03 19:33:04.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 19:50:24.000000 mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:24.950865 mypy-boto3-backup-gateway-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-03 19:33:03.000000 mypy-boto3-backup-gateway-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.274228 mypy-boto3-backup-gateway-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-06 20:59:02.270228 mypy-boto3-backup-gateway-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.266228 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19973 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-07-06 20:34:10.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19673 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:09.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.270228 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15904 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:02.000000 mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.274228 mypy-boto3-backup-gateway-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:34:08.000000 mypy-boto3-backup-gateway-1.28.0/setup.py
```

### Comparing `mypy-boto3-backup-gateway-1.27.0/LICENSE` & `mypy-boto3-backup-gateway-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.27.0
-Summary: Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.BackupGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-backup-gateway-1.27.0/README.md` & `mypy-boto3-backup-gateway-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__init__.pyi` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/__main__.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupGateway 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.BackupGateway 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/client.pyi` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/literals.pyi` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/paginator.pyi` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.py` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway/type_defs.pyi` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup-gateway
-Version: 1.27.0
-Summary: Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.BackupGateway 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup-gateway.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup_gateway/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup-gateway?color=blue)](https://pypistats.org/packages/mypy-boto3-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupGateway 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
+[boto3.BackupGateway 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-backup-gateway-1.27.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt` & `mypy-boto3-backup-gateway-1.28.0/mypy_boto3_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-gateway-1.27.0/setup.py` & `mypy-boto3-backup-gateway-1.28.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup-gateway",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupGateway 1.27.0 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.BackupGateway 1.28.0 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

