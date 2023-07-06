# Comparing `tmp/mypy-boto3-voice-id-1.27.0.tar.gz` & `tmp/mypy-boto3-voice-id-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.27.0.tar", last modified: Mon Jul  3 19:51:35 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.28.0.tar", last modified: Thu Jul  6 21:00:49 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.27.0.tar` & `mypy-boto3-voice-id-1.28.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32450 2023-07-03 19:49:19.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-03 19:51:35.000000 mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 19:51:35.420130 mypy-boto3-voice-id-1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 19:49:18.000000 mypy-boto3-voice-id-1.27.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.874456 mypy-boto3-voice-id-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-06 21:00:49.862456 mypy-boto3-voice-id-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.854456 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32487 2023-07-06 20:57:33.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32450 2023-07-06 20:57:32.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:49.862456 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 21:00:49.000000 mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:49.874456 mypy-boto3-voice-id-1.28.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-06 20:57:31.000000 mypy-boto3-voice-id-1.28.0/setup.py
```

### Comparing `mypy-boto3-voice-id-1.27.0/LICENSE` & `mypy-boto3-voice-id-1.28.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/PKG-INFO` & `mypy-boto3-voice-id-1.28.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.27.0
-Summary: Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-voice-id-1.27.0/README.md` & `mypy-boto3-voice-id-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.27.0\nVersion:         1.27.0\nBuilder version:"
+        "Type annotations for boto3.VoiceID 1.28.0\nVersion:         1.28.0\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.27.0
-Summary: Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.0
+Summary: Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-voice-id?color=blue)](https://pypistats.org/packages/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.27.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-voice-id-1.27.0/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.28.0/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.27.0/setup.py` & `mypy-boto3-voice-id-1.28.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.27.0",
+    version="1.28.0",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VoiceID 1.27.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.VoiceID 1.28.0 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

