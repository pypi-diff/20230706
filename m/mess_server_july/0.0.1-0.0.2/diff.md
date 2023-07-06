# Comparing `tmp/mess_server_july-0.0.1.tar.gz` & `tmp/mess_server_july-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mess_server_july-0.0.1.tar", last modified: Thu Jul  6 15:25:48 2023, max compression
+gzip compressed data, was "dist\mess_server_july-0.0.2.tar", last modified: Thu Jul  6 15:28:06 2023, max compression
```

## Comparing `mess_server_july-0.0.1.tar` & `mess_server_july-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/
--rw-rw-rw-   0        0        0      221 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/
--rw-rw-rw-   0        0        0      221 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/mess_server_july.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/
--rw-rw-rw-   0        0        0        0 2019-05-21 09:36:10.000000 mess_server_july-0.0.1/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/common/
--rw-rw-rw-   0        0        0        0 2019-05-27 09:04:48.000000 mess_server_july-0.0.1/server/common/__init__.py
--rw-rw-rw-   0        0        0     3270 2019-07-07 00:44:32.000000 mess_server_july-0.0.1/server/common/decos.py
--rw-rw-rw-   0        0        0     1213 2019-07-07 00:44:32.000000 mess_server_july-0.0.1/server/common/descryptors.py
--rw-rw-rw-   0        0        0      395 2019-07-07 00:44:32.000000 mess_server_july-0.0.1/server/common/errors.py
--rw-rw-rw-   0        0        0     4249 2019-07-07 00:44:32.000000 mess_server_july-0.0.1/server/common/metaclasses.py
--rw-rw-rw-   0        0        0     1341 2019-07-07 00:44:32.000000 mess_server_july-0.0.1/server/common/utils.py
--rw-rw-rw-   0        0        0     1614 2019-07-03 18:53:48.000000 mess_server_july-0.0.1/server/common/variables.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/doc/
--rw-rw-rw-   0        0        0        0 2023-07-06 15:07:53.000000 mess_server_july-0.0.1/server/doc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/doc/source/
--rw-rw-rw-   0        0        0        0 2023-07-06 15:07:53.000000 mess_server_july-0.0.1/server/doc/source/__init__.py
--rw-rw-rw-   0        0        0     2328 2019-07-08 11:31:54.000000 mess_server_july-0.0.1/server/doc/source/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/logs/
--rw-rw-rw-   0        0        0        0 2019-05-28 17:49:04.000000 mess_server_july-0.0.1/server/logs/__init__.py
--rw-rw-rw-   0        0        0     1105 2019-06-30 18:43:50.000000 mess_server_july-0.0.1/server/logs/config_client_log.py
--rw-rw-rw-   0        0        0     1174 2019-06-14 19:33:48.000000 mess_server_july-0.0.1/server/logs/config_server_log.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/server/
--rw-rw-rw-   0        0        0        0 2019-07-01 19:09:36.000000 mess_server_july-0.0.1/server/server/__init__.py
--rw-rw-rw-   0        0        0     3962 2019-07-07 16:46:04.000000 mess_server_july-0.0.1/server/server/add_user.py
--rw-rw-rw-   0        0        0     5355 2020-09-11 16:35:07.000000 mess_server_july-0.0.1/server/server/config_window.py
--rw-rw-rw-   0        0        0    15290 2019-07-07 17:07:00.000000 mess_server_july-0.0.1/server/server/core.py
--rw-rw-rw-   0        0        0    16685 2020-09-11 16:38:27.000000 mess_server_july-0.0.1/server/server/database.py
--rw-rw-rw-   0        0        0     6091 2019-07-07 17:31:54.000000 mess_server_july-0.0.1/server/server/main_window.py
--rw-rw-rw-   0        0        0     2276 2019-07-07 17:38:16.000000 mess_server_july-0.0.1/server/server/remove_user.py
--rw-rw-rw-   0        0        0     2282 2019-07-07 17:40:16.000000 mess_server_july-0.0.1/server/server/stat_window.py
--rw-rw-rw-   0        0        0     4107 2020-09-11 16:34:15.000000 mess_server_july-0.0.1/server/server.py
-drwxrwxrwx   0        0        0        0 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/server/unit_tests/
--rw-rw-rw-   0        0        0        0 2019-05-27 09:04:48.000000 mess_server_july-0.0.1/server/unit_tests/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-06 15:25:48.000000 mess_server_july-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-07-06 15:16:27.000000 mess_server_july-0.0.1/setup_server.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/
+-rw-rw-rw-   0        0        0      221 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/
+-rw-rw-rw-   0        0        0      221 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/mess_server_july.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/
+-rw-rw-rw-   0        0        0        0 2019-05-21 09:36:10.000000 mess_server_july-0.0.2/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/common/
+-rw-rw-rw-   0        0        0        0 2019-05-27 09:04:48.000000 mess_server_july-0.0.2/server/common/__init__.py
+-rw-rw-rw-   0        0        0     3270 2019-07-07 00:44:32.000000 mess_server_july-0.0.2/server/common/decos.py
+-rw-rw-rw-   0        0        0     1213 2019-07-07 00:44:32.000000 mess_server_july-0.0.2/server/common/descryptors.py
+-rw-rw-rw-   0        0        0      395 2019-07-07 00:44:32.000000 mess_server_july-0.0.2/server/common/errors.py
+-rw-rw-rw-   0        0        0     4249 2019-07-07 00:44:32.000000 mess_server_july-0.0.2/server/common/metaclasses.py
+-rw-rw-rw-   0        0        0     1341 2019-07-07 00:44:32.000000 mess_server_july-0.0.2/server/common/utils.py
+-rw-rw-rw-   0        0        0     1614 2019-07-03 18:53:48.000000 mess_server_july-0.0.2/server/common/variables.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/doc/
+-rw-rw-rw-   0        0        0        0 2023-07-06 15:07:53.000000 mess_server_july-0.0.2/server/doc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/doc/source/
+-rw-rw-rw-   0        0        0        0 2023-07-06 15:07:53.000000 mess_server_july-0.0.2/server/doc/source/__init__.py
+-rw-rw-rw-   0        0        0     2328 2019-07-08 11:31:54.000000 mess_server_july-0.0.2/server/doc/source/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/logs/
+-rw-rw-rw-   0        0        0        0 2019-05-28 17:49:04.000000 mess_server_july-0.0.2/server/logs/__init__.py
+-rw-rw-rw-   0        0        0     1105 2019-06-30 18:43:50.000000 mess_server_july-0.0.2/server/logs/config_client_log.py
+-rw-rw-rw-   0        0        0     1174 2019-06-14 19:33:48.000000 mess_server_july-0.0.2/server/logs/config_server_log.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/server/
+-rw-rw-rw-   0        0        0        0 2019-07-01 19:09:36.000000 mess_server_july-0.0.2/server/server/__init__.py
+-rw-rw-rw-   0        0        0     3962 2019-07-07 16:46:04.000000 mess_server_july-0.0.2/server/server/add_user.py
+-rw-rw-rw-   0        0        0     5355 2020-09-11 16:35:07.000000 mess_server_july-0.0.2/server/server/config_window.py
+-rw-rw-rw-   0        0        0    15290 2019-07-07 17:07:00.000000 mess_server_july-0.0.2/server/server/core.py
+-rw-rw-rw-   0        0        0    16685 2020-09-11 16:38:27.000000 mess_server_july-0.0.2/server/server/database.py
+-rw-rw-rw-   0        0        0     6091 2019-07-07 17:31:54.000000 mess_server_july-0.0.2/server/server/main_window.py
+-rw-rw-rw-   0        0        0     2276 2019-07-07 17:38:16.000000 mess_server_july-0.0.2/server/server/remove_user.py
+-rw-rw-rw-   0        0        0     2282 2019-07-07 17:40:16.000000 mess_server_july-0.0.2/server/server/stat_window.py
+-rw-rw-rw-   0        0        0     4107 2020-09-11 16:34:15.000000 mess_server_july-0.0.2/server/server.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/server/unit_tests/
+-rw-rw-rw-   0        0        0        0 2019-05-27 09:04:48.000000 mess_server_july-0.0.2/server/unit_tests/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:28:06.000000 mess_server_july-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-07-06 15:27:30.000000 mess_server_july-0.0.2/setup_server.py
```

### Comparing `mess_server_july-0.0.1/mess_server_july.egg-info/SOURCES.txt` & `mess_server_july-0.0.2/mess_server_july.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/common/decos.py` & `mess_server_july-0.0.2/server/common/decos.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/common/descryptors.py` & `mess_server_july-0.0.2/server/common/descryptors.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/common/metaclasses.py` & `mess_server_july-0.0.2/server/common/metaclasses.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/common/utils.py` & `mess_server_july-0.0.2/server/common/utils.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/common/variables.py` & `mess_server_july-0.0.2/server/common/variables.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/doc/source/conf.py` & `mess_server_july-0.0.2/server/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/logs/config_client_log.py` & `mess_server_july-0.0.2/server/logs/config_client_log.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/logs/config_server_log.py` & `mess_server_july-0.0.2/server/logs/config_server_log.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/add_user.py` & `mess_server_july-0.0.2/server/server/add_user.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/config_window.py` & `mess_server_july-0.0.2/server/server/config_window.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/core.py` & `mess_server_july-0.0.2/server/server/core.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/database.py` & `mess_server_july-0.0.2/server/server/database.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/main_window.py` & `mess_server_july-0.0.2/server/server/main_window.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/remove_user.py` & `mess_server_july-0.0.2/server/server/remove_user.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server/stat_window.py` & `mess_server_july-0.0.2/server/server/stat_window.py`

 * *Files identical despite different names*

### Comparing `mess_server_july-0.0.1/server/server.py` & `mess_server_july-0.0.2/server/server.py`

 * *Files identical despite different names*

