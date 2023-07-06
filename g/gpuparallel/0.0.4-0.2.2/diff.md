# Comparing `tmp/gpuparallel-0.0.4.tar.gz` & `tmp/gpuparallel-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpuparallel-0.0.4.tar", last modified: Mon May 10 13:13:47 2021, max compression
+gzip compressed data, was "gpuparallel-0.2.2.tar", last modified: Thu Jul  6 10:16:08 2023, max compression
```

## Comparing `gpuparallel-0.0.4.tar` & `gpuparallel-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 vlivashkin  (1000) vlivashkin  (1000)        0 2021-05-10 13:13:47.539560 gpuparallel-0.0.4/
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      274 2021-05-10 13:13:47.539560 gpuparallel-0.0.4/PKG-INFO
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)     2951 2021-05-10 12:56:57.000000 gpuparallel-0.0.4/README.md
-drwxrwxr-x   0 vlivashkin  (1000) vlivashkin  (1000)        0 2021-05-10 13:13:47.539560 gpuparallel-0.0.4/gpuparallel/
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      216 2021-05-10 09:05:57.000000 gpuparallel-0.0.4/gpuparallel/__init__.py
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)     4862 2021-05-10 09:34:47.000000 gpuparallel-0.0.4/gpuparallel/gpuparallel.py
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      575 2021-05-10 13:04:09.000000 gpuparallel-0.0.4/gpuparallel/utils.py
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)       22 2021-05-10 13:12:51.000000 gpuparallel-0.0.4/gpuparallel/version.py
-drwxrwxr-x   0 vlivashkin  (1000) vlivashkin  (1000)        0 2021-05-10 13:13:47.539560 gpuparallel-0.0.4/gpuparallel.egg-info/
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      274 2021-05-10 13:13:47.000000 gpuparallel-0.0.4/gpuparallel.egg-info/PKG-INFO
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      287 2021-05-10 13:13:47.000000 gpuparallel-0.0.4/gpuparallel.egg-info/SOURCES.txt
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)        1 2021-05-10 13:13:47.000000 gpuparallel-0.0.4/gpuparallel.egg-info/dependency_links.txt
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)        5 2021-05-10 13:13:47.000000 gpuparallel-0.0.4/gpuparallel.egg-info/requires.txt
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)       12 2021-05-10 13:13:47.000000 gpuparallel-0.0.4/gpuparallel.egg-info/top_level.txt
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)       38 2021-05-10 13:13:47.539560 gpuparallel-0.0.4/setup.cfg
--rw-rw-r--   0 vlivashkin  (1000) vlivashkin  (1000)      402 2021-03-31 14:15:10.000000 gpuparallel-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/gpuparallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/gpuparallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/gpuparallel/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/gpuparallel/gpuparallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/gpuparallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/gpuparallel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/gpuparallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-06 10:16:08.000000 gpuparallel-0.2.2/gpuparallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 10:16:08.000000 gpuparallel-0.2.2/gpuparallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 10:16:08.000000 gpuparallel-0.2.2/gpuparallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 10:16:08.000000 gpuparallel-0.2.2/gpuparallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 10:16:08.000000 gpuparallel-0.2.2/gpuparallel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 10:16:08.017604 gpuparallel-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/tests/tests_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-06 10:15:58.000000 gpuparallel-0.2.2/tests/tests_gpuparallel.py
```

