# Comparing `tmp/egorovsystem-0.0.1.tar.gz` & `tmp/egorovsystem-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\egorovsystem-0.0.1.tar", last modified: Wed Jul  5 20:08:34 2023, max compression
+gzip compressed data, was "dist\egorovsystem-0.0.2.tar", last modified: Wed Jul  5 20:23:07 2023, max compression
```

## Comparing `egorovsystem-0.0.1.tar` & `egorovsystem-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:08:34.278419 egorovsystem-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1530 2023-07-05 20:08:34.277419 egorovsystem-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 20:08:34.251413 egorovsystem-0.0.1/egolocal/
--rw-rw-rw-   0        0        0     1473 2023-07-05 20:07:45.000000 egorovsystem-0.0.1/egolocal/main.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:08:34.255414 egorovsystem-0.0.1/egorovsystem/
--rw-rw-rw-   0        0        0      475 2023-07-05 19:40:59.000000 egorovsystem-0.0.1/egorovsystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:08:34.269418 egorovsystem-0.0.1/egorovsystem.egg-info/
--rw-rw-rw-   0        0        0     1530 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-05 20:08:34.000000 egorovsystem-0.0.1/egorovsystem.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-05 20:08:34.274419 egorovsystem-0.0.1/egoserver/
--rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.1/egoserver/manage.py
--rw-rw-rw-   0        0        0      533 2023-07-05 19:56:14.000000 egorovsystem-0.0.1/egoserver/run.py
--rw-rw-rw-   0        0        0       42 2023-07-05 20:08:34.278419 egorovsystem-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-07-05 20:08:14.000000 egorovsystem-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.315374 egorovsystem-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 17:14:09.000000 egorovsystem-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1530 2023-07-05 20:23:07.315374 egorovsystem-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-07-05 19:50:38.000000 egorovsystem-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.295370 egorovsystem-0.0.2/egolocal/
+-rw-rw-rw-   0        0        0     1473 2023-07-05 20:07:45.000000 egorovsystem-0.0.2/egolocal/main.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.297371 egorovsystem-0.0.2/egorovsystem/
+-rw-rw-rw-   0        0        0      475 2023-07-05 19:40:59.000000 egorovsystem-0.0.2/egorovsystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.306372 egorovsystem-0.0.2/egorovsystem.egg-info/
+-rw-rw-rw-   0        0        0     1530 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-05 20:23:07.000000 egorovsystem-0.0.2/egorovsystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.309373 egorovsystem-0.0.2/egoserver/
+-rw-rw-rw-   0        0        0      687 2023-07-05 17:33:47.000000 egorovsystem-0.0.2/egoserver/manage.py
+-rw-rw-rw-   0        0        0      533 2023-07-05 19:56:14.000000 egorovsystem-0.0.2/egoserver/run.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 20:23:07.316375 egorovsystem-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      847 2023-07-05 20:23:00.000000 egorovsystem-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 20:23:07.313373 egorovsystem-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2023-07-05 19:43:29.000000 egorovsystem-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-07-05 19:43:40.000000 egorovsystem-0.0.2/test/a.py
```

### Comparing `egorovsystem-0.0.1/LICENSE` & `egorovsystem-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.1/PKG-INFO` & `egorovsystem-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.1
+Version: 0.0.2
 Author: Yongyi Yang
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `egorovsystem-0.0.1/egolocal/main.py` & `egorovsystem-0.0.2/egolocal/main.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.1/egorovsystem.egg-info/PKG-INFO` & `egorovsystem-0.0.2/egorovsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egorovsystem
-Version: 0.0.1
+Version: 0.0.2
 Author: Yongyi Yang
 License: MIT License
         
         Copyright (c) 2023 Yongyi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `egorovsystem-0.0.1/egoserver/manage.py` & `egorovsystem-0.0.2/egoserver/manage.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.1/egoserver/run.py` & `egorovsystem-0.0.2/egoserver/run.py`

 * *Files identical despite different names*

### Comparing `egorovsystem-0.0.1/setup.py` & `egorovsystem-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 with open("README.md", encoding="utf-8") as f:
 	readme = f.read()
 
 with open("LICENSE", encoding="utf-8") as f:
 	license = f.read()
 
-with open("requirements.txt", encoding="utf-8") as f:
-	reqs = f.read()
+# pip 在搞什么飞机
+try:
+	with open("requirements.txt", encoding="utf-8") as f:
+		reqs = f.read()
+except:
+	reqs = ""
 
 setup(
 	name					= "egorovsystem",
-	version					= "0.0.1",
+	version					= "0.0.2",
 	description				= "",
 	long_description		= readme,
 	long_description_content_type	= "text/markdown",
 	license					= license,
 	author					= "Yongyi Yang",
 	python_requires			= ">=3.6",
 	packages				= ["egoserver", "egolocal", "egorovsystem"],
 	install_requires		= reqs.strip().split("\n"),
 	entry_points			= {"console_scripts": [
 		"egoserver-init=egoserver.run:init" , 
 		"egoserver-run=egoserver.run:run" , 
 		"egolocal-run=egolocal.main:run" , 
-	]}
+	]} ,
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

