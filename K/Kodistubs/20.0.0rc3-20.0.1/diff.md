# Comparing `tmp/Kodistubs-20.0.0rc3.tar.gz` & `tmp/Kodistubs-20.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kodistubs-20.0.0rc3.tar", last modified: Tue Dec 27 21:56:19 2022, max compression
+gzip compressed data, was "Kodistubs-20.0.1.tar", last modified: Thu Jul  6 20:34:12 2023, max compression
```

## Comparing `Kodistubs-20.0.0rc3.tar` & `Kodistubs-20.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 21:56:19.801594 Kodistubs-20.0.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 21:56:19.801594 Kodistubs-20.0.0rc3/Kodistubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2022-12-27 21:56:19.000000 Kodistubs-20.0.0rc3/Kodistubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-27 21:56:19.000000 Kodistubs-20.0.0rc3/Kodistubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 21:56:19.000000 Kodistubs-20.0.0rc3/Kodistubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 21:56:19.000000 Kodistubs-20.0.0rc3/Kodistubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-27 21:56:19.000000 Kodistubs-20.0.0rc3/Kodistubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32472 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2022-12-27 21:56:19.801594 Kodistubs-20.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/kodistubs_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-27 21:56:19.801594 Kodistubs-20.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    99210 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmcaddon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmcdrm.py
--rw-r--r--   0 runner    (1001) docker     (123)   164977 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmcgui.py
--rw-r--r--   0 runner    (1001) docker     (123)    17257 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmcplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2022-12-27 21:56:16.000000 Kodistubs-20.0.0rc3/xbmcvfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:12.429669 Kodistubs-20.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:12.429669 Kodistubs-20.0.1/Kodistubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-06 20:34:12.000000 Kodistubs-20.0.1/Kodistubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 20:34:12.000000 Kodistubs-20.0.1/Kodistubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:34:12.000000 Kodistubs-20.0.1/Kodistubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:34:12.000000 Kodistubs-20.0.1/Kodistubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-06 20:34:12.000000 Kodistubs-20.0.1/Kodistubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32472 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-06 20:34:12.429669 Kodistubs-20.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-06 20:34:12.429669 Kodistubs-20.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99210 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmcaddon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmcdrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164977 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmcgui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17257 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmcplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-06 20:34:07.000000 Kodistubs-20.0.1/xbmcvfs.py
```

### Comparing `Kodistubs-20.0.0rc3/Kodistubs.egg-info/PKG-INFO` & `Kodistubs-20.0.1/Kodistubs.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Kodistubs
-Version: 20.0.0rc3
+Version: 20.0.1
 Summary: Stub modules that re-create Kodi Python API
 Home-page: https://github.com/romanvm/Kodistubs
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
-License: GPLv3
+License: GPL-3.0-only
 Keywords: kodi documentation inspection
-Platform: UNKNOWN
+Platform: any
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Kodistubs
 =========
 (former xbmcstubs)
 ------------------
```

### Comparing `Kodistubs-20.0.0rc3/LICENSE.txt` & `Kodistubs-20.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/PKG-INFO` & `Kodistubs-20.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: Kodistubs
-Version: 20.0.0rc3
+Version: 20.0.1
 Summary: Stub modules that re-create Kodi Python API
 Home-page: https://github.com/romanvm/Kodistubs
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
-License: GPLv3
+License: GPL-3.0-only
 Keywords: kodi documentation inspection
-Platform: UNKNOWN
+Platform: any
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 Kodistubs
 =========
 (former xbmcstubs)
 ------------------
```

### Comparing `Kodistubs-20.0.0rc3/README.rst` & `Kodistubs-20.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmc.py` & `Kodistubs-20.0.1/xbmc.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmcaddon.py` & `Kodistubs-20.0.1/xbmcaddon.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmcdrm.py` & `Kodistubs-20.0.1/xbmcdrm.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmcgui.py` & `Kodistubs-20.0.1/xbmcgui.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmcplugin.py` & `Kodistubs-20.0.1/xbmcplugin.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-20.0.0rc3/xbmcvfs.py` & `Kodistubs-20.0.1/xbmcvfs.py`

 * *Files identical despite different names*

