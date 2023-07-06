# Comparing `tmp/scriptime-0.0.4.tar.gz` & `tmp/scriptime-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.0.4.tar", last modified: Thu Jul  6 00:09:09 2023, max compression
+gzip compressed data, was "scriptime-0.0.5.tar", last modified: Thu Jul  6 02:44:59 2023, max compression
```

## Comparing `scriptime-0.0.4.tar` & `scriptime-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 00:09:09.535809 scriptime-0.0.4/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 00:09:09.535676 scriptime-0.0.4/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.4/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 00:09:09.534569 scriptime-0.0.4/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.4/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)     2962 2023-07-06 00:00:02.000000 scriptime-0.0.4/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 00:09:09.535478 scriptime-0.0.4/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 00:09:09.000000 scriptime-0.0.4/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 00:09:09.000000 scriptime-0.0.4/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 00:09:09.000000 scriptime-0.0.4/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 00:09:09.000000 scriptime-0.0.4/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 00:09:09.000000 scriptime-0.0.4/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 00:09:09.535849 scriptime-0.0.4/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-06 00:09:04.000000 scriptime-0.0.4/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.927643 scriptime-0.0.5/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:44:59.927508 scriptime-0.0.5/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.5/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.926593 scriptime-0.0.5/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       45 2023-07-06 00:08:59.000000 scriptime-0.0.5/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     5007 2023-07-06 02:42:34.000000 scriptime-0.0.5/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-06 02:44:59.927328 scriptime-0.0.5/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-06 02:44:59.000000 scriptime-0.0.5/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-06 02:44:59.927680 scriptime-0.0.5/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-06 02:43:37.000000 scriptime-0.0.5/setup.py
```

