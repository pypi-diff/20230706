# Comparing `tmp/creatFiles-0.1.1.tar.gz` & `tmp/creatFiles-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creatFiles-0.1.1.tar", last modified: Thu Jul  6 02:37:28 2023, max compression
+gzip compressed data, was "creatFiles-0.1.2.tar", last modified: Thu Jul  6 03:25:25 2023, max compression
```

## Comparing `creatFiles-0.1.1.tar` & `creatFiles-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 02:37:28.823817 creatFiles-0.1.1/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 creatFiles-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 creatFiles-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      402 2023-07-06 02:37:28.823817 creatFiles-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 creatFiles-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 02:37:28.797808 creatFiles-0.1.1/creatFiles/
--rw-rw-rw-   0        0        0        0 2023-02-28 07:01:01.000000 creatFiles-0.1.1/creatFiles/__init__.py
--rw-rw-rw-   0        0        0   122368 2023-07-06 02:12:23.000000 creatFiles-0.1.1/creatFiles/creatFiles.pyd
--rw-rw-rw-   0        0        0    54272 2023-07-06 02:12:32.000000 creatFiles-0.1.1/creatFiles/function_refer.pyd
--rw-rw-rw-   0        0        0    81920 2023-07-06 02:12:42.000000 creatFiles-0.1.1/creatFiles/function_refer_ui.pyd
-drwxrwxrwx   0        0        0        0 2023-07-06 02:37:28.818848 creatFiles-0.1.1/creatFiles.egg-info/
--rw-rw-rw-   0        0        0      402 2023-07-06 02:37:28.000000 creatFiles-0.1.1/creatFiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-07-06 02:37:28.000000 creatFiles-0.1.1/creatFiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 02:37:28.000000 creatFiles-0.1.1/creatFiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-06 02:37:28.000000 creatFiles-0.1.1/creatFiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-06 02:37:28.826815 creatFiles-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-07-06 02:30:16.000000 creatFiles-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 03:25:25.439523 creatFiles-0.1.2/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 creatFiles-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 creatFiles-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      402 2023-07-06 03:25:25.439523 creatFiles-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-05 02:45:05.000000 creatFiles-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 03:25:25.418535 creatFiles-0.1.2/creatFiles/
+-rw-rw-rw-   0        0        0        0 2023-02-28 07:01:01.000000 creatFiles-0.1.2/creatFiles/__init__.py
+-rw-rw-rw-   0        0        0   122368 2023-07-06 03:22:47.000000 creatFiles-0.1.2/creatFiles/creatFiles.pyd
+-rw-rw-rw-   0        0        0    54272 2023-07-06 02:12:32.000000 creatFiles-0.1.2/creatFiles/function_refer.pyd
+-rw-rw-rw-   0        0        0    81920 2023-07-06 02:12:42.000000 creatFiles-0.1.2/creatFiles/function_refer_ui.pyd
+drwxrwxrwx   0        0        0        0 2023-07-06 03:25:25.436525 creatFiles-0.1.2/creatFiles.egg-info/
+-rw-rw-rw-   0        0        0      402 2023-07-06 03:25:25.000000 creatFiles-0.1.2/creatFiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-07-06 03:25:25.000000 creatFiles-0.1.2/creatFiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 03:25:25.000000 creatFiles-0.1.2/creatFiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 03:25:25.000000 creatFiles-0.1.2/creatFiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-06 03:25:25.442493 creatFiles-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1020 2023-07-06 03:20:12.000000 creatFiles-0.1.2/setup.py
```

### Comparing `creatFiles-0.1.1/setup.py` & `creatFiles-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "creatFiles",
```

