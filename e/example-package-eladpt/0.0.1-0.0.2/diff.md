# Comparing `tmp/example_package_eladpt-0.0.1.tar.gz` & `tmp/example_package_eladpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_eladpt-0.0.1.tar", last modified: Thu Jul  6 09:24:05 2023, max compression
+gzip compressed data, was "example_package_eladpt-0.0.2.tar", last modified: Thu Jul  6 10:40:51 2023, max compression
```

## Comparing `example_package_eladpt-0.0.1.tar` & `example_package_eladpt-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:24:05.319823 example_package_eladpt-0.0.1/
--rw-r--r--   0 elad.pticha   (502) staff       (20)      414 2023-07-06 09:24:05.319649 example_package_eladpt-0.0.1/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 09:14:29.000000 example_package_eladpt-0.0.1/README.md
--rw-r--r--   0 elad.pticha   (502) staff       (20)      416 2023-07-06 09:14:30.000000 example_package_eladpt-0.0.1/pyproject.toml
--rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 09:24:05.319880 example_package_eladpt-0.0.1/setup.cfg
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:24:05.317980 example_package_eladpt-0.0.1/src/
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:24:05.318871 example_package_eladpt-0.0.1/src/example_package_eladpt.egg-info/
--rw-r--r--   0 elad.pticha   (502) staff       (20)      414 2023-07-06 09:24:05.000000 example_package_eladpt-0.0.1/src/example_package_eladpt.egg-info/PKG-INFO
--rw-r--r--   0 elad.pticha   (502) staff       (20)      273 2023-07-06 09:24:05.000000 example_package_eladpt-0.0.1/src/example_package_eladpt.egg-info/SOURCES.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 09:24:05.000000 example_package_eladpt-0.0.1/src/example_package_eladpt.egg-info/dependency_links.txt
--rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 09:24:05.000000 example_package_eladpt-0.0.1/src/example_package_eladpt.egg-info/top_level.txt
-drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:24:05.319126 example_package_eladpt-0.0.1/src/pkg_eladpt/
--rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.1/src/pkg_eladpt/__init__.py
--rw-r--r--   0 elad.pticha   (502) staff       (20)       74 2023-07-06 09:10:33.000000 example_package_eladpt-0.0.1/src/pkg_eladpt/run.py
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:40:51.861980 example_package_eladpt-0.0.2/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:40:51.861845 example_package_eladpt-0.0.2/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       10 2023-07-06 09:14:29.000000 example_package_eladpt-0.0.2/README.md
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      403 2023-07-06 10:40:21.000000 example_package_eladpt-0.0.2/pyproject.toml
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       38 2023-07-06 10:40:51.862029 example_package_eladpt-0.0.2/setup.cfg
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:40:51.860160 example_package_eladpt-0.0.2/src/
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:40:51.861055 example_package_eladpt-0.0.2/src/example_package_eladpt.egg-info/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      401 2023-07-06 10:40:51.000000 example_package_eladpt-0.0.2/src/example_package_eladpt.egg-info/PKG-INFO
+-rw-r--r--   0 elad.pticha   (502) staff       (20)      273 2023-07-06 10:40:51.000000 example_package_eladpt-0.0.2/src/example_package_eladpt.egg-info/SOURCES.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        1 2023-07-06 10:40:51.000000 example_package_eladpt-0.0.2/src/example_package_eladpt.egg-info/dependency_links.txt
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       11 2023-07-06 10:40:51.000000 example_package_eladpt-0.0.2/src/example_package_eladpt.egg-info/top_level.txt
+drwxr-xr-x   0 elad.pticha   (502) staff       (20)        0 2023-07-06 10:40:51.861430 example_package_eladpt-0.0.2/src/pkg_eladpt/
+-rw-r--r--   0 elad.pticha   (502) staff       (20)        0 2023-07-06 09:08:33.000000 example_package_eladpt-0.0.2/src/pkg_eladpt/__init__.py
+-rw-r--r--   0 elad.pticha   (502) staff       (20)       74 2023-07-06 09:10:33.000000 example_package_eladpt-0.0.2/src/pkg_eladpt/run.py
```

