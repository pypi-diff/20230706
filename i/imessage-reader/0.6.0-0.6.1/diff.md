# Comparing `tmp/imessage_reader-0.6.0.tar.gz` & `tmp/imessage_reader-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imessage_reader-0.6.0.tar", last modified: Thu Jun 29 11:39:07 2023, max compression
+gzip compressed data, was "imessage_reader-0.6.1.tar", last modified: Thu Jul  6 07:00:05 2023, max compression
```

## Comparing `imessage_reader-0.6.0.tar` & `imessage_reader-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.535405 imessage_reader-0.6.0/
--rw-r--r--   0 bodo       (501) staff       (20)     1077 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/LICENSE
--rw-r--r--   0 bodo       (501) staff       (20)     4507 2023-06-29 11:39:07.535273 imessage_reader-0.6.0/PKG-INFO
--rw-r--r--   0 bodo       (501) staff       (20)     3866 2023-06-29 11:35:11.000000 imessage_reader-0.6.0/README.md
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.533387 imessage_reader-0.6.0/imessage_reader/
--rw-r--r--   0 bodo       (501) staff       (20)       88 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/imessage_reader/__init__.py
--rw-r--r--   0 bodo       (501) staff       (20)     2823 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/cli.py
--rw-r--r--   0 bodo       (501) staff       (20)     1294 2023-06-29 11:35:11.000000 imessage_reader-0.6.0/imessage_reader/common.py
--rw-r--r--   0 bodo       (501) staff       (20)     1947 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/create_sqlite.py
--rw-r--r--   0 bodo       (501) staff       (20)      997 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/data_container.py
--rw-r--r--   0 bodo       (501) staff       (20)     6071 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/fetch_data.py
--rw-r--r--   0 bodo       (501) staff       (20)      627 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/info.py
--rw-r--r--   0 bodo       (501) staff       (20)     3610 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/imessage_reader/write_excel.py
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.534005 imessage_reader-0.6.0/imessage_reader.egg-info/
--rw-r--r--   0 bodo       (501) staff       (20)     4507 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/PKG-INFO
--rw-r--r--   0 bodo       (501) staff       (20)      659 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/SOURCES.txt
--rw-r--r--   0 bodo       (501) staff       (20)        1 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/dependency_links.txt
--rw-r--r--   0 bodo       (501) staff       (20)       61 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/entry_points.txt
--rw-r--r--   0 bodo       (501) staff       (20)        9 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/requires.txt
--rw-r--r--   0 bodo       (501) staff       (20)       16 2023-06-29 11:39:07.000000 imessage_reader-0.6.0/imessage_reader.egg-info/top_level.txt
--rw-r--r--   0 bodo       (501) staff       (20)       38 2023-06-29 11:39:07.535437 imessage_reader-0.6.0/setup.cfg
--rw-r--r--   0 bodo       (501) staff       (20)     1114 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/setup.py
-drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-06-29 11:39:07.535059 imessage_reader-0.6.0/tests/
--rw-r--r--   0 bodo       (501) staff       (20)      669 2023-06-27 11:11:59.000000 imessage_reader-0.6.0/tests/test_cli.py
--rw-r--r--   0 bodo       (501) staff       (20)     1146 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_create_sqlite.py
--rw-r--r--   0 bodo       (501) staff       (20)      882 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_fetch_db.py
--rw-r--r--   0 bodo       (501) staff       (20)      515 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_get_platform.py
--rw-r--r--   0 bodo       (501) staff       (20)      269 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_info.py
--rw-r--r--   0 bodo       (501) staff       (20)     2440 2023-04-11 15:45:17.000000 imessage_reader-0.6.0/tests/test_message_data.py
--rw-r--r--   0 bodo       (501) staff       (20)     1187 2023-03-09 07:25:18.000000 imessage_reader-0.6.0/tests/test_write_excel.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-07-06 07:00:05.128593 imessage_reader-0.6.1/
+-rw-r--r--   0 bodo       (501) staff       (20)     1077 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/LICENSE
+-rw-r--r--   0 bodo       (501) staff       (20)     4554 2023-07-06 07:00:05.128485 imessage_reader-0.6.1/PKG-INFO
+-rw-r--r--   0 bodo       (501) staff       (20)     3866 2023-06-29 11:35:11.000000 imessage_reader-0.6.1/README.md
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-07-06 07:00:05.126432 imessage_reader-0.6.1/imessage_reader/
+-rw-r--r--   0 bodo       (501) staff       (20)       88 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/imessage_reader/__init__.py
+-rw-r--r--   0 bodo       (501) staff       (20)     2823 2023-06-27 11:11:59.000000 imessage_reader-0.6.1/imessage_reader/cli.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1294 2023-07-06 06:58:41.000000 imessage_reader-0.6.1/imessage_reader/common.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1947 2023-06-27 11:11:59.000000 imessage_reader-0.6.1/imessage_reader/create_sqlite.py
+-rw-r--r--   0 bodo       (501) staff       (20)      997 2023-06-27 11:11:59.000000 imessage_reader-0.6.1/imessage_reader/data_container.py
+-rw-r--r--   0 bodo       (501) staff       (20)     6022 2023-07-06 06:58:41.000000 imessage_reader-0.6.1/imessage_reader/fetch_data.py
+-rw-r--r--   0 bodo       (501) staff       (20)      627 2023-06-27 11:11:59.000000 imessage_reader-0.6.1/imessage_reader/info.py
+-rw-r--r--   0 bodo       (501) staff       (20)     3610 2023-06-27 11:11:59.000000 imessage_reader-0.6.1/imessage_reader/write_excel.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-07-06 07:00:05.127183 imessage_reader-0.6.1/imessage_reader.egg-info/
+-rw-r--r--   0 bodo       (501) staff       (20)     4554 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/PKG-INFO
+-rw-r--r--   0 bodo       (501) staff       (20)      684 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 bodo       (501) staff       (20)        1 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       61 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/entry_points.txt
+-rw-r--r--   0 bodo       (501) staff       (20)        9 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/requires.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       16 2023-07-06 07:00:05.000000 imessage_reader-0.6.1/imessage_reader.egg-info/top_level.txt
+-rw-r--r--   0 bodo       (501) staff       (20)       38 2023-07-06 07:00:05.128626 imessage_reader-0.6.1/setup.cfg
+-rw-r--r--   0 bodo       (501) staff       (20)     1160 2023-07-06 06:58:41.000000 imessage_reader-0.6.1/setup.py
+drwxr-xr-x   0 bodo       (501) staff       (20)        0 2023-07-06 07:00:05.128306 imessage_reader-0.6.1/tests/
+-rw-r--r--   0 bodo       (501) staff       (20)     1093 2023-07-06 06:58:41.000000 imessage_reader-0.6.1/tests/test_cli.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1146 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/tests/test_create_sqlite.py
+-rw-r--r--   0 bodo       (501) staff       (20)      435 2023-07-06 06:58:41.000000 imessage_reader-0.6.1/tests/test_fetch_data.py
+-rw-r--r--   0 bodo       (501) staff       (20)      882 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/tests/test_fetch_db.py
+-rw-r--r--   0 bodo       (501) staff       (20)      515 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/tests/test_get_platform.py
+-rw-r--r--   0 bodo       (501) staff       (20)      269 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/tests/test_info.py
+-rw-r--r--   0 bodo       (501) staff       (20)     2440 2023-04-11 15:45:17.000000 imessage_reader-0.6.1/tests/test_message_data.py
+-rw-r--r--   0 bodo       (501) staff       (20)     1187 2023-03-09 07:25:18.000000 imessage_reader-0.6.1/tests/test_write_excel.py
```

### Comparing `imessage_reader-0.6.0/LICENSE` & `imessage_reader-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/PKG-INFO` & `imessage_reader-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: imessage_reader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Fetch recipients and chat messages from the chat.db database.
 Home-page: https://github.com/niftycode/imessage_reader
 Author: Bodo Schönfeld
 Author-email: bodo.schoenfeld@niftycode.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imessage_reader-0.6.0/README.md` & `imessage_reader-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader/cli.py` & `imessage_reader-0.6.1/imessage_reader/cli.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader/common.py` & `imessage_reader-0.6.1/imessage_reader/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 common.py
 Python 3.9+
 Date created: June 14th, 2020
