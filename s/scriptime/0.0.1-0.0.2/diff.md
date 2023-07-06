# Comparing `tmp/scriptime-0.0.1.tar.gz` & `tmp/scriptime-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptime-0.0.1.tar", last modified: Wed Jul  5 23:38:19 2023, max compression
+gzip compressed data, was "scriptime-0.0.2.tar", last modified: Wed Jul  5 23:52:50 2023, max compression
```

## Comparing `scriptime-0.0.1.tar` & `scriptime-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:38:19.329810 scriptime-0.0.1/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-05 23:38:19.329688 scriptime-0.0.1/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.1/README.md
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:38:19.328706 scriptime-0.0.1/scriptime/
--rw-r--r--   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:24:20.000000 scriptime-0.0.1/scriptime/__init__.py
--rw-r--r--   0 jakestrasler   (501) staff       (20)     2724 2023-07-05 23:20:26.000000 scriptime-0.0.1/scriptime/main.py
-drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:38:19.329511 scriptime-0.0.1/scriptime.egg-info/
--rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-05 23:38:19.000000 scriptime-0.0.1/scriptime.egg-info/PKG-INFO
--rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-05 23:38:19.000000 scriptime-0.0.1/scriptime.egg-info/SOURCES.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-05 23:38:19.000000 scriptime-0.0.1/scriptime.egg-info/dependency_links.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-05 23:38:19.000000 scriptime-0.0.1/scriptime.egg-info/requires.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-05 23:38:19.000000 scriptime-0.0.1/scriptime.egg-info/top_level.txt
--rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-05 23:38:19.329850 scriptime-0.0.1/setup.cfg
--rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-05 23:38:15.000000 scriptime-0.0.1/setup.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:52:50.157239 scriptime-0.0.2/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-05 23:52:50.157112 scriptime-0.0.2/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      142 2023-07-05 21:03:13.000000 scriptime-0.0.2/README.md
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:52:50.156130 scriptime-0.0.2/scriptime/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       23 2023-07-05 23:51:31.000000 scriptime-0.0.2/scriptime/__init__.py
+-rw-r--r--   0 jakestrasler   (501) staff       (20)     2724 2023-07-05 23:20:26.000000 scriptime-0.0.2/scriptime/main.py
+drwxr-xr-x   0 jakestrasler   (501) staff       (20)        0 2023-07-05 23:52:50.156941 scriptime-0.0.2/scriptime.egg-info/
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      247 2023-07-05 23:52:50.000000 scriptime-0.0.2/scriptime.egg-info/PKG-INFO
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      222 2023-07-05 23:52:50.000000 scriptime-0.0.2/scriptime.egg-info/SOURCES.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)        1 2023-07-05 23:52:50.000000 scriptime-0.0.2/scriptime.egg-info/dependency_links.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       19 2023-07-05 23:52:50.000000 scriptime-0.0.2/scriptime.egg-info/requires.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       10 2023-07-05 23:52:50.000000 scriptime-0.0.2/scriptime.egg-info/top_level.txt
+-rw-r--r--   0 jakestrasler   (501) staff       (20)       38 2023-07-05 23:52:50.157277 scriptime-0.0.2/setup.cfg
+-rw-r--r--   0 jakestrasler   (501) staff       (20)      397 2023-07-05 23:52:01.000000 scriptime-0.0.2/setup.py
```

### Comparing `scriptime-0.0.1/scriptime/main.py` & `scriptime-0.0.2/scriptime/main.py`

 * *Files identical despite different names*

