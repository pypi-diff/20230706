# Comparing `tmp/tufup-0.5.0.tar.gz` & `tmp/tufup-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tufup-0.5.0.tar", last modified: Mon May 29 14:14:08 2023, max compression
+gzip compressed data, was "tufup-0.5.1.tar", last modified: Thu Jul  6 15:35:20 2023, max compression
```

## Comparing `tufup-0.5.0.tar` & `tufup-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.812245 tufup-0.5.0/
--rw-rw-rw-   0        0        0     1084 2022-03-25 16:00:29.000000 tufup-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    14727 2023-05-29 14:14:08.812245 tufup-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    12845 2023-05-29 09:58:53.000000 tufup-0.5.0/README.md
--rw-rw-rw-   0        0        0     1366 2023-05-29 14:10:44.000000 tufup-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 14:14:08.812245 tufup-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.781003 tufup-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/
--rw-rw-rw-   0        0        0      893 2023-05-29 14:12:06.000000 tufup-0.5.0/src/tufup/__init__.py
--rw-rw-rw-   0        0        0      292 2022-07-01 14:31:47.000000 tufup-0.5.0/src/tufup/__main__.py
--rw-rw-rw-   0        0        0    15506 2023-05-29 14:10:44.000000 tufup-0.5.0/src/tufup/client.py
--rw-rw-rw-   0        0        0     4907 2022-07-01 14:31:47.000000 tufup-0.5.0/src/tufup/common.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/repo/
--rw-rw-rw-   0        0        0    37645 2023-05-29 14:10:44.000000 tufup-0.5.0/src/tufup/repo/__init__.py
--rw-rw-rw-   0        0        0    12311 2023-05-29 09:58:53.000000 tufup-0.5.0/src/tufup/repo/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup/utils/
--rw-rw-rw-   0        0        0     3739 2022-11-28 08:44:28.000000 tufup-0.5.0/src/tufup/utils/__init__.py
--rw-rw-rw-   0        0        0     9721 2022-11-18 17:21:40.000000 tufup-0.5.0/src/tufup/utils/platform_specific.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.796624 tufup-0.5.0/src/tufup.egg-info/
--rw-rw-rw-   0        0        0    14727 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      141 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-29 14:14:08.000000 tufup-0.5.0/src/tufup.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 14:14:08.812245 tufup-0.5.0/tests/
--rw-rw-rw-   0        0        0    13902 2023-05-29 14:10:44.000000 tufup-0.5.0/tests/test_client.py
--rw-rw-rw-   0        0        0     7162 2022-07-01 14:31:47.000000 tufup-0.5.0/tests/test_common.py
--rw-rw-rw-   0        0        0      279 2022-09-26 20:49:28.000000 tufup-0.5.0/tests/test_package.py
--rw-rw-rw-   0        0        0    35282 2023-05-29 09:58:53.000000 tufup-0.5.0/tests/test_repo.py
--rw-rw-rw-   0        0        0     9484 2023-05-29 09:58:53.000000 tufup-0.5.0/tests/test_repo_cli.py
--rw-rw-rw-   0        0        0     1249 2022-06-22 14:44:45.000000 tufup-0.5.0/tests/test_tests.py
--rw-rw-rw-   0        0        0     3926 2022-11-28 08:44:28.000000 tufup-0.5.0/tests/test_utils.py
--rw-rw-rw-   0        0        0     9387 2022-09-29 11:58:03.000000 tufup-0.5.0/tests/test_utils_platform_specific.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.619284 tufup-0.5.1/
+-rw-rw-rw-   0        0        0     1084 2022-09-21 07:49:55.000000 tufup-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    14727 2023-07-06 15:35:20.619284 tufup-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12845 2023-07-06 14:59:02.000000 tufup-0.5.1/README.md
+-rw-rw-rw-   0        0        0     1366 2023-07-06 15:29:02.000000 tufup-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:35:20.619284 tufup-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.503406 tufup-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.534653 tufup-0.5.1/src/tufup/
+-rw-rw-rw-   0        0        0      893 2023-07-06 15:31:26.000000 tufup-0.5.1/src/tufup/__init__.py
+-rw-rw-rw-   0        0        0      292 2022-09-21 07:49:56.000000 tufup-0.5.1/src/tufup/__main__.py
+-rw-rw-rw-   0        0        0    15506 2023-07-06 14:59:02.000000 tufup-0.5.1/src/tufup/client.py
+-rw-rw-rw-   0        0        0     4907 2022-09-21 07:49:56.000000 tufup-0.5.1/src/tufup/common.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.556780 tufup-0.5.1/src/tufup/repo/
+-rw-rw-rw-   0        0        0    37645 2023-07-06 14:59:02.000000 tufup-0.5.1/src/tufup/repo/__init__.py
+-rw-rw-rw-   0        0        0    12311 2023-07-06 14:59:02.000000 tufup-0.5.1/src/tufup/repo/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.572427 tufup-0.5.1/src/tufup/utils/
+-rw-rw-rw-   0        0        0     3739 2022-09-21 07:49:56.000000 tufup-0.5.1/src/tufup/utils/__init__.py
+-rw-rw-rw-   0        0        0     9721 2022-10-04 13:22:25.000000 tufup-0.5.1/src/tufup/utils/platform_specific.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.556780 tufup-0.5.1/src/tufup.egg-info/
+-rw-rw-rw-   0        0        0    14727 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      141 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-06 15:35:20.000000 tufup-0.5.1/src/tufup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 15:35:20.603659 tufup-0.5.1/tests/
+-rw-rw-rw-   0        0        0    13902 2023-07-06 14:59:02.000000 tufup-0.5.1/tests/test_client.py
+-rw-rw-rw-   0        0        0     7162 2022-09-21 07:49:56.000000 tufup-0.5.1/tests/test_common.py
+-rw-rw-rw-   0        0        0      279 2022-10-04 13:22:25.000000 tufup-0.5.1/tests/test_package.py
+-rw-rw-rw-   0        0        0    35282 2023-07-06 14:59:02.000000 tufup-0.5.1/tests/test_repo.py
+-rw-rw-rw-   0        0        0     9484 2023-07-06 14:59:02.000000 tufup-0.5.1/tests/test_repo_cli.py
+-rw-rw-rw-   0        0        0     1249 2022-09-21 07:49:56.000000 tufup-0.5.1/tests/test_tests.py
+-rw-rw-rw-   0        0        0     3926 2022-09-21 07:49:56.000000 tufup-0.5.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0     9387 2022-10-04 13:22:25.000000 tufup-0.5.1/tests/test_utils_platform_specific.py
```

### Comparing `tufup-0.5.0/LICENSE` & `tufup-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/PKG-INFO` & `tufup-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tufup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
 Author-email: dennisvang <djvg@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dennis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tufup-0.5.0/README.md` & `tufup-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/pyproject.toml` & `tufup-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.8"
 dependencies = [
     # direct dependencies
     "bsdiff4==1.2.*",
-    "packaging==21.*",
+    "packaging>=21.3",
     "securesystemslib[crypto,pynacl]>=0.26.0",
     "setuptools>=65.5.1",
     "tuf==3.0.*",
     # constraints on sub-dependencies
     "certifi>=2022.12.7",
     "cryptography>=38.0.3",
 ]
