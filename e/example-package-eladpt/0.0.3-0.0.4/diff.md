# Comparing `tmp/example_package_eladpt-0.0.3.tar.gz` & `tmp/example_package_eladpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_eladpt-0.0.3.tar", last modified: Thu Jul  6 10:43:17 2023, max compression
+gzip compressed data, was "example_package_eladpt-0.0.4.tar", last modified: Thu Jul  6 10:47:45 2023, max compression
```

## Comparing `example_package_eladpt-0.0.3.tar` & `example_package_eladpt-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:43:17.360884 example_package_eladpt-0.0.3/
--rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:43:17.360653 example_package_eladpt-0.0.3/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 09:14:29.000000 example_package_eladpt-0.0.3/README.md
--rw-r--r--   0 elad.pticha   (502) staff       (20)      422 2023-07-06 10:43:10.000000 example_package_eladpt-0.0.3/pyproject.toml
--rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 10:43:17.360957 example_package_eladpt-0.0.3/setup.cfg
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:43:17.358958 example_package_eladpt-0.0.3/src/
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:43:17.359829 example_package_eladpt-0.0.3/src/example_package_eladpt.egg-info/
--rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:43:17.000000 example_package_eladpt-0.0.3/src/example_package_eladpt.egg-info/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)      273 2023-07-06 10:43:17.000000 example_package_eladpt-0.0.3/src/example_package_eladpt.egg-info/SOURCES.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 10:43:17.000000 example_package_eladpt-0.0.3/src/example_package_eladpt.egg-info/dependency_links.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 10:43:17.000000 example_package_eladpt-0.0.3/src/example_package_eladpt.egg-info/top_level.txt
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:43:17.360102 example_package_eladpt-0.0.3/src/pkg_eladpt/
--rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.3/src/pkg_eladpt/__init__.py
--rw-r--r--   0 elad.pticha   (502) staff       (20)      111 2023-07-06 10:42:48.000000 example_package_eladpt-0.0.3/src/pkg_eladpt/run.py
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:47:45.866061 example_package_eladpt-0.0.4/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:47:45.865893 example_package_eladpt-0.0.4/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 09:14:29.000000 example_package_eladpt-0.0.4/README.md
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      438 2023-07-06 10:47:35.000000 example_package_eladpt-0.0.4/pyproject.toml
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 10:47:45.866123 example_package_eladpt-0.0.4/setup.cfg
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:47:45.864117 example_package_eladpt-0.0.4/src/
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:47:45.865150 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:47:45.000000 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      322 2023-07-06 10:47:45.000000 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/SOURCES.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 10:47:45.000000 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/dependency_links.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 10:47:45.000000 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/requires.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 10:47:45.000000 example_package_eladpt-0.0.4/src/example_package_eladpt.egg-info/top_level.txt
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:47:45.865416 example_package_eladpt-0.0.4/src/pkg_eladpt/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.4/src/pkg_eladpt/__init__.py
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      111 2023-07-06 10:42:48.000000 example_package_eladpt-0.0.4/src/pkg_eladpt/run.py
```

