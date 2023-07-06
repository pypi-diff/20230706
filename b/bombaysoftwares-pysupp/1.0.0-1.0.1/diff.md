# Comparing `tmp/bombaysoftwares-pysupp-1.0.0.tar.gz` & `tmp/bombaysoftwares-pysupp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bombaysoftwares-pysupp-1.0.0.tar", last modified: Wed Jul  5 06:45:40 2023, max compression
+gzip compressed data, was "bombaysoftwares-pysupp-1.0.1.tar", last modified: Wed Jul  5 11:47:01 2023, max compression
```

## Comparing `bombaysoftwares-pysupp-1.0.0.tar` & `bombaysoftwares-pysupp-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1073 2023-07-05 06:20:56.000000 bombaysoftwares-pysupp-1.0.0/LICENSE
--rw-rw-r--   0 divy      (1000) divy      (1000)       33 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.0/MANIFEST.in
--rw-rw-r--   0 divy      (1000) divy      (1000)      548 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)     2760 2023-07-05 06:33:21.000000 bombaysoftwares-pysupp-1.0.0/README.md
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/bombaysoftwares_pysupp.egg-info/
--rw-rw-r--   0 divy      (1000) divy      (1000)      548 2023-07-05 06:45:40.000000 bombaysoftwares-pysupp-1.0.0/bombaysoftwares_pysupp.egg-info/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)      297 2023-07-05 06:45:40.000000 bombaysoftwares-pysupp-1.0.0/bombaysoftwares_pysupp.egg-info/SOURCES.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-05 06:45:40.000000 bombaysoftwares-pysupp-1.0.0/bombaysoftwares_pysupp.egg-info/dependency_links.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)       12 2023-07-05 06:45:40.000000 bombaysoftwares-pysupp-1.0.0/bombaysoftwares_pysupp.egg-info/top_level.txt
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/pykit/
--rw-rw-r--   0 divy      (1000) divy      (1000)      388 2023-07-05 06:45:33.000000 bombaysoftwares-pysupp-1.0.0/pykit/__init__.py
--rw-rw-r--   0 divy      (1000) divy      (1000)    15955 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.0/pykit/utils.py
--rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/setup.cfg
--rw-rw-r--   0 divy      (1000) divy      (1000)      653 2023-07-05 06:34:34.000000 bombaysoftwares-pysupp-1.0.0/setup.py
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 06:45:40.448440 bombaysoftwares-pysupp-1.0.0/tests/
--rw-rw-r--   0 divy      (1000) divy      (1000)        0 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.0/tests/__init__.py
--rw-rw-r--   0 divy      (1000) divy      (1000)    11355 2023-07-05 06:28:36.000000 bombaysoftwares-pysupp-1.0.0/tests/test_my_module.py
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 11:47:01.499248 bombaysoftwares-pysupp-1.0.1/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1073 2023-07-05 06:20:56.000000 bombaysoftwares-pysupp-1.0.1/LICENSE
+-rw-rw-r--   0 divy      (1000) divy      (1000)       33 2023-07-05 06:20:36.000000 bombaysoftwares-pysupp-1.0.1/MANIFEST.in
+-rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-05 11:47:01.499248 bombaysoftwares-pysupp-1.0.1/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)     2760 2023-07-05 06:33:21.000000 bombaysoftwares-pysupp-1.0.1/README.md
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-05 11:47:01.499248 bombaysoftwares-pysupp-1.0.1/bombaysoftwares_pysupp.egg-info/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     4662 2023-07-05 11:47:01.000000 bombaysoftwares-pysupp-1.0.1/bombaysoftwares_pysupp.egg-info/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)      222 2023-07-05 11:47:01.000000 bombaysoftwares-pysupp-1.0.1/bombaysoftwares_pysupp.egg-info/SOURCES.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-05 11:47:01.000000 bombaysoftwares-pysupp-1.0.1/bombaysoftwares_pysupp.egg-info/dependency_links.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-05 11:47:01.000000 bombaysoftwares-pysupp-1.0.1/bombaysoftwares_pysupp.egg-info/top_level.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-05 11:47:01.499248 bombaysoftwares-pysupp-1.0.1/setup.cfg
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1335 2023-07-05 11:45:34.000000 bombaysoftwares-pysupp-1.0.1/setup.py
```

### Comparing `bombaysoftwares-pysupp-1.0.0/LICENSE` & `bombaysoftwares-pysupp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bombaysoftwares-pysupp-1.0.0/README.md` & `bombaysoftwares-pysupp-1.0.1/README.md`

 * *Files identical despite different names*

