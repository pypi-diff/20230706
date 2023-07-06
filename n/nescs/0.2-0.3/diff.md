# Comparing `tmp/nescs-0.2.tar.gz` & `tmp/nescs-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nescs-0.2.tar", last modified: Thu Jul  6 16:59:43 2023, max compression
+gzip compressed data, was "nescs-0.3.tar", last modified: Thu Jul  6 17:00:53 2023, max compression
```

## Comparing `nescs-0.2.tar` & `nescs-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 16:59:43.732134 nescs-0.2/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-06 15:30:37.000000 nescs-0.2/MANIFEST.in
--rw-r--r--   0 twoics    (1000) twoics    (1000)      467 2023-07-06 16:59:43.732134 nescs-0.2/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      210 2023-07-06 15:48:59.000000 nescs-0.2/README.rst
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 16:59:43.731134 nescs-0.2/nesc/
--rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-06 16:08:50.000000 nescs-0.2/nesc/__init__.py
--rw-r--r--   0 twoics    (1000) twoics    (1000)     5062 2023-07-06 15:30:37.000000 nescs-0.2/nesc/service.py
-drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 16:59:43.732134 nescs-0.2/nescs.egg-info/
--rw-r--r--   0 twoics    (1000) twoics    (1000)      467 2023-07-06 16:59:43.000000 nescs-0.2/nescs.egg-info/PKG-INFO
--rw-r--r--   0 twoics    (1000) twoics    (1000)      205 2023-07-06 16:59:43.000000 nescs-0.2/nescs.egg-info/SOURCES.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-06 16:59:43.000000 nescs-0.2/nescs.egg-info/dependency_links.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-06 16:59:43.000000 nescs-0.2/nescs.egg-info/top_level.txt
--rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-06 15:30:37.000000 nescs-0.2/pyproject.toml
--rw-r--r--   0 twoics    (1000) twoics    (1000)      338 2023-07-06 16:59:43.732134 nescs-0.2/setup.cfg
--rw-r--r--   0 twoics    (1000) twoics    (1000)      108 2023-07-06 16:32:47.000000 nescs-0.2/setup.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:00:53.957418 nescs-0.3/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      104 2023-07-06 15:30:37.000000 nescs-0.3/MANIFEST.in
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      467 2023-07-06 17:00:53.957418 nescs-0.3/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      210 2023-07-06 15:48:59.000000 nescs-0.3/README.rst
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:00:53.956418 nescs-0.3/nesc/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       45 2023-07-06 16:08:50.000000 nescs-0.3/nesc/__init__.py
+-rw-r--r--   0 twoics    (1000) twoics    (1000)     5062 2023-07-06 15:30:37.000000 nescs-0.3/nesc/service.py
+drwxr-xr-x   0 twoics    (1000) twoics    (1000)        0 2023-07-06 17:00:53.957418 nescs-0.3/nescs.egg-info/
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      467 2023-07-06 17:00:53.000000 nescs-0.3/nescs.egg-info/PKG-INFO
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      205 2023-07-06 17:00:53.000000 nescs-0.3/nescs.egg-info/SOURCES.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        1 2023-07-06 17:00:53.000000 nescs-0.3/nescs.egg-info/dependency_links.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)        5 2023-07-06 17:00:53.000000 nescs-0.3/nescs.egg-info/top_level.txt
+-rw-r--r--   0 twoics    (1000) twoics    (1000)       88 2023-07-06 15:30:37.000000 nescs-0.3/pyproject.toml
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      338 2023-07-06 17:00:53.957418 nescs-0.3/setup.cfg
+-rw-r--r--   0 twoics    (1000) twoics    (1000)      108 2023-07-06 16:32:47.000000 nescs-0.3/setup.py
```

### Comparing `nescs-0.2/nesc/service.py` & `nescs-0.3/nesc/service.py`

 * *Files identical despite different names*

