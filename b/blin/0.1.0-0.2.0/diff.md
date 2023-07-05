# Comparing `tmp/blin-0.1.0.tar.gz` & `tmp/blin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blin-0.1.0.tar", last modified: Fri Jun 16 01:01:15 2023, max compression
+gzip compressed data, was "blin-0.2.0.tar", last modified: Wed Jul  5 22:48:57 2023, max compression
```

## Comparing `blin-0.1.0.tar` & `blin-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.681123 blin-0.1.0/
--rw-rw-rw-   0        0        0      177 2023-06-16 01:01:15.680124 blin-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-27 00:54:36.000000 blin-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.659119 blin-0.1.0/blin/
--rw-rw-rw-   0        0        0     5343 2023-06-15 23:33:53.000000 blin-0.1.0/blin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 01:01:15.679124 blin-0.1.0/blin.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 01:01:15.000000 blin-0.1.0/blin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.1.0/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 01:01:15.681123 blin-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      211 2023-06-16 01:00:20.000000 blin-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.075543 blin-0.2.0/
+-rw-rw-rw-   0        0        0     6955 2023-07-05 22:48:57.074542 blin-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6733 2023-07-05 21:14:07.000000 blin-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.049536 blin-0.2.0/blin/
+-rw-rw-rw-   0        0        0     6252 2023-07-05 22:47:23.000000 blin-0.2.0/blin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 22:48:57.073542 blin-0.2.0/blin.egg-info/
+-rw-rw-rw-   0        0        0     6955 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-05 22:48:57.000000 blin-0.2.0/blin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-05 22:48:56.000000 blin-0.2.0/blin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1063 2023-05-27 00:54:38.000000 blin-0.2.0/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 22:48:57.075543 blin-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      475 2023-07-05 22:48:18.000000 blin-0.2.0/setup.py
```

### Comparing `blin-0.1.0/license.txt` & `blin-0.2.0/license.txt`

 * *Files identical despite different names*

