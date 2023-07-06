# Comparing `tmp/safepull-1.1.0.tar.gz` & `tmp/safepull-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-1.1.0.tar", last modified: Wed Jun 28 03:04:46 2023, max compression
+gzip compressed data, was "safepull-2.0.0.tar", last modified: Thu Jul  6 14:10:21 2023, max compression
```

## Comparing `safepull-1.1.0.tar` & `safepull-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 03:04:46.460860 safepull-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-28 03:04:37.000000 safepull-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-28 03:04:46.460860 safepull-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-28 03:04:37.000000 safepull-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-28 03:04:37.000000 safepull-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 03:04:46.460860 safepull-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 03:04:46.460860 safepull-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 03:04:46.460860 safepull-1.1.0/src/safepull/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 03:04:37.000000 safepull-1.1.0/src/safepull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 03:04:37.000000 safepull-1.1.0/src/safepull/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-28 03:04:37.000000 safepull-1.1.0/src/safepull/safepull.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 03:04:46.460860 safepull-1.1.0/src/safepull.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-28 03:04:46.000000 safepull-1.1.0/src/safepull.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 14:10:07.000000 safepull-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-06 14:10:21.637467 safepull-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-06 14:10:07.000000 safepull-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-06 14:10:07.000000 safepull-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 14:10:21.637467 safepull-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.633467 safepull-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/src/safepull/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-06 14:10:07.000000 safepull-2.0.0/src/safepull/safepull.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:10:21.637467 safepull-2.0.0/src/safepull.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 14:10:21.000000 safepull-2.0.0/src/safepull.egg-info/top_level.txt
```

### Comparing `safepull-1.1.0/LICENSE` & `safepull-2.0.0/LICENSE`

 * *Files identical despite different names*

