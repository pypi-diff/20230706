# Comparing `tmp/pyams_scheduler-1.9.0.tar.gz` & `tmp/pyams_scheduler-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyams_scheduler-1.9.0.tar", last modified: Tue Aug  2 15:23:04 2022, max compression
+gzip compressed data, was "dist/pyams_scheduler-1.9.1.tar", last modified: Fri Sep 30 22:26:02 2022, max compression
```

## Comparing `pyams_scheduler-1.9.0.tar` & `pyams_scheduler-1.9.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)      104 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6032 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/docs/
--rwxrwxrwx   0 root         (0) root         (0)     2731 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/docs/HISTORY.txt
--rw-rw-rw-   0 root         (0) root         (0)     1428 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/docs/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2902 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      860 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/doctests/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/doctests/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/generations/
--rw-rw-rw-   0 root         (0) root         (0)     2020 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/generations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/include.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)     5537 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/
--rw-rw-rw-   0 root         (0) root         (0)    12577 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     3507 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)     8391 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    25989 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo
--rw-rw-rw-   0 root         (0) root         (0)    40878 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po
--rw-rw-rw-   0 root         (0) root         (0)    26573 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/locales/pyams_scheduler.pot
--rw-rw-rw-   0 root         (0) root         (0)    11184 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/process.py
--rw-rw-rw-   0 root         (0) root         (0)     4384 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/
--rw-rw-rw-   0 root         (0) root         (0)    20946 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/
--rw-rw-rw-   0 root         (0) root         (0)     2087 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5777 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/ftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/local.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     5539 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     9189 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     6281 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)    11984 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     8205 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10812 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     8750 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     4576 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/ssh.py
--rw-rw-rw-   0 root         (0) root         (0)     6260 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/tests/
--rw-rw-rw-   0 root         (0) root         (0)      804 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/tests/test_utilsdocs.py
--rw-rw-rw-   0 root         (0) root         (0)     1870 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/tests/test_utilsdocstrings.py
--rw-rw-rw-   0 root         (0) root         (0)     7580 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/
--rw-rw-rw-   0 root         (0) root         (0)     6265 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8067 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     3735 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/templates/
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/templates/directory-host-display.pt
--rw-rw-rw-   0 root         (0) root         (0)      725 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/templates/directory-host-input.pt
--rw-rw-rw-   0 root         (0) root         (0)    10091 2022-08-02 15:22:40.000000 pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6032 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2046 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      372 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-08-02 15:23:04.000000 pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6112 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/PKG-INFO
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2779 2022-09-30 22:21:12.000000 pyams_scheduler-1.9.1/docs/HISTORY.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/docs/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2912 2022-09-30 22:21:12.000000 pyams_scheduler-1.9.1/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/__init__.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/doctests/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/doctests/README.rst
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/generations/
+-rw-rw-rw-   0 root         (0) root         (0)     2020 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/generations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6521 2022-04-17 07:16:32.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/include.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)     5537 2021-10-16 12:41:38.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/__init__.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/
+-rw-rw-rw-   0 root         (0) root         (0)    12577 2022-08-02 15:26:14.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2022-05-17 07:35:22.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3507 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)     8391 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/sync.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    25989 2022-08-02 15:26:14.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo
+-rw-rw-rw-   0 root         (0) root         (0)    40878 2022-08-02 15:26:14.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po
+-rw-rw-rw-   0 root         (0) root         (0)    26573 2022-05-17 07:35:22.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/locales/pyams_scheduler.pot
+-rw-rw-rw-   0 root         (0) root         (0)    11184 2022-03-01 17:19:59.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     4384 2021-10-16 12:41:38.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/scheduler.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/
+-rw-rw-rw-   0 root         (0) root         (0)    20946 2022-08-02 15:26:14.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/__init__.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5777 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5539 2021-07-13 16:02:31.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     9274 2022-09-30 22:21:12.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6355 2022-09-30 22:21:12.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)    12058 2022-09-30 22:21:12.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/sync.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     8205 2021-10-01 22:59:55.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10812 2022-04-17 07:16:32.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8750 2022-05-17 07:35:22.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2021-07-31 22:05:06.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/ssh.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2021-07-31 22:05:06.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/sync.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/tests/test_utilsdocs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/tests/test_utilsdocstrings.py
+-rw-rw-rw-   0 root         (0) root         (0)     7580 2022-02-18 20:10:53.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/trigger.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/
+-rw-rw-rw-   0 root         (0) root         (0)     6265 2021-10-01 22:59:55.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8067 2021-09-12 11:05:34.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3735 2021-10-16 12:41:38.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/scheduler.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      598 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/templates/directory-host-display.pt
+-rw-rw-rw-   0 root         (0) root         (0)      725 2021-05-31 20:20:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/templates/directory-host-input.pt
+-rw-rw-rw-   0 root         (0) root         (0)    10091 2021-07-31 22:05:06.000000 pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/trigger.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6112 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2046 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      380 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2022-09-30 22:26:02.000000 pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/top_level.txt
```

### Comparing `pyams_scheduler-1.9.0/PKG-INFO` & `pyams_scheduler-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams_scheduler
-Version: 1.9.0
+Version: 1.9.1
 Summary: PyAMS tasks scheduler
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: =======================
         PyAMS scheduler package
