# Comparing `tmp/x11-automation-0.3.1.tar.gz` & `tmp/x11-automation-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x11-automation-0.3.1.tar", last modified: Wed Jul  5 21:09:41 2023, max compression
+gzip compressed data, was "x11-automation-0.3.2.tar", last modified: Thu Jul  6 14:40:53 2023, max compression
```

## Comparing `x11-automation-0.3.1.tar` & `x11-automation-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-05 21:09:41.235429 x11-automation-0.3.1/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1071 2023-06-26 23:44:38.000000 x11-automation-0.3.1/LICENSE.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-05 21:09:41.235429 x11-automation-0.3.1/PKG-INFO
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      266 2023-06-26 23:44:01.000000 x11-automation-0.3.1/README.md
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      409 2023-07-05 21:09:41.235429 x11-automation-0.3.1/setup.cfg
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       37 2023-06-26 23:41:00.000000 x11-automation-0.3.1/setup.py
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-05 21:09:40.959425 x11-automation-0.3.1/x11_automation/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      361 2023-07-01 02:22:06.000000 x11-automation-0.3.1/x11_automation/__init__.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        0 2023-06-26 23:46:08.000000 x11-automation-0.3.1/x11_automation/__main__.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      619 2023-07-01 02:21:34.000000 x11-automation-0.3.1/x11_automation/get_win_geometry.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1214 2023-07-01 01:18:51.000000 x11-automation-0.3.1/x11_automation/move_mouse_to_new_window.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      485 2023-07-01 03:20:51.000000 x11-automation-0.3.1/x11_automation/send.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      122 2023-06-27 02:52:06.000000 x11-automation-0.3.1/x11_automation/win_activate.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      807 2023-07-01 02:05:02.000000 x11-automation-0.3.1/x11_automation/win_exists.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      209 2023-06-27 01:15:56.000000 x11-automation-0.3.1/x11_automation/win_get_process.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      499 2023-06-27 01:15:56.000000 x11-automation-0.3.1/x11_automation/win_wait_active.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       46 2023-06-27 01:13:09.000000 x11-automation-0.3.1/x11_automation/x11_automation.py
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-05 21:09:41.235429 x11-automation-0.3.1/x11_automation.egg-info/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-05 21:09:39.000000 x11-automation-0.3.1/x11_automation.egg-info/PKG-INFO
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      545 2023-07-05 21:09:39.000000 x11-automation-0.3.1/x11_automation.egg-info/SOURCES.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        1 2023-07-05 21:09:39.000000 x11-automation-0.3.1/x11_automation.egg-info/dependency_links.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       31 2023-07-05 21:09:39.000000 x11-automation-0.3.1/x11_automation.egg-info/requires.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       15 2023-07-05 21:09:39.000000 x11-automation-0.3.1/x11_automation.egg-info/top_level.txt
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-06 14:40:53.821274 x11-automation-0.3.2/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1071 2023-06-26 23:44:38.000000 x11-automation-0.3.2/LICENSE.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-06 14:40:53.821274 x11-automation-0.3.2/PKG-INFO
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      266 2023-06-26 23:44:01.000000 x11-automation-0.3.2/README.md
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      409 2023-07-06 14:40:53.821274 x11-automation-0.3.2/setup.cfg
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       37 2023-06-26 23:41:00.000000 x11-automation-0.3.2/setup.py
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-06 14:40:53.821274 x11-automation-0.3.2/x11_automation/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      361 2023-07-01 02:22:06.000000 x11-automation-0.3.2/x11_automation/__init__.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        0 2023-06-26 23:46:08.000000 x11-automation-0.3.2/x11_automation/__main__.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      619 2023-07-01 02:21:34.000000 x11-automation-0.3.2/x11_automation/get_win_geometry.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1214 2023-07-01 01:18:51.000000 x11-automation-0.3.2/x11_automation/move_mouse_to_new_window.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      536 2023-07-06 14:38:38.000000 x11-automation-0.3.2/x11_automation/send.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      122 2023-06-27 02:52:06.000000 x11-automation-0.3.2/x11_automation/win_activate.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      807 2023-07-06 01:10:36.000000 x11-automation-0.3.2/x11_automation/win_exists.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      209 2023-06-27 01:15:56.000000 x11-automation-0.3.2/x11_automation/win_get_process.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      499 2023-06-27 01:15:56.000000 x11-automation-0.3.2/x11_automation/win_wait_active.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       46 2023-06-27 01:13:09.000000 x11-automation-0.3.2/x11_automation/x11_automation.py
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-06 14:40:53.821274 x11-automation-0.3.2/x11_automation.egg-info/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        2 2023-07-06 14:40:01.000000 x11-automation-0.3.2/x11_automation.egg-info/.gitignore
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-06 14:40:53.000000 x11-automation-0.3.2/x11_automation.egg-info/PKG-INFO
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      580 2023-07-06 14:40:53.000000 x11-automation-0.3.2/x11_automation.egg-info/SOURCES.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        1 2023-07-06 14:40:53.000000 x11-automation-0.3.2/x11_automation.egg-info/dependency_links.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       31 2023-07-06 14:40:53.000000 x11-automation-0.3.2/x11_automation.egg-info/requires.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       15 2023-07-06 14:40:53.000000 x11-automation-0.3.2/x11_automation.egg-info/top_level.txt
```

### Comparing `x11-automation-0.3.1/LICENSE.txt` & `x11-automation-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.1/PKG-INFO` & `x11-automation-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x11-automation
-Version: 0.3.1
+Version: 0.3.2
 Summary: X11-Automation
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: opensuse12@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `x11-automation-0.3.1/x11_automation/get_win_geometry.py` & `x11-automation-0.3.2/x11_automation/get_win_geometry.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.1/x11_automation/move_mouse_to_new_window.py` & `x11-automation-0.3.2/x11_automation/move_mouse_to_new_window.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.1/x11_automation/win_exists.py` & `x11-automation-0.3.2/x11_automation/win_exists.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.1/x11_automation.egg-info/PKG-INFO` & `x11-automation-0.3.2/x11_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x11-automation
-Version: 0.3.1
+Version: 0.3.2
 Summary: X11-Automation
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: opensuse12@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `x11-automation-0.3.1/x11_automation.egg-info/SOURCES.txt` & `x11-automation-0.3.2/x11_automation.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 x11_automation/move_mouse_to_new_window.py
 x11_automation/send.py
 x11_automation/win_activate.py
 x11_automation/win_exists.py
 x11_automation/win_get_process.py
 x11_automation/win_wait_active.py
 x11_automation/x11_automation.py
+x11_automation.egg-info/.gitignore
 x11_automation.egg-info/PKG-INFO
 x11_automation.egg-info/SOURCES.txt
 x11_automation.egg-info/dependency_links.txt
 x11_automation.egg-info/requires.txt
 x11_automation.egg-info/top_level.txt
```

