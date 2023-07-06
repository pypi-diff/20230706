# Comparing `tmp/sicdeploy-0.1.2.tar.gz` & `tmp/sicdeploy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sicdeploy-0.1.2.tar", last modified: Thu Jul  6 08:35:09 2023, max compression
+gzip compressed data, was "sicdeploy-0.1.3.tar", last modified: Thu Jul  6 08:37:03 2023, max compression
```

## Comparing `sicdeploy-0.1.2.tar` & `sicdeploy-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:35:09.856716 sicdeploy-0.1.2/
--rw-r--r--   0 samuel.c   (505) staff       (20)       70 2023-07-06 08:35:09.856454 sicdeploy-0.1.2/PKG-INFO
--rw-r--r--   0 samuel.c   (505) staff       (20)     1239 2023-07-06 08:15:23.000000 sicdeploy-0.1.2/README.rst
--rw-r--r--   0 samuel.c   (505) staff       (20)       38 2023-07-06 08:35:09.856801 sicdeploy-0.1.2/setup.cfg
--rw-r--r--   0 samuel.c   (505) staff       (20)      392 2023-07-06 08:35:00.000000 sicdeploy-0.1.2/setup.py
-drwxr-xr-x   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:35:09.856144 sicdeploy-0.1.2/sicdeploy.egg-info/
--rw-r--r--   0 samuel.c   (505) staff       (20)       70 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/PKG-INFO
--rw-r--r--   0 samuel.c   (505) staff       (20)      219 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 samuel.c   (505) staff       (20)        1 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 samuel.c   (505) staff       (20)       48 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/entry_points.txt
--rw-r--r--   0 samuel.c   (505) staff       (20)       31 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/requires.txt
--rw-r--r--   0 samuel.c   (505) staff       (20)        1 2023-07-06 08:35:09.000000 sicdeploy-0.1.2/sicdeploy.egg-info/top_level.txt
+drwxr-xr-x   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:37:03.093946 sicdeploy-0.1.3/
+-rw-r--r--   0 samuel.c   (505) staff       (20)       70 2023-07-06 08:37:03.093718 sicdeploy-0.1.3/PKG-INFO
+-rw-r--r--   0 samuel.c   (505) staff       (20)     1239 2023-07-06 08:15:23.000000 sicdeploy-0.1.3/README.rst
+-rw-r--r--   0 samuel.c   (505) staff       (20)       38 2023-07-06 08:37:03.094071 sicdeploy-0.1.3/setup.cfg
+-rw-r--r--   0 samuel.c   (505) staff       (20)      392 2023-07-06 08:37:00.000000 sicdeploy-0.1.3/setup.py
+drwxr-xr-x   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:37:03.091972 sicdeploy-0.1.3/sicdeploy/
+-rw-r--r--   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:36:28.000000 sicdeploy-0.1.3/sicdeploy/__init__.py
+-rw-r--r--   0 samuel.c   (505) staff       (20)       94 2023-07-06 08:03:31.000000 sicdeploy-0.1.3/sicdeploy/run.py
+drwxr-xr-x   0 samuel.c   (505) staff       (20)        0 2023-07-06 08:37:03.093422 sicdeploy-0.1.3/sicdeploy.egg-info/
+-rw-r--r--   0 samuel.c   (505) staff       (20)       70 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 samuel.c   (505) staff       (20)      258 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel.c   (505) staff       (20)        1 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel.c   (505) staff       (20)       48 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 samuel.c   (505) staff       (20)       31 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/requires.txt
+-rw-r--r--   0 samuel.c   (505) staff       (20)       10 2023-07-06 08:37:03.000000 sicdeploy-0.1.3/sicdeploy.egg-info/top_level.txt
```

### Comparing `sicdeploy-0.1.2/README.rst` & `sicdeploy-0.1.3/README.rst`

 * *Files identical despite different names*

