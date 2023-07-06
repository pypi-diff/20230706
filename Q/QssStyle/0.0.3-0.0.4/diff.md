# Comparing `tmp/QssStyle-0.0.3.tar.gz` & `tmp/QssStyle-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QssStyle-0.0.3.tar", last modified: Thu Jul  6 07:45:53 2023, max compression
+gzip compressed data, was "QssStyle-0.0.4.tar", last modified: Thu Jul  6 08:04:41 2023, max compression
```

## Comparing `QssStyle-0.0.3.tar` & `QssStyle-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 07:45:53.039013 QssStyle-0.0.3/
--rw-rw-rw-   0        0        0       55 2023-07-06 07:45:53.039013 QssStyle-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 07:45:53.037021 QssStyle-0.0.3/QssStyle/
--rw-rw-rw-   0        0        0       20 2023-07-06 07:21:58.000000 QssStyle-0.0.3/QssStyle/__init__.py
--rw-rw-rw-   0        0        0       16 2023-07-06 07:21:57.000000 QssStyle-0.0.3/QssStyle/main.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:45:53.039013 QssStyle-0.0.3/QssStyle.egg-info/
--rw-rw-rw-   0        0        0       55 2023-07-06 07:45:53.000000 QssStyle-0.0.3/QssStyle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-07-06 07:45:53.000000 QssStyle-0.0.3/QssStyle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 07:45:53.000000 QssStyle-0.0.3/QssStyle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 07:45:53.000000 QssStyle-0.0.3/QssStyle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-07-06 07:44:34.000000 QssStyle-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       90 2023-07-06 07:45:53.040011 QssStyle-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       85 2023-07-06 07:44:34.000000 QssStyle-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:04:41.114963 QssStyle-0.0.4/
+-rw-rw-rw-   0        0        0       55 2023-07-06 08:04:41.114963 QssStyle-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 08:04:41.111972 QssStyle-0.0.4/QssStyle/
+-rw-rw-rw-   0        0        0       57 2023-07-06 08:03:37.000000 QssStyle-0.0.4/QssStyle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:04:41.114963 QssStyle-0.0.4/QssStyle/core/
+-rw-rw-rw-   0        0        0       33 2023-07-06 07:56:29.000000 QssStyle-0.0.4/QssStyle/core/main.py
+drwxrwxrwx   0        0        0        0 2023-07-06 08:04:41.113966 QssStyle-0.0.4/QssStyle.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-07-06 08:04:41.000000 QssStyle-0.0.4/QssStyle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-06 08:04:41.000000 QssStyle-0.0.4/QssStyle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 08:04:41.000000 QssStyle-0.0.4/QssStyle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 08:04:41.000000 QssStyle-0.0.4/QssStyle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2023-07-06 07:55:12.000000 QssStyle-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       90 2023-07-06 08:04:41.115960 QssStyle-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       85 2023-07-06 07:55:12.000000 QssStyle-0.0.4/setup.py
```

