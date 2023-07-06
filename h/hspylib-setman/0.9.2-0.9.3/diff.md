# Comparing `tmp/hspylib-setman-0.9.2.tar.gz` & `tmp/hspylib-setman-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.2.tar", last modified: Thu Jul  6 16:29:01 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.3.tar", last modified: Thu Jul  6 16:29:37 2023, max compression
```

## Comparing `hspylib-setman-0.9.2.tar` & `hspylib-setman-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:01.374103 hspylib-setman-0.9.2/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2023-07-05 21:53:39.000000 hspylib-setman-0.9.2/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:01.372044 hspylib-setman-0.9.2/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 16:29:00.000000 hspylib-setman-0.9.2/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:01.341570 hspylib-setman-0.9.2/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:01.000000 hspylib-setman-0.9.2/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      584 2023-07-06 16:29:01.000000 hspylib-setman-0.9.2/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 16:29:01.000000 hspylib-setman-0.9.2/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 16:29:01.000000 hspylib-setman-0.9.2/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 16:29:01.000000 hspylib-setman-0.9.2/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:01.346309 hspylib-setman-0.9.2/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.2/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 16:29:00.000000 hspylib-setman-0.9.2/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4752 2023-07-05 23:38:47.000000 hspylib-setman-0.9.2/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:01.354488 hspylib-setman-0.9.2/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 16:29:00.000000 hspylib-setman-0.9.2/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6164 2023-07-05 23:02:34.000000 hspylib-setman-0.9.2/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.2/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.2/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:01.370466 hspylib-setman-0.9.2/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 16:29:00.000000 hspylib-setman-0.9.2/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9241 2023-07-05 23:11:54.000000 hspylib-setman-0.9.2/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.2/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.2/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3887 2023-07-05 22:08:56.000000 hspylib-setman-0.9.2/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2054 2023-07-05 22:30:45.000000 hspylib-setman-0.9.2/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 16:29:01.374373 hspylib-setman-0.9.2/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.2/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.436548 hspylib-setman-0.9.3/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.3/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:37.435739 hspylib-setman-0.9.3/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.404110 hspylib-setman-0.9.3/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 16:29:37.000000 hspylib-setman-0.9.3/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.413527 hspylib-setman-0.9.3/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.3/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4752 2023-07-05 23:38:47.000000 hspylib-setman-0.9.3/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.421895 hspylib-setman-0.9.3/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6164 2023-07-05 23:02:34.000000 hspylib-setman-0.9.3/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.3/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.3/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 16:29:37.434053 hspylib-setman-0.9.3/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 16:29:36.000000 hspylib-setman-0.9.3/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9241 2023-07-05 23:11:54.000000 hspylib-setman-0.9.3/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.3/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.3/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3887 2023-07-05 22:08:56.000000 hspylib-setman-0.9.3/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2054 2023-07-05 22:30:45.000000 hspylib-setman-0.9.3/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-05 22:41:51.000000 hspylib-setman-0.9.3/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 16:29:37.436706 hspylib-setman-0.9.3/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.3/setup.py
```

### Comparing `hspylib-setman-0.9.2/PKG-INFO` & `hspylib-setman-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.2
+Version: 0.9.3
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.2/README.md` & `hspylib-setman-0.9.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.2/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.3/hspylib_setman.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.2
+Version: 0.9.3
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.2/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.3/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.2/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.3/hspylib_setman.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 README.md
 setup.py
 hspylib_setman.egg-info/PKG-INFO
 hspylib_setman.egg-info/SOURCES.txt
 hspylib_setman.egg-info/dependency_links.txt
 hspylib_setman.egg-info/requires.txt
 hspylib_setman.egg-info/top_level.txt
+setman/.version
 setman/__classpath__.py
 setman/__init__.py
 setman/__main__.py
+setman/welcome.txt
 setman/core/__init__.py
 setman/core/setman.py
 setman/core/setman_config.py
 setman/core/setman_enums.py
 setman/settings/__init__.py
 setman/settings/settings.py
 setman/settings/settings_config.py
```

### Comparing `hspylib-setman-0.9.2/setman/__classpath__.py` & `hspylib-setman-0.9.3/setman/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/__main__.py` & `hspylib-setman-0.9.3/setman/__main__.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/core/setman.py` & `hspylib-setman-0.9.3/setman/core/setman.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/core/setman_config.py` & `hspylib-setman-0.9.3/setman/core/setman_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/core/setman_enums.py` & `hspylib-setman-0.9.3/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/settings/settings.py` & `hspylib-setman-0.9.3/setman/settings/settings.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/settings/settings_config.py` & `hspylib-setman-0.9.3/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/settings/settings_entry.py` & `hspylib-setman-0.9.3/setman/settings/settings_entry.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/settings/settings_repository.py` & `hspylib-setman-0.9.3/setman/settings/settings_repository.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setman/settings/settings_service.py` & `hspylib-setman-0.9.3/setman/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.2/setup.py` & `hspylib-setman-0.9.3/setup.py`

 * *Files identical despite different names*

