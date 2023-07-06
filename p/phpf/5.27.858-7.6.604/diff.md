# Comparing `tmp/phpf-5.27.858.tar.gz` & `tmp/phpf-7.6.604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpf-5.27.858.tar", last modified: Sat May 27 09:01:01 2023, max compression
+gzip compressed data, was "phpf-7.6.604.tar", last modified: Thu Jul  6 06:09:29 2023, max compression
```

## Comparing `phpf-5.27.858.tar` & `phpf-7.6.604.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:01:01.427800 phpf-5.27.858/
--rw-rw-rw-   0        0        0      829 2023-05-27 08:58:36.000000 phpf-5.27.858/LICENSE
--rw-rw-rw-   0        0        0      203 2023-05-27 09:01:01.427800 phpf-5.27.858/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-05-27 08:58:36.000000 phpf-5.27.858/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 09:01:01.380906 phpf-5.27.858/phpf/
--rw-rw-rw-   0        0        0    18033 2023-05-27 08:58:36.000000 phpf-5.27.858/phpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:01:01.427800 phpf-5.27.858/phpf.egg-info/
--rw-rw-rw-   0        0        0      203 2023-05-27 09:01:01.000000 phpf-5.27.858/phpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-05-27 09:01:01.000000 phpf-5.27.858/phpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:01:01.000000 phpf-5.27.858/phpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-27 09:01:01.000000 phpf-5.27.858/phpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 09:01:01.427800 phpf-5.27.858/setup.cfg
--rw-rw-rw-   0        0        0      375 2023-05-27 08:58:36.000000 phpf-5.27.858/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:09:29.712011 phpf-7.6.604/
+-rw-rw-rw-   0        0        0      829 2023-07-06 06:04:53.000000 phpf-7.6.604/LICENSE
+-rw-rw-rw-   0        0        0      202 2023-07-06 06:09:29.701193 phpf-7.6.604/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-07-06 06:04:53.000000 phpf-7.6.604/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 06:09:29.658351 phpf-7.6.604/phpf/
+-rw-rw-rw-   0        0        0    18076 2023-07-06 06:04:53.000000 phpf-7.6.604/phpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:09:29.701193 phpf-7.6.604/phpf.egg-info/
+-rw-rw-rw-   0        0        0      202 2023-07-06 06:09:29.000000 phpf-7.6.604/phpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-07-06 06:09:29.000000 phpf-7.6.604/phpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:09:29.000000 phpf-7.6.604/phpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-06 06:09:29.000000 phpf-7.6.604/phpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:09:29.712011 phpf-7.6.604/setup.cfg
+-rw-rw-rw-   0        0        0      374 2023-07-06 06:04:53.000000 phpf-7.6.604/setup.py
```

### Comparing `phpf-5.27.858/LICENSE` & `phpf-7.6.604/LICENSE`

 * *Files identical despite different names*

### Comparing `phpf-5.27.858/phpf/__init__.py` & `phpf-7.6.604/phpf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,17 @@
 	
 	return time.strftime(s, time.localtime(t))
 #----------------------------------------------------------------------------------
 def print_r(vv):
 	import pprint
 	pprint.pprint(vv)
 #----------------------------------------------------------------------------------
-
+def sleep(i):
+	import time
+	time.sleep(i)
 
 def is_array(v):
 	v = str(type(v))
 	return True if v == ("<class 'list'>" or "<class 'tuple'>" or "<class 'range'>" or "<class 'dict'>" or "<class 'frozenset'>" or "<class 'set'>") else False
 #----------------------------------------------------------------------------------
 def is_dict(v):
 	v = str(type(v))
```

