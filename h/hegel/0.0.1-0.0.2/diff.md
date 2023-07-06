# Comparing `tmp/hegel-0.0.1.tar.gz` & `tmp/hegel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hegel-0.0.1.tar", last modified: Fri Jun 16 20:23:02 2023, max compression
+gzip compressed data, was "hegel-0.0.2.tar", last modified: Thu Jul  6 15:23:00 2023, max compression
```

## Comparing `hegel-0.0.1.tar` & `hegel-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,21 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-06-16 20:23:02.316547 hegel-0.0.1/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     1056 2023-06-16 20:22:25.000000 hegel-0.0.1/LICENSE
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      506 2023-06-16 20:23:02.316337 hegel-0.0.1/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-06-16 20:22:25.000000 hegel-0.0.1/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-06-16 20:23:02.316073 hegel-0.0.1/hegel.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      506 2023-06-16 20:23:02.000000 hegel-0.0.1/hegel.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      148 2023-06-16 20:23:02.000000 hegel-0.0.1/hegel.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-06-16 20:23:02.000000 hegel-0.0.1/hegel.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-06-16 20:23:02.000000 hegel-0.0.1/hegel.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      571 2023-06-16 20:22:25.000000 hegel-0.0.1/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-06-16 20:23:02.316609 hegel-0.0.1/setup.cfg
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.496710 hegel-0.0.2/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:52:07.000000 hegel-0.0.2/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:23:00.496337 hegel-0.0.2/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2288 2023-07-05 23:53:02.000000 hegel-0.0.2/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.494056 hegel-0.0.2/hegel/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 00:08:03.000000 hegel-0.0.2/hegel/__init__.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     9418 2023-07-05 23:53:02.000000 hegel-0.0.2/hegel/scribe.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      796 2023-07-05 23:53:02.000000 hegel-0.0.2/hegel/utils.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       89 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel/version.py
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 15:23:00.495869 hegel-0.0.2/hegel.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2865 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      308 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-05 21:38:27.000000 hegel-0.0.2/hegel.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       22 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        6 2023-07-06 15:23:00.000000 hegel-0.0.2/hegel.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      684 2023-07-06 15:22:37.000000 hegel-0.0.2/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       13 2023-07-05 21:37:08.000000 hegel-0.0.2/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 15:23:00.496807 hegel-0.0.2/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3635 2023-07-05 21:38:08.000000 hegel-0.0.2/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 00:10:46.000000 hegel-0.0.2/version.txt
```

