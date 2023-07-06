# Comparing `tmp/pipcoloringskitsV1-1.0.0.tar.gz` & `tmp/pipcoloringskitsV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcoloringskitsV1-1.0.0.tar", last modified: Thu Jul  6 14:50:38 2023, max compression
+gzip compressed data, was "pipcoloringskitsV1-1.1.0.tar", last modified: Thu Jul  6 14:52:43 2023, max compression
```

## Comparing `pipcoloringskitsV1-1.0.0.tar` & `pipcoloringskitsV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:50:38.425339 pipcoloringskitsV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-06 14:50:38.425339 pipcoloringskitsV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:50:38.425339 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-06 14:50:37.000000 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:50:38.425339 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-06 14:50:38.000000 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-06 14:50:38.000000 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:50:38.000000 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 14:50:38.000000 pipcoloringskitsV1-1.0.0/pipcoloringskitsV1.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:50:38.429339 pipcoloringskitsV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-06 14:50:37.000000 pipcoloringskitsV1-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:52:43.876881 pipcoloringskitsV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-06 14:52:43.876881 pipcoloringskitsV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:52:43.872881 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:52:43.876881 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/pipcoloringskitsV1.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:52:43.876881 pipcoloringskitsV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-06 14:52:43.000000 pipcoloringskitsV1-1.1.0/setup.py
```

### Comparing `pipcoloringskitsV1-1.0.0/setup.py` & `pipcoloringskitsV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcoloringskitsV1",
     version=VERSION,
```

