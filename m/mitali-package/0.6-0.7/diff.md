# Comparing `tmp/mitali_package-0.6.tar.gz` & `tmp/mitali_package-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitali_package-0.6.tar", last modified: Thu Jul  6 20:09:35 2023, max compression
+gzip compressed data, was "mitali_package-0.7.tar", last modified: Thu Jul  6 20:13:38 2023, max compression
```

## Comparing `mitali_package-0.6.tar` & `mitali_package-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:09:35.436420 mitali_package-0.6/
--rw-r--r--   0 mitalibo   (504) staff       (20)      212 2023-07-06 20:09:35.436643 mitali_package-0.6/PKG-INFO
--rw-rw-r--   0 mitalibo   (504) staff       (20)      362 2023-07-06 20:01:28.000000 mitali_package-0.6/README.rst
--rw-rw-r--   0 mitalibo   (504) staff       (20)      107 2023-07-06 20:09:35.437685 mitali_package-0.6/setup.cfg
--rw-rw-r--   0 mitalibo   (504) staff       (20)      340 2023-07-06 20:09:24.000000 mitali_package-0.6/setup.py
-drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:09:35.429134 mitali_package-0.6/src/
-drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:09:35.431307 mitali_package-0.6/src/example_publish_pypi_medium/
--rw-rw-r--   0 mitalibo   (504) staff       (20)        0 2022-01-08 23:56:05.000000 mitali_package-0.6/src/example_publish_pypi_medium/__init__.py
-drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:09:35.432230 mitali_package-0.6/src/example_publish_pypi_medium/example/
--rw-rw-r--   0 mitalibo   (504) staff       (20)        0 2022-01-08 23:56:05.000000 mitali_package-0.6/src/example_publish_pypi_medium/example/__init__.py
--rw-rw-r--   0 mitalibo   (504) staff       (20)       75 2022-01-08 23:56:05.000000 mitali_package-0.6/src/example_publish_pypi_medium/example/custom_sklearn.py
-drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:09:35.435725 mitali_package-0.6/src/mitali_package.egg-info/
--rw-r--r--   0 mitalibo   (504) staff       (20)      212 2023-07-06 20:09:35.000000 mitali_package-0.6/src/mitali_package.egg-info/PKG-INFO
--rw-r--r--   0 mitalibo   (504) staff       (20)      392 2023-07-06 20:09:35.000000 mitali_package-0.6/src/mitali_package.egg-info/SOURCES.txt
--rw-r--r--   0 mitalibo   (504) staff       (20)        1 2023-07-06 20:09:35.000000 mitali_package-0.6/src/mitali_package.egg-info/dependency_links.txt
--rw-r--r--   0 mitalibo   (504) staff       (20)       13 2023-07-06 20:09:35.000000 mitali_package-0.6/src/mitali_package.egg-info/requires.txt
--rw-r--r--   0 mitalibo   (504) staff       (20)       28 2023-07-06 20:09:35.000000 mitali_package-0.6/src/mitali_package.egg-info/top_level.txt
+drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:13:38.775808 mitali_package-0.7/
+-rw-r--r--   0 mitalibo   (504) staff       (20)      212 2023-07-06 20:13:38.776119 mitali_package-0.7/PKG-INFO
+-rw-rw-r--   0 mitalibo   (504) staff       (20)      362 2023-07-06 20:01:28.000000 mitali_package-0.7/README.rst
+-rw-rw-r--   0 mitalibo   (504) staff       (20)      107 2023-07-06 20:13:38.777308 mitali_package-0.7/setup.cfg
+-rw-rw-r--   0 mitalibo   (504) staff       (20)      340 2023-07-06 20:13:35.000000 mitali_package-0.7/setup.py
+drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:13:38.766120 mitali_package-0.7/src/
+drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:13:38.769339 mitali_package-0.7/src/example_publish_pypi_medium/
+-rw-rw-r--   0 mitalibo   (504) staff       (20)        0 2022-01-08 23:56:05.000000 mitali_package-0.7/src/example_publish_pypi_medium/__init__.py
+drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:13:38.770133 mitali_package-0.7/src/example_publish_pypi_medium/example/
+-rw-rw-r--   0 mitalibo   (504) staff       (20)        0 2022-01-08 23:56:05.000000 mitali_package-0.7/src/example_publish_pypi_medium/example/__init__.py
+-rw-rw-r--   0 mitalibo   (504) staff       (20)       75 2022-01-08 23:56:05.000000 mitali_package-0.7/src/example_publish_pypi_medium/example/custom_sklearn.py
+drwxr-xr-x   0 mitalibo   (504) staff       (20)        0 2023-07-06 20:13:38.774657 mitali_package-0.7/src/mitali_package.egg-info/
+-rw-r--r--   0 mitalibo   (504) staff       (20)      212 2023-07-06 20:13:38.000000 mitali_package-0.7/src/mitali_package.egg-info/PKG-INFO
+-rw-r--r--   0 mitalibo   (504) staff       (20)      392 2023-07-06 20:13:38.000000 mitali_package-0.7/src/mitali_package.egg-info/SOURCES.txt
+-rw-r--r--   0 mitalibo   (504) staff       (20)        1 2023-07-06 20:13:38.000000 mitali_package-0.7/src/mitali_package.egg-info/dependency_links.txt
+-rw-r--r--   0 mitalibo   (504) staff       (20)       13 2023-07-06 20:13:38.000000 mitali_package-0.7/src/mitali_package.egg-info/requires.txt
+-rw-r--r--   0 mitalibo   (504) staff       (20)       28 2023-07-06 20:13:38.000000 mitali_package-0.7/src/mitali_package.egg-info/top_level.txt
```

