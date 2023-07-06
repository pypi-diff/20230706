# Comparing `tmp/egorovsystem-0.0.2.tar.gz` & `tmp/egorovsystem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\egorovsystem-0.0.2.tar", last modified: Wed Jul  5 20:23:07 2023, max compression
+gzip compressed data, was "dist\egorovsystem-0.0.4.tar", last modified: Thu Jul  6 02:04:34 2023, max compression
```

## Comparing `egorovsystem-0.0.2.tar` & `egorovsystem-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.315374 egorovsystem-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1530 2023-07-05 20:23:07.315374 egorovsystem-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.295370 egorovsystem-0.0.2/egolocal/
--rw-rw-rw-   0        0        0     1473 2023-07-05 20:07:45.000000 egorovsystem-0.0.2/egolocal/main.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.297371 egorovsystem-0.0.2/egorovsystem/
--rw-rw-rw-   0        0        0      475 2023-07-05 19:40:59.000000 egorovsystem-0.0.2/egorovsystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.306372 egorovsystem-0.0.2/egorovsystem.egg-info/
--rw-rw-rw-   0        0        0     1530 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.309373 egorovsystem-0.0.2/egoserver/
--rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.2/egoserver/manage.py
--rw-rw-rw-   0        0        0      533 2023-07-05 19:56:14.000000 egorovsystem-0.0.2/egoserver/run.py
--rw-rw-rw-   0        0        0       42 2023-07-05 20:23:07.316375 egorovsystem-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      847 2023-07-05 20:23:00.000000 egorovsystem-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.313373 egorovsystem-0.0.2/test/
--rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.2/test/__init__.py
--rw-rw-rw-   0        0        0       63 2023-07-05 19:43:40.000000 egorovsystem-0.0.2/test/a.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.468390 egorovsystem-0.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1562 2023-07-06 02:04:34.467389 egorovsystem-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.417379 egorovsystem-0.0.4/egolocal/
+-rw-rw-rw-   0        0        0     1473 2023-07-05 20:07:45.000000 egorovsystem-0.0.4/egolocal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.419379 egorovsystem-0.0.4/egorovsystem/
+-rw-rw-rw-   0        0        0      475 2023-07-05 19:40:59.000000 egorovsystem-0.0.4/egorovsystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.428381 egorovsystem-0.0.4/egorovsystem.egg-info/
+-rw-rw-rw-   0        0        0     1562 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-06 02:04:34.000000 egorovsystem-0.0.4/egorovsystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.432382 egorovsystem-0.0.4/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-06 02:03:41.000000 egorovsystem-0.0.4/egoserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.444383 egorovsystem-0.0.4/egoserver/egoserver/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:33:47.000000 egorovsystem-0.0.4/egoserver/egoserver/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.4/egoserver/egoserver/asgi.py
+-rw-rw-rw-   0        0        0       83 2023-07-05 17:41:34.000000 egorovsystem-0.0.4/egoserver/egoserver/secret.py
+-rw-rw-rw-   0        0        0     3369 2023-07-05 19:09:44.000000 egorovsystem-0.0.4/egoserver/egoserver/settings.py
+-rw-rw-rw-   0        0        0      847 2023-07-05 17:55:04.000000 egorovsystem-0.0.4/egoserver/egoserver/urls.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 17:33:47.000000 egorovsystem-0.0.4/egoserver/egoserver/wsgi.py
+-rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.4/egoserver/manage.py
+-rw-rw-rw-   0        0        0      533 2023-07-05 19:56:14.000000 egorovsystem-0.0.4/egoserver/run.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.458387 egorovsystem-0.0.4/egoserver/server/
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.4/egoserver/server/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-05 17:41:04.000000 egorovsystem-0.0.4/egoserver/server/admin.py
+-rw-rw-rw-   0        0        0      150 2023-07-05 17:35:32.000000 egorovsystem-0.0.4/egoserver/server/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.462389 egorovsystem-0.0.4/egoserver/server/migrations/
+-rw-rw-rw-   0        0        0     1387 2023-07-05 18:07:03.000000 egorovsystem-0.0.4/egoserver/server/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 17:35:32.000000 egorovsystem-0.0.4/egoserver/server/migrations/__init__.py
+-rw-rw-rw-   0        0        0      747 2023-07-05 18:02:46.000000 egorovsystem-0.0.4/egoserver/server/models.py
+-rw-rw-rw-   0        0        0       63 2023-07-05 17:35:32.000000 egorovsystem-0.0.4/egoserver/server/tests.py
+-rw-rw-rw-   0        0        0      405 2023-07-05 18:59:18.000000 egorovsystem-0.0.4/egoserver/server/urls.py
+-rw-rw-rw-   0        0        0      215 2023-07-05 17:59:31.000000 egorovsystem-0.0.4/egoserver/server/utils.py
+-rw-rw-rw-   0        0        0     2466 2023-07-05 20:02:50.000000 egorovsystem-0.0.4/egoserver/server/views.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 02:04:34.468390 egorovsystem-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      950 2023-07-06 02:04:00.000000 egorovsystem-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 02:04:34.465389 egorovsystem-0.0.4/test/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.4/test/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-07-05 19:43:40.000000 egorovsystem-0.0.4/test/a.py
```

### Comparing `egorovsystem-0.0.2/LICENSE` & `egorovsystem-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.2/PKG-INFO` & `egorovsystem-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.2
+Version: 0.0.4
 Author: Yongyi Yang
+Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `egorovsystem-0.0.2/egolocal/main.py` & `egorovsystem-0.0.4/egolocal/main.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.2/egorovsystem.egg-info/PKG-INFO` & `egorovsystem-0.0.4/egorovsystem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.2
+Version: 0.0.4
 Author: Yongyi Yang
+Author-email: yongyi@umich.edu
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `egorovsystem-0.0.2/egoserver/manage.py` & `egorovsystem-0.0.4/egoserver/manage.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.2/egoserver/run.py` & `egorovsystem-0.0.4/egoserver/run.py`

 * *Files identical despite different names*

