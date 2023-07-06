# Comparing `tmp/helper-mapilio-1.1.8.tar.gz` & `tmp/helper-mapilio-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/helper-mapilio-1.1.8.tar", last modified: Fri Mar 12 07:04:32 2021, max compression
+gzip compressed data, was "dist/helper-mapilio-1.1.9.tar", last modified: Fri Mar 12 07:33:14 2021, max compression
```

## Comparing `helper-mapilio-1.1.8.tar` & `helper-mapilio-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:04:32.000000 helper-mapilio-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)      241 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:04:32.000000 helper-mapilio-1.1.8/helper/
--rw-r--r--   0 runner    (1001) docker     (116)     3823 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/rule.py
--rw-r--r--   0 runner    (1001) docker     (116)     1721 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/convertor.py
--rw-r--r--   0 runner    (1001) docker     (116)     9417 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/geo.py
--rw-r--r--   0 runner    (1001) docker     (116)      371 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/handler.py
--rw-r--r--   0 runner    (1001) docker     (116)     1862 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     5338 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/generator.py
--rw-r--r--   0 runner    (1001) docker     (116)      186 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/util.py
--rw-r--r--   0 runner    (1001) docker     (116)      560 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13642 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/helper/exif_read.py
--rw-r--r--   0 runner    (1001) docker     (116)      482 2021-03-12 07:04:32.000000 helper-mapilio-1.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:04:32.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-12 07:04:31.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-03-12 07:04:31.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-03-12 07:04:31.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      482 2021-03-12 07:04:31.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-12 07:04:31.000000 helper-mapilio-1.1.8/helper_mapilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-12 07:04:32.000000 helper-mapilio-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1253 2021-03-12 07:04:13.000000 helper-mapilio-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      241 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper/
+-rw-r--r--   0 runner    (1001) docker     (116)     3823 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1721 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9417 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/geo.py
+-rw-r--r--   0 runner    (1001) docker     (116)      371 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/handler.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1862 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5338 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/generator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      223 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/util.py
+-rw-r--r--   0 runner    (1001) docker     (116)      580 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13642 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/helper/exif_read.py
+-rw-r--r--   0 runner    (1001) docker     (116)      482 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      482 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      365 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/helper_mapilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-12 07:33:14.000000 helper-mapilio-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1224 2021-03-12 07:32:55.000000 helper-mapilio-1.1.9/setup.py
```

### Comparing `helper-mapilio-1.1.8/helper/rule.py` & `helper-mapilio-1.1.9/helper/rule.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/helper/convertor.py` & `helper-mapilio-1.1.9/helper/convertor.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/helper/geo.py` & `helper-mapilio-1.1.9/helper/geo.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/helper/logger.py` & `helper-mapilio-1.1.9/helper/logger.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/helper/generator.py` & `helper-mapilio-1.1.9/helper/generator.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/helper/__init__.py` & `helper-mapilio-1.1.9/helper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 from .generator import Generator
 from .logger import Logger, TimeLogger
 from .handler import Handler
 from .convertor import Convertor
 from .rule import Utilities
 
 
-from .util import __version__, get_version
+from .util import __version__, __major__, __minor__, __patch__
```

### Comparing `helper-mapilio-1.1.8/helper/exif_read.py` & `helper-mapilio-1.1.9/helper/exif_read.py`

 * *Files identical despite different names*

### Comparing `helper-mapilio-1.1.8/setup.py` & `helper-mapilio-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,25 @@
     raise RuntimeError(
         "Mapilio Helper tools supports Python 3.6 and above. "
     )
 
 # This import must be below the above `sys.version_info` check,
 # because the code being imported here is not compatible with the older
 # versions of Python.
-from helper.util import __version__ as version # noqa
 from increment_version import __version__
+from helper.util import __name__
 
 INSTALL_REQUIRES = [
     'trianglesolver==1.2',
     'opencv-python==4.5.1.48',
     'addict==2.4.0'
 ]
 
 setup(
-    name='helper-mapilio',
+    name=__name__,
     version=__version__,
     description='Mapilio Helper Library',
     url='https://github.com/mapilio/helper.git',
     author='Mapilio - Ozcan Durak & M.Can VARER',
     author_email='ozcan@visiosoft.com.tr',
     license='licensed',
     packages=find_packages(),
```

