# Comparing `tmp/prompttools-0.0.1.tar.gz` & `tmp/prompttools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompttools-0.0.1.tar", last modified: Sun Jun 25 19:35:38 2023, max compression
+gzip compressed data, was "prompttools-0.0.2.tar", last modified: Thu Jul  6 16:09:35 2023, max compression
```

## Comparing `prompttools-0.0.1.tar` & `prompttools-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-06-25 19:35:38.453330 prompttools-0.0.1/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      432 2023-06-25 19:35:38.453064 prompttools-0.0.1/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       13 2023-06-25 19:33:20.000000 prompttools-0.0.1/README.md
-drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-06-25 19:35:38.452735 prompttools-0.0.1/prompttools.egg-info/
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      432 2023-06-25 19:35:38.000000 prompttools-0.0.1/prompttools.egg-info/PKG-INFO
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      164 2023-06-25 19:35:38.000000 prompttools-0.0.1/prompttools.egg-info/SOURCES.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-06-25 19:35:38.000000 prompttools-0.0.1/prompttools.egg-info/dependency_links.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-06-25 19:35:38.000000 prompttools-0.0.1/prompttools.egg-info/top_level.txt
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      519 2023-06-25 19:34:43.000000 prompttools-0.0.1/pyproject.toml
--rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-06-25 19:35:38.453405 prompttools-0.0.1/setup.cfg
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 16:09:35.248520 prompttools-0.0.2/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     2102 2023-07-05 23:51:56.000000 prompttools-0.0.2/LICENSE
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 16:09:35.248231 prompttools-0.0.2/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     4508 2023-07-05 23:52:26.000000 prompttools-0.0.2/README.md
+drwxr-xr-x   0 stevenkrawczyk   (501) staff       (20)        0 2023-07-06 16:09:35.247830 prompttools-0.0.2/prompttools.egg-info/
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     5109 2023-07-06 16:09:35.000000 prompttools-0.0.2/prompttools.egg-info/PKG-INFO
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      278 2023-07-06 16:09:35.000000 prompttools-0.0.2/prompttools.egg-info/SOURCES.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 16:09:35.000000 prompttools-0.0.2/prompttools.egg-info/dependency_links.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-04 19:41:18.000000 prompttools-0.0.2/prompttools.egg-info/not-zip-safe
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-06 16:09:35.000000 prompttools-0.0.2/prompttools.egg-info/requires.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        1 2023-07-06 16:09:35.000000 prompttools-0.0.2/prompttools.egg-info/top_level.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)      698 2023-07-06 16:00:08.000000 prompttools-0.0.2/pyproject.toml
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       98 2023-07-05 21:42:59.000000 prompttools-0.0.2/requirements.txt
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)       38 2023-07-06 16:09:35.248598 prompttools-0.0.2/setup.cfg
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)     3671 2023-07-06 16:09:27.000000 prompttools-0.0.2/setup.py
+-rw-r--r--   0 stevenkrawczyk   (501) staff       (20)        8 2023-07-06 15:50:11.000000 prompttools-0.0.2/version.txt
```

