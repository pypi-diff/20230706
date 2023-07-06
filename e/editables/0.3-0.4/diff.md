# Comparing `tmp/editables-0.3.tar.gz` & `tmp/editables-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editables-0.3.tar", last modified: Sun Apr 10 15:33:58 2022, max compression
+gzip compressed data, was "editables-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `editables-0.3.tar` & `editables-0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-04-10 15:33:58.420775 editables-0.3/
--rw-rw-rw-   0        0        0     1072 2021-04-08 16:24:47.000000 editables-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3292 2022-04-10 15:33:58.421759 editables-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2022-04-09 15:49:08.000000 editables-0.3/README.md
--rw-rw-rw-   0        0        0       88 2022-04-09 15:13:03.000000 editables-0.3/pyproject.toml
--rw-rw-rw-   0        0        0     1591 2022-04-10 15:33:58.428794 editables-0.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-04-08 16:24:47.000000 editables-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-10 15:33:58.388758 editables-0.3/src/
-drwxrwxrwx   0        0        0        0 2022-04-10 15:33:58.400758 editables-0.3/src/editables/
--rw-rw-rw-   0        0        0     2727 2022-04-10 15:33:25.000000 editables-0.3/src/editables/__init__.py
--rw-rw-rw-   0        0        0      761 2021-06-12 11:40:39.000000 editables-0.3/src/editables/redirector.py
-drwxrwxrwx   0        0        0        0 2022-04-10 15:33:58.419757 editables-0.3/src/editables.egg-info/
--rw-rw-rw-   0        0        0     3292 2022-04-10 15:33:57.000000 editables-0.3/src/editables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-04-10 15:33:58.000000 editables-0.3/src/editables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-10 15:33:58.000000 editables-0.3/src/editables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-04-10 15:33:58.000000 editables-0.3/src/editables.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2021-04-08 16:24:47.187184 editables-0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1996 2022-04-09 15:49:08.690254 editables-0.4/README.md
+-rw-r--r--   0        0        0      658 2022-04-09 15:49:08.691217 editables-0.4/docs/Makefile
+-rwxr-xr-x   0        0        0      799 2022-04-09 15:49:08.692220 editables-0.4/docs/make.bat
+-rw-r--r--   0        0        0       27 2022-04-09 15:49:08.692220 editables-0.4/docs/requirements.txt
+-rw-r--r--   0        0        0     1957 2023-07-06 14:58:12.743793 editables-0.4/docs/source/conf.py
+-rw-r--r--   0        0        0     6485 2023-06-29 15:09:33.531062 editables-0.4/docs/source/implementation.md
+-rw-r--r--   0        0        0      427 2023-07-06 14:57:18.057853 editables-0.4/docs/source/index.md
+-rw-r--r--   0        0        0     4707 2023-07-06 14:57:18.106888 editables-0.4/docs/source/usage.md
+-rw-r--r--   0        0        0     5962 2023-07-06 14:57:18.111892 editables-0.4/docs/source/use-cases.md
+-rw-r--r--   0        0        0     1304 2023-07-06 14:58:12.742811 editables-0.4/pyproject.toml
+-rw-r--r--   0        0        0     3645 2023-07-06 14:58:12.742811 editables-0.4/src/editables/__init__.py
+-rw-r--r--   0        0        0     1122 2023-06-28 16:25:44.327179 editables-0.4/src/editables/redirector.py
+-rw-r--r--   0        0        0       76 2023-06-28 12:32:00.757014 editables-0.4/tests/requirements.txt
+-rw-r--r--   0        0        0     5070 2023-06-29 15:09:33.532063 editables-0.4/tests/test_editable.py
+-rw-r--r--   0        0        0     2130 2021-06-12 11:40:39.885457 editables-0.4/tests/test_redirects.py
+-rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 editables-0.4/PKG-INFO
```

### Comparing `editables-0.3/LICENSE.txt` & `editables-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `editables-0.3/README.md` & `editables-0.4/README.md`

 * *Files identical despite different names*