```

### Comparing `tufup-0.5.0/src/tufup/__init__.py` & `tufup-0.5.1/src/tufup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 from tufup.repo import cli
 from tufup.utils import input_bool
 
 # https://packaging.python.org/en/latest/guides/single-sourcing-package-version/
 # https://semver.org/
-__version__ = '0.5.0'
+__version__ = '0.5.1'
 
 logger = logging.getLogger(__name__)
 
 
 def main(args=None):
     print(f'tufup version: {__version__}')
     # default to --help
```

### Comparing `tufup-0.5.0/src/tufup/client.py` & `tufup-0.5.1/src/tufup/client.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup/common.py` & `tufup-0.5.1/src/tufup/common.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup/repo/__init__.py` & `tufup-0.5.1/src/tufup/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup/repo/cli.py` & `tufup-0.5.1/src/tufup/repo/cli.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup/utils/__init__.py` & `tufup-0.5.1/src/tufup/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup/utils/platform_specific.py` & `tufup-0.5.1/src/tufup/utils/platform_specific.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/src/tufup.egg-info/PKG-INFO` & `tufup-0.5.1/src/tufup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tufup
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automated updates for stand-alone Python applications, built upon python-tuf.
 Author-email: dennisvang <djvg@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Dennis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tufup-0.5.0/src/tufup.egg-info/SOURCES.txt` & `tufup-0.5.1/src/tufup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_client.py` & `tufup-0.5.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_common.py` & `tufup-0.5.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_repo.py` & `tufup-0.5.1/tests/test_repo.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_repo_cli.py` & `tufup-0.5.1/tests/test_repo_cli.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_tests.py` & `tufup-0.5.1/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_utils.py` & `tufup-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tufup-0.5.0/tests/test_utils_platform_specific.py` & `tufup-0.5.1/tests/test_utils_platform_specific.py`

 * *Files identical despite different names*

