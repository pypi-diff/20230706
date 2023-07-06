# Comparing `tmp/scriptime-0.1.0.tar.gz` & `tmp/scriptime-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.1.0.tar", last modified: Thu Jul  6 19:57:16 2023, max compression
+gzip compressed data, was "scriptime-0.1.1.tar", last modified: Thu Jul  6 20:02:02 2023, max compression
```

## Comparing `scriptime-0.1.0.tar` & `scriptime-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 19:57:16.151140 scriptime-0.1.0/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       27 2023-07-06 14:55:07.000000 scriptime-0.1.0/MANIFEST.in
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 19:57:16.150979 scriptime-0.1.0/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)     4943 2023-07-06 19:42:35.000000 scriptime-0.1.0/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 19:57:16.149813 scriptime-0.1.0/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.0/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.0/scriptime/alert.wav
--rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.0/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 19:57:16.150747 scriptime-0.1.0/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 19:57:16.000000 scriptime-0.1.0/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      254 2023-07-06 19:57:16.000000 scriptime-0.1.0/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 19:57:16.000000 scriptime-0.1.0/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-06 19:57:16.000000 scriptime-0.1.0/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 19:57:16.000000 scriptime-0.1.0/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 19:57:16.151185 scriptime-0.1.0/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      476 2023-07-06 19:56:58.000000 scriptime-0.1.0/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:02:02.290063 scriptime-0.1.1/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 20:01:46.000000 scriptime-0.1.1/MANIFEST.in
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 20:02:02.289909 scriptime-0.1.1/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     4943 2023-07-06 19:42:35.000000 scriptime-0.1.1/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:02:02.288020 scriptime-0.1.1/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.1.1/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)   701148 2023-07-05 22:10:39.000000 scriptime-0.1.1/scriptime/alert.wav
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     9874 2023-07-06 19:55:45.000000 scriptime-0.1.1/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 20:02:02.289703 scriptime-0.1.1/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 20:02:02.000000 scriptime-0.1.1/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      254 2023-07-06 20:02:02.000000 scriptime-0.1.1/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 20:02:02.000000 scriptime-0.1.1/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       30 2023-07-06 20:02:02.000000 scriptime-0.1.1/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 20:02:02.000000 scriptime-0.1.1/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 20:02:02.290109 scriptime-0.1.1/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      476 2023-07-06 20:01:57.000000 scriptime-0.1.1/setup.py
```

### Comparing `scriptime-0.1.0/README.md` & `scriptime-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.0/scriptime/alert.wav` & `scriptime-0.1.1/scriptime/alert.wav`

 * *Files identical despite different names*

### Comparing `scriptime-0.1.0/scriptime/main.py` & `scriptime-0.1.1/scriptime/main.py`

 * *Files identical despite different names*

