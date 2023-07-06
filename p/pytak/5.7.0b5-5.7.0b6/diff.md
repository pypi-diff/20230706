# Comparing `tmp/pytak-5.7.0b5.tar.gz` & `tmp/pytak-5.7.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytak-5.7.0b5.tar", last modified: Thu Jun 22 23:09:56 2023, max compression
+gzip compressed data, was "pytak-5.7.0b6.tar", last modified: Thu Jul  6 04:25:26 2023, max compression
```

## Comparing `pytak-5.7.0b5.tar` & `pytak-5.7.0b6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 23:09:56.574993 pytak-5.7.0b5/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 23:09:46.000000 pytak-5.7.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-22 23:09:46.000000 pytak-5.7.0b5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 23:09:56.574993 pytak-5.7.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-06-22 23:09:46.000000 pytak-5.7.0b5/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 23:09:56.566993 pytak-5.7.0b5/pytak/
--rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 23:09:56.570993 pytak-5.7.0b5/pytak/asyncio_dgram/
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/asyncio_dgram/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/asyncio_dgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9911 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/asyncio_dgram/aio.py
--rw-r--r--   0 runner    (1001) docker     (122)    13245 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    15504 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/client_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/crypto_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5263 2023-06-22 23:09:46.000000 pytak-5.7.0b5/pytak/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 23:09:56.570993 pytak-5.7.0b5/pytak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-06-22 23:09:56.000000 pytak-5.7.0b5/pytak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-06-22 23:09:56.000000 pytak-5.7.0b5/pytak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 23:09:56.000000 pytak-5.7.0b5/pytak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-22 23:09:56.000000 pytak-5.7.0b5/pytak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-22 23:09:56.000000 pytak-5.7.0b5/pytak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-06-22 23:09:56.574993 pytak-5.7.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-22 23:09:46.000000 pytak-5.7.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 04:25:26.770093 pytak-5.7.0b6/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-07-06 04:25:16.000000 pytak-5.7.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-06 04:25:16.000000 pytak-5.7.0b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-07-06 04:25:26.770093 pytak-5.7.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-06 04:25:16.000000 pytak-5.7.0b6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 04:25:26.770093 pytak-5.7.0b6/pytak/
+-rw-r--r--   0 runner    (1001) docker     (122)     1820 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 04:25:26.770093 pytak-5.7.0b6/pytak/asyncio_dgram/
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/asyncio_dgram/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/asyncio_dgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9911 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/asyncio_dgram/aio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13245 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15504 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/client_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      998 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2938 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/crypto_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5263 2023-07-06 04:25:16.000000 pytak-5.7.0b6/pytak/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 04:25:26.770093 pytak-5.7.0b6/pytak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2970 2023-07-06 04:25:26.000000 pytak-5.7.0b6/pytak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-06 04:25:26.000000 pytak-5.7.0b6/pytak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 04:25:26.000000 pytak-5.7.0b6/pytak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-06 04:25:26.000000 pytak-5.7.0b6/pytak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-06 04:25:26.000000 pytak-5.7.0b6/pytak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-07-06 04:25:26.770093 pytak-5.7.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-07-06 04:25:16.000000 pytak-5.7.0b6/setup.py
```

### Comparing `pytak-5.7.0b5/LICENSE` & `pytak-5.7.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/PKG-INFO` & `pytak-5.7.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 5.7.0b5
+Version: 5.7.0b6
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/pytak/actions
```

### Comparing `pytak-5.7.0b5/README.rst` & `pytak-5.7.0b6/README.rst`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/__init__.py` & `pytak-5.7.0b6/pytak/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 
 """Python Team Awareness Kit (PyTAK) Module.
 
 :source: <https://github.com/snstac/pytak>
 """
 
-__version__ = "5.7.0-beta5"
+__version__ = "5.7.0-beta6"
 
 
 from .constants import (  # NOQA
     LOG_LEVEL,
     LOG_FORMAT,
     DEFAULT_COT_PORT,
     DEFAULT_BACKOFF,
```

### Comparing `pytak-5.7.0b5/pytak/asyncio_dgram/LICENSE` & `pytak-5.7.0b6/pytak/asyncio_dgram/LICENSE`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/asyncio_dgram/aio.py` & `pytak-5.7.0b6/pytak/asyncio_dgram/aio.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/classes.py` & `pytak-5.7.0b6/pytak/classes.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/client_functions.py` & `pytak-5.7.0b6/pytak/client_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/commands.py` & `pytak-5.7.0b6/pytak/commands.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/constants.py` & `pytak-5.7.0b6/pytak/constants.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/crypto_functions.py` & `pytak-5.7.0b6/pytak/crypto_functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak/functions.py` & `pytak-5.7.0b6/pytak/functions.py`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/pytak.egg-info/PKG-INFO` & `pytak-5.7.0b6/pytak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytak
-Version: 5.7.0b5
+Version: 5.7.0b6
 Summary: PyTAK: Python Team Awareness Kit Module
 Home-page: https://github.com/snstac/pytak
 Author-email: Greg Albrecht <oss@undef.net>
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/pytak/actions
```

### Comparing `pytak-5.7.0b5/setup.cfg` & `pytak-5.7.0b6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytak-5.7.0b5/setup.py` & `pytak-5.7.0b6/setup.py`

 * *Files identical despite different names*