@@ -41,14 +41,18 @@
         
         The package relies on ZeroMQ for process synchronisation, and APScheduler for tasks scheduling.
         
         
         Changelog
         =========
         
+        1.9.1
+        -----
+         - use new PyAMS_security constant
+        
         1.9.0
         -----
          - added new status to be used on task execution failure
          - added new task status class mapping
         
         1.8.0
         -----
```

### Comparing `pyams_scheduler-1.9.0/docs/HISTORY.txt` & `pyams_scheduler-1.9.1/docs/HISTORY.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+1.9.1
+-----
+ - use new PyAMS_security constant
+
 1.9.0
 -----
  - added new status to be used on task execution failure
  - added new task status class mapping
 
 1.8.0
 -----
```

### Comparing `pyams_scheduler-1.9.0/docs/README.txt` & `pyams_scheduler-1.9.1/docs/README.txt`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/setup.py` & `pyams_scheduler-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 DOCS = os.path.join(os.path.dirname(__file__),
                     'docs')
 
 README = os.path.join(DOCS, 'README.txt')
 HISTORY = os.path.join(DOCS, 'HISTORY.txt')
 
-version = '1.9.0'
+version = '1.9.1'
 long_description = open(README).read() + '\n\n' + open(HISTORY).read()
 
 tests_require = [
     'pyams_zmi',
     'pyramid_zcml',
     'zope.exceptions'
 ]
@@ -64,15 +64,15 @@
           # -*- Extra requirements: -*-
           'apscheduler',
           'chardet',
           'paramiko',
           'persistent',
           'pyams_layer',
           'pyams_mail',
-          'pyams_security',
+          'pyams_security >= 1.10.5',
           'pyams_site',
           'pyams_utils',
           'pyams_zmq',
           'pyramid',
           'pyramid_mailer',
           'requests',
           'transaction',
```

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/doctests/README.rst` & `pyams_scheduler-1.9.1/src/pyams_scheduler/doctests/README.rst`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/generations/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/generations/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/include.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/include.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/rest.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/ssh.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/ssh.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/interfaces/task/sync.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/interfaces/task/sync.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo` & `pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.mo`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po` & `pyams_scheduler-1.9.1/src/pyams_scheduler/locales/fr/LC_MESSAGES/pyams_scheduler.po`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/locales/pyams_scheduler.pot` & `pyams_scheduler-1.9.1/src/pyams_scheduler/locales/pyams_scheduler.pot`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/process.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/process.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/scheduler.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/ftp.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/ftp.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/local.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/local.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/handler/sftp.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/handler/sftp.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/notification.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/rest.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import requests
 from requests import ConnectionError
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_scheduler.interfaces.task import TASK_STATUS_ERROR, TASK_STATUS_FAIL, TASK_STATUS_OK
 from pyams_scheduler.interfaces.task.rest import IRESTCallerTask
 from pyams_scheduler.task import Task
+from pyams_security.interfaces.names import UNCHANGED_PASSWORD
 from pyams_utils.dict import format_dict
 from pyams_utils.factory import factory_config
 from pyams_utils.html import html_to_text
 
 
 __docformat__ = 'restructuredtext'
 
@@ -74,27 +75,27 @@
     def password(self):
         """Password getter"""
         return self._password
 
     @password.setter
     def password(self, value):
         """Password setter"""