-Date modified: June 3rd, 2023
+Date modified: July 3rd, 2023
 """
 
 import platform
 import sqlite3
 import sys
 from enum import Enum
 
-VERSION = "0.6.0"
+VERSION = "0.6.1"
 
 
 class Platform(Enum):
     """An enum used to indicate the running operating system
     """
 
     OTHER = 0
```

### Comparing `imessage_reader-0.6.0/imessage_reader/create_sqlite.py` & `imessage_reader-0.6.1/imessage_reader/create_sqlite.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader/data_container.py` & `imessage_reader-0.6.1/imessage_reader/data_container.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader/fetch_data.py` & `imessage_reader-0.6.1/imessage_reader/fetch_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         :param system: Operating System
         """
         self.db_path = db_path
         if system is None:
             self.operating_system = common.get_platform()
 
     def _check_system(self):
-        # TODO: Change this later (So, it can be used on Windows too.)
+        # TODO: Change this later
         if self.operating_system == "WINDOWS":
             sys.exit("Your operating system is not supported yet!")
 
     def _read_database(self) -> list:
         """Fetch data from the database and store the data in a list.
 
         :return: list containing the user id, messages, the service and the account
@@ -165,15 +165,14 @@
         print("List of Recipients")
         print("------------------------")
         print()
 
         for recipient in recipients:
             print(recipient)
 
-    '''
     def get_messages(self) -> list:
         """Create a list with tuples (user id, message, date, service, account, is_from_me)
         (This method is for module usage.)
 
         :return: list with tuples (user id, message, date, service, account, is_from_me)
         """
         fetched_data = self._read_database()
@@ -192,8 +191,7 @@
             service.append(data.service)
             account.append(data.account)
             is_from_me.append(data.is_from_me)
 
         data = list(zip(users, messages, dates, service, account, is_from_me))
 
         return data
-'''
```

### Comparing `imessage_reader-0.6.0/imessage_reader/info.py` & `imessage_reader-0.6.1/imessage_reader/info.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader/write_excel.py` & `imessage_reader-0.6.1/imessage_reader/write_excel.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/imessage_reader.egg-info/PKG-INFO` & `imessage_reader-0.6.1/imessage_reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: imessage-reader
-Version: 0.6.0
+Version: 0.6.1
 Summary: Fetch recipients and chat messages from the chat.db database.
 Home-page: https://github.com/niftycode/imessage_reader
 Author: Bodo Schönfeld
 Author-email: bodo.schoenfeld@niftycode.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `imessage_reader-0.6.0/imessage_reader.egg-info/SOURCES.txt` & `imessage_reader-0.6.1/imessage_reader.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 imessage_reader.egg-info/SOURCES.txt
 imessage_reader.egg-info/dependency_links.txt
 imessage_reader.egg-info/entry_points.txt
 imessage_reader.egg-info/requires.txt
 imessage_reader.egg-info/top_level.txt
 tests/test_cli.py
 tests/test_create_sqlite.py
+tests/test_fetch_data.py
 tests/test_fetch_db.py
 tests/test_get_platform.py
 tests/test_info.py
 tests/test_message_data.py
 tests/test_write_excel.py
```

### Comparing `imessage_reader-0.6.0/setup.py` & `imessage_reader-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     author='Bodo Schönfeld',
     author_email='bodo.schoenfeld@niftycode.de',
     url='https://github.com/niftycode/imessage_reader',
 
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: MacOS',
+        'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
 
     packages=find_packages(exclude=('tests', 'docs')),
```

### Comparing `imessage_reader-0.6.0/tests/test_create_sqlite.py` & `imessage_reader-0.6.1/tests/test_create_sqlite.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/tests/test_fetch_db.py` & `imessage_reader-0.6.1/tests/test_fetch_db.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/tests/test_get_platform.py` & `imessage_reader-0.6.1/tests/test_get_platform.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/tests/test_message_data.py` & `imessage_reader-0.6.1/tests/test_message_data.py`

 * *Files identical despite different names*

### Comparing `imessage_reader-0.6.0/tests/test_write_excel.py` & `imessage_reader-0.6.1/tests/test_write_excel.py`

 * *Files identical despite different names*

