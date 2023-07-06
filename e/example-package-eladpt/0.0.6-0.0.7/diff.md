# Comparing `tmp/example_package_eladpt-0.0.6.tar.gz` & `tmp/example_package_eladpt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_eladpt-0.0.6.tar", last modified: Thu Jul  6 10:50:21 2023, max compression
+gzip compressed data, was "example_package_eladpt-0.0.7.tar", last modified: Thu Jul  6 10:51:06 2023, max compression
```

## Comparing `example_package_eladpt-0.0.6.tar` & `example_package_eladpt-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:50:21.560202 example_package_eladpt-0.0.6/
--rw-r--r--   0 elad.pticha   (502) staff       (20)     6130 2023-07-06 10:50:21.560059 example_package_eladpt-0.0.6/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)     5738 2023-07-06 10:50:05.000000 example_package_eladpt-0.0.6/README.md
--rw-r--r--   0 elad.pticha   (502) staff       (20)      438 2023-07-06 10:50:15.000000 example_package_eladpt-0.0.6/pyproject.toml
--rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 10:50:21.560257 example_package_eladpt-0.0.6/setup.cfg
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:50:21.558394 example_package_eladpt-0.0.6/src/
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:50:21.559363 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/
--rw-r--r--   0 elad.pticha   (502) staff       (20)     6130 2023-07-06 10:50:21.000000 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)      322 2023-07-06 10:50:21.000000 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/SOURCES.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 10:50:21.000000 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/dependency_links.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 10:50:21.000000 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/requires.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 10:50:21.000000 example_package_eladpt-0.0.6/src/example_package_eladpt.egg-info/top_level.txt
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:50:21.559628 example_package_eladpt-0.0.6/src/pkg_eladpt/
--rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.6/src/pkg_eladpt/__init__.py
--rw-r--r--   0 elad.pticha   (502) staff       (20)      111 2023-07-06 10:42:48.000000 example_package_eladpt-0.0.6/src/pkg_eladpt/run.py
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:51:06.808344 example_package_eladpt-0.0.7/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      412 2023-07-06 10:51:06.808192 example_package_eladpt-0.0.7/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       20 2023-07-06 10:50:48.000000 example_package_eladpt-0.0.7/README.md
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      438 2023-07-06 10:50:56.000000 example_package_eladpt-0.0.7/pyproject.toml
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 10:51:06.808429 example_package_eladpt-0.0.7/setup.cfg
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:51:06.805861 example_package_eladpt-0.0.7/src/
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:51:06.807419 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      412 2023-07-06 10:51:06.000000 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      322 2023-07-06 10:51:06.000000 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/SOURCES.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 10:51:06.000000 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/dependency_links.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 10:51:06.000000 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/requires.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 10:51:06.000000 example_package_eladpt-0.0.7/src/example_package_eladpt.egg-info/top_level.txt
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:51:06.807726 example_package_eladpt-0.0.7/src/pkg_eladpt/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.7/src/pkg_eladpt/__init__.py
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      111 2023-07-06 10:42:48.000000 example_package_eladpt-0.0.7/src/pkg_eladpt/run.py
```

