# Comparing `tmp/alireza-0.0.3.tar.gz` & `tmp/alireza-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alireza-0.0.3.tar", last modified: Mon Jul  3 08:26:02 2023, max compression
+gzip compressed data, was "alireza-0.0.4.tar", last modified: Thu Jul  6 01:14:40 2023, max compression
```

## Comparing `alireza-0.0.3.tar` & `alireza-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-07-03 08:26:02.423488 alireza-0.0.3/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.3/README.md
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       36 2023-07-03 08:11:46.000000 alireza-0.0.3/alireza/__init__.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza/__managers/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       30 2023-07-03 08:06:03.000000 alireza-0.0.3/alireza/__managers/__init__.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1151 2023-07-03 08:02:39.000000 alireza-0.0.3/alireza/__managers/_django_manager.py
--rw-rw-r--   0 alireza   (1000) alireza   (1000)     1719 2023-07-03 08:12:43.000000 alireza-0.0.3/alireza/_django_tools.py
-drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-03 08:26:02.423488 alireza-0.0.3/alireza.egg-info/
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      704 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/PKG-INFO
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      256 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/SOURCES.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/dependency_links.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-07-03 08:26:02.000000 alireza-0.0.3/alireza.egg-info/top_level.txt
--rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-03 08:26:02.423488 alireza-0.0.3/setup.cfg
--rw-rw-r--   0 alireza   (1000) alireza   (1000)      934 2023-07-03 08:23:33.000000 alireza-0.0.3/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1775 2023-07-06 01:14:40.936100 alireza-0.0.4/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-06-14 12:34:33.000000 alireza-0.0.4/README.md
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.932100 alireza-0.0.4/alireza/
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza/DjangoTools/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1590 2023-07-05 21:36:04.000000 alireza-0.0.4/alireza/DjangoTools/__Error_Handler.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 07:20:15.000000 alireza-0.0.4/alireza/DjangoTools/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     3349 2023-07-06 00:52:33.000000 alireza-0.0.4/alireza/DjangoTools/__manager.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza/UsefulTools/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     5256 2023-07-06 00:24:10.000000 alireza-0.0.4/alireza/UsefulTools/__Error_Handler.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       24 2023-07-04 22:28:11.000000 alireza-0.0.4/alireza/UsefulTools/__init__.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     4117 2023-07-06 00:29:41.000000 alireza-0.0.4/alireza/UsefulTools/__manager.py
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       52 2023-07-04 09:14:57.000000 alireza-0.0.4/alireza/__init__.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/alireza.egg-info/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     1775 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/PKG-INFO
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)      383 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/SOURCES.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        1 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/dependency_links.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        8 2023-07-06 01:14:40.000000 alireza-0.0.4/alireza.egg-info/top_level.txt
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)       38 2023-07-06 01:14:40.936100 alireza-0.0.4/setup.cfg
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)     2009 2023-07-06 01:14:05.000000 alireza-0.0.4/setup.py
+drwxrwxr-x   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:14:40.936100 alireza-0.0.4/test/
+-rw-rw-r--   0 alireza   (1000) alireza   (1000)        0 2023-07-06 01:09:15.000000 alireza-0.0.4/test/test.py
```

