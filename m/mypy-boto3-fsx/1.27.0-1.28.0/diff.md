# Comparing `tmp/mypy-boto3-fsx-1.27.0.tar.gz` & `tmp/mypy-boto3-fsx-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fsx-1.27.0.tar", last modified: Mon Jul  3 19:50:47 2023, max compression
+gzip compressed data, was "mypy-boto3-fsx-1.28.0.tar", last modified: Thu Jul  6 20:59:37 2023, max compression
```

## Comparing `mypy-boto3-fsx-1.27.0.tar` & `mypy-boto3-fsx-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-03 19:38:05.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    79400 2023-07-03 19:38:07.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79303 2023-07-03 19:38:05.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 19:50:47.000000 mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:50:47.979278 mypy-boto3-fsx-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-03 19:38:04.000000 mypy-boto3-fsx-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.846308 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38786 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38733 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-07-06 20:41:31.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-06 20:41:29.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79400 2023-07-06 20:41:33.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79303 2023-07-06 20:41:32.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:37.000000 mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:37.854308 mypy-boto3-fsx-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:41:28.000000 mypy-boto3-fsx-1.28.0/setup.py
```

### Comparing `mypy-boto3-fsx-1.27.0/LICENSE` & `mypy-boto3-fsx-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/PKG-INFO` & `mypy-boto3-fsx-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.27.0
-Summary: Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-fsx-1.27.0/README.md` & `mypy-boto3-fsx-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__init__.pyi` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/__main__.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FSx 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.FSx 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/client.pyi` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/literals.pyi` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/paginator.pyi` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.py` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2498,15 +2498,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2573,15 +2573,15 @@
         "Name": str,
         "OntapConfiguration": OntapVolumeConfigurationTypeDef,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "VolumeId": str,
         "VolumeType": VolumeTypeType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
```

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx/type_defs.pyi` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx/type_defs.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2413,15 +2413,15 @@
         "NetworkInterfaceIds": List[str],
         "DNSName": str,
         "KmsKeyId": str,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "WindowsConfiguration": WindowsFileSystemConfigurationTypeDef,
         "LustreConfiguration": LustreFileSystemConfigurationTypeDef,
-        "AdministrativeActions": List[Dict[str, Any]],
+        "AdministrativeActions": List["AdministrativeActionTypeDef"],
         "OntapConfiguration": OntapFileSystemConfigurationTypeDef,
         "FileSystemTypeVersion": str,
         "OpenZFSConfiguration": OpenZFSFileSystemConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -2484,15 +2484,15 @@
         "Name": str,
         "OntapConfiguration": OntapVolumeConfigurationTypeDef,
         "ResourceARN": str,
         "Tags": List[TagTypeDef],
         "VolumeId": str,
         "VolumeType": VolumeTypeType,
         "LifecycleTransitionReason": LifecycleTransitionReasonTypeDef,
-        "AdministrativeActions": List["AdministrativeActionTypeDef"],
+        "AdministrativeActions": List[Dict[str, Any]],
         "OpenZFSConfiguration": OpenZFSVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateVolumeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVolumeRequestRequestTypeDef",
```

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/PKG-INFO` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fsx
-Version: 1.27.0
-Summary: Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fsx.svg?color=blue)](https://pypi.org/project/mypy-boto3-fsx)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fsx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-fsx?color=blue)](https://pypistats.org/packages/mypy-boto3-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FSx 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[boto3.FSx 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-fsx-1.27.0/mypy_boto3_fsx.egg-info/SOURCES.txt` & `mypy-boto3-fsx-1.28.0/mypy_boto3_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fsx-1.27.0/setup.py` & `mypy-boto3-fsx-1.28.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fsx",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FSx 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.FSx 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