-        if value == '*****':
+        if value == UNCHANGED_PASSWORD:
             return
         self._password = value
 
     @property
     def proxy_password(self):
         """Proxy password getter"""
         return self._proxy_password
 
     @proxy_password.setter
     def proxy_password(self, value):
         """Proxy password setter"""
-        if value == '*****':
+        if value == UNCHANGED_PASSWORD:
             return
         self._proxy_password = value
 
     @property
     def ok_status_list(self):
         """OK status list getter"""
         return map(int, self.ok_status.split(','))
```

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/ssh.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from paramiko import AutoAddPolicy, SSHClient, SSHException
 from persistent import Persistent
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_scheduler.interfaces.task import TASK_STATUS_FAIL, TASK_STATUS_OK
 from pyams_scheduler.interfaces.task.ssh import ISSHCallerTask, ISSHConnectionInfo
 from pyams_scheduler.task import Task
+from pyams_security.interfaces.names import UNCHANGED_PASSWORD
 from pyams_utils.factory import factory_config
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_scheduler import _  # pylint: disable=ungrouped-imports
 
@@ -64,15 +65,15 @@
     def password(self):
         """Password getter"""
         return self._password
 
     @password.setter
     def password(self, value):
         """Password setter"""
-        if value == '*****':
+        if value == UNCHANGED_PASSWORD:
             return
         self._password = value
 
     @contextmanager
     def get_connection(self):
         """Open SSH connection"""
         ssh = SSHClient()
```

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/sync.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from zope.schema.fieldproperty import FieldProperty
 
 from pyams_scheduler.interfaces.task import TASK_STATUS_EMPTY, TASK_STATUS_ERROR, \
     TASK_STATUS_FAIL, TASK_STATUS_OK
 from pyams_scheduler.interfaces.task.sync import DirectorySyncError, IDirectoryHandler, \
     IDirectoryInfo, IDirectorySyncTask
 from pyams_scheduler.task import Task
+from pyams_security.interfaces.names import UNCHANGED_PASSWORD
 from pyams_utils.factory import factory_config
 from pyams_utils.size import get_human_size
 
 
 __docformat__ = 'restructuredtext'
 
 from pyams_scheduler import _  # pylint: disable=ungrouped-imports
@@ -72,15 +73,15 @@
     def password(self):
         """Password getter"""
         return self._password
 
     @password.setter
     def password(self, value):
         """Password setter"""
-        if value == '*****':
+        if value == UNCHANGED_PASSWORD:
             return
         self._password = value
 
     @contextmanager
     def get_handler(self):
         """Get protocol handler"""
         protocol, _hostname = self.host or (None, None)
```

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/notification.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/notification.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/rest.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/rest.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/ssh.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/ssh.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/task/zmi/sync.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/task/zmi/sync.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/tests/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/tests/test_utilsdocs.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/tests/test_utilsdocs.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/tests/test_utilsdocstrings.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/tests/test_utilsdocstrings.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/trigger.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/trigger.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/__init__.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/history.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/history.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/interfaces.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/interfaces.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/jobs.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/jobs.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/scheduler.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/scheduler.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/templates/directory-host-display.pt` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/templates/directory-host-display.pt`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/templates/directory-host-input.pt` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/templates/directory-host-input.pt`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler/zmi/trigger.py` & `pyams_scheduler-1.9.1/src/pyams_scheduler/zmi/trigger.py`

 * *Files identical despite different names*

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/PKG-INFO` & `pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyams-scheduler
-Version: 1.9.0
+Version: 1.9.1
 Summary: PyAMS tasks scheduler
 Home-page: https://pyams.readthedocs.io
 Author: Thierry Florac
 Author-email: tflorac@ulthar.net
 License: ZPL
 Description: =======================
         PyAMS scheduler package
@@ -41,14 +41,18 @@
         
         The package relies on ZeroMQ for process synchronisation, and APScheduler for tasks scheduling.
         
         
         Changelog
         =========
         
+        1.9.1
+        -----
+         - use new PyAMS_security constant
+        
         1.9.0
         -----
          - added new status to be used on task execution failure
          - added new task status class mapping
         
         1.8.0
         -----
```

### Comparing `pyams_scheduler-1.9.0/src/pyams_scheduler.egg-info/SOURCES.txt` & `pyams_scheduler-1.9.1/src/pyams_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

