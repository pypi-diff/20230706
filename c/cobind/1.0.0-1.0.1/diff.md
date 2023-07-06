# Comparing `tmp/cobind-1.0.0.tar.gz` & `tmp/cobind-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cobind-1.0.0.tar", last modified: Sat Jan 22 16:58:58 2022, max compression
+gzip compressed data, was "cobind-1.0.1.tar", last modified: Thu Jul  6 19:24:39 2023, max compression
```

## Comparing `cobind-1.0.0.tar` & `cobind-1.0.1.tar`

### file list

```diff
@@ -1,94 +1,104 @@
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.857097 cobind-1.0.0/
--rw-r--r--   0 m102324  (1381454652) 1387956079       66 2021-12-04 04:26:53.000000 cobind-1.0.0/.gitattributes
--rw-r--r--   0 m102324  (1381454652) 1387956079       95 2021-12-30 16:40:07.000000 cobind-1.0.0/.gitignore
--rw-r--r--   0 m102324  (1381454652) 1387956079     1067 2021-12-04 04:26:53.000000 cobind-1.0.0/LICENSE
--rw-r--r--   0 m102324  (1381454652) 1387956079      791 2022-01-22 16:58:58.856695 cobind-1.0.0/PKG-INFO
--rw-r--r--   0 m102324  (1381454652) 1387956079      694 2022-01-21 19:01:19.000000 cobind-1.0.0/README.md
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.354879 cobind-1.0.0/bin/
--rwxr-xr-x   0 m102324  (1381454652) 1387956079    23341 2022-01-20 20:50:21.000000 cobind-1.0.0/bin/cobind.py
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.450743 cobind-1.0.0/docs/
--rw-r--r--   0 m102324  (1381454652) 1387956079      634 2021-12-24 02:46:48.000000 cobind-1.0.0/docs/Makefile
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.602552 cobind-1.0.0/docs/_static/
--rw-r--r--   0 m102324  (1381454652) 1387956079    75232 2022-01-10 16:31:33.000000 cobind-1.0.0/docs/_static/SD_1.jpeg
--rw-r--r--   0 m102324  (1381454652) 1387956079    32695 2022-01-11 17:53:53.000000 cobind-1.0.0/docs/_static/SD_1.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    48476 2022-01-06 23:30:24.000000 cobind-1.0.0/docs/_static/SD_1.png
--rw-r--r--   0 m102324  (1381454652) 1387956079    17885 2022-01-10 16:31:47.000000 cobind-1.0.0/docs/_static/SD_2.jpeg
--rw-r--r--   0 m102324  (1381454652) 1387956079    19172 2022-01-11 18:01:29.000000 cobind-1.0.0/docs/_static/SD_2.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    15398 2022-01-06 23:37:14.000000 cobind-1.0.0/docs/_static/SD_2.png
--rw-r--r--   0 m102324  (1381454652) 1387956079    37570 2022-01-12 16:04:52.000000 cobind-1.0.0/docs/_static/SS.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    18516 2022-01-12 16:05:08.000000 cobind-1.0.0/docs/_static/SS_bound.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    23684 2022-01-20 20:36:04.000000 cobind-1.0.0/docs/_static/fisher_or.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    57934 2022-01-20 20:35:48.000000 cobind-1.0.0/docs/_static/fisher_p.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    52430 2022-01-11 17:45:50.000000 cobind-1.0.0/docs/_static/jaccard_1.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    16523 2022-01-11 17:47:16.000000 cobind-1.0.0/docs/_static/jaccard_2.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    51728 2022-01-11 17:46:04.000000 cobind-1.0.0/docs/_static/jaccard_3.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    11027 2021-12-25 03:28:11.000000 cobind-1.0.0/docs/_static/logo.png
--rw-r--r--   0 m102324  (1381454652) 1387956079   162318 2022-01-15 04:16:22.000000 cobind-1.0.0/docs/_static/npmi.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    23653 2022-01-11 19:59:06.000000 cobind-1.0.0/docs/_static/npmi_bound.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    29527 2022-01-11 17:10:35.000000 cobind-1.0.0/docs/_static/ov_coef_1.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079   139109 2022-01-11 17:20:35.000000 cobind-1.0.0/docs/_static/ov_coef_2.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    18092 2022-01-10 16:30:23.000000 cobind-1.0.0/docs/_static/ov_coef_3.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    46282 2022-01-11 20:03:44.000000 cobind-1.0.0/docs/_static/p.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    54577 2022-01-11 19:58:22.000000 cobind-1.0.0/docs/_static/pmi.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079    59235 2022-01-11 19:58:38.000000 cobind-1.0.0/docs/_static/pmi_bound.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079   227900 2022-01-11 16:44:02.000000 cobind-1.0.0/docs/_static/set_symbols.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079   382922 2022-01-11 17:11:56.000000 cobind-1.0.0/docs/_static/srog.jpg
--rw-r--r--   0 m102324  (1381454652) 1387956079       88 2021-12-24 04:10:05.000000 cobind-1.0.0/docs/change_log.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     8448 2021-12-29 04:23:37.000000 cobind-1.0.0/docs/conf.py
--rw-r--r--   0 m102324  (1381454652) 1387956079     3884 2022-01-21 20:23:19.000000 cobind-1.0.0/docs/dataset.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     7293 2022-01-22 03:36:20.000000 cobind-1.0.0/docs/definition.rst
--rwxr-xr-x   0 m102324  (1381454652) 1387956079      818 2022-01-22 04:05:49.000000 cobind-1.0.0/docs/index.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     1898 2022-01-22 03:40:15.000000 cobind-1.0.0/docs/input_format.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     1477 2022-01-22 03:38:01.000000 cobind-1.0.0/docs/installation.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     2522 2022-01-22 03:30:23.000000 cobind-1.0.0/docs/introduction.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     1083 2021-12-23 23:06:14.000000 cobind-1.0.0/docs/license.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079      795 2021-12-24 02:46:48.000000 cobind-1.0.0/docs/make.bat
--rw-r--r--   0 m102324  (1381454652) 1387956079      105 2021-12-23 23:12:27.000000 cobind-1.0.0/docs/reference.rst
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.681635 cobind-1.0.0/docs/usage/
--rw-r--r--   0 m102324  (1381454652) 1387956079     5522 2022-01-20 16:26:10.000000 cobind-1.0.0/docs/usage/NPMI.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     5720 2022-01-20 16:25:23.000000 cobind-1.0.0/docs/usage/PMI.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     5602 2022-01-20 16:25:03.000000 cobind-1.0.0/docs/usage/SD.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     3088 2022-01-21 03:12:41.000000 cobind-1.0.0/docs/usage/SROG.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     5588 2022-01-20 16:24:39.000000 cobind-1.0.0/docs/usage/SS.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     2507 2022-01-22 04:07:37.000000 cobind-1.0.0/docs/usage/cobind.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     4682 2022-01-21 19:38:15.000000 cobind-1.0.0/docs/usage/cooccur.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     6241 2022-01-20 21:11:11.000000 cobind-1.0.0/docs/usage/covary.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     5438 2022-01-20 16:26:34.000000 cobind-1.0.0/docs/usage/jaccard.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     5494 2022-01-22 03:45:36.000000 cobind-1.0.0/docs/usage/overlap.rst
--rw-r--r--   0 m102324  (1381454652) 1387956079     3922 2022-01-21 19:40:06.000000 cobind-1.0.0/docs/usage/stat.rst
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.328835 cobind-1.0.0/lib/
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.690413 cobind-1.0.0/lib/cobind.egg-info/
--rw-r--r--   0 m102324  (1381454652) 1387956079      791 2022-01-22 16:58:57.000000 cobind-1.0.0/lib/cobind.egg-info/PKG-INFO
--rw-r--r--   0 m102324  (1381454652) 1387956079     2274 2022-01-22 16:58:57.000000 cobind-1.0.0/lib/cobind.egg-info/SOURCES.txt
--rw-r--r--   0 m102324  (1381454652) 1387956079        1 2022-01-22 16:58:57.000000 cobind-1.0.0/lib/cobind.egg-info/dependency_links.txt
--rw-r--r--   0 m102324  (1381454652) 1387956079        1 2021-11-04 21:30:55.000000 cobind-1.0.0/lib/cobind.egg-info/not-zip-safe
--rw-r--r--   0 m102324  (1381454652) 1387956079       38 2022-01-22 16:58:57.000000 cobind-1.0.0/lib/cobind.egg-info/requires.txt
--rw-r--r--   0 m102324  (1381454652) 1387956079       25 2022-01-22 16:58:57.000000 cobind-1.0.0/lib/cobind.egg-info/top_level.txt
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.773556 cobind-1.0.0/lib/cobindability/
--rwxr-xr-x   0 m102324  (1381454652) 1387956079    31577 2022-01-18 03:45:04.000000 cobind-1.0.0/lib/cobindability/BED.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2021-11-04 21:29:46.000000 cobind-1.0.0/lib/cobindability/__init__.py
-drwxr-xr-x   0 m102324  (1381454652) 1387956079        0 2022-01-22 16:58:58.856096 cobind-1.0.0/lib/cobindability/__pycache__/
--rw-r--r--   0 m102324  (1381454652) 1387956079    23979 2022-01-20 17:29:27.000000 cobind-1.0.0/lib/cobindability/__pycache__/BED.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079      160 2021-11-04 21:31:08.000000 cobind-1.0.0/lib/cobindability/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079      531 2021-11-04 20:14:20.000000 cobind-1.0.0/lib/cobindability/__pycache__/bbreader.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     3741 2022-01-12 17:49:57.000000 cobind-1.0.0/lib/cobindability/__pycache__/bw.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     4201 2022-01-16 03:53:06.000000 cobind-1.0.0/lib/cobindability/__pycache__/coefcal.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     1904 2022-01-12 17:49:57.000000 cobind-1.0.0/lib/cobindability/__pycache__/ireader.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     7453 2022-01-16 16:58:58.000000 cobind-1.0.0/lib/cobindability/__pycache__/ovbootstrap.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     5751 2022-01-12 20:26:04.000000 cobind-1.0.0/lib/cobindability/__pycache__/ovcoef.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     4576 2022-01-14 02:57:33.000000 cobind-1.0.0/lib/cobindability/__pycache__/ovjaccard.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     3324 2022-01-12 17:49:57.000000 cobind-1.0.0/lib/cobindability/__pycache__/ovpmi.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079     4428 2022-01-15 03:58:38.000000 cobind-1.0.0/lib/cobindability/__pycache__/ovstat.cpython-38.pyc
--rw-r--r--   0 m102324  (1381454652) 1387956079      175 2022-01-16 19:09:50.000000 cobind-1.0.0/lib/cobindability/__pycache__/version.cpython-38.pyc
--rwxr-xr-x   0 m102324  (1381454652) 1387956079      592 2022-01-12 15:53:55.000000 cobind-1.0.0/lib/cobindability/bbreader.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079      448 2021-11-04 20:13:41.000000 cobind-1.0.0/lib/cobindability/bbreader.py~
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     4267 2022-01-12 15:53:53.000000 cobind-1.0.0/lib/cobindability/bw.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     4069 2022-01-16 03:53:00.000000 cobind-1.0.0/lib/cobindability/coefcal.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     1219 2021-11-05 03:13:39.000000 cobind-1.0.0/lib/cobindability/findbed.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     1572 2022-01-12 15:53:54.000000 cobind-1.0.0/lib/cobindability/ireader.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     9343 2022-01-16 16:58:13.000000 cobind-1.0.0/lib/cobindability/ovbootstrap.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079      276 2021-12-12 02:06:32.000000 cobind-1.0.0/lib/cobindability/ovcovary.py
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     4963 2022-01-15 03:58:05.000000 cobind-1.0.0/lib/cobindability/ovstat.py
--rw-r--r--   0 m102324  (1381454652) 1387956079       18 2022-01-22 04:08:50.000000 cobind-1.0.0/lib/cobindability/version.py
--rw-r--r--   0 m102324  (1381454652) 1387956079       38 2022-01-22 16:58:58.857220 cobind-1.0.0/setup.cfg
--rwxr-xr-x   0 m102324  (1381454652) 1387956079     1724 2022-01-22 16:58:16.000000 cobind-1.0.0/setup.py
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:39.101531 cobind-1.0.1/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       66 2021-12-04 04:26:53.000000 cobind-1.0.1/.gitattributes
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       61 2023-07-05 22:16:36.000000 cobind-1.0.1/.gitignore
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1067 2021-12-04 04:26:53.000000 cobind-1.0.1/LICENSE
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      724 2023-07-06 19:24:39.100698 cobind-1.0.1/PKG-INFO
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      694 2022-01-21 19:01:19.000000 cobind-1.0.1/README.md
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:38.889051 cobind-1.0.1/bin/
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    35485 2023-07-06 19:14:15.000000 cobind-1.0.1/bin/cobind.py
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:38.905749 cobind-1.0.1/docs/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      634 2021-12-24 02:46:48.000000 cobind-1.0.1/docs/Makefile
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:38.969360 cobind-1.0.1/docs/_static/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    75232 2022-01-10 16:31:33.000000 cobind-1.0.1/docs/_static/SD_1.jpeg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    32695 2022-01-11 17:53:53.000000 cobind-1.0.1/docs/_static/SD_1.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    48476 2022-01-06 23:30:24.000000 cobind-1.0.1/docs/_static/SD_1.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    17885 2022-01-10 16:31:47.000000 cobind-1.0.1/docs/_static/SD_2.jpeg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    19172 2022-01-11 18:01:29.000000 cobind-1.0.1/docs/_static/SD_2.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    15398 2022-01-06 23:37:14.000000 cobind-1.0.1/docs/_static/SD_2.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    37570 2022-01-12 16:04:52.000000 cobind-1.0.1/docs/_static/SS.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    18516 2022-01-12 16:05:08.000000 cobind-1.0.1/docs/_static/SS_bound.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    23684 2022-01-20 20:36:04.000000 cobind-1.0.1/docs/_static/fisher_or.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    57934 2022-01-20 20:35:48.000000 cobind-1.0.1/docs/_static/fisher_p.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    52430 2022-01-11 17:45:50.000000 cobind-1.0.1/docs/_static/jaccard_1.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    16523 2022-01-11 17:47:16.000000 cobind-1.0.1/docs/_static/jaccard_2.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    51728 2022-01-11 17:46:04.000000 cobind-1.0.1/docs/_static/jaccard_3.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    11027 2022-01-24 19:23:07.000000 cobind-1.0.1/docs/_static/logo.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   134271 2022-01-24 22:22:34.000000 cobind-1.0.1/docs/_static/logo2.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   250629 2022-01-25 02:51:27.000000 cobind-1.0.1/docs/_static/logo3.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   162318 2022-01-15 04:16:22.000000 cobind-1.0.1/docs/_static/npmi.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    23653 2022-01-11 19:59:06.000000 cobind-1.0.1/docs/_static/npmi_bound.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    81148 2022-07-08 21:50:26.000000 cobind-1.0.1/docs/_static/ov_coef_1.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   141748 2022-02-25 01:12:09.000000 cobind-1.0.1/docs/_static/ov_coef_2.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    48648 2022-07-08 21:51:02.000000 cobind-1.0.1/docs/_static/ov_coef_3.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    46282 2022-01-11 20:03:44.000000 cobind-1.0.1/docs/_static/p.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    54577 2022-01-11 19:58:22.000000 cobind-1.0.1/docs/_static/pmi.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    59235 2022-01-11 19:58:38.000000 cobind-1.0.1/docs/_static/pmi_bound.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)  1979126 2022-07-09 15:21:10.000000 cobind-1.0.1/docs/_static/rank_comparison.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)  1345645 2022-02-04 02:07:29.000000 cobind-1.0.1/docs/_static/score_comparison.png
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   227900 2022-01-11 16:44:02.000000 cobind-1.0.1/docs/_static/set_symbols.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)   382922 2022-01-11 17:11:56.000000 cobind-1.0.1/docs/_static/srog.jpg
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      233 2022-02-03 02:09:37.000000 cobind-1.0.1/docs/acknowledgements.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      336 2023-07-06 18:37:07.000000 cobind-1.0.1/docs/change_log.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4084 2023-07-06 18:29:40.000000 cobind-1.0.1/docs/comparison.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     8467 2022-02-08 20:39:11.000000 cobind-1.0.1/docs/conf.py
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       97 2022-02-08 20:41:15.000000 cobind-1.0.1/docs/contact.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     3381 2023-07-03 18:50:22.000000 cobind-1.0.1/docs/dataset.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6818 2023-07-06 18:41:30.000000 cobind-1.0.1/docs/definition.rst
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1063 2023-07-06 15:24:32.000000 cobind-1.0.1/docs/index.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1949 2022-02-25 01:33:00.000000 cobind-1.0.1/docs/input_format.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1806 2023-07-06 03:19:40.000000 cobind-1.0.1/docs/installation.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     2083 2023-07-06 18:38:05.000000 cobind-1.0.1/docs/introduction.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1083 2021-12-23 23:06:14.000000 cobind-1.0.1/docs/license.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      795 2021-12-24 02:46:48.000000 cobind-1.0.1/docs/make.bat
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      974 2023-02-18 00:03:09.000000 cobind-1.0.1/docs/performance.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      105 2021-12-23 23:12:27.000000 cobind-1.0.1/docs/reference.rst
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:38.998317 cobind-1.0.1/docs/usage/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6074 2023-07-06 16:11:36.000000 cobind-1.0.1/docs/usage/NPMI.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6261 2023-07-06 16:10:56.000000 cobind-1.0.1/docs/usage/PMI.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6143 2023-07-06 16:31:16.000000 cobind-1.0.1/docs/usage/SD.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     3648 2023-07-06 16:13:57.000000 cobind-1.0.1/docs/usage/SROG.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6138 2023-07-06 16:10:13.000000 cobind-1.0.1/docs/usage/SS.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     8703 2023-07-06 16:05:16.000000 cobind-1.0.1/docs/usage/cobind.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     5643 2023-07-06 16:12:20.000000 cobind-1.0.1/docs/usage/cooccur.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6510 2023-07-06 16:13:17.000000 cobind-1.0.1/docs/usage/covary.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6064 2023-07-06 16:08:30.000000 cobind-1.0.1/docs/usage/jaccard.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     6519 2023-07-06 16:07:25.000000 cobind-1.0.1/docs/usage/overlap.rst
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4797 2023-07-06 16:14:39.000000 cobind-1.0.1/docs/usage/stat.rst
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:38.881424 cobind-1.0.1/lib/
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:39.020679 cobind-1.0.1/lib/cobind.egg-info/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      724 2023-07-06 19:24:38.000000 cobind-1.0.1/lib/cobind.egg-info/PKG-INFO
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     2485 2023-07-06 19:24:38.000000 cobind-1.0.1/lib/cobind.egg-info/SOURCES.txt
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        1 2023-07-06 19:24:38.000000 cobind-1.0.1/lib/cobind.egg-info/dependency_links.txt
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        1 2021-11-04 21:30:55.000000 cobind-1.0.1/lib/cobind.egg-info/not-zip-safe
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       38 2023-07-06 19:24:38.000000 cobind-1.0.1/lib/cobind.egg-info/requires.txt
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       25 2023-07-06 19:24:38.000000 cobind-1.0.1/lib/cobind.egg-info/top_level.txt
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:39.068181 cobind-1.0.1/lib/cobindability/
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    37938 2023-07-05 21:16:30.000000 cobind-1.0.1/lib/cobindability/BED.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2021-11-04 21:29:46.000000 cobind-1.0.1/lib/cobindability/__init__.py
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:39.097120 cobind-1.0.1/lib/cobindability/__pycache__/
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    24150 2022-02-22 03:30:10.000000 cobind-1.0.1/lib/cobindability/__pycache__/BED.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      160 2021-11-04 21:31:08.000000 cobind-1.0.1/lib/cobindability/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      531 2021-11-04 20:14:20.000000 cobind-1.0.1/lib/cobindability/__pycache__/bbreader.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     3741 2022-01-12 17:49:57.000000 cobind-1.0.1/lib/cobindability/__pycache__/bw.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4209 2022-05-09 19:56:03.000000 cobind-1.0.1/lib/cobindability/__pycache__/coefcal.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1904 2022-01-12 17:49:57.000000 cobind-1.0.1/lib/cobindability/__pycache__/ireader.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     7584 2022-05-11 15:53:19.000000 cobind-1.0.1/lib/cobindability/__pycache__/ovbootstrap.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     5751 2022-01-12 20:26:04.000000 cobind-1.0.1/lib/cobindability/__pycache__/ovcoef.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4576 2022-01-14 02:57:33.000000 cobind-1.0.1/lib/cobindability/__pycache__/ovjaccard.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     3324 2022-01-12 17:49:57.000000 cobind-1.0.1/lib/cobindability/__pycache__/ovpmi.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4443 2022-07-09 14:43:22.000000 cobind-1.0.1/lib/cobindability/__pycache__/ovstat.cpython-38.pyc
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      175 2022-01-23 17:38:17.000000 cobind-1.0.1/lib/cobindability/__pycache__/version.cpython-38.pyc
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      592 2022-01-12 15:53:55.000000 cobind-1.0.1/lib/cobindability/bbreader.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)      448 2021-11-04 20:13:41.000000 cobind-1.0.1/lib/cobindability/bbreader.py~
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     5072 2023-07-05 20:46:24.000000 cobind-1.0.1/lib/cobindability/bw.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     4078 2022-05-09 17:07:10.000000 cobind-1.0.1/lib/cobindability/coefcal.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1219 2021-11-05 03:13:39.000000 cobind-1.0.1/lib/cobindability/findbed.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1572 2022-01-12 15:53:54.000000 cobind-1.0.1/lib/cobindability/ireader.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)    11472 2023-07-05 20:00:49.000000 cobind-1.0.1/lib/cobindability/ovbootstrap.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     5434 2023-07-05 18:24:15.000000 cobind-1.0.1/lib/cobindability/ovstat.py
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     2228 2023-07-06 15:20:02.000000 cobind-1.0.1/lib/cobindability/utils.py
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       18 2023-07-05 21:52:32.000000 cobind-1.0.1/lib/cobindability/version.py
+-rw-r--r--   0 m102324  (1381454652) MFAD\Domain Users (1387956079)       38 2023-07-06 19:24:39.101740 cobind-1.0.1/setup.cfg
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     1686 2023-07-06 19:17:09.000000 cobind-1.0.1/setup.py
+drwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)        0 2023-07-06 19:24:39.098913 cobind-1.0.1/test/
+-rwxr-xr-x   0 m102324  (1381454652) MFAD\Domain Users (1387956079)     2208 2022-02-22 03:29:51.000000 cobind-1.0.1/test/test_bed.py
```

### Comparing `cobind-1.0.0/LICENSE` & `cobind-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/PKG-INFO` & `cobind-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: cobind
-Version: 1.0.0
-Summary: collocation analysis of genomics regions
+Version: 1.0.1
+Summary: collocation analysis of genomics intervals
 Home-page: https://cobind.readthedocs.io/en/latest/
 Author: Liguo Wang
 Author-email: wangliguo78@gmail.com
-License: UNKNOWN
-Keywords: genome regions,overlap coefficient,cooccur,pointwise mutual information
+Keywords: genome regions,collocation,overlap,cooccur
 Platform: Linux
 Platform: MacOS
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cobind-1.0.0/README.md` & `cobind-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/Makefile` & `cobind-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_1.jpeg` & `cobind-1.0.1/docs/_static/SD_1.jpeg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_1.jpg` & `cobind-1.0.1/docs/_static/SD_1.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_1.png` & `cobind-1.0.1/docs/_static/SD_1.png`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_2.jpeg` & `cobind-1.0.1/docs/_static/SD_2.jpeg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_2.jpg` & `cobind-1.0.1/docs/_static/SD_2.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SD_2.png` & `cobind-1.0.1/docs/_static/SD_2.png`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SS.jpg` & `cobind-1.0.1/docs/_static/SS.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/SS_bound.jpg` & `cobind-1.0.1/docs/_static/SS_bound.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/fisher_or.jpg` & `cobind-1.0.1/docs/_static/fisher_or.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/fisher_p.jpg` & `cobind-1.0.1/docs/_static/fisher_p.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/jaccard_1.jpg` & `cobind-1.0.1/docs/_static/jaccard_1.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/jaccard_2.jpg` & `cobind-1.0.1/docs/_static/jaccard_2.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/jaccard_3.jpg` & `cobind-1.0.1/docs/_static/jaccard_3.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/logo.png` & `cobind-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/npmi.jpg` & `cobind-1.0.1/docs/_static/npmi.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/npmi_bound.jpg` & `cobind-1.0.1/docs/_static/npmi_bound.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/ov_coef_2.jpg` & `cobind-1.0.1/docs/_static/ov_coef_2.jpg`

 * *Files 8% similar despite different names*

#### Image content

```diff
@@ -1,9 +1,9 @@
 .@8888.                                 .%8X@t%;            
   ;...  .  .  . .  .  . .  .  . .  .  .  t%St:;: .  .  . .  
- .        .       .       .       .   %%%%%%%%%%%:.   .    .
-   .  . .   . 8%%8S . .     . .     . @ t@88%8888::      .  
-     X;8888@88t@88@88t@8888S  :;;@.  .8@8%88888888: .  .    
- %S%@%@ t88:888.@8.888.88@ :  @@;8S   88X8 8.8:8: .: ;;;: . 
-  . .%%@8888.888 @8 888 888S :.    .  888.X88;X888: %X8@X%8 
-     . ; X8%:SX: %  X@. @8S: ..       8X88S8 X88.    .      
-  .     .     .             . .      .8 88X8888@88;   .  .  
+ .        .       .       .       .   %S%%%%%%%%%:.   .    .
+   .  . .   . 8S;@t . .     . .     . X %@88%8888::      .  
+     X88888@88t@88@88t@8888S  :;;@.   8@8%88888888: .  .    
+ 8@%8888S888.X8 @8.888.88@ :  @@;8S . 888.8:8t8888:: ;;;: . 
+    . 8;8 888.88 @8 888 888S :.    .  8 8888:X8X  . %X8@X%8 
+ .   St . :@S.X: %  @@. @8S: ..      .88 8 8888888:  .      
+       .     ..             . .      .888;Xt8:8888;.     .
```

#### Image metadata

```diff
@@ -1,9 +1,9 @@
 Image format: JPEG
-File size: 139109B
+File size: 141748B
 Height: 980
 Width: 3602
 Orientation: Undefined
 Compression type: JPEG
 Compression quality: 93
 Colorspace: sRGB
 Channels: srgb
@@ -11,15 +11,15 @@
 Interlace mode: None
 Rendering intent: Perceptual
 X resolution: 330
 Y resolution: 330
 Resolution units: PixelsPerInch
 Transparency channel enabled: False
 Gamma: 0.454545
-Number of unique colors: 4596
+Number of unique colors: 5574
 Comment: 
 EXIF data: exif:ColorSpace=1
 exif:ExifOffset=78
 exif:PixelXDimension=3602
 exif:PixelYDimension=980
 exif:ResolutionUnit=2
 exif:XResolution=330/1
```

### Comparing `cobind-1.0.0/docs/_static/p.jpg` & `cobind-1.0.1/docs/_static/p.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/pmi.jpg` & `cobind-1.0.1/docs/_static/pmi.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/pmi_bound.jpg` & `cobind-1.0.1/docs/_static/pmi_bound.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/set_symbols.jpg` & `cobind-1.0.1/docs/_static/set_symbols.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/_static/srog.jpg` & `cobind-1.0.1/docs/_static/srog.jpg`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/conf.py` & `cobind-1.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'cobind'
-copyright = u'2021, Liguo Wang'
+copyright = u'2022, Liguo Wang'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.0.0'
@@ -123,36 +123,36 @@
     'sidebarwidth':150
 }
 
 
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-html_title = "Cobind documentation"
+html_title = "Cobind: Collocation Analysis of Genomics Intervals"
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 html_short_title = "cobind"
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-html_logo = '_static/logo.png'
+html_logo = '_static/logo3.png'
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-html_last_updated_fmt = 'Dec 23, 2021'
+html_last_updated_fmt = ''
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
 #html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
 #html_sidebars = {}
```

### Comparing `cobind-1.0.0/docs/definition.rst` & `cobind-1.0.1/docs/definition.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,136 @@
 Definitions
 ============
 
+
 Symbols definitions
 -------------------
+We have two sets of genomic intervals **A** and **B**, and the genomic background is **G**.
+In Figure 1 below, both A and B contain only one genomic region for the purpose of clarity, but the definitions
+are still applicable if **A** and **B** have many intervals. 
 
-We have two sets of genomic intervals, **A** and **B**. The genomic background is **G** (e.g., all the cis-regulatory elements in the genome).
-In Figure 1 below, for simplicity, both A and B contain only 1 genomic region.  
+Symbols are defined as:
 
 .. image:: _static/set_symbols.jpg
   :width: 600
   :alt: Figure_1
 
 
-Symbols are defined as:
-
 \|A\|
-  All the **non-redundant** bases covered by genomic interval A. For example, if A contains two genomic intervals: "chr1 0 10", "chr1 5 15", then \|A\| = 15. 
+  The `cardinality <https://en.wikipedia.org/wiki/Cardinality>`_ of **A** (i.e., all the **non-redundant** bases covered by **A**). For example, if A contains two genomic intervals: "chr1 0 10", "chr1 5 15", then \|A\| = 15. 
 \|B\|
-  All the **non-redundant** bases covered by genomic interval B.
+  The `cardinality <https://en.wikipedia.org/wiki/Cardinality>`_ of **B** (i.e., all the **non-redundant** bases covered by **B**).
 \|G\|
-  The genomic background (user defined). Depending on the context, this can be *all the cis-regulatory elements*, *all the promoters*, *all the TF binding sites* in the genome.
+  The genomic background. Depending on the context, this can be *the whole genome*, *all the cis-regulatory elements*, *all the promoters*, *all the TF binding sites* in the genome, etc. **A** and **B** must be the subsets of **G**. 
 \|A ∪ B\|
-  Union (A or B). In A or B (or both).
+  Union of A and B (i.e., bases covered by A or B).
 \|A ∩ B\|
-  Intersection (A and B). In both A and B.
+  Intersection of A and B (i.e., bases covered by A and B simultaneously). This is commonly used to measure the *collocation* of A and B.
 \|A − B\|
-  Difference (A not B). in A but not in B.
+  Difference (A not B) (i.e., bases covered by only A but not B).
 \|B − A\|
-  Difference (B not A). in B but not in A.
+  Difference (B not A) (i.e., bases covered by only B but not A).
 \|A ∪ B\|^𝐶
-  Complement of \|A ∪ B\| (Neither A nor B).
+  Complement of \|A ∪ B\| (i.e., bases NOT covered by A or B).
+
 
 Spacial Relations of Genomic regions (SROG)
 -------------------------------------------
 
-There are six different spacial relations between two genomic regions (A and B): 
+There are six different spacial relations between two genomic regions (A and B). As illustrated below:
 
 .. image:: _static/srog.jpg
   :width: 700
   :alt: Alternative text
 
 
-Overlap coefficient (O)
------------------------
-The overlap coefficient between A and B is calculated as the ratio between the *intersection of A and B*, and the *geometric mean of A and B*.
-
- - O(A,B) is a value between [0, 1], with 0 indicating 'no overlap', and 1 indicating '100% overlap' (i.e., A and B are identical). 
- - O(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
+Collocation coefficient (C)
+---------------------------
+The collocation coefficient between A and B is calculated as the ratio between \|A ∩ B\| and the *geometric mean of \|A\| and \|B\|*.
+C(A,B) is a value between [0, 1], with 0 indicating 'no overlap', and 1 indicating '100% overlap' (i.e., A and B are identical). C(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
 
 .. image:: _static/ov_coef_1.jpg
   :width: 250
   :alt: Alternative text
 
 .. image:: _static/ov_coef_3.jpg
   :width: 200
   :alt: Alternative text
 
+Overall collocation coefficient
+  The collocation coefficient between two **sets** of genomic regions. For example, you can use the *overall collocation coefficient* to measure the cobindability of two transcription factors. 
 
-The geometrical interpretation of O^2 is illustrated as below:
-
-.. image:: _static/ov_coef_2.jpg
-  :width: 600
-  :alt: Alternative text
-
-Overall overlap coefficient
-  The overlap coefficient between two **sets** of genomic regions. For example, you can use the *overall overlap coefficient* to measure the cobindability of two transcription factors. 
-
-peakwise overlap coefficient
-  The overlap coefficient between two genomic regions (A protein-bound genomic region is called "peak" in `ChIP-seq <https://en.wikipedia.org/wiki/ChIP_sequencing>`_ experiment). 
+peakwise collocation coefficient
+  The collocation coefficient between **two** genomic intervals (A protein-bound genomic region is called "peak" in `ChIP-seq <https://en.wikipedia.org/wiki/ChIP_sequencing>`_ experiment). 
 
 
 
 Jaccard coefficient (J)
 -------------------------
-The `Jaccard similarity coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_, also known as the Jaccard index. It is the ratio between **intersection** and **union**.
+The `Jaccard similarity coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_, also known as the Jaccard index. It is the ratio between **intersection** and **union**. J(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
 
 
 .. image:: _static/jaccard_1.jpg
   :width: 400
   :alt: Alternative text
 
 .. image:: _static/jaccard_2.jpg
   :width: 180
   :alt: Alternative text
 
-J(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
 
 The Jaccard distance *Dj* is calculated as:
 
 .. image:: _static/jaccard_3.jpg
   :width: 450
   :alt: Alternative text
 
 
 Similar to O(A,B), we have an **overall Jaccard coefficient** and **peakwise Jaccard coefficient**.
 
+.. note::
+   The Jaccard coefficient implemented here is slightly different from `BEDTools <https://bedtools.readthedocs.io/en/latest/content/tools/jaccard.html>`_ :code:`jaccard` function.
+   When calculating the union, BEDTools only use the intervals that are overlapped with each other, while we use all the intervals.
+
 overall Jaccard coefficient
   The Jaccard coefficient between two **sets** of genomic regions. 
 peakwise Jaccard coefficient
-  The Jaccard coefficient between two genomic regions (A protein-bound genomic region is called "peak" in `ChIP-seq <https://en.wikipedia.org/wiki/ChIP_sequencing>`_ experiment).
-
+  The Jaccard coefficient between **two** genomic intervals.
 
 
 Sørensen–Dice coefficient (SD)
 ------------------------------
-`Sørensen–Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_,  also called *Sørensen–Dice index*, *Sørensen index* or *Dice's coefficient*.
+`Sørensen–Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_,  also called *Sørensen–Dice index*, *Sørensen index* or *Dice's coefficient*. SD(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
 
 .. image:: _static/SD_1.jpg
   :width: 200
   :alt: Alternative text
 
 .. image:: _static/SD_2.jpg
   :width: 180
   :alt: Alternative text
 
-SD(A, B) is defined as 0 when \|A\| = 0 or \|B\| = 0, or  \|A\| = \|B\| = 0.
-
 Jaccard coefficient (J) can be converted into Sørensen–Dice coefficient (SD) and vice versa:
 
 *J = SD/(2-SD)* and *SD = 2J/(1+J)*
 
+
 Szymkiewicz–Simpson coefficient (SS)
 -------------------------------------
-`Szymkiewicz–Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ is defined as the size of the intersection divided by the smaller of the size of the two sets.
+`Szymkiewicz–Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ is defined as the size of the intersection divided by the smaller size of the two sets.
 
 .. image:: _static/SS.jpg
   :width: 250
   :alt: Alternative text
 
 .. image:: _static/SS_bound.jpg
   :width: 180
   :alt: Alternative text
 
 
-Coefficients comparison
-------------------------
-
- - **O(A,B)**, **J(A,B)**, and **SD(A,B)** are all within [0, 1] with 0 indicating 'no overlap', and 1 indicating '100% overlap' (i.e., A equals B).
- - **SS(A,B)** is different, with 0 indicating 'no overlap', and 1 indicating "A equals B", or "A within B" or "B within A" .
- - When the sizes of two genomic regions are significantly different, the **SS(A,B)** gives more weight to the smaller genomic region, while the **J(A,B)** and **SD(A,B)** give more weight to the larger genomic region, **O(A,B)** is a compromised index between the two extremes. 
-
-.. list-table:: **O(A,B)** vs **J(A,B)** vs **SD(A,B)** vs **SS(A,B)**
-   :widths: 15,15,15,15,15,15,15,15,20
-   :header-rows: 1
-
-   * - *SROG*
-     - \|A\|
-     - \|B\|
-     - \|A ∩ B\|
-     - \|A ∪ B\|
-     - *O*
-     - *J*
-     - *SD*
-     - *SS*
-   * - A equals B
-     - 1000
-     - 1000
-     - 1000
-     - 1000
-     - 1
-     - 1
-     - 1
-     - 1
-   * - A disjoint B 
-     - 1000
-     - 1000
-     - 0
-     - 2000
-     - 0
-     - 0
-     - 0
-     - 0
-   * - A overlaps B 
-     - 100
-     - 1000
-     - 50
-     - 1050
-     - 0.158
-     - 0.0476
-     - 0.0909
-     - 0.5
-   * - A within B 
-     - 100
-     - 1000
-     - 100
-     - 1000
-     - 0.316
-     - 0.1
-     - 0.182
-     - 1
-
-
 Pointwise mutual information (PMI)
 ----------------------------------
 `Pointwise mutual information (PMI) <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ is one of the standard association measures in collocation analysis. 
 It measures how much the observed overlaps differ from what we would expect them to be. Assume A and B represent two sets of genomic regions bound by `transcription factors <https://en.wikipedia.org/wiki/Transcription_factor>`_ A and B; respectively, PMI measures if A and B bind together or separately.
 
 
 PMI is calculated as:
@@ -211,22 +147,23 @@
 
 
 PMI = 0
   Indicates that A and B are independent.
 PMI > 0
   Indicates that the overlapping between A and B is in a frequency *higher* than what we would expect if A and B are independent (i.e, A and B tend to bind together). 
 PMI < 0
-  Indicates that the overlapping between A and B is in frequency *lower* than what we would expect if A and B are independent. (i.e., A and B tend to bind separately). 
+  Indicates that the overlapping between A and B is in frequency *lower* than what we would expect if A and B were independent. (i.e., A and B tend to bind separately). 
 
 Note, PMI has no boundaries:
 
 .. image:: _static/pmi_bound.jpg
   :width: 500
   :alt: Alternative text
 
+
 Normalized pointwise mutual information (NPMI)
 ----------------------------------------------
 Normalized pointwise mutual information (NPMI) is calculated as:
 
 .. image:: _static/npmi.jpg
   :width: 650
   :alt: Alternative text
@@ -234,10 +171,17 @@
 Note, after normalization, NPMI is confined to [-1, 1]:
 
 .. image:: _static/npmi_bound.jpg
   :width: 250
   :alt: Alternative text
 
 
+Which metric to use? 
+---------------------
+
+Based on our evaluation, the **Collocation coefficient (C)** and **NPMI** are the best two metrics one can use to quantify the overlap (collocation)
+between two sets of genomic intervals.
+
+`Metric evaluation <https://cobind.readthedocs.io/en/latest/comparison.html>`_
```

### Comparing `cobind-1.0.0/docs/index.rst` & `cobind-1.0.1/docs/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -33,18 +33,41 @@
    usage/SS.rst
    usage/PMI.rst
    usage/NPMI.rst
    usage/cooccur.rst
    usage/covary.rst
    usage/SROG.rst
    usage/stat.rst
+   usage/zscore.rst
+
+.. toctree::
+   :caption: Evaluation
+
+   comparison
+
+.. toctree::
+   :caption: Performance
+
+   performance
 
 .. toctree::
    :caption: License
 
    license
 
 .. toctree::
+   :caption: Acknowledgements
+   
+   acknowledgements
+
+.. toctree::
+   :caption: Contact
+
+   contact
+
+.. toctree::
    :caption: Reference
 
    reference
 
+
+
```

### Comparing `cobind-1.0.0/docs/input_format.rst` & `cobind-1.0.1/docs/input_format.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 Input file and data format
 ===========================
 
 BED format
 ----------
 `BED (Browser Extensible Data) <https://genome.ucsc.edu/FAQ/FAQformat.html#format1>`_ 
-format is commonly used to describe genomic intervals. BED files used by **cobind** must 
-have at least the first three columns::
+format is commonly used to describe genomic intervals. Standard BED file has 12 columns, but **cobind** only requires the first three columns (all the other columns are optional)::
 
  # BED3 format (chrom, start, end)
  chr1    629149    629391
  chr1    629720    630165
  chr1    631404    631758
  ...
```

### Comparing `cobind-1.0.0/docs/installation.rst` & `cobind-1.0.1/docs/installation.rst`

 * *Files 15% similar despite different names*

```diff
@@ -11,29 +11,39 @@
 - `scipy <https://www.scipy.org/>`_
 - `bx-python <https://github.com/bxlab/bx-python>`_
 - `pyBigWig <https://pypi.org/project/pyBigWig/>`_
 
 .. note::
    These packages will be automatically installed when you use `pip3 <https://pip.pypa.io/en/stable/installing/>`_ to install cobind.
 
-Virtual environment
--------------------
-If you would like to install *cobind* into a virtual environment, please follow `these instructions <https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-and-using-virtual-environments>`_. 
-
-Install
--------
+Install pip
+-----------------
 Please install `pip <https://pypi.org/project/pip/>`_ (Package Installer for Python) first if you do not have it.
 
 .. code-block::
    
    #check if pip is available. 
    $ pip --version
-   pip 20.1.1 from /Users/home/opt/anaconda3/lib/python3.8/site-packages/pip (python 3.8)
+   pip 23.0.1 from /Users/m102324/miniconda3/lib/python3.10/site-packages/pip (python 3.10)
+
+Install to virtual environment
+-------------------------------
+Python's **Virtual Environments** allow Python packages to be installed in an isolated location rather than being installed globally. If you would like to install *cobind* into a virtual environment, please follow `these instructions <https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-and-using-virtual-environments>`_. 
+Specifically, follow these steps:
+
+.. code-block::
+
+   $python3 -m venv cobind
+   $source cobind/bin/activate
+   $pip install cobind
+
 
-Then you can install *cobind* using `pip <https://pypi.org/project/pip/>`_ from `PyPI <https://pypi.org/project/cobind/>`_ or `GitHub <https://github.com/liguowang/cobind>`_
+Install globally
+-----------------
+Install *cobind* using `pip <https://pypi.org/project/pip/>`_ from `PyPI <https://pypi.org/project/cobind/>`_ or `GitHub <https://github.com/liguowang/cobind>`_
 
 .. code-block::
  
    $ pip install cobind
    #or 
    $ pip install git+https://github.com/liguowang/cobind.git
```

### Comparing `cobind-1.0.0/docs/license.rst` & `cobind-1.0.1/docs/license.rst`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/make.bat` & `cobind-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/docs/usage/NPMI.rst` & `cobind-1.0.1/docs/usage/NPMI.rst`

 * *Files 10% similar despite different names*

```diff
@@ -24,54 +24,73 @@
 
 Usage
 -----
 
 :code:`cobind.py npmi -h`
 
 ::
-
- usage: cobind.py npmi [-h] [-n ITER] [-f SUBSAMPLE] [-b BGSIZE] [-o] [-d] input_A.bed input_B.bed
  
-  positional arguments:
-    input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-    input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-  
-  optional arguments:
-    -h, --help            show this help message and exit
-    -n ITER, --ndraws ITER
-                          Times of resampling to estimate confidence intervals. Set to '0' to turn
-                          off resampling.(default: 20)
-    -f SUBSAMPLE, --fraction SUBSAMPLE
-                          Resampling fraction. (default: 0.75)
-    -b BGSIZE, --background BGSIZE
-                          The size of the cis-regulatory genomic regions. This is about 1.4Gb For the
-                          human genome. (default: 1400000000)
-    -o, --save            If set, will save peak-wise coefficients to files
-                          ("input_A_peakwise_scores.tsv" and "input_B_peakwise_scores.tsv").
-    -d, --debug           Print detailed information for debugging.
-
+ usage: cobind.py npmi [-h] [--nameA NAMEA] [--nameB NAMEB] [-n ITER]
+                       [-f SUBSAMPLE] [-b BGSIZE] [-o] [-l log_file] [-d]
+                       input_A.bed input_B.bed
+
+ positional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+
+ options:
+   -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified (None), the file name ("input_A.bed") will
+                         be used.
+   --nameB NAMEB         Name to represent the 2nd set of genomic interval. If
+                         not specified (None), the file name ("input_B.bed")
+                         will be used.
+   -n ITER, --ndraws ITER
+                         Times of resampling to estimate confidence intervals.
+                         Set to '0' to turn off resampling. For the resampling
+                         process to work properly, overlapped intervals in each
+                         bed file must be merged. (default: 20)
+   -f SUBSAMPLE, --fraction SUBSAMPLE
+                         Resampling fraction. (default: 0.75)
+   -b BGSIZE, --background BGSIZE
+                         The size of the cis-regulatory genomic regions. This
+                         is about 1.4Gb For the human genome. (default:
+                         1400000000)
+   -o, --save            If set, will save peak-wise coefficients to files
+                         ("input_A_peakwise_scores.tsv" and
+                         "input_B_peakwise_scores.tsv").
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 Example
 -------
 
-Calculate the **overall** NPMI and **peak-wise** NPMI between CTCF binding sites and RAD21 binding sites.
+Calculate the **overall** NPMI and **peak-wise** NPMI between `CTCF binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#ctcf-chip-seq>`_ and `RAD21 binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#rad21-chip-seq>`_.
 
 :code:`python3 ../bin/cobind.py npmi CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed --save`
 
-The overall NPMI between *CTCF_ENCFF660GHM.bed* and *RAD21_ENCFF057JFH.bed* was printed to screen
+The overall NPMI between :code:`CTCF_ENCFF660GHM.bed` and :code:`RAD21_ENCFF057JFH.bed` was printed to screen
 
 ::
 
  2022-01-16 09:26:50 [INFO]  Calculate the normalized pointwise mutual information (NPMI) ...
  A.name               CTCF_ENCFF660GHM.bed
  B.name              RAD21_ENCFF057JFH.bed
  A.interval_count                    58684
@@ -84,22 +103,18 @@
  Coef(expected)                     0.0000
  Coef(95% CI)              [0.6945,0.6977]
  dtype: object
  2022-01-16 09:27:18 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-16 09:27:19 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed" : 58584
  2022-01-16 09:27:19 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-16 09:27:19 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed" : 31955
- 2022-01-16 09:27:19 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed"
- 2022-01-16 09:27:19 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed"
- 2022-01-16 09:27:19 [INFO]  Calculate the overlap coefficient of each genomic region in CTCF_ENCFF660GHM.bed ...
- 2022-01-16 09:27:22 [INFO]  Save peakwise scores to CTCF_ENCFF660GHM.bed_peakwise_scores.tsv ...
- 2022-01-16 09:27:22 [INFO]  Calculate the overlap coefficient of each genomic region in RAD21_ENCFF057JFH.bed ...
- 2022-01-16 09:27:23 [INFO]  Save peakwise scores to RAD21_ENCFF057JFH.bed_peakwise_scores.tsv ...
+ ...
+
+If :code:`--save` was specified, the peakwise coefficients were saved to :code:`CTCF_ENCFF660GHM.bed_peakwise_scores.tsv` and :code:`RAD21_ENCFF057JFH.bed_peakwise_scores.tsv`, respectively.
 
-If :code:`--save` was specified, the peakwise NPMI were saved to *CTCF_ENCFF660GHM.bed_peakwise_scores.tsv* and *RAD21_ENCFF057JFH.bed_peakwise_scores.tsv*, respectively.
 ::
 
  $ head -5 CTCF_ENCFF660GHM.bed_peakwise_scores.tsv
   
  chrom start end A.size  B.size  A∩B A∪B B.list  Score
  chr12 108043  108283  240 404 240 404 chr12:107919-108323 0.9665721394030915
  chr12 153232  153470  238 222 222 238 chr12:153236-153458 0.9955551496433741
```

### Comparing `cobind-1.0.0/docs/usage/PMI.rst` & `cobind-1.0.1/docs/usage/PMI.rst`

 * *Files 11% similar despite different names*

```diff
@@ -24,55 +24,74 @@
 
 Usage
 -----
 
 :code:`cobind.py pmi -h`
 
 ::
-
- usage: cobind.py pmi [-h] [-n ITER] [-f SUBSAMPLE] [-b BGSIZE] [-o] [-d] input_A.bed input_B.bed
  
-  positional arguments:
-    input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-    input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-  
-  optional arguments:
-    -h, --help            show this help message and exit
-    -n ITER, --ndraws ITER
-                          Times of resampling to estimate confidence intervals. Set to '0' to turn
-                          off resampling.(default: 20)
-    -f SUBSAMPLE, --fraction SUBSAMPLE
-                          Resampling fraction. (default: 0.75)
-    -b BGSIZE, --background BGSIZE
-                          The size of the cis-regulatory genomic regions. This is about 1.4Gb For the
-                          human genome. (default: 1400000000)
-    -o, --save            If set, will save peak-wise coefficients to files
-                          ("input_A_peakwise_scores.tsv" and "input_B_peakwise_scores.tsv").
-    -d, --debug           Print detailed information for debugging.
-
+ usage: cobind.py pmi [-h] [--nameA NAMEA] [--nameB NAMEB] [-n ITER]
+                      [-f SUBSAMPLE] [-b BGSIZE] [-o] [-l log_file] [-d]
+                      input_A.bed input_B.bed
+
+ positional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+
+ options:
+   -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified (None), the file name ("input_A.bed") will
+                         be used.
+   --nameB NAMEB         Name to represent the 2nd set of genomic interval. If
+                         not specified (None), the file name ("input_B.bed")
+                         will be used.
+   -n ITER, --ndraws ITER
+                         Times of resampling to estimate confidence intervals.
+                         Set to '0' to turn off resampling. For the resampling
+                         process to work properly, overlapped intervals in each
+                         bed file must be merged. (default: 20)
+   -f SUBSAMPLE, --fraction SUBSAMPLE
+                         Resampling fraction. (default: 0.75)
+   -b BGSIZE, --background BGSIZE
+                         The size of the cis-regulatory genomic regions. This
+                         is about 1.4Gb For the human genome. (default:
+                         1400000000)
+   -o, --save            If set, will save peak-wise coefficients to files
+                         ("input_A_peakwise_scores.tsv" and
+                         "input_B_peakwise_scores.tsv").
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 
 Example
 -------
 
-Calculate the **overall** `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ and **peak-wise** `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ between CTCF binding sites and RAD21 binding sites.
+Calculate the **overall** `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ and **peak-wise** `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ between `CTCF binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#ctcf-chip-seq>`_ and `RAD21 binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#rad21-chip-seq>`_.
 
 :code:`python3 ../bin/cobind.py pmi CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed --save`
 
-The overall `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ between *CTCF_ENCFF660GHM.bed* and *RAD21_ENCFF057JFH.bed* was printed to screen
+The overall `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ between :code:`CTCF_ENCFF660GHM.bed` and :code:`RAD21_ENCFF057JFH.bed` was printed to screen
 
 ::
 
  2022-01-16 09:01:34 [INFO]  Calculate the pointwise mutual information (PMI) ...
  A.name               CTCF_ENCFF660GHM.bed
  B.name              RAD21_ENCFF057JFH.bed
  A.interval_count                    58684
@@ -85,22 +104,17 @@
  Coef(expected)                     0.0000
  Coef(95% CI)              [3.9230,3.9343]
  dtype: object
  2022-01-16 09:02:02 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-16 09:02:03 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed" : 58584
  2022-01-16 09:02:03 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-16 09:02:03 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed" : 31955
- 2022-01-16 09:02:03 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed"
- 2022-01-16 09:02:03 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed"
- 2022-01-16 09:02:03 [INFO]  Calculate the overlap coefficient of each genomic region in CTCF_ENCFF660GHM.bed ...
- 2022-01-16 09:02:06 [INFO]  Save peakwise scores to CTCF_ENCFF660GHM.bed_peakwise_scores.tsv ...
- 2022-01-16 09:02:06 [INFO]  Calculate the overlap coefficient of each genomic region in RAD21_ENCFF057JFH.bed ...
- 2022-01-16 09:02:07 [INFO]  Save peakwise scores to RAD21_ENCFF057JFH.bed_peakwise_scores.tsv ...
+ ...
 
-If :code:`--save` was specified, the peakwise `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ were saved to *CTCF_ENCFF660GHM.bed_peakwise_scores.tsv* and *RAD21_ENCFF057JFH.bed_peakwise_scores.tsv*, respectively.
+If :code:`--save` was specified, the peakwise `PMI <https://en.wikipedia.org/wiki/Pointwise_mutual_information>`_ were saved to :code:`CTCF_ENCFF660GHM.bed_peakwise_scores.tsv` and :code:`RAD21_ENCFF057JFH.bed_peakwise_scores.tsv`, respectively.
 ::
 
  $ head -5 CTCF_ENCFF660GHM.bed_peakwise_scores.tsv
   
  chrom start end A.size  B.size  A∩B A∪B B.list  Score
  chr12 108043  108283  240 404 240 404 chr12:107919-108323 15.058323195606475
  chr12 153232  153470  238 222 222 238 chr12:153236-153458 15.58746739989615
```

### Comparing `cobind-1.0.0/docs/usage/SD.rst` & `cobind-1.0.1/docs/usage/SD.rst`

 * *Files 18% similar despite different names*

```diff
@@ -7,64 +7,83 @@
 Calculate the `Sørensen–Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_ between two sets of genomic regions. 
 
 .. image:: ../_static/SD_1.jpg
   :width: 200
   :alt: Alternative text
 
 .. image:: ../_static/SD_2.jpg
-  :width: 180
+  :width: 60
   :alt: Alternative text
 
 Usage
 -----
 
 :code:`cobind.py dice -h`
 
 ::
 
- usage: cobind.py dice [-h] [-n ITER] [-f SUBSAMPLE] [-b BGSIZE] [-o] [-d] input_A.bed input_B.bed
- 
-  positional arguments:
-    input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-    input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-  
-  optional arguments:
-    -h, --help            show this help message and exit
-    -n ITER, --ndraws ITER
-                          Times of resampling to estimate confidence intervals. Set to '0' to turn
-                          off resampling.(default: 20)
-    -f SUBSAMPLE, --fraction SUBSAMPLE
-                          Resampling fraction. (default: 0.75)
-    -b BGSIZE, --background BGSIZE
-                          The size of the cis-regulatory genomic regions. This is about 1.4Gb For the
-                          human genome. (default: 1400000000)
-    -o, --save            If set, will save peak-wise coefficients to files
-                          ("input_A_peakwise_scores.tsv" and "input_B_peakwise_scores.tsv").
-    -d, --debug           Print detailed information for debugging.
-
+ usage: cobind.py dice [-h] [--nameA NAMEA] [--nameB NAMEB] [-n ITER]
+                       [-f SUBSAMPLE] [-b BGSIZE] [-o] [-l log_file] [-d]
+                       input_A.bed input_B.bed
+
+ positional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+
+ options:
+   -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified (None), the file name ("input_A.bed") will
+                         be used.
+   --nameB NAMEB         Name to represent the 2nd set of genomic interval. If
+                         not specified (None), the file name ("input_B.bed")
+                         will be used.
+   -n ITER, --ndraws ITER
+                         Times of resampling to estimate confidence intervals.
+                         Set to '0' to turn off resampling. For the resampling
+                         process to work properly, overlapped intervals in each
+                         bed file must be merged. (default: 20)
+   -f SUBSAMPLE, --fraction SUBSAMPLE
+                         Resampling fraction. (default: 0.75)
+   -b BGSIZE, --background BGSIZE
+                         The size of the cis-regulatory genomic regions. This
+                         is about 1.4Gb For the human genome. (default:
+                         1400000000)
+   -o, --save            If set, will save peak-wise coefficients to files
+                         ("input_A_peakwise_scores.tsv" and
+                         "input_B_peakwise_scores.tsv").
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 
 Example
 -------
 
-Calculate the **overall** `Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_ and **peak-wise** `Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_ between CTCF binding sites and RAD21 binding sites.
+Calculate the **overall** `Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_ and **peak-wise** `Dice coefficient <https://en.wikipedia.org/wiki/S%C3%B8rensen%E2%80%93Dice_coefficient>`_ between `CTCF binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#ctcf-chip-seq>`_ and `RAD21 binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#rad21-chip-seq>`_.
 
 :code:`python3 ../bin/cobind.py dice CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed --save`
 
-The overall Dice coefficient between *CTCF_ENCFF660GHM.bed* and *RAD21_ENCFF057JFH.bed* was printed to screen
+The overall Dice coefficient between :code:`CTCF_ENCFF660GHM.bed` and :code:`RAD21_ENCFF057JFH.bed` was printed to screen
 
 ::
 
  2022-01-16 08:43:40 [INFO]  Calculate Sørensen–Dice coefficient (overall) ...
  A.name               CTCF_ENCFF660GHM.bed
  B.name              RAD21_ENCFF057JFH.bed
  A.interval_count                    58684
@@ -78,23 +97,18 @@
  Coef(95% CI)              [0.4222,0.4275]
  dtype: object
  2022-01-16 08:44:08 [INFO]  Calculate Sørensen–Dice coefficient (peakwise) ...
  2022-01-16 08:44:08 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-16 08:44:08 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed" : 58584
  2022-01-16 08:44:08 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-16 08:44:09 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed" : 31955
- 2022-01-16 08:44:09 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed"
- 2022-01-16 08:44:09 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed"
- 2022-01-16 08:44:09 [INFO]  Calculate the overlap coefficient of each genomic region in CTCF_ENCFF660GHM.bed ...
- 2022-01-16 08:44:11 [INFO]  Save peakwise scores to CTCF_ENCFF660GHM.bed_peakwise_scores.tsv ...
- 2022-01-16 08:44:11 [INFO]  Calculate the overlap coefficient of each genomic region in RAD21_ENCFF057JFH.bed ...
- 2022-01-16 08:44:12 [INFO]  Save peakwise scores to RAD21_ENCFF057JFH.bed_peakwise_scores.tsv ...
+ ...
 
 
-If :code:`--save` was specified, the peakwise coefficients were saved to *CTCF_ENCFF660GHM.bed_peakwise_scores.tsv* and *RAD21_ENCFF057JFH.bed_peakwise_scores.tsv*, respectively.
+If :code:`--save` was specified, the peakwise coefficients were saved to :code:`CTCF_ENCFF660GHM.bed_peakwise_scores.tsv` and :code:`RAD21_ENCFF057JFH.bed_peakwise_scores.tsv`, respectively.
 ::
 
  $ head -5 CTCF_ENCFF660GHM.bed_peakwise_scores.tsv
   
  chrom start end A.size  B.size  A∩B A∪B B.list  Score
  chr12 108043  108283  240 404 240 404 chr12:107919-108323 0.7453416149068323
  chr12 153232  153470  238 222 222 238 chr12:153236-153458 0.9652173913043478
```

### Comparing `cobind-1.0.0/docs/usage/SROG.rst` & `cobind-1.0.1/docs/usage/SROG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 Spatial Relation Of Genomic (SROG) intervals
 ============================================
 
 Description
 -------------
 Match up two sets of genomic intervals, and report the code of Spatial Relation Of Genomic (SROG).
-SROG codes include 'disjoint','touch','equal','overlap','contain','within'.
+SROG codes include :code:`disjoint`, :code:`touch`, :code:`equal`, :code:`overlap`, :code:`contain`, :code:`within`.
 
 .. image:: ../_static/srog.jpg
   :width: 700
   :alt: Alternative text
 
 
 Usage
 -----
 
 :code:`cobind.py srog -h`
 
 ::
  
- usage: cobind.py srog [-h] [--dist MAX_DIST] [-d] input_A.bed input_B.bed output.tsv
- 
- positional arguments:
-   input_A.bed      Genomic regions in BED, BED-like or bigBed format. If 'name' (the 4th column) is not
-                    provided, the default name is "chrom:start-end". If strand (the 6th column) is not
-                    provided, the default strand is "+".
-   input_B.bed      Genomic regions in BED, BED-like or bigBed format. If 'name' (the 4th column) is not
-                    provided, the default name is "chrom:start-end". If strand (the 6th column) is not
-                    provided, the default strand is "+".
-   output.tsv       Generate spatial relation code (disjoint, touch, equal, overlap, contain, within)
-                    for each genomic interval in "input_A.bed".
- 
- optional arguments:
-   -h, --help       show this help message and exit
-   --dist MAX_DIST  When intervals are disjoint, find the closest up- and down-stream intervals that are
-                    no further than `max_dist` away. default: 250000000)
-   -d, --debug      Print detailed information for debugging.
+ usage: cobind.py srog [-h] [--dist MAX_DIST] [-l log_file] [-d]
+                       input_A.bed input_B.bed output.tsv
 
+ positional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. If
+                         'name' (the 4th column) is not provided, the default
+                         name is "chrom:start-end". If strand (the 6th column)
+                         is not provided, the default strand is "+".
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. If
+                         'name' (the 4th column) is not provided, the default
+                         name is "chrom:start-end". If strand (the 6th column)
+                         is not provided, the default strand is "+".
+   output.tsv            Generate spatial relation code (disjoint, touch,
+                         equal, overlap, contain, within) for each genomic
+                         interval in "input_A.bed".
+
+ options:
+   -h, --help            show this help message and exit
+   --dist MAX_DIST       When intervals are disjoint, find the closest up- and
+                         down-stream intervals that are no further than
+                         `max_dist` away. default: 250000000)
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 Example
 -------
 
 :code:`cobind.py srog CTCF_ENCFF660GHM.bed3 RAD21_ENCFF057JFH.bed3 output.tsv`
 
 ::
@@ -52,30 +60,32 @@
  contain      1695
  within      23214
  touch           0
  equal           1
  other           0
  dtype: int64
 
-Match up results were saved to "output.tsv"::
+Match up results were saved to :code:`output.tsv` ::
 
  $head -10 output.tsv
  
  chr12 53676079  53676369  within  chr12:53676060-53676382
  chr12 57905364  57905661  within  chr12:57905272-57905699
  chr22 20564334  20564661  contain chr22:20564370-20564581
  chr16 57649065  57649362  within  chr16:57649007-57649370
  chr17 45135294  45135610  overlap chr17:45135296-45135642
  chr15 40274737  40275016  within  chr15:40274714-40275018
  chr1  114346538 114346847 within  chr1:114346526-114346903
  chr7  151172578 151172888 overlap chr7:151172565-151172865
  chr1  225474965 225475268 within  chr1:225474919-225475330
  chr5  179668464 179668730 contain chr5:179668495-179668674
  ...
- chr22   23128466        23128723        disjoint        UpInterval=chr22:22651059-22651463,DownInterval=chr22:23385972-23386169
+ chr22   23128466        23128723        disjoint        UpInterval=chr22:22651059-22651463,
+                                                         DownInterval=chr22:23385972-23386169
+ ...
 
 Column 1-3
   Genome intervals from "CTCF_ENCFF660GHM.bed3".
 Column 4
-  SROG code. When SORG = 'disjoint', two closest intervals (up- and down-stream) from "RAD21_ENCFF057JFH.bed3" were reported.
+  SROG code. When SORG = :code:`disjoint`, two closest intervals (up- and down-stream) from :code:`RAD21_ENCFF057JFH.bed3` were reported.
 column 5
-  Genomic intervals from "RAD21_ENCFF057JFH.bed3".
+  Genomic intervals from :code:`RAD21_ENCFF057JFH.bed3`.
```

### Comparing `cobind-1.0.0/docs/usage/SS.rst` & `cobind-1.0.1/docs/usage/SS.rst`

 * *Files 12% similar despite different names*

```diff
@@ -17,53 +17,73 @@
 Usage
 -----
 
 :code:`cobind.py simpson -h`
 
 ::
 
- usage: cobind.py simpson [-h] [-n ITER] [-f SUBSAMPLE] [-b BGSIZE] [-o] [-d] input_A.bed input_B.bed
- 
-  positional arguments:
-    input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-    input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                          includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                          'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                          compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://,
-                          ftp://) files. Do not compress BigBed foramt. BigBed file can also be a
-                          remote file.
-  
-  optional arguments:
-    -h, --help            show this help message and exit
-    -n ITER, --ndraws ITER
-                          Times of resampling to estimate confidence intervals. Set to '0' to turn
-                          off resampling.(default: 20)
-    -f SUBSAMPLE, --fraction SUBSAMPLE
-                          Resampling fraction. (default: 0.75)
-    -b BGSIZE, --background BGSIZE
-                          The size of the cis-regulatory genomic regions. This is about 1.4Gb For the
-                          human genome. (default: 1400000000)
-    -o, --save            If set, will save peak-wise coefficients to files
-                          ("input_A_peakwise_scores.tsv" and "input_B_peakwise_scores.tsv").
-    -d, --debug           Print detailed information for debugging.
+ usage: cobind.py simpson [-h] [--nameA NAMEA] [--nameB NAMEB] [-n ITER]
+                          [-f SUBSAMPLE] [-b BGSIZE] [-o] [-l log_file] [-d]
+                          input_A.bed input_B.bed
+
+ positional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+
+ options:
+   -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified (None), the file name ("input_A.bed") will
+                         be used.
+   --nameB NAMEB         Name to represent the 2nd set of genomic interval. If
+                         not specified (None), the file name ("input_B.bed")
+                         will be used.
+   -n ITER, --ndraws ITER
+                         Times of resampling to estimate confidence intervals.
+                         Set to '0' to turn off resampling. For the resampling
+                         process to work properly, overlapped intervals in each
+                         bed file must be merged. (default: 20)
+   -f SUBSAMPLE, --fraction SUBSAMPLE
+                         Resampling fraction. (default: 0.75)
+   -b BGSIZE, --background BGSIZE
+                         The size of the cis-regulatory genomic regions. This
+                         is about 1.4Gb For the human genome. (default:
+                         1400000000)
+   -o, --save            If set, will save peak-wise coefficients to files
+                         ("input_A_peakwise_scores.tsv" and
+                         "input_B_peakwise_scores.tsv").
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 
 Example
 -------
 
-Calculate the **overall** `Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ and **peak-wise** `Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ between CTCF binding sites and RAD21 binding sites.
+Calculate the **overall** `Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ and **peak-wise** `Simpson coefficient <https://en.wikipedia.org/wiki/Overlap_coefficient>`_ between `CTCF binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#ctcf-chip-seq>`_ and `RAD21 binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#rad21-chip-seq>`_.
 
 :code:`python3 ../bin/cobind.py simpson CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed --save`
 
-The overall Simpson coefficient between *CTCF_ENCFF660GHM.bed* and *RAD21_ENCFF057JFH.bed* was printed to screen
+The overall Simpson coefficient between :code:`CTCF_ENCFF660GHM.bed` and :code:`RAD21_ENCFF057JFH.bed` was printed to screen
 
 ::
 
  2022-01-16 08:52:41 [INFO]  Calculate Szymkiewicz–Simpson coefficient (overall) ...
  A.name               CTCF_ENCFF660GHM.bed
  B.name              RAD21_ENCFF057JFH.bed
  A.interval_count                    58684
@@ -77,22 +97,18 @@
  Coef(95% CI)              [0.4413,0.4475]
  dtype: object
  2022-01-16 08:53:09 [INFO]  Calculate Szymkiewicz–Simpson coefficient (peakwise) ...
  2022-01-16 08:53:09 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-16 08:53:10 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed" : 58584
  2022-01-16 08:53:10 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-16 08:53:10 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed" : 31955
- 2022-01-16 08:53:10 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed"
- 2022-01-16 08:53:10 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed"
- 2022-01-16 08:53:10 [INFO]  Calculate the overlap coefficient of each genomic region in CTCF_ENCFF660GHM.bed ...
- 2022-01-16 08:53:12 [INFO]  Save peakwise scores to CTCF_ENCFF660GHM.bed_peakwise_scores.tsv ...
- 2022-01-16 08:53:12 [INFO]  Calculate the overlap coefficient of each genomic region in RAD21_ENCFF057JFH.bed ...
- 2022-01-16 08:53:14 [INFO]  Save peakwise scores to RAD21_ENCFF057JFH.bed_peakwise_scores.tsv ...
+ ...
+
+If :code:`--save` was specified, the peakwise coefficients were saved to :code:`CTCF_ENCFF660GHM.bed_peakwise_scores.tsv` and :code:`RAD21_ENCFF057JFH.bed_peakwise_scores.tsv`, respectively.
 
-If :code:`--save` was specified, the peakwise coefficients were saved to *CTCF_ENCFF660GHM.bed_peakwise_scores.tsv* and *RAD21_ENCFF057JFH.bed_peakwise_scores.tsv*, respectively.
 ::
 
  $ head -5 CTCF_ENCFF660GHM.bed_peakwise_scores.tsv
   
  chrom start end A.size  B.size  A∩B A∪B B.list  Score
  chr12 108043  108283  240 404 240 404 chr12:107919-108323 1.0
  chr12 153232  153470  238 222 222 238 chr12:153236-153458 1.0
```

### Comparing `cobind-1.0.0/docs/usage/cooccur.rst` & `cobind-1.0.1/docs/usage/cooccur.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Cooccurrence
 ============
 
 Description
 -------------
-Use `Fisher's exact test <https://en.wikipedia.org/wiki/Fisher%27s_exact_test>`_ to evaluate if two sets of genomic intervals (A and B) are significantly cooccured [#f1]_. Genomic intervals (**g**) in the background BED file will be divided into 4 groups: **a** (A specific), **b** (B specific), **c** (i.e., A and B cooccur), and **n** (neith A nor B). 
+Use `Fisher's exact test <https://en.wikipedia.org/wiki/Fisher%27s_exact_test>`_ to evaluate if two sets of genomic intervals (A and B) are significantly cooccured [#f1]_. Genomic intervals (**g**) in the background BED file will be divided into 4 groups: **a** (A specific), **b** (B specific), **c** (A and B cooccur), and **n** (neith A nor B). 
 
 +------------+--------+------+--------------------+
 |            | Not A  | A    | Total              |
 +============+========+======+====================+
 | **Not B**  | n      | a    | n+a                |
 +------------+--------+------+--------------------+
 | **B**      | b      | c    | b+c                |
@@ -32,44 +32,66 @@
 
 Usage
 -----
 
 :code:`cobind.py cooccur -h`
 
 ::
- 
- usage: cobind.py cooccur [-h] [--ncut N_CUT] [--pcut P_CUT] [-d] [--dist MAX_DIST] input_A.bed input_B.bed background.bed output.tsv
- 
+
+ usage: cobind.py cooccur [-h] [--nameA NAMEA] [--nameB NAMEB] [--ncut N_CUT]
+                          [--pcut P_CUT] [-l log_file] [-d]
+                          input_A.bed input_B.bed background.bed output.tsv
+
  positional arguments:
-   input_A.bed      Genomic regions in BED, BED-like or bigBed format. The BED-like format includes: 'bed3', 'bed4', 'bed6', 'bed12',
-                    'bedgraph', 'narrowpeak', 'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text, compressed (.gz,
-                    .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress BigBed foramt. BigBed file
-                    can also be a remote file.
-   input_B.bed      Genomic regions in BED, BED-like or bigBed format. The BED-like format includes: 'bed3', 'bed4', 'bed6', 'bed12',
-                    'bedgraph', 'narrowpeak', 'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text, compressed (.gz,
-                    .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress BigBed foramt. BigBed file
-                    can also be a remote file.
-   background.bed   Genomic regions as the background (e.g., all promoters, all enhancers).
-   output.tsv       For each genomic region in the "background.bed" file, add another column indicating if this region is "input_A
-                    specific (i.e., A+B-)", "input_B specific (i.e., A-B+)", "co-occur (i.e., A+B+)" or "neither (i.e, A-B-)".
- 
- optional arguments:
-   -h, --help       show this help message and exit
-   --ncut N_CUT     The minimum overlap size. (default: 1)
-   --pcut P_CUT     The minimum overlap percentage. (default: 0.000000)
-   -d, --debug      Print detailed information for debugging.
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   background.bed        Genomic regions as the background (e.g., all
+                         promoters, all enhancers).
+   output.tsv            For each genomic region in the "background.bed" file,
+                         add another column indicating if this region is
+                         "input_A specific (i.e., A+B-)", "input_B specific
+                         (i.e., A-B+)", "co-occur (i.e., A+B+)" or "neither
+                         (i.e, A-B-)".
+
+ options:
+   -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified "A" will be used.
+   --nameB NAMEB         Name to represent 2nd set of genomic interval. If not
+                         specified "B" will be used.
+   --ncut N_CUT          The minimum overlap size. (default: 1)
+   --pcut P_CUT          The minimum overlap percentage. (default: 0.000000)
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
+   -d, --debug           Print detailed information for debugging.
 
 
 Example
 -------
 
 :code:`cobind.py cooccur CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed hg38_gene_hancer_v4.4.bed output.tsv`
 
 ::
-
+ 
  2022-01-20 01:24:40 [INFO]  Calculate the co-occurrence of two sets of genomic intervals ...
  2022-01-20 01:24:40 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-20 01:24:41 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-20 01:24:41 [INFO]  Read and union background BED file: "hg38_gene_hancer_v4.4.bed"
  2022-01-20 01:24:42 [INFO]  Build interval tree for : "CTCF_ENCFF660GHM.bed"
  2022-01-20 01:24:42 [INFO]  Build interval tree for: "RAD21_ENCFF057JFH.bed"
  A.name         CTCF_ENCFF660GHM.bed
@@ -98,8 +120,8 @@
 A+,B+ 
   Number of unique genomic intervals that are overlapped with both A and B (**c**).
 A-,B- 
   Number of unique genomic intervals that are overlapped with neither A nor B (**n**).
 
 
 
-.. [#f1] Note: "cooccur" does NOT necessarily mean "overlap". For example, two transcription factors could bind to the same promoter region without touching each other. 
+.. [#f1] Note: "cooccur" does NOT necessarily mean "overlap" or "cobinding". For example, two transcription factors could bind to the same promoter region without touching each other.
```

### Comparing `cobind-1.0.0/docs/usage/covary.rst` & `cobind-1.0.1/docs/usage/covary.rst`

 * *Files 16% similar despite different names*

```diff
@@ -11,87 +11,116 @@
 Usage
 -----
 
 :code:`cobind.py covary -h`
 
 ::
  
- usage: cobind.py covary [-h] [--na NA_LABEL] [--type {mean,min,max}] [--topx TOP_X] [--min_sig MIN_SIGNAL] [--exact] [--keepna] [-d]
-                         input_A.bed input_A.bw input_B.bed input_B.bw output_prefix
+ usage: cobind.py covary [-h] [--nameA NAMEA] [--nameB NAMEB] [--na NA_LABEL]
+                         [--type {mean,min,max}] [--topx TOP_X]
+                         [--min_sig MIN_SIGNAL] [--exact] [--keepna]
+                         [-l log_file] [-d]
+                         input_A.bed input_A.bw input_B.bed input_B.bw
+                         output_prefix
  
  positional arguments:
-   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format includes: 'bed3', 'bed4', 'bed6',
-                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                         compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress BigBed
-                         foramt. BigBed file can also be a remote file.
-   input_A.bw            Input bigWig file matched to 'input_A.bed'. BigWig file can be local or remote. Note: the chromosome IDs must
-                         be consistent between BED and bigWig files.
-   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format includes: 'bed3', 'bed4', 'bed6',
-                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                         compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress BigBed
-                         foramt. BigBed file can also be a remote file.
-   input_B.bw            Input bigWig file matched to 'input_B.bed'. BigWig file can be local or remote. Note: the chromosome IDs must
-                         be consistent between BED and bigWig files.
-   output_prefix         Prefix of output files. Three files will be generated: "output_prefix_bedA_unique.tsv" (input_A.bed specific
-                         regions and their bigWig scores), "output_prefix_bedB_unique.tsv" (input_B.bed specific regions and their
-                         bigWig scores), and "output_prefix_common.tsv"(input_A.bed and input_B.bed overlapped regions and their
-                         bigWig scores). 
- 
- optional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_A.bw            Input bigWig file matched to 'input_A.bed'. BigWig
+                         file can be local or remote. Note: the chromosome IDs
+                         must be consistent between BED and bigWig files.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bw            Input bigWig file matched to 'input_B.bed'. BigWig
+                         file can be local or remote. Note: the chromosome IDs
+                         must be consistent between BED and bigWig files.
+   output_prefix         Prefix of output files. Three files will be generated:
+                         "output_prefix_bedA_unique.tsv" (input_A.bed specific
+                         regions and their bigWig scores),
+                         "output_prefix_bedB_unique.tsv" (input_B.bed specific
+                         regions and their bigWig scores), and
+                         "output_prefix_common.tsv"(input_A.bed and input_B.bed
+                         overlapped regions and their bigWig scores).
+
+ options:
    -h, --help            show this help message and exit
-   --na NA_LABEL         Symbols used to represent the missing values. (default: nan)
+   --nameA NAMEA         Name of the 1st set of genomic interval, if not
+                         proviced, "bedA" will be used. Only affects the name
+                         of output file.
+   --nameB NAMEB         Name of the 2nd set of genomic interval, if not
+                         proviced, "bedB" will be used. Only affects the name
+                         of output file.
+   --na NA_LABEL         Symbols used to represent the missing values.
+                         (default: nan)
    --type {mean,min,max}
-                         Summary statistic score type ('min','mean' or 'max') of a genomic region. (default: mean)
-   --topx TOP_X          Fraction (if 0 < top_X <= 1) or number (if top_X > 1) of genomic regions used to calculate Pearson, Spearman,
-                         Kendall's correlations. If TOP_X == 1 (i.e., 100%), all the genomic regions will be used to calculate
-                         correlations. (default: 1.0)
-   --min_sig MIN_SIGNAL  Genomic region with summary statistic score <= this will be removed. (default: 0)
-   --exact               If set, calculate the "exact" summary statistic score rather than "zoom-level" score for each genomic region.
-   --keepna              If set, a genomic region will be kept even it does not have summary statistical score in either of the two
-                         bigWig files. This flag only affects the output TSV files.
+                         Summary statistic score type ('min','mean' or 'max')
+                         of a genomic region. (default: mean)
+   --topx TOP_X          Fraction (if 0 < top_X <= 1) or number (if top_X > 1)
+                         of genomic regions used to calculate Pearson,
+                         Spearman, Kendall's correlations. If TOP_X == 1 (i.e.,
+                         100%), all the genomic regions will be used to
+                         calculate correlations. (default: 1.0)
+   --min_sig MIN_SIGNAL  Genomic region with summary statistic score <= this
+                         will be removed. (default: 0)
+   --exact               If set, calculate the "exact" summary statistic score
+                         rather than "zoom-level" score for each genomic
+                         region.
+   --keepna              If set, a genomic region will be kept even it does not
+                         have summary statistical score in either of the two
+                         bigWig files. This flag only affects the output TSV
+                         files.
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
    -d, --debug           Print detailed information for debugging.
 
 Example
 -------
 
-:code:`cobind.py covary CTCF_ENCFF660GHM.bed3 CTCF_ENCFF682MFJ_FC.bigWig RAD21_ENCFF057JFH.bed3 RAD21_ENCFF130GMP.bigWig output`
+::
+ 
+ cobind.py covary CTCF_ENCFF660GHM.bed3 CTCF_ENCFF682MFJ_FC.bigWig RAD21_ENCFF057JFH.bed3 
+ RAD21_ENCFF130GMP.bigWig output
+
 
 ::
  
  2022-01-20 02:56:53 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed3"
  2022-01-20 02:56:54 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed3" : 58584
  2022-01-20 02:56:54 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed3"
  2022-01-20 02:56:54 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed3" : 31955
- 2022-01-20 02:56:54 [INFO]  Merge BED files "CTCF_ENCFF660GHM.bed3" and "RAD21_ENCFF057JFH.bed3"
- 2022-01-20 02:56:55 [INFO]  Unioned regions of two BED files : 62303
- 2022-01-20 02:56:55 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed3"
- 2022-01-20 02:56:55 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed3"
- 2022-01-20 02:56:55 [INFO]  Find common and specific regions ...
- 2022-01-20 02:56:55 [INFO]  "CTCF_ENCFF660GHM.bed3" unique regions: 30350
- 2022-01-20 02:56:55 [INFO]  "RAD21_ENCFF057JFH.bed3" unique regions: 3824
- 2022-01-20 02:56:55 [INFO]  Common (overlapped) regions: 28129
- 2022-01-20 02:56:55 [INFO]  Calculate covariabilities of overlapped regions ...
- 2022-01-20 02:57:06 [INFO]  Sort dataframe by summary statistical scores ...
- 2022-01-20 02:57:06 [INFO]  Save dataframe to: "output_common.tsv"
- 2022-01-20 02:57:06 [INFO]  Note: NumExpr detected 16 cores but "NUMEXPR_MAX_THREADS" not set, so enforcing safe limit of 8.
- 2022-01-20 02:57:06 [INFO]  NumExpr defaulting to 8 threads.
- 2022-01-20 02:57:06 [INFO]  Select 28129 regions ...
+ ...
                 Correlation  P-value
  Pearson_cor:        0.6378   0.0000
  Spearman_rho:       0.6355   0.0000
  Kendall_tau:        0.4406   0.0000
- 2022-01-20 02:57:06 [INFO]  Calculate covariabilities of "CTCF_ENCFF660GHM.bed3" unique regions ...
+ 2022-01-20 02:57:06 [INFO]  Calculate covariabilities of "CTCF_ENCFF660GHM.bed3"
+                             unique regions ...
  2022-01-20 02:57:16 [INFO]  Sort dataframe by summary statistical scores ...
  2022-01-20 02:57:16 [INFO]  Save dataframe to: "output_bedA_unique.tsv"
  2022-01-20 02:57:16 [INFO]  Select 30347 regions ...
                 Correlation  P-value
  Pearson_cor:        0.3356   0.0000
  Spearman_rho:       0.3667   0.0000
  Kendall_tau:        0.2489   0.0000
- 2022-01-20 02:57:16 [INFO]  Calculate covariabilities of "RAD21_ENCFF057JFH.bed3" unique regions ...
+ 2022-01-20 02:57:16 [INFO]  Calculate covariabilities of "RAD21_ENCFF057JFH.bed3"
+                             unique regions ...
  2022-01-20 02:57:18 [INFO]  Sort dataframe by summary statistical scores ...
  2022-01-20 02:57:18 [INFO]  Save dataframe to: "output_bedB_unique.tsv"
  2022-01-20 02:57:18 [INFO]  Select 3822 regions ...
                 Correlation  P-value
  Pearson_cor:        0.2511   0.0000
  Spearman_rho:       0.2261   0.0000
  Kendall_tau:        0.1534   0.0000
```

### Comparing `cobind-1.0.0/docs/usage/jaccard.rst` & `cobind-1.0.1/docs/usage/jaccard.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,52 +16,74 @@
 
 Usage
 -----
 
 :code:`cobind.py jacard -h`
 
 ::
-
- usage: cobind.py jaccard [-h] [-n ITER] [-f SUBSAMPLE] [-b BGSIZE] [-o] [-d] input_A.bed input_B.bed
  
+ usage: cobind.py jaccard [-h] [--nameA NAMEA] [--nameB NAMEB] [-n ITER]
+                          [-f SUBSAMPLE] [-b BGSIZE] [-o] [-l log_file] [-d]
+                          input_A.bed input_B.bed
+
  positional arguments:
-   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                         includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                         'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                         compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://)
-                         files. Do not compress BigBed foramt. BigBed file can also be a remote file.
-   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The BED-like format
-                         includes: 'bed3', 'bed4', 'bed6', 'bed12', 'bedgraph', 'narrowpeak',
-                         'broadpeak', 'gappedpeak'. BED and BED-like format can be plain text,
-                         compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://)
-                         files. Do not compress BigBed foramt. BigBed file can also be a remote file.
- 
- optional arguments:
+   input_A.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+   input_B.bed           Genomic regions in BED, BED-like or bigBed format. The
+                         BED-like format includes:'bed3', 'bed4', 'bed6',
+                         'bed12', 'bedgraph', 'narrowpeak', 'broadpeak',
+                         'gappedpeak'. BED and BED-like format can be plain
+                         text, compressed (.gz, .z, .bz, .bz2, .bzip2) or
+                         remote (http://, https://, ftp://) files. Do not
+                         compress BigBed foramt. BigBed file can also be a
+                         remote file.
+
+ options:
    -h, --help            show this help message and exit
+   --nameA NAMEA         Name to represent 1st set of genomic interval. If not
+                         specified (None), the file name ("input_A.bed") will
+                         be used.
+   --nameB NAMEB         Name to represent the 2nd set of genomic interval. If
+                         not specified (None), the file name ("input_B.bed")
+                         will be used.
    -n ITER, --ndraws ITER
-                         Times of resampling to estimate confidence intervals. Set to '0' to turn off
-                         resampling.(default: 20)
+                         Times of resampling to estimate confidence intervals.
+                         Set to '0' to turn off resampling. For the resampling
+                         process to work properly, overlapped intervals in each
+                         bed file must be merged. (default: 20)
    -f SUBSAMPLE, --fraction SUBSAMPLE
                          Resampling fraction. (default: 0.75)
    -b BGSIZE, --background BGSIZE
-                         The size of the cis-regulatory genomic regions. This is about 1.4Gb For the
-                         human genome. (default: 1400000000)
+                         The size of the cis-regulatory genomic regions. This
+                         is about 1.4Gb For the human genome. (default:
+                         1400000000)
    -o, --save            If set, will save peak-wise coefficients to files
-                         ("input_A_peakwise_scores.tsv" and "input_B_peakwise_scores.tsv").
+                         ("input_A_peakwise_scores.tsv" and
+                         "input_B_peakwise_scores.tsv").
+   -l log_file, --log log_file
+                         This file is used to save the log information. By
+                         default, if no file is specified (None), the log
+                         information will be printed to the screen.
    -d, --debug           Print detailed information for debugging.
 
-
 Example
 -------
 
-Calculate the **overall** `Jaccard coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_ and **peak-wise** `Jaccard coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_ between CTCF binding sites and RAD21 binding sites.
+Calculate the **overall** `Jaccard coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_ and **peak-wise** `Jaccard coefficient <https://en.wikipedia.org/wiki/Jaccard_index>`_ between `CTCF binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#ctcf-chip-seq>`_ and `RAD21 binding sites <https://cobind.readthedocs.io/en/latest/dataset.html#rad21-chip-seq>`_.
+
 
 :code:`python3 ../bin/cobind.py jaccard CTCF_ENCFF660GHM.bed RAD21_ENCFF057JFH.bed --save`
 
-The overall Jaccard coefficient between *CTCF_ENCFF660GHM.bed* and *RAD21_ENCFF057JFH.bed* was printed to screen
+The overall Jaccard coefficient between :code:`CTCF_ENCFF660GHM.bed` and :code:`RAD21_ENCFF057JFH.bed` was printed to screen
 
 ::
 
  2022-01-16 08:24:12 [INFO]  Calculate Jaccard coefficient (overall) ...
  A.name               CTCF_ENCFF660GHM.bed
  B.name              RAD21_ENCFF057JFH.bed
  A.interval_count                    58684
@@ -75,23 +97,17 @@
  Coef(95% CI)              [0.2672,0.2713]
  dtype: object
  2022-01-16 08:24:40 [INFO]  Calculate Jaccard coefficient (peakwise) ...
  2022-01-16 08:24:40 [INFO]  Read and union BED file: "CTCF_ENCFF660GHM.bed"
  2022-01-16 08:24:40 [INFO]  Unioned regions of "CTCF_ENCFF660GHM.bed" : 58584
  2022-01-16 08:24:40 [INFO]  Read and union BED file: "RAD21_ENCFF057JFH.bed"
  2022-01-16 08:24:41 [INFO]  Unioned regions of "RAD21_ENCFF057JFH.bed" : 31955
- 2022-01-16 08:24:41 [INFO]  Build interval tree for unioned BED file: "CTCF_ENCFF660GHM.bed"
- 2022-01-16 08:24:41 [INFO]  Build interval tree for unioned BED file: "RAD21_ENCFF057JFH.bed"
- 2022-01-16 08:24:41 [INFO]  Calculate the overlap coefficient of each genomic region in CTCF_ENCFF660GHM.bed ...
- 2022-01-16 08:24:43 [INFO]  Save peakwise scores to CTCF_ENCFF660GHM.bed_peakwise_scores.tsv ...
- 2022-01-16 08:24:43 [INFO]  Calculate the overlap coefficient of each genomic region in RAD21_ENCFF057JFH.bed ...
- 2022-01-16 08:24:44 [INFO]  Save peakwise scores to RAD21_ENCFF057JFH.bed_peakwise_scores.tsv ...
-
+ ...
 
-If :code:`--save` was specified, the peakwise coefficients were saved to *CTCF_ENCFF660GHM.bed_peakwise_scores.tsv* and *RAD21_ENCFF057JFH.bed_peakwise_scores.tsv*, respectively.
+If :code:`--save` was specified, the peakwise coefficients were saved to :code:`CTCF_ENCFF660GHM.bed_peakwise_scores.tsv` and :code:`RAD21_ENCFF057JFH.bed_peakwise_scores.tsv`, respectively.
 ::
 
  $ head -5 CTCF_ENCFF660GHM.bed_peakwise_scores.tsv
   
  chrom start end A.size  B.size  A∩B A∪B B.list  Score
  chr12 108043  108283  240 404 240 404 chr12:107919-108323 0.594059405940594
  chr12 153232  153470  238 222 222 238 chr12:153236-153458 0.9327731092436975
```

### Comparing `cobind-1.0.0/lib/cobind.egg-info/PKG-INFO` & `cobind-1.0.1/lib/cobind.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: cobind
-Version: 1.0.0
-Summary: collocation analysis of genomics regions
+Version: 1.0.1
+Summary: collocation analysis of genomics intervals
 Home-page: https://cobind.readthedocs.io/en/latest/
 Author: Liguo Wang
 Author-email: wangliguo78@gmail.com
-License: UNKNOWN
-Keywords: genome regions,overlap coefficient,cooccur,pointwise mutual information
+Keywords: genome regions,collocation,overlap,cooccur
 Platform: Linux
 Platform: MacOS
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.5
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `cobind-1.0.0/lib/cobind.egg-info/SOURCES.txt` & `cobind-1.0.1/lib/cobind.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 .gitattributes
 .gitignore
 LICENSE
 README.md
 setup.py
 bin/cobind.py
 docs/Makefile
+docs/acknowledgements.rst
 docs/change_log.rst
+docs/comparison.rst
 docs/conf.py
+docs/contact.rst
 docs/dataset.rst
 docs/definition.rst
 docs/index.rst
 docs/input_format.rst
 docs/installation.rst
 docs/introduction.rst
 docs/license.rst
 docs/make.bat
+docs/performance.rst
 docs/reference.rst
 docs/_static/SD_1.jpeg
 docs/_static/SD_1.jpg
 docs/_static/SD_1.png
 docs/_static/SD_2.jpeg
 docs/_static/SD_2.jpg
 docs/_static/SD_2.png
@@ -26,22 +30,26 @@
 docs/_static/SS_bound.jpg
 docs/_static/fisher_or.jpg
 docs/_static/fisher_p.jpg
 docs/_static/jaccard_1.jpg
 docs/_static/jaccard_2.jpg
 docs/_static/jaccard_3.jpg
 docs/_static/logo.png
+docs/_static/logo2.png
+docs/_static/logo3.png
 docs/_static/npmi.jpg
 docs/_static/npmi_bound.jpg
 docs/_static/ov_coef_1.jpg
 docs/_static/ov_coef_2.jpg
 docs/_static/ov_coef_3.jpg
 docs/_static/p.jpg
 docs/_static/pmi.jpg
 docs/_static/pmi_bound.jpg
+docs/_static/rank_comparison.png
+docs/_static/score_comparison.png
 docs/_static/set_symbols.jpg
 docs/_static/srog.jpg
 docs/usage/NPMI.rst
 docs/usage/PMI.rst
 docs/usage/SD.rst
 docs/usage/SROG.rst
 docs/usage/SS.rst
@@ -62,22 +70,23 @@
 lib/cobindability/bbreader.py
 lib/cobindability/bbreader.py~
 lib/cobindability/bw.py
 lib/cobindability/coefcal.py
 lib/cobindability/findbed.py
 lib/cobindability/ireader.py
 lib/cobindability/ovbootstrap.py
-lib/cobindability/ovcovary.py
 lib/cobindability/ovstat.py
+lib/cobindability/utils.py
 lib/cobindability/version.py
 lib/cobindability/__pycache__/BED.cpython-38.pyc
 lib/cobindability/__pycache__/__init__.cpython-38.pyc
 lib/cobindability/__pycache__/bbreader.cpython-38.pyc
 lib/cobindability/__pycache__/bw.cpython-38.pyc
 lib/cobindability/__pycache__/coefcal.cpython-38.pyc
 lib/cobindability/__pycache__/ireader.cpython-38.pyc
 lib/cobindability/__pycache__/ovbootstrap.cpython-38.pyc
 lib/cobindability/__pycache__/ovcoef.cpython-38.pyc
 lib/cobindability/__pycache__/ovjaccard.cpython-38.pyc
 lib/cobindability/__pycache__/ovpmi.cpython-38.pyc
 lib/cobindability/__pycache__/ovstat.cpython-38.pyc
-lib/cobindability/__pycache__/version.cpython-38.pyc
+lib/cobindability/__pycache__/version.cpython-38.pyc
+test/test_bed.py
```

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/BED.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/BED.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Jan 18 03:45:04 2022 UTC, .py size: 31577 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 c037 e661 597b 0000  U........7.aY{..
+00000000: 550d 0d0a 0000 0000 b453 1462 147c 0000  U........S.b.|..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 4c01 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a06 6400 6402 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c09 6d0a 5a0a 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 6d0d 5a0d 0100 6400  d.l.m.Z.m.Z...d.
@@ -26,18 +26,18 @@
 00000190: da0c 6669 7368 6572 5f65 7861 6374 2902  ..fisher_exact).
 000001a0: da18 6269 6e6e 6564 5f62 6974 7365 7473  ..binned_bitsets
 000001b0: 5f66 726f 6d5f 6669 6c65 da18 6269 6e6e  _from_file..binn
 000001c0: 6564 5f62 6974 7365 7473 5f66 726f 6d5f  ed_bitsets_from_
 000001d0: 6c69 7374 2902 da08 496e 7465 7276 616c  list)...Interval
 000001e0: da0b 496e 7465 7273 6563 7465 7229 02da  ..Intersecter)..
 000001f0: 0769 7265 6164 6572 da07 7665 7273 696f  .ireader..versio
-00000200: 6e7a 0a4c 6967 756f 2057 616e 67da 0843  nz.Liguo Wang..C
+00000200: 6e7a 0a4c 6967 756f 2057 616e 675a 0843  nz.Liguo WangZ.C
 00000210: 6f70 796c 6566 745a 034d 4954 7a13 7761  opyleftZ.MITz.wa
 00000220: 6e67 2e6c 6967 756f 406d 6179 6f2e 6564  ng.liguo@mayo.ed
-00000230: 75da 0b44 6576 656c 6f70 6d65 6e74 6301  u..Developmentc.
+00000230: 755a 0b44 6576 656c 6f70 6d65 6e74 6301  uZ.Developmentc.
 00000240: 0000 0000 0000 0000 0000 0007 0000 0007  ................
 00000250: 0000 0043 0000 0073 da00 0000 6700 7d01  ...C...s....g.}.
 00000260: 7400 7c00 8301 7401 6b08 722a 7402 7c00  t.|...t.k.r*t.|.
 00000270: 8301 6401 6b02 7220 7c01 5300 7403 7c00  ..d.k.r |.S.t.|.
 00000280: 8301 7d02 6e5e 7400 7c00 8301 7404 6b08  ..}.n^t.|...t.k.
 00000290: 7270 7a12 7405 7406 a007 7c00 a101 8301  rpz.t.t...|.....
 000002a0: 7d02 5700 7188 0100 0100 0100 7408 a009  }.W.q.......t...
@@ -45,1455 +45,1466 @@
 000002c0: a101 0100 5900 7188 5800 6e18 7408 a009  ....Y.q.X.n.t...
 000002d0: 6402 7c00 1600 a101 0100 740a a00b 6403  d.|.......t...d.
 000002e0: a101 0100 7c02 4400 5d42 7d03 7c02 7c03  ....|.D.]B}.|.|.
 000002f0: 1900 7d04 6401 7d05 7c04 a00c 7c05 a101  ..}.d.}.|...|...
 00000300: 7d06 7c06 7c04 6a0d 6b02 72b2 718c 7c04  }.|.|.j.k.r.q.|.
 00000310: a00e 7c06 a101 7d05 7c01 a00f 7c03 7c06  ..|...}.|...|.|.
 00000320: 7c05 6603 a101 0100 719c 718c 7410 8300  |.f.....q.q.t...
-00000330: 7d02 7c01 5300 2904 6139 0200 000a 094d  }.|.S.).a9.....M
-00000340: 6572 6765 2f75 6e69 6f6e 2067 656e 6f6d  erge/union genom
-00000350: 6963 2069 6e74 6572 7661 6c73 2e20 4966  ic intervals. If
-00000360: 2069 6e70 7574 2069 7320 6120 4245 4420   input is a BED 
-00000370: 6669 6c65 2c20 6f6e 6c79 2063 6f6e 7369  file, only consi
-00000380: 6465 7220 7468 650a 0966 6972 7374 2074  der the..first t
-00000390: 6872 6565 2063 6f6c 756d 6e73 2028 6368  hree columns (ch
-000003a0: 726f 6d2c 2073 7461 7274 2c20 656e 6429  rom, start, end)
-000003b0: 2c20 6f74 6865 7220 636f 6c75 6d6e 7320  , other columns 
-000003c0: 7769 6c6c 2062 6520 6967 6e6f 7265 642e  will be ignored.
-000003d0: 0a0a 0950 6172 616d 6574 6572 730a 092d  ...Parameters..-
-000003e0: 2d2d 2d2d 2d2d 2d2d 2d0a 0969 6e62 6564  ---------..inbed
-000003f0: 203a 2073 7472 206f 7220 6c69 7374 0a09   : str or list..
-00000400: 094e 616d 6520 6f66 2061 2042 4544 2066  .Name of a BED f
-00000410: 696c 6520 6f72 206c 6973 7420 6f66 2067  ile or list of g
-00000420: 656e 6f6d 6963 2069 6e74 6572 7661 6c73  enomic intervals
-00000430: 2028 666f 7220 6578 616d 706c 652c 0a09   (for example,..
-00000440: 095b 2863 6872 3120 3130 3020 3230 3029  .[(chr1 100 200)
-00000450: 2c20 2863 6872 3220 3135 3020 2033 3030  , (chr2 150  300
-00000460: 292c 2028 6368 7232 2031 3030 3020 3132  ), (chr2 1000 12
-00000470: 3030 295d 290a 0a09 5265 7475 726e 730a  00)])...Returns.
-00000480: 092d 2d2d 2d2d 2d2d 0a09 756e 696f 6e65  .-------..unione
-00000490: 645f 696e 7465 7276 616c 7320 3a20 6c69  d_intervals : li
-000004a0: 7374 0a09 094c 6973 7420 6f66 2067 656e  st...List of gen
-000004b0: 6f6d 6963 2069 6e74 6572 7661 6c73 2077  omic intervals w
-000004c0: 6974 6820 7468 6520 6f76 6572 6c61 7070  ith the overlapp
-000004d0: 6564 2072 6567 696f 6e73 206d 6572 6765  ed regions merge
-000004e0: 642e 0a0a 0945 7861 6d70 6c65 730a 092d  d....Examples..-
-000004f0: 2d2d 2d2d 2d2d 2d0a 093e 3e3e 2075 6e69  -------..>>> uni
-00000500: 6f6e 4265 6433 285b 2827 6368 7231 272c  onBed3([('chr1',
-00000510: 2031 2c20 3130 292c 2028 2763 6872 3127   1, 10), ('chr1'
-00000520: 2c20 332c 2031 3529 2c20 2827 6368 7231  , 3, 15), ('chr1
-00000530: 272c 2032 302c 2033 3529 2c20 2827 6368  ', 20, 35), ('ch
-00000540: 7231 272c 2032 302c 2035 3029 5d29 0a09  r1', 20, 50)])..
-00000550: 5b28 2763 6872 3127 2c20 312c 2031 3529  [('chr1', 1, 15)
-00000560: 2c20 2827 6368 7231 272c 2032 302c 2035  , ('chr1', 20, 5
-00000570: 3029 5d0a 0a09 7201 0000 00fa 1169 6e76  0)]...r......inv
-00000580: 616c 6964 2069 6e70 7574 3a20 2573 e901  alid input: %s..
-00000590: 0000 0029 11da 0474 7970 65da 046c 6973  ...)...type..lis
-000005a0: 74da 036c 656e 7205 0000 00da 0373 7472  t..lenr......str
-000005b0: 7204 0000 0072 0800 0000 da06 7265 6164  r....r......read
-000005c0: 6572 da07 6c6f 6767 696e 67da 0565 7272  er..logging..err
-000005d0: 6f72 da03 7379 73da 0465 7869 74da 086e  or..sys..exit..n
-000005e0: 6578 745f 7365 74da 0473 697a 65da 0a6e  ext_set..size..n
-000005f0: 6578 745f 636c 6561 72da 0661 7070 656e  ext_clear..appen
-00000600: 64da 0464 6963 7429 075a 0569 6e62 6564  d..dict).Z.inbed
-00000610: 5a11 756e 696f 6e65 645f 696e 7465 7276  Z.unioned_interv
-00000620: 616c 73da 0762 6974 7365 7473 da05 6368  als..bitsets..ch
-00000630: 726f 6dda 0462 6974 73da 0365 6e64 da05  rom..bits..end..
-00000640: 7374 6172 74a9 0072 2100 0000 fa3f 2f55  start..r!....?/U
-00000650: 7365 7273 2f6d 3130 3233 3234 2f44 6f63  sers/m102324/Doc
-00000660: 756d 656e 7473 2f47 6974 4875 622f 636f  uments/GitHub/co
-00000670: 6269 6e64 2f6c 6962 2f63 6f62 696e 6461  bind/lib/cobinda
-00000680: 6269 6c69 7479 2f42 4544 2e70 79da 0975  bility/BED.py..u
-00000690: 6e69 6f6e 4265 6433 1700 0000 732e 0000  nionBed3....s...
-000006a0: 0000 1604 010c 010c 0104 020a 010c 0102  ................
-000006b0: 0112 0106 010e 0112 020e 010a 0208 0108  ................
-000006c0: 0104 020a 010a 0002 010a 0114 0106 0172  ...............r
-000006d0: 2300 0000 6302 0000 0000 0000 0000 0000  #...c...........
-000006e0: 000b 0000 0007 0000 0043 0000 0073 b201  .........C...s..
-000006f0: 0000 6700 7d02 7400 7c00 8301 7401 6b08  ..g.}.t.|...t.k.
-00000700: 722a 7402 7c00 8301 6401 6b02 7220 7c02  r*t.|...d.k.r |.
-00000710: 5300 7403 7c00 8301 7d03 6e5e 7400 7c00  S.t.|...}.n^t.|.
-00000720: 8301 7404 6b08 7270 7a12 7405 7406 a007  ..t.k.rpz.t.t...
-00000730: 7c00 a101 8301 7d03 5700 7188 0100 0100  |.....}.W.q.....
-00000740: 0100 7408 a009 6402 7c00 1600 a101 0100  ..t...d.|.......
-00000750: 740a a00b 6403 a101 0100 5900 7188 5800  t...d.....Y.q.X.
-00000760: 6e18 7408 a009 6402 7c00 1600 a101 0100  n.t...d.|.......
-00000770: 740a a00b 6403 a101 0100 7400 7c01 8301  t...d.....t.|...
-00000780: 7401 6b08 72ae 7402 7c01 8301 6401 6b02  t.k.r.t.|...d.k.
-00000790: 72a4 7c02 5300 7403 7c01 8301 7d04 6e5e  r.|.S.t.|...}.n^
-000007a0: 7400 7c01 8301 7404 6b08 72f4 7a12 7405  t.|...t.k.r.z.t.
-000007b0: 7406 a007 7c01 a101 8301 7d04 5700 6e24  t...|.....}.W.n$
-000007c0: 0100 0100 0100 7408 a009 6402 7c01 1600  ......t...d.|...
-000007d0: a101 0100 740a a00b 6403 a101 0100 5900  ....t...d.....Y.
-000007e0: 6e02 5800 6e18 7408 a009 6402 7c01 1600  n.X.n.t...d.|...
-000007f0: a101 0100 740a a00b 6403 a101 0100 740c  ....t...d.....t.
-00000800: 8300 7d05 7c03 4400 5d2e 7d06 7c06 7c04  ..}.|.D.].}.|.|.
-00000810: 6b06 9001 7216 7c03 7c06 1900 a00d 7c04  k...r.|.|.....|.
-00000820: 7c06 1900 a101 0100 7c03 7c06 1900 7c05  |.......|.|...|.
-00000830: 7c06 3c00 9001 7116 7c05 4400 5d4a 7d07  |.<...q.|.D.]J}.
-00000840: 7c05 7c07 1900 7d08 6401 7d09 7c08 a00e  |.|...}.d.}.|...
-00000850: 7c09 a101 7d0a 7c0a 7c08 6a0f 6b02 9001  |...}.|.|.j.k...
-00000860: 7274 9001 714a 7c08 a010 7c0a a101 7d09  rt..qJ|...|...}.
-00000870: 7c02 a011 7c07 7c0a 7c09 6603 a101 0100  |...|.|.|.f.....
-00000880: 9001 715a 9001 714a 7c03 a012 a100 0100  ..qZ..qJ|.......
-00000890: 7c04 a012 a100 0100 7c05 a012 a100 0100  |.......|.......
-000008a0: 7c02 5300 2904 6114 0300 000a 0952 6574  |.S.).a......Ret
-000008b0: 7572 6e20 7468 6520 7368 6172 6564 2067  urn the shared g
-000008c0: 656e 6f6d 6963 2069 6e74 6572 7661 6c73  enomic intervals
-000008d0: 2062 6565 7477 6565 6e20 696e 6265 6431   beetween inbed1
-000008e0: 2061 6e64 2069 6e62 6564 322e 2049 6e70   and inbed2. Inp
-000008f0: 7574 7320 6172 650a 0974 776f 2042 4544  uts are..two BED
-00000900: 2066 696c 6573 206f 7220 7477 6f20 6c69   files or two li
-00000910: 7374 7320 6f66 2067 656e 6f6d 6963 2069  sts of genomic i
-00000920: 6e74 6572 7661 6c73 2e20 4966 2069 6e70  ntervals. If inp
-00000930: 7574 2069 7320 6120 4245 4420 6669 6c65  ut is a BED file
-00000940: 2c0a 096f 6e6c 7920 636f 6e73 6964 6572  ,..only consider
-00000950: 2074 6865 2066 6972 7374 2074 6872 6565   the first three
-00000960: 2063 6f6c 756d 6e73 2028 6368 726f 6d2c   columns (chrom,
-00000970: 2073 7461 7274 2c20 656e 6429 2c20 6f74   start, end), ot
-00000980: 6865 7220 636f 6c75 6d6e 730a 0977 696c  her columns..wil
-00000990: 6c20 6265 2069 676e 6f72 6564 2e0a 0a09  l be ignored....
-000009a0: 5061 7261 6d65 7465 7273 0a09 2d2d 2d2d  Parameters..----
-000009b0: 2d2d 2d2d 2d2d 0a09 696e 6265 6431 203a  ------..inbed1 :
-000009c0: 2073 7472 206f 7220 6c69 7374 0a09 094e   str or list...N
-000009d0: 616d 6520 6f66 2061 2042 4544 2066 696c  ame of a BED fil
-000009e0: 6520 6f72 206c 6973 7420 6f66 2067 656e  e or list of gen
-000009f0: 6f6d 6963 2069 6e74 6572 7661 6c73 2c20  omic intervals, 
-00000a00: 666f 7220 6578 616d 706c 652c 0a09 095b  for example,...[
-00000a10: 2863 6872 3120 3130 3020 3230 3029 2c20  (chr1 100 200), 
-00000a20: 2863 6872 3220 3130 3030 2031 3230 3029  (chr2 1000 1200)
-00000a30: 5d0a 0969 6e62 6564 3220 3a20 7374 7220  ]..inbed2 : str 
-00000a40: 6f72 206c 6973 740a 0909 4e61 6d65 206f  or list...Name o
-00000a50: 6620 6120 4245 4420 6669 6c65 206f 7220  f a BED file or 
-00000a60: 6c69 7374 206f 6620 6765 6e6f 6d69 6320  list of genomic 
-00000a70: 696e 7465 7276 616c 7373 2c20 666f 7220  intervalss, for 
-00000a80: 6578 616d 706c 652c 0a09 095b 2863 6872  example,...[(chr
-00000a90: 3120 3135 3020 3232 3029 2c20 2863 6872  1 150 220), (chr
-00000aa0: 3220 3131 3030 2031 3330 3029 5d0a 0a09  2 1100 1300)]...
-00000ab0: 5265 7475 726e 730a 092d 2d2d 2d2d 2d2d  Returns..-------
-00000ac0: 0a09 7368 6172 6564 5f69 6e74 6572 7661  ..shared_interva
-00000ad0: 6c73 203a 206c 6973 740a 0909 4c69 7374  ls : list...List
-00000ae0: 206f 6620 6765 6e6f 6d69 6320 696e 7465   of genomic inte
-00000af0: 7276 616c 7320 7368 6172 6564 2062 6574  rvals shared bet
-00000b00: 7765 656e 2074 6865 2074 776f 2069 6e70  ween the two inp
-00000b10: 7574 2042 4544 2066 696c 6573 2028 6f72  ut BED files (or
-00000b20: 206c 6973 7473 292e 0a0a 0945 7861 6d70   lists)....Examp
-00000b30: 6c65 730a 092d 2d2d 2d2d 2d2d 2d0a 093e  les..--------..>
-00000b40: 3e3e 2069 6e74 6572 7365 6374 4265 6433  >> intersectBed3
-00000b50: 285b 2827 6368 7231 272c 2031 2c20 3130  ([('chr1', 1, 10
-00000b60: 292c 2028 2763 6872 3127 2c20 3230 2c20  ), ('chr1', 20, 
-00000b70: 3335 295d 2c20 5b28 2763 6872 3127 2c33  35)], [('chr1',3
-00000b80: 2c20 3135 292c 2028 2763 6872 3127 2c32  , 15), ('chr1',2
-00000b90: 302c 2035 3029 5d29 0a09 5b28 2763 6872  0, 50)])..[('chr
-00000ba0: 3127 2c20 332c 2031 3029 2c20 2827 6368  1', 3, 10), ('ch
-00000bb0: 7231 272c 2032 302c 2033 3529 5d0a 0972  r1', 20, 35)]..r
-00000bc0: 0100 0000 720c 0000 0072 0d00 0000 2913  ....r....r....).
-00000bd0: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000be0: 0500 0000 7211 0000 0072 0400 0000 7208  ....r....r....r.
-00000bf0: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
-00000c00: 0000 7215 0000 0072 1600 0000 721b 0000  ..r....r....r...
-00000c10: 00da 0469 616e 6472 1700 0000 7218 0000  ...iandr....r...
-00000c20: 0072 1900 0000 721a 0000 00da 0563 6c65  .r....r......cle
-00000c30: 6172 290b da06 696e 6265 6431 da06 696e  ar)...inbed1..in
-00000c40: 6265 6432 5a10 7368 6172 6564 5f69 6e74  bed2Z.shared_int
-00000c50: 6572 7661 6c73 da05 6269 7473 31da 0562  ervals..bits1..b
-00000c60: 6974 7332 721c 0000 00da 036b 6579 721d  its2r......keyr.
-00000c70: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
-00000c80: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-00000c90: 00da 0d69 6e74 6572 7365 6374 4265 6433  ...intersectBed3
-00000ca0: 4900 0000 7354 0000 0000 1a04 020c 010c  I...sT..........
-00000cb0: 0104 020a 010c 0102 0112 0106 010e 0112  ................
-00000cc0: 020e 010a 030c 010c 0104 020a 010c 0102  ................
-00000cd0: 0112 0106 010e 0112 020e 010a 0106 0308  ................
-00000ce0: 010a 0112 0110 0108 0108 0104 020a 010c  ................
-00000cf0: 0004 010a 0118 0108 0108 0108 0172 2b00  .............r+.
-00000d00: 0000 6302 0000 0000 0000 0000 0000 000a  ..c.............
-00000d10: 0000 0007 0000 0043 0000 0073 b601 0000  .......C...s....
-00000d20: 6700 7d02 7400 7c00 8301 7401 6b08 722a  g.}.t.|...t.k.r*
-00000d30: 7402 7c00 8301 6401 6b02 7220 7c02 5300  t.|...d.k.r |.S.
-00000d40: 7403 7c00 8301 7d03 6e5e 7400 7c00 8301  t.|...}.n^t.|...
-00000d50: 7404 6b08 7270 7a12 7405 7406 a007 7c00  t.k.rpz.t.t...|.
-00000d60: a101 8301 7d03 5700 7188 0100 0100 0100  ....}.W.q.......
-00000d70: 7408 a009 6402 7c00 1600 a101 0100 740a  t...d.|.......t.
-00000d80: a00b 6403 a101 0100 5900 7188 5800 6e18  ..d.....Y.q.X.n.
-00000d90: 7408 a009 6402 7c00 1600 a101 0100 740a  t...d.|.......t.
-00000da0: a00b 6403 a101 0100 7400 7c01 8301 7401  ..d.....t.|...t.
-00000db0: 6b08 72c4 7402 7c01 8301 6401 6b02 72ba  k.r.t.|...d.k.r.
-00000dc0: 7400 7c00 8301 7401 6b08 72b0 7c00 5300  t.|...t.k.r.|.S.
-00000dd0: 740c 7c00 8301 5300 6e08 7403 7c01 8301  t.|...S.n.t.|...
-00000de0: 7d04 6e60 7400 7c01 8301 7404 6b08 9001  }.n`t.|...t.k...
-00000df0: 720c 7a12 7405 7406 a007 7c01 a101 8301  r.z.t.t...|.....
-00000e00: 7d04 5700 6e24 0100 0100 0100 7408 a009  }.W.n$......t...
-00000e10: 6402 7c01 1600 a101 0100 740a a00b 6403  d.|.......t...d.
-00000e20: a101 0100 5900 6e02 5800 6e18 7408 a009  ....Y.n.X.n.t...
-00000e30: 6402 7c01 1600 a101 0100 740a a00b 6403  d.|.......t...d.
-00000e40: a101 0100 7c03 4400 5d7c 7d05 7c05 7c03  ....|.D.]|}.|.|.
-00000e50: 6b07 9001 723a 9001 7128 7c03 7c05 1900  k...r:..q(|.|...
-00000e60: 7d06 7c05 7c04 6b06 9001 7266 7c04 7c05  }.|.|.k...rf|.|.
-00000e70: 1900 7d07 7c07 a00d a100 0100 7c06 a00e  ..}.|.......|...
-00000e80: 7c07 a101 0100 6401 7d08 7c06 a00f 7c08  |.....d.}.|...|.
-00000e90: a101 7d09 7c09 7c06 6a10 6b02 9001 7284  ..}.|.|.j.k...r.
-00000ea0: 9001 7128 7c06 a011 7c09 a101 7d08 7c02  ..q(|...|...}.|.
-00000eb0: a012 7c05 7c09 7c08 6603 a101 0100 9001  ..|.|.|.f.......
-00000ec0: 716a 9001 7128 7413 8300 7d03 7413 8300  qj..q(t...}.t...
-00000ed0: 7d04 7c02 5300 2904 6145 0200 000a 0953  }.|.S.).aE.....S
-00000ee0: 7562 7472 6163 7420 696e 6265 6432 2066  ubtract inbed2 f
-00000ef0: 726f 6d20 696e 6265 6431 2028 696e 6265  rom inbed1 (inbe
-00000f00: 6431 202d 2069 6e62 6564 3229 0a0a 0950  d1 - inbed2)...P
-00000f10: 6172 616d 6574 6572 730a 092d 2d2d 2d2d  arameters..-----
-00000f20: 2d2d 2d2d 2d0a 0969 6e62 6564 3120 3a20  -----..inbed1 : 
-00000f30: 7374 7220 6f72 206c 6973 740a 0909 4e61  str or list...Na
-00000f40: 6d65 206f 6620 6120 4245 4420 6669 6c65  me of a BED file
-00000f50: 206f 7220 6c69 7374 206f 6620 6765 6e6f   or list of geno
-00000f60: 6d69 6320 696e 7465 7276 616c 732c 2066  mic intervals, f
-00000f70: 6f72 2065 7861 6d70 6c65 2c0a 0909 5b28  or example,...[(
-00000f80: 6368 7231 2031 3030 2032 3030 292c 2028  chr1 100 200), (
-00000f90: 6368 7232 2031 3030 3020 3132 3030 295d  chr2 1000 1200)]
-00000fa0: 0a09 696e 6265 6432 203a 2073 7472 206f  ..inbed2 : str o
-00000fb0: 7220 6c69 7374 0a09 094e 616d 6520 6f66  r list...Name of
-00000fc0: 2061 2042 4544 2066 696c 6520 6f72 206c   a BED file or l
-00000fd0: 6973 7420 6f66 2067 656e 6f6d 6963 2069  ist of genomic i
-00000fe0: 6e74 6572 7661 6c73 2c20 666f 7220 6578  ntervals, for ex
-00000ff0: 616d 706c 652c 0a09 095b 2863 6872 3120  ample,...[(chr1 
-00001000: 3135 3020 3232 3029 2c20 2863 6872 3220  150 220), (chr2 
-00001010: 3131 3030 2031 3330 3029 5d0a 0a09 5265  1100 1300)]...Re
-00001020: 7475 726e 730a 092d 2d2d 2d2d 2d2d 0a09  turns..-------..
-00001030: 7265 6d61 696e 5f69 6e74 6572 7661 6c73  remain_intervals
-00001040: 203a 206c 6973 740a 0909 4c69 7374 206f   : list...List o
-00001050: 6620 6765 6e6f 6d69 6320 696e 7465 7276  f genomic interv
-00001060: 616c 7320 6672 6f6d 2069 6e62 6564 3120  als from inbed1 
-00001070: 7769 7468 2074 686f 7365 2073 6861 7265  with those share
-00001080: 6420 7265 6769 6f6e 7320 7769 7468 2069  d regions with i
-00001090: 6e62 6564 3220 7265 6d6f 7665 642e 0a0a  nbed2 removed...
-000010a0: 0945 7861 6d70 6c65 730a 092d 2d2d 2d2d  .Examples..-----
-000010b0: 2d2d 2d0a 093e 3e3e 2073 7562 7472 6163  ---..>>> subtrac
-000010c0: 7442 6564 3328 5b28 2763 6872 3127 2c20  tBed3([('chr1', 
-000010d0: 312c 2031 3029 2c20 2827 6368 7231 272c  1, 10), ('chr1',
-000010e0: 2032 302c 2033 3529 5d2c 205b 2827 6368   20, 35)], [('ch
-000010f0: 7231 272c 332c 2031 3529 2c20 2827 6368  r1',3, 15), ('ch
-00001100: 7231 272c 3230 2c20 3530 295d 290a 095b  r1',20, 50)])..[
-00001110: 2827 6368 7231 272c 2031 2c20 3329 5d0a  ('chr1', 1, 3)].
-00001120: 0a09 7201 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00001130: 0029 1472 0e00 0000 720f 0000 0072 1000  .).r....r....r..
-00001140: 0000 7205 0000 0072 1100 0000 7204 0000  ..r....r....r...
-00001150: 0072 0800 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001160: 7214 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
-00001170: 0962 6564 746f 6c69 7374 da06 696e 7665  .bedtolist..inve
-00001180: 7274 7224 0000 0072 1700 0000 7218 0000  rtr$...r....r...
-00001190: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
-000011a0: 290a 7226 0000 0072 2700 0000 5a10 7265  ).r&...r'...Z.re
-000011b0: 6d61 696e 5f69 6e74 6572 7661 6c73 5a08  main_intervalsZ.
-000011c0: 6269 7473 6574 7331 5a08 6269 7473 6574  bitsets1Z.bitset
-000011d0: 7332 721d 0000 0072 2800 0000 7229 0000  s2r....r(...r)..
-000011e0: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-000011f0: 7221 0000 0072 2200 0000 da0c 7375 6274  r!...r".....subt
-00001200: 7261 6374 4265 6433 9800 0000 7358 0000  ractBed3....sX..
-00001210: 0000 1804 020c 010c 0104 020a 010c 0102  ................
-00001220: 0112 0106 010e 0112 020e 010a 020c 010c  ................
-00001230: 010c 0104 020a 020a 010e 0102 0112 0106  ................
-00001240: 010e 0112 020e 010a 0108 010a 0104 0108  ................
-00001250: 010a 0108 0108 010a 0104 020a 010c 0004  ................
-00001260: 010a 0118 0106 0106 0172 2e00 0000 6300  .........r....c.
-00001270: 0000 0000 0000 0000 0000 000a 0000 0006  ................
-00001280: 0000 0047 0000 0073 c800 0000 6700 7d01  ...G...s....g.}.
-00001290: 7c00 4400 5dba 7d02 6401 7d03 7400 7c02  |.D.].}.d.}.t.|.
-000012a0: 8301 7401 6b08 7242 7c02 4400 5d1e 5c03  ..t.k.rB|.D.].\.
-000012b0: 7d04 7d05 7d06 7c03 7402 7c06 8301 7402  }.}.}.|.t.|...t.
-000012c0: 7c05 8301 1800 3700 7d03 7120 6e76 7400  |.....7.}.q nvt.
-000012d0: 7c02 8301 7403 6b08 72b8 7404 a005 7c02  |...t.k.r.t...|.
-000012e0: a101 4400 5d5e 7d07 7c07 a006 6402 a101  ..D.]^}.|...d...
-000012f0: 7268 7158 7c07 a007 a100 7d08 7408 7c08  rhqX|.....}.t.|.
-00001300: 8301 6403 6b00 728c 7409 a00a 6404 7c07  ..d.k.r.t...d.|.
-00001310: 1600 a101 0100 7158 7402 7c08 6405 1900  ......qXt.|.d...
-00001320: 8301 7402 7c08 6406 1900 8301 1800 7d09  ..t.|.d.......}.
-00001330: 7c09 6401 6b01 72ae 7158 7c03 7c09 3700  |.d.k.r.qX|.|.7.
-00001340: 7d03 7158 7c01 a00b 7c03 a101 0100 7108  }.qX|...|.....q.
-00001350: 7c01 5300 2907 6132 0200 000a 0943 616c  |.S.).a2.....Cal
-00001360: 6375 6c61 7465 2074 6865 2061 6767 7265  culate the aggre
-00001370: 6761 7465 6420 7369 7a65 206f 6620 6765  gated size of ge
-00001380: 6e6f 6d69 6320 696e 7465 7276 616c 732e  nomic intervals.
-00001390: 0a0a 0950 6172 616d 6574 6572 730a 092d  ...Parameters..-
-000013a0: 2d2d 2d2d 2d2d 2d2d 2d0a 0961 7267 7620  ---------..argv 
-000013b0: 3a20 6c69 7374 206f 6620 6765 6e6f 6d69  : list of genomi
-000013c0: 6320 7265 6769 6f6e 732e 0a09 0945 6163  c regions....Eac
-000013d0: 6820 6172 6775 6d65 6e74 2063 616e 2062  h argument can b
-000013e0: 6520 6120 6c69 7374 2c20 4245 442d 6c69  e a list, BED-li
-000013f0: 6b65 2066 696c 652c 206f 7220 6120 6269  ke file, or a bi
-00001400: 6742 6564 2066 696c 652e 2042 4544 2066  gBed file. BED f
-00001410: 696c 650a 0909 6361 6e20 6265 2072 6567  ile...can be reg
-00001420: 756c 6172 2c20 636f 6d70 7265 7373 6564  ular, compressed
-00001430: 2c20 6f72 2072 656d 6f74 6520 6669 6c65  , or remote file
-00001440: 2e20 5468 6520 7375 6666 6978 206f 6620  . The suffix of 
-00001450: 6269 6742 6564 2066 696c 650a 0909 6d75  bigBed file...mu
-00001460: 7374 2062 6520 6f6e 6520 6f66 2028 272e  st be one of ('.
-00001470: 6262 272c 272e 6269 6762 6564 272c 272e  bb','.bigbed','.
-00001480: 6269 6742 6564 272c 272e 4269 6742 6564  bigBed','.BigBed
-00001490: 272c 2027 2e42 4227 2c27 2042 4947 4245  ', '.BB',' BIGBE
-000014a0: 4427 292e 0a0a 0952 6574 7572 6e73 0a09  D')....Returns..
-000014b0: 2d2d 2d2d 2d2d 2d0a 094c 6973 7420 6f66  -------..List of
-000014c0: 2061 6767 7265 6761 7465 6420 7369 7a65   aggregated size
-000014d0: 2e0a 0a09 4578 616d 706c 6573 0a09 2d2d  ....Examples..--
-000014e0: 2d2d 2d2d 2d2d 0a09 3e3e 3e20 696e 7465  ------..>>> inte
-000014f0: 7276 616c 735f 3120 3d20 5b28 2763 6872  rvals_1 = [('chr
-00001500: 3127 2c20 312c 2031 3029 2c20 2827 6368  1', 1, 10), ('ch
-00001510: 7231 272c 2032 302c 2033 3529 5d0a 093e  r1', 20, 35)]..>
-00001520: 3e3e 2069 6e74 6572 7661 6c73 5f32 203d  >> intervals_2 =
-00001530: 205b 2827 6368 7231 272c 332c 2031 3529   [('chr1',3, 15)
-00001540: 2c20 2827 6368 7231 272c 3230 2c20 3530  , ('chr1',20, 50
-00001550: 295d 0a09 3e3e 3e20 6265 645f 6163 7475  )]..>>> bed_actu
-00001560: 616c 5f73 697a 6528 696e 7465 7276 616c  al_size(interval
-00001570: 735f 312c 2069 6e74 6572 7661 6c73 5f32  s_1, intervals_2
-00001580: 290a 095b 3234 2c20 3432 5d0a 0972 0100  )..[24, 42]..r..
-00001590: 0000 a903 da07 6272 6f77 7365 72fa 0123  ......browser..#
-000015a0: da05 7472 6163 6be9 0300 0000 fa14 696e  ..track.......in
-000015b0: 7661 6c69 6420 4245 4420 6c69 6e65 3a20  valid BED line: 
-000015c0: 2573 e902 0000 0072 0d00 0000 290c 720e  %s.....r....).r.
-000015d0: 0000 0072 0f00 0000 da03 696e 7472 1100  ...r......intr..
-000015e0: 0000 7208 0000 0072 1200 0000 da0a 7374  ..r....r......st
-000015f0: 6172 7473 7769 7468 da05 7370 6c69 7472  artswith..splitr
-00001600: 1000 0000 7213 0000 00da 0777 6172 6e69  ....r......warni
-00001610: 6e67 721a 0000 0029 0ada 0461 7267 76da  ngr....)...argv.
-00001620: 0573 697a 6573 da03 6172 6772 1800 0000  .sizes..argr....
-00001630: 721d 0000 0072 2000 0000 721f 0000 00da  r....r ...r.....
-00001640: 016c da01 66da 0374 6d70 7221 0000 0072  .l..f..tmpr!...r
-00001650: 2100 0000 7222 0000 00da 0f62 6564 5f61  !...r".....bed_a
-00001660: 6374 7561 6c5f 7369 7a65 e400 0000 7328  ctual_size....s(
-00001670: 0000 0000 1604 0108 0104 010c 010e 0118  ................
-00001680: 010c 010e 010a 0002 0108 010c 010e 0102  ................
-00001690: 0118 0108 0102 010a 010c 0172 4000 0000  ...........r@...
-000016a0: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
-000016b0: 0006 0000 0047 0000 0073 8a00 0000 6700  .....G...s....g.
-000016c0: 7d01 7c00 4400 5d7c 7d02 6401 7d03 7400  }.|.D.]|}.d.}.t.
-000016d0: 7c02 8301 7401 6b08 7226 7402 7c02 8301  |...t.k.r&t.|...
-000016e0: 7d03 6e54 7400 7c02 8301 7403 6b08 727a  }.nTt.|...t.k.rz
-000016f0: 7404 a005 7c02 a101 4400 5d3c 7d04 7c04  t...|...D.]<}.|.
-00001700: a006 6402 a101 724c 713c 7c04 a007 a100  ..d...rLq<|.....
-00001710: 7d05 7402 7c05 8301 6403 6b00 7270 7408  }.t.|...d.k.rpt.
-00001720: a009 6404 7c04 1600 a101 0100 713c 7c03  ..d.|.......q<|.
-00001730: 6405 3700 7d03 713c 7c01 a00a 7c03 a101  d.7.}.q<|...|...
-00001740: 0100 7108 7c01 5300 2906 6125 0200 000a  ..q.|.S.).a%....
-00001750: 0943 616c 6375 6c61 7465 2074 6865 206e  .Calculate the n
-00001760: 756d 6265 7220 6f66 2067 656e 6f6d 6963  umber of genomic
-00001770: 2069 6e74 6572 7661 6c73 2069 6e20 4245   intervals in BE
-00001780: 4420 6669 6c65 2e0a 0a0a 0950 6172 616d  D file.....Param
-00001790: 6574 6572 730a 092d 2d2d 2d2d 2d2d 2d2d  eters..---------
-000017a0: 2d0a 0961 7267 7620 3a20 6c69 7374 206f  -..argv : list o
-000017b0: 6620 6765 6e6f 6d69 6320 7265 6769 6f6e  f genomic region
-000017c0: 732e 0a09 0945 6163 6820 6172 6775 6d65  s....Each argume
-000017d0: 6e74 2063 616e 2062 6520 6120 6c69 7374  nt can be a list
-000017e0: 2c20 4245 442d 6c69 6b65 2066 696c 652c  , BED-like file,
-000017f0: 206f 7220 6120 6269 6742 6564 2066 696c   or a bigBed fil
-00001800: 652e 2042 4544 2066 696c 650a 0909 6361  e. BED file...ca
-00001810: 6e20 6265 2072 6567 756c 6172 2c20 636f  n be regular, co
-00001820: 6d70 7265 7373 6564 2c20 6f72 2072 656d  mpressed, or rem
-00001830: 6f74 6520 6669 6c65 2e20 5468 6520 7375  ote file. The su
-00001840: 6666 6978 206f 6620 6269 6742 6564 2066  ffix of bigBed f
-00001850: 696c 650a 0909 6d75 7374 2062 6520 6f6e  ile...must be on
-00001860: 6520 6f66 2028 272e 6262 272c 272e 6269  e of ('.bb','.bi
-00001870: 6762 6564 272c 272e 6269 6742 6564 272c  gbed','.bigBed',
-00001880: 272e 4269 6742 6564 272c 2027 2e42 4227  '.BigBed', '.BB'
-00001890: 2c27 2042 4947 4245 4427 292e 0a0a 0952  ,' BIGBED')....R
-000018a0: 6574 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a  eturns..-------.
-000018b0: 094c 6973 7420 6f66 2061 6767 7265 6761  .List of aggrega
-000018c0: 7465 6420 7369 7a65 2e0a 0a09 4578 616d  ted size....Exam
-000018d0: 706c 6573 0a09 2d2d 2d2d 2d2d 2d2d 0a09  ples..--------..
-000018e0: 3e3e 3e20 6265 6431 203d 205b 2827 6368  >>> bed1 = [('ch
-000018f0: 7231 272c 2031 2c20 3130 292c 2028 2763  r1', 1, 10), ('c
-00001900: 6872 3127 2c20 3230 2c20 3335 295d 0a09  hr1', 20, 35)]..
-00001910: 3e3e 3e20 6265 6432 203d 205b 2827 6368  >>> bed2 = [('ch
-00001920: 7231 272c 332c 2031 3529 2c20 2827 6368  r1',3, 15), ('ch
-00001930: 7231 272c 3230 2c20 3530 292c 2028 2763  r1',20, 50), ('c
-00001940: 6872 3227 2c31 3030 2c32 3030 295d 0a09  hr2',100,200)]..
-00001950: 3e3e 3e20 6265 645f 636f 756e 7473 2862  >>> bed_counts(b
-00001960: 6564 312c 2062 6564 3229 0a09 5b32 2c20  ed1, bed2)..[2, 
-00001970: 335d 0a09 7201 0000 0072 2f00 0000 7233  3]..r....r/...r3
-00001980: 0000 0072 3400 0000 720d 0000 0029 0b72  ...r4...r....).r
-00001990: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
-000019a0: 0000 0072 0800 0000 7212 0000 0072 3700  ...r....r....r7.
-000019b0: 0000 7238 0000 0072 1300 0000 7239 0000  ..r8...r....r9..
-000019c0: 0072 1a00 0000 2906 723a 0000 00da 0a62  .r....).r:.....b
-000019d0: 6564 5f63 6f75 6e74 7372 3c00 0000 da05  ed_countsr<.....
-000019e0: 636f 756e 7472 3d00 0000 723e 0000 0072  countr=...r>...r
-000019f0: 2100 0000 7221 0000 0072 2200 0000 7241  !...r!...r"...rA
-00001a00: 0000 000f 0100 0073 2000 0000 0017 0401  .......s .......
-00001a10: 0801 0401 0c01 0a01 0c01 0e01 0a00 0201  ................
-00001a20: 0801 0c01 0e01 0201 0a01 0c01 7241 0000  ............rA..
-00001a30: 0063 0000 0000 0000 0000 0000 0000 0900  .c..............
-00001a40: 0000 0800 0000 4700 0000 73d8 0000 0067  ......G...s....g
-00001a50: 007d 017c 0044 005d ca7d 0274 007c 0283  .}.|.D.].}.t.|..
-00001a60: 0174 016b 0872 2274 027c 0283 017d 036e  .t.k.r"t.|...}.n
-00001a70: 5e74 007c 0283 0174 036b 0872 687a 1274  ^t.|...t.k.rhz.t
-00001a80: 0474 05a0 067c 02a1 0183 017d 0357 0071  .t...|.....}.W.q
-00001a90: 8001 0001 0001 0074 07a0 0864 017c 0216  .......t...d.|..
-00001aa0: 00a1 0101 0074 09a0 0a64 02a1 0101 0059  .....t...d.....Y
-00001ab0: 0071 8058 006e 1874 07a0 0864 017c 0216  .q.X.n.t...d.|..
-00001ac0: 00a1 0101 0074 09a0 0a64 02a1 0101 0064  .....t...d.....d
-00001ad0: 037d 047c 0344 005d 3e7d 057c 037c 0519  .}.|.D.]>}.|.|..
-00001ae0: 007d 0664 037d 077c 06a0 0b7c 07a1 017d  .}.d.}.|...|...}
-00001af0: 087c 087c 066a 0c6b 0272 ae71 887c 06a0  .|.|.j.k.r.q.|..
-00001b00: 0d7c 08a1 017d 077c 047c 077c 0818 0037  .|...}.|.|.|...7
-00001b10: 007d 0471 9871 887c 01a0 0e7c 04a1 0101  .}.q.q.|...|....
-00001b20: 0071 087c 0153 0029 0461 c802 0000 0a09  .q.|.S.).a......
-00001b30: 4361 6c63 756c 6174 6520 7468 6520 2a67  Calculate the *g
-00001b40: 656e 6f6d 6963 2f75 6e69 7175 6520 7369  enomic/unique si
-00001b50: 7a65 2a20 6f66 2042 4544 2066 696c 6573  ze* of BED files
-00001b60: 2028 6f72 206c 6973 7473 206f 6620 6765   (or lists of ge
-00001b70: 6e6f 6d69 6320 696e 7465 7276 616c 7329  nomic intervals)
-00001b80: 2e0a 094e 6f74 652c 2067 656e 6f6d 6963  ...Note, genomic
-00001b90: 5f73 697a 6520 3c3d 2061 6374 7561 6c5f  _size <= actual_
-00001ba0: 7369 7a65 2e0a 0a09 5061 7261 6d65 7465  size....Paramete
-00001bb0: 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09  rs..----------..
-00001bc0: 6172 6776 203a 206c 6973 7420 6f66 2067  argv : list of g
-00001bd0: 656e 6f6d 6963 2072 6567 696f 6e73 2e0a  enomic regions..
-00001be0: 0909 4561 6368 2061 7267 756d 656e 7420  ..Each argument 
-00001bf0: 6361 6e20 6265 2061 206c 6973 742c 2042  can be a list, B
-00001c00: 4544 2d6c 696b 6520 6669 6c65 2c20 6f72  ED-like file, or
-00001c10: 2061 2062 6967 4265 6420 6669 6c65 2e20   a bigBed file. 
-00001c20: 4245 4420 6669 6c65 0a09 0963 616e 2062  BED file...can b
-00001c30: 6520 7265 6775 6c61 722c 2063 6f6d 7072  e regular, compr
-00001c40: 6573 7365 642c 206f 7220 7265 6d6f 7465  essed, or remote
-00001c50: 2066 696c 652e 2054 6865 2073 7566 6669   file. The suffi
-00001c60: 7820 6f66 2062 6967 4265 6420 6669 6c65  x of bigBed file
-00001c70: 0a09 096d 7573 7420 6265 206f 6e65 206f  ...must be one o
-00001c80: 6620 2827 2e62 6227 2c27 2e62 6967 6265  f ('.bb','.bigbe
-00001c90: 6427 2c27 2e62 6967 4265 6427 2c27 2e42  d','.bigBed','.B
-00001ca0: 6967 4265 6427 2c20 272e 4242 272c 2720  igBed', '.BB',' 
-00001cb0: 4249 4742 4544 2729 2e0a 0a09 5265 7475  BIGBED')....Retu
-00001cc0: 726e 730a 092d 2d2d 2d2d 2d2d 0a09 4c69  rns..-------..Li
-00001cd0: 7374 206f 6620 6765 6e6f 6d69 6320 7369  st of genomic si
-00001ce0: 7a65 2e0a 0a09 4578 616d 706c 650a 092d  ze....Example..-
-00001cf0: 2d2d 2d2d 2d2d 0a09 3e3e 3e20 6265 6431  ------..>>> bed1
-00001d00: 203d 205b 2827 6368 7231 272c 2030 2c20   = [('chr1', 0, 
-00001d10: 3130 3029 2c20 2827 6368 7231 272c 2035  100), ('chr1', 5
-00001d20: 302c 2031 3530 292c 2028 2763 6872 3127  0, 150), ('chr1'
-00001d30: 2c20 3830 2c20 3138 3029 5d0a 093e 3e3e  , 80, 180)]..>>>
-00001d40: 2062 6564 5f67 656e 6f6d 6963 5f73 697a   bed_genomic_siz
-00001d50: 6528 6265 6431 290a 095b 3138 305d 0a09  e(bed1)..[180]..
-00001d60: 3e3e 3e20 6265 6432 203d 205b 2827 6368  >>> bed2 = [('ch
-00001d70: 7231 272c 2030 2c20 3130 3029 2c20 2827  r1', 0, 100), ('
-00001d80: 6368 7232 272c 2035 302c 2031 3530 292c  chr2', 50, 150),
-00001d90: 2028 2763 6872 3327 2c20 3830 2c20 3138   ('chr3', 80, 18
-00001da0: 3029 5d0a 093e 3e3e 2062 6564 5f67 656e  0)]..>>> bed_gen
-00001db0: 6f6d 6963 5f73 697a 6528 6265 6432 290a  omic_size(bed2).
-00001dc0: 095b 3330 305d 0a09 3e3e 3e20 6265 645f  .[300]..>>> bed_
-00001dd0: 6765 6e6f 6d69 635f 7369 7a65 2862 6564  genomic_size(bed
-00001de0: 312c 2062 6564 3229 0a09 5b31 3830 2c20  1, bed2)..[180, 
-00001df0: 3330 305d 0a09 7a11 496e 7661 6c69 6420  300]..z.Invalid 
-00001e00: 696e 7075 743a 2025 7372 0d00 0000 7201  input: %sr....r.
-00001e10: 0000 0029 0f72 0e00 0000 720f 0000 0072  ...).r....r....r
-00001e20: 0500 0000 7211 0000 0072 0400 0000 7208  ....r....r....r.
-00001e30: 0000 0072 1200 0000 7213 0000 0072 1400  ...r....r....r..
-00001e40: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00001e50: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00001e60: 2909 723a 0000 005a 0b75 6e69 6f6e 5f73  ).r:...Z.union_s
-00001e70: 697a 6573 723c 0000 0072 1c00 0000 da0a  izesr<...r......
-00001e80: 756e 696f 6e5f 7369 7a65 721d 0000 0072  union_sizer....r
-00001e90: 1e00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
-00001ea0: 0000 0072 2100 0000 7222 0000 00da 1062  ...r!...r".....b
-00001eb0: 6564 5f67 656e 6f6d 6963 5f73 697a 6537  ed_genomic_size7
-00001ec0: 0100 0073 2e00 0000 001b 0401 0801 0c01  ...s............
-00001ed0: 0a01 0c01 0201 1201 0601 0e01 1202 0e01  ................
-00001ee0: 0a01 0401 0801 0801 0402 0a01 0a00 0201  ................
-00001ef0: 0a01 1001 0c01 7244 0000 0063 0200 0000  ......rD...c....
-00001f00: 0000 0000 0000 0000 0b00 0000 0500 0000  ................
-00001f10: 4300 0000 73ca 0000 0064 017d 0274 007c  C...s....d.}.t.|
-00001f20: 0083 0174 016b 0872 1a74 027c 0083 017d  ...t.k.r.t.|...}
-00001f30: 036e 0e74 0374 04a0 057c 00a1 0183 017d  .n.t.t...|.....}
-00001f40: 0374 007c 0183 0174 016b 0872 3e74 027c  .t.|...t.k.r>t.|
-00001f50: 0183 017d 046e 0e74 0374 04a0 057c 01a1  ...}.n.t.t...|..
-00001f60: 0183 017d 0474 0683 007d 057c 0344 005d  ...}.t...}.|.D.]
-00001f70: 2a7d 067c 067c 046b 0672 567c 037c 0619  *}.|.|.k.rV|.|..
-00001f80: 00a0 077c 047c 0619 00a1 0101 007c 037c  ...|.|.......|.|
-00001f90: 0619 007c 057c 063c 0071 567c 0544 005d  ...|.|.<.qV|.D.]
-00001fa0: 3e7d 077c 057c 0719 007d 0864 017d 097c  >}.|.|...}.d.}.|
-00001fb0: 08a0 087c 09a1 017d 0a7c 0a7c 086a 096b  ...|...}.|.|.j.k
-00001fc0: 0272 ac71 867c 08a0 0a7c 0aa1 017d 097c  .r.q.|...|...}.|
-00001fd0: 027c 097c 0a18 0037 007d 0271 9671 867c  .|.|...7.}.q.q.|
-00001fe0: 0253 0029 0261 c501 0000 0a09 4361 6c63  .S.).a......Calc
-00001ff0: 756c 6174 6520 7468 6520 746f 7461 6c20  ulate the total 
-00002000: 6e75 6d62 6572 206f 6620 2a62 6173 6573  number of *bases
-00002010: 2a20 6f76 6572 6c61 7070 6564 2062 6574  * overlapped bet
-00002020: 7765 656e 2074 776f 2062 6564 2066 696c  ween two bed fil
-00002030: 6573 206f 720a 0974 776f 206c 6973 7473  es or..two lists
-00002040: 206f 6620 6765 6e6f 6d69 6320 696e 7465   of genomic inte
-00002050: 7276 616c 732e 0a0a 0950 6172 616d 6574  rvals....Paramet
-00002060: 6572 730a 092d 2d2d 2d2d 2d2d 2d2d 2d0a  ers..----------.
-00002070: 0962 6564 3120 3a20 7374 7220 6f72 206c  .bed1 : str or l
-00002080: 6973 740a 0909 4669 6c65 206e 616d 6520  ist...File name 
-00002090: 6f66 2074 6865 2066 6972 7374 2042 4544  of the first BED
-000020a0: 2066 696c 652e 2043 616e 2061 6c73 6f20   file. Can also 
-000020b0: 6265 2061 206c 6973 742c 2073 7563 6820  be a list, such 
-000020c0: 6173 0a09 095b 2863 6872 3120 3130 3020  as...[(chr1 100 
-000020d0: 3230 3029 2c20 2863 6872 3220 3135 3020  200), (chr2 150 
-000020e0: 2033 3030 292c 2028 6368 7232 2031 3030   300), (chr2 100
-000020f0: 3020 3132 3030 295d 0a09 6265 6432 203a  0 1200)]..bed2 :
-00002100: 2073 7472 206f 7220 6c69 7374 0a09 0946   str or list...F
-00002110: 696c 6520 6e61 6d65 206f 6620 7468 6520  ile name of the 
-00002120: 7365 636f 6e64 2042 4544 2066 696c 652e  second BED file.
-00002130: 2043 616e 2061 6c73 6f20 6265 2061 206c   Can also be a l
-00002140: 6973 742c 2073 7563 6820 6173 0a09 095b  ist, such as...[
-00002150: 2863 6872 3120 3130 3020 3230 3029 2c20  (chr1 100 200), 
-00002160: 2863 6872 3220 3135 3020 2033 3030 292c  (chr2 150  300),
-00002170: 2028 6368 7232 2031 3030 3020 3132 3030   (chr2 1000 1200
-00002180: 295d 0a0a 0952 6574 7572 6e73 0a09 2d2d  )]...Returns..--
-00002190: 2d2d 2d2d 2d0a 0949 6e74 2e20 4f76 6572  -----..Int. Over
-000021a0: 6c61 7070 6564 2073 697a 652e 0a0a 0972  lapped size....r
-000021b0: 0100 0000 290b 720e 0000 0072 0f00 0000  ....).r....r....
-000021c0: 7205 0000 0072 0400 0000 7208 0000 0072  r....r....r....r
-000021d0: 1200 0000 721b 0000 0072 2400 0000 7217  ....r....r$...r.
-000021e0: 0000 0072 1800 0000 7219 0000 0029 0bda  ...r....r....)..
-000021f0: 0462 6564 31da 0462 6564 32da 0c6f 7665  .bed1..bed2..ove
-00002200: 726c 6170 5f73 697a 6572 2800 0000 7229  rlap_sizer(...r)
-00002210: 0000 0072 1c00 0000 722a 0000 0072 1d00  ...r....r*...r..
-00002220: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00002230: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00002240: da10 6265 645f 6f76 6572 6c61 705f 7369  ..bed_overlap_si
-00002250: 7a65 6b01 0000 732a 0000 0000 1304 010c  zek...s*........
-00002260: 010a 020e 010c 010a 020e 0106 0108 0108  ................
-00002270: 0112 010e 0108 0108 0104 020a 010a 0002  ................
-00002280: 010a 0110 0172 4800 0000 6301 0000 0000  .....rH...c.....
-00002290: 0000 0000 0000 0006 0000 0005 0000 0043  ...............C
-000022a0: 0000 0073 3e01 0000 7400 a001 6401 7c00  ...s>...t...d.|.
-000022b0: 1600 a101 0100 6900 7d01 7402 7c00 8301  ......i.}.t.|...
-000022c0: 7c01 6402 3c00 7403 7c00 8301 6403 1900  |.d.<.t.|...d...
-000022d0: 7c01 6404 3c00 6403 7c01 6405 3c00 6403  |.d.<.d.|.d.<.d.
-000022e0: 7c01 6406 3c00 6403 7d02 6700 7d03 7404  |.d.<.d.}.g.}.t.
-000022f0: a005 7c00 a101 4400 5d9e 7d04 7c04 a006  ..|...D.].}.|...
-00002300: 6407 a101 7260 7150 7c04 a007 a100 7d05  d...r`qP|.....}.
-00002310: 7408 7c05 8301 6408 6b00 7282 7400 a009  t.|...d.k.r.t...
-00002320: 6409 7c04 1600 a101 0100 740a 7c05 640a  d.|.......t.|.d.
-00002330: 1900 8301 740a 7c05 640b 1900 8301 1800  ....t.|.d.......
-00002340: 6403 6b00 72ac 7400 a009 6409 7c04 1600  d.k.r.t...d.|...
-00002350: a101 0100 7c01 6406 0500 1900 640b 3700  ....|.d.....d.7.
-00002360: 0300 3c00 740a 7c05 640a 1900 8301 740a  ..<.t.|.d.....t.
-00002370: 7c05 640b 1900 8301 1800 7d02 7c01 6405  |.d.......}.|.d.
-00002380: 0500 1900 7c02 3700 0300 3c00 7c03 a00b  ....|.7...<.|...
-00002390: 7c02 a101 0100 7150 740c a00d 7c03 a101  |.....qPt...|...
-000023a0: 7c01 640c 3c00 740c a00e 7c03 a101 7c01  |.d.<.t...|...|.
-000023b0: 640d 3c00 740c a00f 7c03 a101 7c01 640e  d.<.t...|...|.d.
-000023c0: 3c00 740c a010 7c03 a101 7c01 640f 3c00  <.t...|...|.d.<.
-000023d0: 740c 6a11 7c03 640b 6410 8d02 7c01 6411  t.j.|.d.d...|.d.
-000023e0: 3c00 7c01 5300 2912 7a2b 0a09 4261 7369  <.|.S.).z+..Basi
-000023f0: 6320 696e 666f 726d 6174 696f 6e20 6f66  c information of
-00002400: 2067 656e 6f6d 6963 2069 6e74 6572 7661   genomic interva
-00002410: 6c73 2e0a 097a 2e47 6174 6865 7269 6e67  ls...z.Gathering
-00002420: 2074 6568 2062 6173 6963 2073 7461 7469   teh basic stati
-00002430: 7374 6963 7320 6f66 2042 4544 2066 696c  stics of BED fil
-00002440: 653a 2025 73da 044e 616d 6572 0100 0000  e: %s..Namer....
-00002450: 5a0c 4765 6e6f 6d69 635f 7369 7a65 5a0a  Z.Genomic_sizeZ.
-00002460: 546f 7461 6c5f 7369 7a65 5a05 436f 756e  Total_sizeZ.Coun
-00002470: 7472 2f00 0000 7233 0000 0072 3400 0000  tr/...r3...r4...
-00002480: 7235 0000 0072 0d00 0000 5a09 4d65 616e  r5...r....Z.Mean
-00002490: 5f73 697a 655a 0b4d 6564 6961 6e5f 7369  _sizeZ.Median_si
-000024a0: 7a65 5a08 4d69 6e5f 7369 7a65 5a08 4d61  zeZ.Min_sizeZ.Ma
-000024b0: 785f 7369 7a65 2901 da04 6464 6f66 da03  x_size)...ddof..
-000024c0: 5354 4429 1272 1300 0000 da05 6465 6275  STD).r......debu
-000024d0: 6772 0200 0000 7244 0000 0072 0800 0000  gr....rD...r....
-000024e0: 7212 0000 0072 3700 0000 7238 0000 0072  r....r7...r8...r
-000024f0: 1000 0000 7214 0000 0072 3600 0000 721a  ....r....r6...r.
-00002500: 0000 00da 026e 70da 046d 6561 6eda 066d  .....np..mean..m
-00002510: 6564 6961 6eda 036d 696e da03 6d61 78da  edian..min..max.
-00002520: 0373 7464 2906 da06 696e 6669 6c65 5a09  .std)...infileZ.
-00002530: 6265 645f 696e 666f 7272 1800 0000 723b  bed_inforr....r;
-00002540: 0000 0072 3d00 0000 723e 0000 0072 2100  ...r=...r>...r!.
-00002550: 0000 7221 0000 0072 2200 0000 da07 6265  ..r!...r".....be
-00002560: 6469 6e66 6f96 0100 0073 3400 0000 0004  dinfo....s4.....
-00002570: 0e01 0401 0c01 1001 0801 0801 0401 0401  ................
-00002580: 0e01 0a01 0201 0801 0c01 0e01 1c01 0e01  ................
-00002590: 1001 1801 1001 0c01 0e01 0e01 0e01 0e01  ................
-000025a0: 1202 7254 0000 0063 0100 0000 0000 0000  ..rT...c........
-000025b0: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-000025c0: 73c4 0000 0067 007d 0174 00a0 017c 00a1  s....g.}.t...|..
-000025d0: 0144 005d b07d 027c 02a0 02a1 007d 027c  .D.].}.|.....}.|
-000025e0: 02a0 0364 01a1 0173 0e7c 02a0 0364 02a1  ...d...s.|...d..
-000025f0: 0173 0e7c 02a0 0364 03a1 0172 3a71 0e7c  .s.|...d...r:q.|
-00002600: 02a0 04a1 007d 0374 057c 0383 0164 046b  .....}.t.|...d.k
-00002610: 0072 6674 06a0 0764 057c 0216 00a1 0101  .rft...d.|......
-00002620: 0074 08a0 0964 06a1 0101 0074 0a7c 0364  .t...d.....t.|.d
-00002630: 0719 0083 0174 0a7c 0364 0619 0083 0118  .....t.|.d......
-00002640: 0064 086b 0072 9a74 06a0 0764 057c 0216  .d.k.r.t...d.|..
-00002650: 00a1 0101 0074 08a0 0964 06a1 0101 007c  .....t...d.....|
-00002660: 01a0 0b7c 0364 0819 0074 0a7c 0364 0619  ...|.d...t.|.d..
-00002670: 0083 0174 0a7c 0364 0719 0083 0166 03a1  ...t.|.d.....f..
-00002680: 0101 0071 0e7c 0153 0029 097a 210a 0943  ...q.|.S.).z!..C
-00002690: 6f6e 7665 7274 2042 4544 2066 696c 6520  onvert BED file 
-000026a0: 696e 746f 2061 206c 6973 742e 0a09 7230  into a list...r0
-000026b0: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
-000026c0: 0000 7234 0000 0072 0d00 0000 7235 0000  ..r4...r....r5..
-000026d0: 0072 0100 0000 290c 7208 0000 0072 1200  .r....).r....r..
-000026e0: 0000 da05 7374 7269 7072 3700 0000 7238  ....stripr7...r8
-000026f0: 0000 0072 1000 0000 7213 0000 0072 1400  ...r....r....r..
-00002700: 0000 7215 0000 0072 1600 0000 7236 0000  ..r....r....r6..
-00002710: 0072 1a00 0000 2904 5a07 6265 6466 696c  .r....).Z.bedfil
-00002720: 655a 0772 6567 696f 6e73 723d 0000 0072  eZ.regionsr=...r
-00002730: 3e00 0000 7221 0000 0072 2100 0000 7222  >...r!...r!...r"
-00002740: 0000 0072 2c00 0000 b701 0000 731c 0000  ...r,.......s...
-00002750: 0000 0404 020e 0108 011e 0102 0108 010c  ................
-00002760: 010e 010a 011c 010e 010a 0126 0172 2c00  ...........&.r,.
-00002770: 0000 6302 0000 0000 0000 0000 0000 0013  ..c.............
-00002780: 0000 0006 0000 0043 0000 0073 6402 0000  .......C...sd...
-00002790: 7400 a001 6401 7c00 1600 a101 0100 7402  t...d.|.......t.
-000027a0: 7c00 8301 7d02 7400 a001 6402 7c00 7403  |...}.t...d.|.t.
-000027b0: 7c02 8301 6602 1600 a101 0100 7400 a001  |...f.......t...
-000027c0: 6401 7c01 1600 a101 0100 7402 7c01 8301  d.|.......t.|...
-000027d0: 7d03 7400 a001 6402 7c01 7403 7c03 8301  }.t...d.|.t.|...
-000027e0: 6602 1600 a101 0100 7400 a001 6403 7c00  f.......t...d.|.
-000027f0: 7c01 6602 1600 a101 0100 7402 7c02 7c03  |.f.......t.|.|.
-00002800: 1700 8301 7d04 7400 a001 6404 7403 7c04  ....}.t...d.t.|.
-00002810: 8301 1600 a101 0100 7400 a001 6405 7c00  ........t...d.|.
-00002820: 1600 a101 0100 6900 7d05 7c02 4400 5d30  ......i.}.|.D.]0
-00002830: 5c03 7d06 7d07 7d08 7c06 7c05 6b07 72ba  \.}.}.}.|.|.k.r.
-00002840: 7404 8300 7c05 7c06 3c00 7c05 7c06 1900  t...|.|.<.|.|...
-00002850: a005 7406 7c07 7c08 8302 a101 0100 719e  ..t.|.|.......q.
-00002860: 7400 a001 6405 7c01 1600 a101 0100 6900  t...d.|.......i.
-00002870: 7d09 7c03 4400 5d32 5c03 7d0a 7d0b 7d0c  }.|.D.]2\.}.}.}.
-00002880: 7c0a 7c09 6b07 9001 7204 7404 8300 7c09  |.|.k...r.t...|.
-00002890: 7c0a 3c00 7c09 7c0a 1900 a005 7406 7c0b  |.<.|.|.....t.|.
-000028a0: 7c0c 8302 a101 0100 71e6 7400 a001 6406  |.......q.t...d.
-000028b0: a101 0100 6700 7d0d 6700 7d0e 6700 7d0f  ....g.}.g.}.g.}.
-000028c0: 7c04 4400 5de6 5c03 7d10 7d11 7d12 7c10  |.D.].\.}.}.}.|.
-000028d0: 7c05 6b06 9001 72dc 7c10 7c09 6b06 9001  |.k...r.|.|.k...
-000028e0: 72dc 7403 7c05 7c10 1900 a007 7c11 7c12  r.t.|.|.....|.|.
-000028f0: a102 8301 6407 6b04 9001 72aa 7403 7c09  ....d.k...r.t.|.
-00002900: 7c10 1900 a007 7c11 7c12 a102 8301 6407  |.....|.|.....d.
-00002910: 6b04 9001 7298 7c0f a008 7c10 7c11 7c12  k...r.|...|.|.|.
-00002920: 6603 a101 0100 6e10 7c0d a008 7c10 7c11  f.....n.|...|.|.
-00002930: 7c12 6603 a101 0100 6e30 7403 7c09 7c10  |.f.....n0t.|.|.
-00002940: 1900 a007 7c11 7c12 a102 8301 6407 6b04  ....|.|.....d.k.
-00002950: 9001 7234 7c0e a008 7c10 7c11 7c12 6603  ..r4|...|.|.|.f.
-00002960: a101 0100 6e04 9001 7134 6e3c 7c10 7c05  ....n...q4n<|.|.
-00002970: 6b06 9001 72f8 7c0d a008 7c10 7c11 7c12  k...r.|...|.|.|.
-00002980: 6603 a101 0100 6e20 7c10 7c09 6b06 9001  f.....n |.|.k...
-00002990: 7234 7c0e a008 7c10 7c11 7c12 6603 a101  r4|...|.|.|.f...
-000029a0: 0100 6e04 9001 7134 9001 7134 7400 a001  ..n...q4..q4t...
-000029b0: 6408 7c00 7403 7c0d 8301 6602 1600 a101  d.|.t.|...f.....
-000029c0: 0100 7400 a001 6408 7c01 7403 7c0e 8301  ..t...d.|.t.|...
-000029d0: 6602 1600 a101 0100 7400 a001 6409 7403  f.......t...d.t.
-000029e0: 7c0f 8301 1600 a101 0100 7c0d 7c0e 7c0f  |.........|.|.|.
-000029f0: 6603 5300 290a 61d7 0300 000a 0943 6f6d  f.S.).a......Com
-00002a00: 7061 7265 2074 776f 2042 4544 2066 696c  pare two BED fil
-00002a10: 6573 2028 6f72 206c 6973 7473 292e 2054  es (or lists). T
-00002a20: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
-00002a30: 7369 6d69 6c61 7220 746f 204c 696e 7578  similar to Linux
-00002a40: 2022 636f 6d6d 2220 636f 6d6d 616e 642e   "comm" command.
-00002a50: 0a0a 0950 6172 616d 6574 6572 730a 092d  ...Parameters..-
-00002a60: 2d2d 2d2d 2d2d 2d2d 2d0a 0969 6e62 6564  ---------..inbed
-00002a70: 3120 3a20 7374 7220 6f72 206c 6973 740a  1 : str or list.
-00002a80: 0909 4e61 6d65 206f 6620 6120 4245 4420  ..Name of a BED 
-00002a90: 6669 6c65 206f 7220 6c69 7374 206f 6620  file or list of 
-00002aa0: 4245 4420 7265 6769 6f6e 732c 2066 6f72  BED regions, for
-00002ab0: 2065 7861 6d70 6c65 2c0a 0909 5b28 6368   example,...[(ch
-00002ac0: 7231 2031 3030 2032 3030 292c 2028 6368  r1 100 200), (ch
-00002ad0: 7232 2031 3530 2020 3330 3029 2c20 2863  r2 150  300), (c
-00002ae0: 6872 3220 3130 3030 2031 3230 3029 5d0a  hr2 1000 1200)].
-00002af0: 0969 6e62 6564 3220 3a20 7374 7220 6f72  .inbed2 : str or
-00002b00: 206c 6973 740a 0909 4e61 6d65 206f 6620   list...Name of 
-00002b10: 6120 4245 4420 6669 6c65 206f 7220 6c69  a BED file or li
-00002b20: 7374 206f 6620 4245 4420 7265 6769 6f6e  st of BED region
-00002b30: 732c 2066 6f72 2065 7861 6d70 6c65 2c0a  s, for example,.
-00002b40: 0909 5b28 6368 7231 2031 3030 2032 3030  ..[(chr1 100 200
-00002b50: 292c 2028 6368 7232 2031 3530 2020 3330  ), (chr2 150  30
-00002b60: 3029 2c20 2863 6872 3220 3130 3030 2031  0), (chr2 1000 1
-00002b70: 3230 3029 5d0a 0a09 5265 7475 726e 730a  200)]...Returns.
-00002b80: 092d 2d2d 2d2d 2d2d 0a09 6265 6431 5f75  .-------..bed1_u
-00002b90: 6e69 7120 3a20 6c69 7374 0a09 0947 656e  niq : list...Gen
-00002ba0: 6f6d 6963 2072 6567 696f 6e73 2074 6861  omic regions tha
-00002bb0: 7420 6172 6520 696e 6265 6431 2075 6e69  t are inbed1 uni
-00002bc0: 7175 6520 2869 2e65 2e2c 2072 6567 696f  que (i.e., regio
-00002bd0: 6e73 206f 6e6c 7920 7072 6573 656e 7420  ns only present 
-00002be0: 696e 2069 6e62 6564 3120 6275 740a 0909  in inbed1 but...
-00002bf0: 646f 206e 6f74 206f 7665 726c 6170 2077  do not overlap w
-00002c00: 6974 6820 616e 7920 7265 6769 6f6e 7320  ith any regions 
-00002c10: 696e 2069 6e62 6564 3229 2e0a 0962 6564  in inbed2)...bed
-00002c20: 325f 756e 6971 203a 206c 6973 740a 0909  2_uniq : list...
-00002c30: 4765 6e6f 6d69 6320 7265 6769 6f6e 7320  Genomic regions 
-00002c40: 7468 6174 2061 7265 2069 6e62 6564 3220  that are inbed2 
-00002c50: 756e 6971 7565 2028 692e 652e 2c20 7265  unique (i.e., re
-00002c60: 6769 6f6e 7320 6f6e 6c79 2070 7265 7365  gions only prese
-00002c70: 6e74 2069 6e20 696e 6265 6432 2062 7574  nt in inbed2 but
-00002c80: 0a09 0964 6f20 6e6f 7420 6f76 6572 6c61  ...do not overla
-00002c90: 7020 7769 7468 2061 6e79 2072 6567 696f  p with any regio
-00002ca0: 6e73 2069 6e20 696e 6265 6431 292e 0a09  ns in inbed1)...
-00002cb0: 636f 6d6d 6f6e 203a 206c 6973 740a 0909  common : list...
-00002cc0: 4765 6e6f 6d69 6320 7265 6769 6f6e 7320  Genomic regions 
-00002cd0: 6f76 6572 6c61 7070 6564 2062 6574 7765  overlapped betwe
-00002ce0: 656e 2069 6e62 6564 3120 616e 6420 696e  en inbed1 and in
-00002cf0: 6265 6432 2e20 4e6f 7465 2c20 7468 650a  bed2. Note, the.
-00002d00: 0909 6f76 6572 6c61 7070 6564 2072 6567  ..overlapped reg
-00002d10: 696f 6e73 2077 6572 6520 6d65 7267 6564  ions were merged
-00002d20: 2e20 466f 7220 6578 616d 706c 652c 2028  . For example, (
-00002d30: 6368 7231 2031 2031 3029 2061 6e64 2028  chr1 1 10) and (
-00002d40: 6368 7231 2035 2031 3529 0a09 0977 696c  chr1 5 15)...wil
-00002d50: 6c20 6265 206d 6572 6765 6420 6173 2028  l be merged as (
-00002d60: 6368 7231 2031 2031 3529 2e0a 0a09 4e6f  chr1 1 15)....No
-00002d70: 7465 0a09 2d2d 2d2d 0a09 4f76 6572 6c61  te..----..Overla
-00002d80: 7070 6564 2072 6567 696f 6e73 202a 7769  pped regions *wi
-00002d90: 7468 696e 2a20 696e 7075 7420 4245 4420  thin* input BED 
-00002da0: 6669 6c65 7320 286f 7220 6c69 7374 7329  files (or lists)
-00002db0: 2061 7265 206d 6572 6765 6420 6265 666f   are merged befo
-00002dc0: 7265 0a09 636f 6d70 6172 6973 6f6e 2e0a  re..comparison..
-00002dd0: 0a09 fa1d 5265 6164 2061 6e64 2075 6e69  ....Read and uni
-00002de0: 6f6e 2042 4544 2066 696c 653a 2022 2573  on BED file: "%s
-00002df0: 22fa 1c55 6e69 6f6e 6564 2072 6567 696f  "..Unioned regio
-00002e00: 6e73 206f 6620 2225 7322 203a 2025 647a  ns of "%s" : %dz
-00002e10: 1d4d 6572 6765 2042 4544 2066 696c 6573  .Merge BED files
-00002e20: 2022 2573 2220 616e 6420 2225 7322 7a25   "%s" and "%s"z%
-00002e30: 556e 696f 6e65 6420 7265 6769 6f6e 7320  Unioned regions 
-00002e40: 6f66 2074 776f 2042 4544 2066 696c 6573  of two BED files
-00002e50: 203a 2025 64fa 2e42 7569 6c64 2069 6e74   : %d..Build int
-00002e60: 6572 7661 6c20 7472 6565 2066 6f72 2075  erval tree for u
-00002e70: 6e69 6f6e 6564 2042 4544 2066 696c 653a  nioned BED file:
-00002e80: 2022 2573 227a 2446 696e 6420 636f 6d6d   "%s"z$Find comm
-00002e90: 6f6e 2061 6e64 2073 7065 6369 6669 6320  on and specific 
-00002ea0: 7265 6769 6f6e 7320 2e2e 2e72 0100 0000  regions ...r....
-00002eb0: 7a17 2225 7322 2075 6e69 7175 6520 7265  z."%s" unique re
-00002ec0: 6769 6f6e 733a 2025 647a 1f43 6f6d 6d6f  gions: %dz.Commo
-00002ed0: 6e20 286f 7665 726c 6170 7065 6429 2072  n (overlapped) r
-00002ee0: 6567 696f 6e73 3a20 2564 2909 7213 0000  egions: %d).r...
-00002ef0: 00da 0469 6e66 6f72 2300 0000 7210 0000  ...infor#...r...
-00002f00: 0072 0700 0000 da0c 6164 645f 696e 7465  .r......add_inte
-00002f10: 7276 616c 7206 0000 00da 0466 696e 6472  rvalr......findr
-00002f20: 1a00 0000 2913 7226 0000 0072 2700 0000  ....).r&...r'...
-00002f30: da0a 6265 6431 5f75 6e69 6f6e da0a 6265  ..bed1_union..be
-00002f40: 6432 5f75 6e69 6f6e 5a0b 6265 6431 325f  d2_unionZ.bed12_
-00002f50: 756e 696f 6eda 056d 6170 7331 da05 6963  union..maps1..ic
-00002f60: 6872 31da 0769 7374 6172 7431 da05 6965  hr1..istart1..ie
-00002f70: 6e64 31da 056d 6170 7332 da05 6963 6872  nd1..maps2..ichr
-00002f80: 32da 0769 7374 6172 7432 da05 6965 6e64  2..istart2..iend
-00002f90: 325a 0962 6564 315f 756e 6971 5a09 6265  2Z.bed1_uniqZ.be
-00002fa0: 6432 5f75 6e69 71da 0663 6f6d 6d6f 6e72  d2_uniq..commonr
-00002fb0: 1d00 0000 7220 0000 0072 1f00 0000 7221  ....r ...r....r!
-00002fc0: 0000 0072 2100 0000 7222 0000 00da 0b63  ...r!...r".....c
-00002fd0: 6f6d 7061 7265 5f62 6564 cc01 0000 7356  ompare_bed....sV
-00002fe0: 0000 0000 220e 0108 0216 020e 0108 0216  ...."...........
-00002ff0: 0212 010c 0112 030e 0104 010e 0108 010a  ................
-00003000: 0116 020e 0104 010e 010a 010a 0116 020a  ................
-00003010: 0104 0104 0104 010e 0114 021a 021a 0112  ................
-00003020: 0312 041a 0112 0306 010a 0112 010a 0112  ................
-00003030: 0208 0116 0116 0112 0172 6700 0000 da02  .........rg.....
-00003040: 4e41 6305 0000 0000 0000 0000 0000 0020  NAc............ 
-00003050: 0000 0011 0000 0043 0000 0073 b404 0000  .......C...s....
-00003060: 7400 a001 6401 7c00 1600 a101 0100 7402  t...d.|.......t.
-00003070: 7c00 8301 7d05 7400 a001 6402 7c00 7403  |...}.t...d.|.t.
-00003080: 7c05 8301 6602 1600 a101 0100 7400 a001  |...f.......t...
-00003090: 6401 7c01 1600 a101 0100 7402 7c01 8301  d.|.......t.|...
-000030a0: 7d06 7400 a001 6402 7c01 7403 7c06 8301  }.t...d.|.t.|...
-000030b0: 6602 1600 a101 0100 7400 a001 6403 7c00  f.......t...d.|.
-000030c0: 1600 a101 0100 6900 7d07 7c05 4400 5d30  ......i.}.|.D.]0
-000030d0: 5c03 7d08 7d09 7d0a 7c08 7c07 6b07 728a  \.}.}.}.|.|.k.r.
-000030e0: 7404 8300 7c07 7c08 3c00 7c07 7c08 1900  t...|.|.<.|.|...
-000030f0: a005 7406 7c09 7c0a 8302 a101 0100 716e  ..t.|.|.......qn
-00003100: 7400 a001 6403 7c01 1600 a101 0100 6900  t...d.|.......i.
-00003110: 7d0b 7c06 4400 5d30 5c03 7d0c 7d0d 7d0e  }.|.D.]0\.}.}.}.
-00003120: 7c0c 7c0b 6b07 72d2 7404 8300 7c0b 7c0c  |.|.k.r.t...|.|.
-00003130: 3c00 7c0b 7c0c 1900 a005 7406 7c0d 7c0e  <.|.|.....t.|.|.
-00003140: 8302 a101 0100 71b6 7400 a001 6404 7c00  ......q.t...d.|.
-00003150: 1600 a101 0100 7407 6a08 a009 7c00 a101  ......t.j...|...
-00003160: 6405 1700 7d0f 740a 7c0f 6406 8302 7d10  d...}.t.|.d...}.
-00003170: 740b 6407 a00c 6408 6409 640a 640b 640c  t.d...d.d.d.d.d.
-00003180: 640d 640e 640f 6410 6709 a101 7c10 6411  d.d.d.d.g...|.d.
-00003190: 8d02 0100 7c05 4400 9001 5d82 5c03 7d11  ....|.D...].\.}.
-000031a0: 7d12 7d13 9001 7a38 7c13 7c12 1800 7d14  }.}...z8|.|...}.
-000031b0: 7c14 6412 6b01 9001 7280 7400 a00d 6413  |.d.k...r.t...d.
-000031c0: 7c11 6414 1700 740e 7c12 8301 1700 6415  |.d...t.|.....d.
-000031d0: 1700 740e 7c13 8301 1700 1600 a101 0100  ..t.|...........
-000031e0: 7c11 7c12 7c13 6603 6701 7d15 6412 7d16  |.|.|.f.g.}.d.}.
-000031f0: 6700 7d17 7c0b 7c11 1900 a00f 7c12 7c13  g.}.|.|.....|.|.
-00003200: a102 7d18 7403 7c18 8301 6412 6b02 9001  ..}.t.|...d.k...
-00003210: 72e2 740b 6407 a00c 6416 6417 8400 7c11  r.t.d...d.d...|.
-00003220: 7c12 7c13 7c14 7c04 7c04 7c04 7c04 7c04  |.|.|.|.|.|.|.|.
-00003230: 6609 4400 8301 a101 7c10 6411 8d02 0100  f.D.....|.d.....
-00003240: 6e9a 7c18 4400 5d2a 7d19 7c16 7c19 6a10  n.|.D.]*}.|.|.j.
-00003250: 7c19 6a11 1800 3700 7d16 7c17 a012 7c11  |.j...7.}.|...|.
-00003260: 7c19 6a11 7c19 6a10 6603 a101 0100 9001  |.j.|.j.f.......
-00003270: 71e6 7413 7c15 7c17 8302 7d1a 7414 7c15  q.t.|.|...}.t.|.
-00003280: 7c17 1700 8301 6412 1900 7d1b 7c02 7c14  |.....d...}.|.|.
-00003290: 7c16 7c1a 7c03 8304 7d1c 6418 a00c 6419  |.|.|...}.d...d.
-000032a0: 6417 8400 7c17 4400 8301 a101 7d1d 740b  d...|.D.....}.t.
-000032b0: 6407 a00c 641a 6417 8400 7c11 7c12 7c13  d...d.d...|.|.|.
-000032c0: 7c14 7c16 7c1a 7c1b 7c1d 7c1c 6609 4400  |.|.|.|.|.|.f.D.
-000032d0: 8301 a101 7c10 6411 8d02 0100 5700 6e3a  ....|.d.....W.n:
-000032e0: 0100 0100 0100 740b 6407 a00c 641b 6417  ......t.d...d.d.
-000032f0: 8400 7c11 7c12 7c13 7c14 7c04 7c04 7c04  ..|.|.|.|.|.|.|.
-00003300: 7c04 7c04 6609 4400 8301 a101 7c10 6411  |.|.f.D.....|.d.
-00003310: 8d02 0100 5900 6e02 5800 9001 7138 7c10  ....Y.n.X...q8|.
-00003320: a015 a100 0100 7400 a001 641c 7c0f 1600  ......t...d.|...
-00003330: a101 0100 7400 a001 6404 7c01 1600 a101  ....t...d.|.....
-00003340: 0100 7407 6a08 a009 7c01 a101 6405 1700  ..t.j...|...d...
-00003350: 7d1e 740a 7c1e 6406 8302 7d1f 740b 6407  }.t.|.d...}.t.d.
-00003360: a00c 6408 6409 640a 640b 640c 640d 640e  ..d.d.d.d.d.d.d.
-00003370: 640f 6410 6709 a101 7c1f 6411 8d02 0100  d.d.g...|.d.....
-00003380: 7c06 4400 9001 5d72 5c03 7d11 7d12 7d13  |.D...]r\.}.}.}.
-00003390: 9001 7a28 7c13 7c12 1800 7d16 7c16 6412  ..z(|.|...}.|.d.
-000033a0: 6b01 9003 726c 7400 a00d 6413 7c11 6414  k...rlt...d.|.d.
-000033b0: 1700 740e 7c12 8301 1700 6415 1700 740e  ..t.|.....d...t.
-000033c0: 7c13 8301 1700 1600 a101 0100 7c11 7c12  |...........|.|.
-000033d0: 7c13 6603 6701 7d17 6412 7d14 6700 7d15  |.f.g.}.d.}.g.}.
-000033e0: 7c07 7c11 1900 a00f 7c12 7c13 a102 7d18  |.|.....|.|...}.
-000033f0: 7403 7c18 8301 6412 6b02 9003 72ce 740b  t.|...d.k...r.t.
-00003400: 6407 a00c 641d 6417 8400 7c11 7c12 7c13  d...d.d...|.|.|.
-00003410: 7c14 7c04 7c04 7c04 7c04 7c04 6609 4400  |.|.|.|.|.|.f.D.
-00003420: 8301 a101 7c1f 6411 8d02 0100 6e8a 7c18  ....|.d.....n.|.
-00003430: 4400 5d2a 7d19 7c14 7c19 6a10 7c19 6a11  D.]*}.|.|.j.|.j.
-00003440: 1800 3700 7d14 7c15 a012 7c11 7c19 6a11  ..7.}.|...|.|.j.
-00003450: 7c19 6a10 6603 a101 0100 9003 71d2 7413  |.j.f.......q.t.
-00003460: 7c17 7c15 8302 7d1a 7c02 7c14 7c16 7c1a  |.|...}.|.|.|.|.
-00003470: 7c03 8304 7d1c 6418 a00c 641e 6417 8400  |...}.d...d.d...
-00003480: 7c15 4400 8301 a101 7d1d 740b 6407 a00c  |.D.....}.t.d...
-00003490: 641f 6417 8400 7c11 7c12 7c13 7c14 7c16  d.d...|.|.|.|.|.
-000034a0: 7c1a 7c1b 7c1d 7c1c 6609 4400 8301 a101  |.|.|.|.f.D.....
-000034b0: 7c1f 6411 8d02 0100 5700 6e3a 0100 0100  |.d.....W.n:....
-000034c0: 0100 740b 6407 a00c 6420 6417 8400 7c11  ..t.d...d d...|.
-000034d0: 7c12 7c13 7c14 7c04 7c04 7c04 7c04 7c04  |.|.|.|.|.|.|.|.
-000034e0: 6609 4400 8301 a101 7c1f 6411 8d02 0100  f.D.....|.d.....
-000034f0: 5900 6e02 5800 9003 7124 7c1f a015 a100  Y.n.X...q$|.....
-00003500: 0100 7400 a001 641c 7c1e 1600 a101 0100  ..t...d.|.......
-00003510: 6421 5300 2922 6176 0100 000a 0943 616c  d!S.)"av.....Cal
-00003520: 6375 6c61 7465 7320 7065 616b 2d77 6973  culates peak-wis
-00003530: 6520 6f76 6572 6c61 7020 2e0a 0a09 5061  e overlap ....Pa
-00003540: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
-00003550: 2d2d 2d2d 0a09 696e 6265 6431 203a 2073  ----..inbed1 : s
-00003560: 7472 0a09 094e 616d 6520 6f66 2061 2042  tr...Name of a B
-00003570: 4544 2066 696c 652e 0a09 696e 6265 6432  ED file...inbed2
-00003580: 203a 2073 7472 0a09 094e 616d 6520 6f66   : str...Name of
-00003590: 2061 6e6f 7468 6572 2042 4544 2066 696c   another BED fil
-000035a0: 652e 0a09 7363 6f72 655f 6675 6e63 203a  e...score_func :
-000035b0: 2066 756e 6374 696f 6e0a 0909 4675 6e63   function...Func
-000035c0: 7469 6f6e 2074 6f20 6361 6c63 756c 6174  tion to calculat
-000035d0: 6520 6f76 6572 6c61 7020 696e 6465 782e  e overlap index.
-000035e0: 2049 6e63 6c75 6465 206f 765f 636f 6566   Include ov_coef
-000035f0: 2c20 6f76 5f6a 6163 6361 7264 2c20 6f76  , ov_jaccard, ov
-00003600: 5f73 732c 206f 765f 7364 2e0a 0967 203a  _ss, ov_sd...g :
-00003610: 2069 6e74 0a09 0953 697a 6520 6f66 2074   int...Size of t
-00003620: 6865 2067 656e 6f6d 6963 2062 6163 6b67  he genomic backg
-00003630: 726f 756e 642e 0a09 6e61 5f6c 6162 656c  round...na_label
-00003640: 203a 2073 7472 0a09 0953 7472 696e 6720   : str...String 
-00003650: 6c61 6265 6c20 7573 6564 2074 6f20 7265  label used to re
-00003660: 7072 6573 656e 7420 6d69 7373 696e 6720  present missing 
-00003670: 7661 6c75 652e 0a0a 0952 6574 7572 6e73  value....Returns
-00003680: 0a09 2d2d 2d2d 2d2d 2d0a 094e 6f6e 650a  ..-------..None.
-00003690: 0972 5600 0000 7257 0000 0072 5800 0000  .rV...rW...rX...
-000036a0: 7a42 4361 6c63 756c 6174 6520 7468 6520  zBCalculate the 
-000036b0: 6f76 6572 6c61 7020 636f 6566 6669 6369  overlap coeffici
-000036c0: 656e 7420 6f66 2065 6163 6820 6765 6e6f  ent of each geno
-000036d0: 6d69 6320 7265 6769 6f6e 2069 6e20 2573  mic region in %s
-000036e0: 202e 2e2e 7a14 5f70 6561 6b77 6973 655f   ...z._peakwise_
-000036f0: 7363 6f72 6573 2e74 7376 da01 77fa 0109  scores.tsv..w...
-00003700: 721d 0000 0072 2000 0000 721f 0000 007a  r....r ...r....z
-00003710: 0641 2e73 697a 657a 0642 2e73 697a 6575  .A.sizez.B.sizeu
-00003720: 0500 0000 41e2 88a9 4275 0500 0000 41e2  ....A...Bu....A.
-00003730: 88aa 427a 0642 2e6c 6973 745a 0553 636f  ..Bz.B.listZ.Sco
-00003740: 7265 a901 da04 6669 6c65 7201 0000 007a  re....filer....z
-00003750: 0753 6b69 7020 2573 fa01 3afa 012d 6301  .Skip %s..:..-c.
-00003760: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00003770: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00003780: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00003790: 7221 0000 00a9 0172 1100 0000 a902 da02  r!.....r........
-000037a0: 2e30 da01 6972 2100 0000 7221 0000 0072  .0..ir!...r!...r
-000037b0: 2200 0000 da0a 3c6c 6973 7463 6f6d 703e  ".....<listcomp>
-000037c0: 6f02 0000 7304 0000 0006 0002 007a 2370  o...s........z#p
-000037d0: 6561 6b77 6973 655f 6f76 636f 6566 2e3c  eakwise_ovcoef.<
-000037e0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-000037f0: 703e fa01 2c63 0100 0000 0000 0000 0000  p>..,c..........
-00003800: 0000 0200 0000 0600 0000 5300 0000 7334  ..........S...s4
-00003810: 0000 0067 007c 005d 2c7d 017c 0164 0019  ...g.|.],}.|.d..
-00003820: 0064 0117 0074 007c 0164 0219 0083 0117  .d...t.|.d......
-00003830: 0064 0317 0074 007c 0164 0419 0083 0117  .d...t.|.d......
-00003840: 0091 0271 0453 00a9 0572 0100 0000 726d  ...q.S...r....rm
-00003850: 0000 0072 0d00 0000 726e 0000 0072 3500  ...r....rn...r5.
-00003860: 0000 726f 0000 0072 7000 0000 7221 0000  ..ro...rp...r!..
-00003870: 0072 2100 0000 7222 0000 0072 7300 0000  .r!...r"...rs...
-00003880: 7702 0000 7304 0000 0006 0002 0063 0100  w...s........c..
-00003890: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000038a0: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
-000038b0: 0c7d 0174 007c 0183 0191 0271 0453 0072  .}.t.|.....q.S.r
-000038c0: 2100 0000 726f 0000 0072 7000 0000 7221  !...ro...rp...r!
-000038d0: 0000 0072 2100 0000 7222 0000 0072 7300  ...r!...r"...rs.
-000038e0: 0000 7802 0000 7304 0000 0006 0002 0063  ..x...s........c
-000038f0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003900: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00003910: 005d 0c7d 0174 007c 0183 0191 0271 0453  .].}.t.|.....q.S
-00003920: 0072 2100 0000 726f 0000 0072 7000 0000  .r!...ro...rp...
-00003930: 7221 0000 0072 2100 0000 7222 0000 0072  r!...r!...r"...r
-00003940: 7300 0000 7a02 0000 7304 0000 0006 0002  s...z...s.......
-00003950: 007a 1e53 6176 6520 7065 616b 7769 7365  .z.Save peakwise
-00003960: 2073 636f 7265 7320 746f 2025 7320 2e2e   scores to %s ..
-00003970: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
-00003980: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00003990: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
-000039a0: 0453 0072 2100 0000 726f 0000 0072 7000  .S.r!...ro...rp.
-000039b0: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
-000039c0: 0072 7300 0000 8e02 0000 7304 0000 0006  .rs.......s.....
-000039d0: 0002 0063 0100 0000 0000 0000 0000 0000  ...c............
-000039e0: 0200 0000 0600 0000 5300 0000 7334 0000  ........S...s4..
-000039f0: 0067 007c 005d 2c7d 017c 0164 0019 0064  .g.|.],}.|.d...d
-00003a00: 0117 0074 007c 0164 0219 0083 0117 0064  ...t.|.d.......d
-00003a10: 0317 0074 007c 0164 0419 0083 0117 0091  ...t.|.d........
-00003a20: 0271 0453 0072 7500 0000 726f 0000 0072  .q.S.ru...ro...r
-00003a30: 7000 0000 7221 0000 0072 2100 0000 7222  p...r!...r!...r"
-00003a40: 0000 0072 7300 0000 9502 0000 7304 0000  ...rs.......s...
-00003a50: 0006 0002 0063 0100 0000 0000 0000 0000  .....c..........
-00003a60: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00003a70: 0000 0067 007c 005d 0c7d 0174 007c 0183  ...g.|.].}.t.|..
-00003a80: 0191 0271 0453 0072 2100 0000 726f 0000  ...q.S.r!...ro..
-00003a90: 0072 7000 0000 7221 0000 0072 2100 0000  .rp...r!...r!...
-00003aa0: 7222 0000 0072 7300 0000 9602 0000 7304  r"...rs.......s.
-00003ab0: 0000 0006 0002 0063 0100 0000 0000 0000  .......c........
-00003ac0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00003ad0: 7314 0000 0067 007c 005d 0c7d 0174 007c  s....g.|.].}.t.|
-00003ae0: 0183 0191 0271 0453 0072 2100 0000 726f  .....q.S.r!...ro
-00003af0: 0000 0072 7000 0000 7221 0000 0072 2100  ...rp...r!...r!.
-00003b00: 0000 7222 0000 0072 7300 0000 9802 0000  ..r"...rs.......
-00003b10: 7304 0000 0006 0002 004e 2916 7213 0000  s........N).r...
-00003b20: 0072 5900 0000 7223 0000 0072 1000 0000  .rY...r#...r....
-00003b30: 7207 0000 0072 5a00 0000 7206 0000 00da  r....rZ...r.....
-00003b40: 026f 73da 0470 6174 6872 0200 0000 da04  .os..pathr......
-00003b50: 6f70 656e da05 7072 696e 74da 046a 6f69  open..print..joi
-00003b60: 6e72 4c00 0000 7211 0000 0072 5b00 0000  nrL...r....r[...
-00003b70: 721f 0000 0072 2000 0000 721a 0000 0072  r....r ...r....r
-00003b80: 4800 0000 7244 0000 00da 0563 6c6f 7365  H...rD.....close
-00003b90: 2920 7226 0000 0072 2700 0000 da0a 7363  ) r&...r'.....sc
-00003ba0: 6f72 655f 6675 6e63 da01 67da 086e 615f  ore_func..g..na_
-00003bb0: 6c61 6265 6c72 5c00 0000 725d 0000 0072  labelr\...r]...r
-00003bc0: 5e00 0000 725f 0000 0072 6000 0000 7261  ^...r_...r`...ra
-00003bd0: 0000 0072 6200 0000 7263 0000 0072 6400  ...rb...rc...rd.
-00003be0: 0000 7265 0000 005a 0d6f 7574 6669 6c65  ..re...Z.outfile
-00003bf0: 5f6e 616d 6531 5a07 4245 4431 4f55 5472  _name1Z.BED1OUTr
-00003c00: 1d00 0000 7220 0000 0072 1f00 0000 5a0a  ....r ...r....Z.
-00003c10: 6265 645f 315f 7369 7a65 5a09 6265 645f  bed_1_sizeZ.bed_
-00003c20: 315f 6c73 745a 0a62 6564 5f32 5f73 697a  1_lstZ.bed_2_siz
-00003c30: 655a 0962 6564 5f32 5f6c 7374 da08 6f76  eZ.bed_2_lst..ov
-00003c40: 6572 6c61 7073 da01 6f72 4700 0000 7243  erlaps..orG...rC
-00003c50: 0000 005a 0c70 6561 6b5f 6f76 5f63 6f65  ...Z.peak_ov_coe
-00003c60: 665a 0b74 6172 6765 745f 6c69 7374 5a0d  fZ.target_listZ.
-00003c70: 6f75 7466 696c 655f 6e61 6d65 325a 0742  outfile_name2Z.B
-00003c80: 4544 324f 5554 7221 0000 0072 2100 0000  ED2OUTr!...r!...
-00003c90: 7222 0000 00da 0f70 6561 6b77 6973 655f  r".....peakwise_
-00003ca0: 6f76 636f 6566 2d02 0000 738e 0000 0000  ovcoef-...s.....
-00003cb0: 170e 0108 0116 020e 0108 0116 060e 0104  ................
-00003cc0: 010e 0108 010a 0116 020e 0104 010e 0108  ................
-00003cd0: 010a 0116 030e 0110 010a 0124 0110 0104  ...........$....
-00003ce0: 0108 010a 0126 010c 0104 0104 0210 020e  .....&..........
-00003cf0: 0130 0208 0110 0118 010a 0110 010e 0114  .0..............
-00003d00: 0132 0106 0138 0108 010e 030e 0110 010a  .2...8..........
-00003d10: 0124 0110 0104 0108 010a 0126 010c 0104  .$.........&....
-00003d20: 0104 0210 010e 0130 0208 0110 0118 010a  .......0........
-00003d30: 010e 0114 0132 0106 0138 0108 0172 8100  .....2...8...r..
-00003d40: 0000 720d 0000 00e7 0000 0000 0000 0000  ..r.............
-00003d50: 6306 0000 0000 0000 0000 0000 002d 0000  c............-..
-00003d60: 0007 0000 0043 0000 0073 c405 0000 6900  .....C...s....i.
-00003d70: 7d06 7400 6a01 a002 7c00 a101 7d07 7400  }.t.j...|...}.t.
-00003d80: 6a01 a002 7c01 a101 7d08 7c07 7c06 6401  j...|...}.|.|.d.
-00003d90: 3c00 7c08 7c06 6402 3c00 7403 a004 6403  <.|.|.d.<.t...d.
-00003da0: 7c00 1600 a101 0100 7405 7c00 8301 7d09  |.......t.|...}.
-00003db0: 7406 7c09 8301 7c06 6404 3c00 7403 a004  t.|...|.d.<.t...
-00003dc0: 6403 7c01 1600 a101 0100 7405 7c01 8301  d.|.......t.|...
-00003dd0: 7d0a 7406 7c0a 8301 7c06 6405 3c00 7403  }.t.|...|.d.<.t.
-00003de0: a004 6406 7c02 1600 a101 0100 7405 7c02  ..d.|.......t.|.
-00003df0: 8301 7d0b 7406 7c0b 8301 7c06 6407 3c00  ..}.t.|...|.d.<.
-00003e00: 7403 a004 6408 7c00 1600 a101 0100 6900  t...d.|.......i.
-00003e10: 7d0c 7c09 4400 5d30 5c03 7d0d 7d0e 7d0f  }.|.D.]0\.}.}.}.
-00003e20: 7c0d 7c0c 6b07 72c4 7407 8300 7c0c 7c0d  |.|.k.r.t...|.|.
-00003e30: 3c00 7c0c 7c0d 1900 a008 7409 7c0e 7c0f  <.|.|.....t.|.|.
-00003e40: 8302 a101 0100 71a8 7403 a004 6409 7c01  ......q.t...d.|.
-00003e50: 1600 a101 0100 6900 7d10 7c0a 4400 5d32  ......i.}.|.D.]2
-00003e60: 5c03 7d11 7d12 7d13 7c11 7c10 6b07 9001  \.}.}.}.|.|.k...
-00003e70: 720e 7407 8300 7c10 7c11 3c00 7c10 7c11  r.t...|.|.<.|.|.
-00003e80: 1900 a008 7409 7c12 7c13 8302 a101 0100  ....t.|.|.......
-00003e90: 71f0 640a 7d14 640a 7d15 640a 7d16 640a  q.d.}.d.}.d.}.d.
-00003ea0: 7d17 740a 7c03 640b 8302 7d18 7c0b 4400  }.t.|.d...}.|.D.
-00003eb0: 9003 5df8 5c03 7d19 7d1a 7d1b 7c19 640c  ..].\.}.}.}.|.d.
-00003ec0: 1700 740b 7c1a 8301 1700 640c 1700 740b  ..t.|.....d...t.
-00003ed0: 7c1b 8301 1700 7d1c 640d 7d1d 640d 7d1e  |.....}.d.}.d.}.
-00003ee0: 7c19 7c0c 6b07 9001 728a 7c19 7c10 6b07  |.|.k...r.|.|.k.
-00003ef0: 9001 728a 9003 6e30 7c19 7c0c 6b07 9002  ..r...n0|.|.k...
-00003f00: 7236 7c19 7c10 6b06 9002 7236 7c10 7c19  r6|.|.k...r6|.|.
-00003f10: 1900 a00c 7c1a 7c1b a102 7d1f 7406 7c1f  ....|.|...}.t.|.
-00003f20: 8301 640a 6b02 9001 72be 6e74 6700 7d20  ..d.k...r.ntg.} 
-00003f30: 7c1f 4400 5d1a 7d21 7c20 a00d 7c19 7c21  |.D.].}!| ..|.|!
-00003f40: 6a0e 7c21 6a0f 6603 a101 0100 9001 71c6  j.|!j.f.......q.
-00003f50: 7410 7c19 7c1a 7c1b 6603 6701 7c20 8302  t.|.|.|.f.g.| ..
-00003f60: 7d22 7411 7c20 8301 7d23 7a0c 7c22 7c23  }"t.| ..}#z.|"|#
-00003f70: 1b00 7d24 5700 6e10 0100 0100 0100 640a  ..}$W.n.......d.
-00003f80: 7d24 5900 6e02 5800 7c22 7c04 6b05 9004  }$Y.n.X.|"|.k...
-00003f90: 72ba 7c24 7c05 6b05 9004 72ba 640e 7d1e  r.|$|.k...r.d.}.
-00003fa0: 9002 6e84 7c19 7c0c 6b06 9002 72e2 7c19  ..n.|.|.k...r.|.
-00003fb0: 7c10 6b07 9002 72e2 7c0c 7c19 1900 a00c  |.k...r.|.|.....
-00003fc0: 7c1a 7c1b a102 7d25 7406 7c1f 8301 640a  |.|...}%t.|...d.
-00003fd0: 6b02 9002 726a 6e74 6700 7d26 7c25 4400  k...rjntg.}&|%D.
-00003fe0: 5d1a 7d21 7c26 a00d 7c19 7c21 6a0e 7c21  ].}!|&..|.|!j.|!
-00003ff0: 6a0f 6603 a101 0100 9002 7172 7410 7c19  j.f.......qrt.|.
-00004000: 7c1a 7c1b 6603 6701 7c26 8302 7d27 7411  |.|.f.g.|&..}'t.
-00004010: 7c26 8301 7d28 7a0c 7c27 7c28 1b00 7d29  |&..}(z.|'|(..})
-00004020: 5700 6e10 0100 0100 0100 640a 7d29 5900  W.n.......d.})Y.
-00004030: 6e02 5800 7c27 7c04 6b05 9004 72ba 7c29  n.X.|'|.k...r.|)
-00004040: 7c05 6b05 9004 72ba 640e 7d1d 9001 6ed8  |.k...r.d.}...n.
-00004050: 7c0c 7c19 1900 a00c 7c1a 7c1b a102 7d25  |.|.....|.|...}%
-00004060: 7c10 7c19 1900 a00c 7c1a 7c1b a102 7d1f  |.|.....|.|...}.
-00004070: 7406 7c25 8301 640a 6b02 9003 72a6 7406  t.|%..d.k...r.t.
-00004080: 7c1f 8301 640a 6b02 9003 7220 6e82 7406  |...d.k...r n.t.
-00004090: 7c1f 8301 640a 6b04 9004 72ba 6700 7d20  |...d.k...r.g.} 
-000040a0: 7c1f 4400 5d1a 7d21 7c20 a00d 7c19 7c21  |.D.].}!| ..|.|!
-000040b0: 6a0e 7c21 6a0f 6603 a101 0100 9003 7136  j.|!j.f.......q6
-000040c0: 7410 7c19 7c1a 7c1b 6603 6701 7c20 8302  t.|.|.|.f.g.| ..
-000040d0: 7d22 7411 7c20 8301 7d23 7a0c 7c22 7c23  }"t.| ..}#z.|"|#
-000040e0: 1b00 7d24 5700 6e10 0100 0100 0100 640a  ..}$W.n.......d.
-000040f0: 7d24 5900 6e02 5800 7c22 7c04 6b05 9004  }$Y.n.X.|"|.k...
-00004100: 72ba 7c24 7c05 6b05 9004 72ba 640e 7d1e  r.|$|.k...r.d.}.
-00004110: 9001 6e14 7406 7c25 8301 640a 6b04 9004  ..n.t.|%..d.k...
-00004120: 72ba 6700 7d26 7c25 4400 5d1a 7d21 7c26  r.g.}&|%D.].}!|&
-00004130: a00d 7c19 7c21 6a0e 7c21 6a0f 6603 a101  ..|.|!j.|!j.f...
-00004140: 0100 9003 71bc 7410 7c19 7c1a 7c1b 6603  ....q.t.|.|.|.f.
-00004150: 6701 7c26 8302 7d27 7411 7c26 8301 7d28  g.|&..}'t.|&..}(
-00004160: 7a0c 7c27 7c28 1b00 7d29 5700 6e10 0100  z.|'|(..})W.n...
-00004170: 0100 0100 640a 7d29 5900 6e02 5800 7c27  ....d.})Y.n.X.|'
-00004180: 7c04 6b05 9004 7228 7c29 7c05 6b05 9004  |.k...r(|)|.k...
-00004190: 7228 640e 7d1d 7406 7c1f 8301 640a 6b02  r(d.}.t.|...d.k.
-000041a0: 9004 7238 6e82 7406 7c1f 8301 640a 6b04  ..r8n.t.|...d.k.
-000041b0: 9004 72ba 6700 7d20 7c1f 4400 5d1a 7d21  ..r.g.} |.D.].}!
-000041c0: 7c20 a00d 7c19 7c21 6a0e 7c21 6a0f 6603  | ..|.|!j.|!j.f.
-000041d0: a101 0100 9004 714e 7410 7c19 7c1a 7c1b  ......qNt.|.|.|.
-000041e0: 6603 6701 7c20 8302 7d22 7411 7c20 8301  f.g.| ..}"t.| ..
-000041f0: 7d23 7a0c 7c22 7c23 1b00 7d24 5700 6e10  }#z.|"|#..}$W.n.
-00004200: 0100 0100 0100 640a 7d24 5900 6e02 5800  ......d.}$Y.n.X.
-00004210: 7c22 7c04 6b05 9004 72ba 7c24 7c05 6b05  |"|.k...r.|$|.k.
-00004220: 9004 72ba 640e 7d1e 7c1d 9004 72fe 7c1e  ..r.d.}.|...r.|.
-00004230: 9004 72e0 7c16 640f 3700 7d16 7412 7c1c  ..r.|.d.7.}.t.|.
-00004240: 6410 1700 7c18 6411 8d02 0100 6e1c 7c14  d...|.d.....n.|.
-00004250: 640f 3700 7d14 7412 7c1c 6412 7c07 1600  d.7.}.t.|.d.|...
-00004260: 1700 7c18 6411 8d02 0100 6e3c 7c1e 9005  ..|.d.....n<|...
-00004270: 7222 7c15 640f 3700 7d15 7412 7c1c 6412  r"|.d.7.}.t.|.d.
-00004280: 7c08 1600 1700 7c18 6411 8d02 0100 6e18  |.....|.d.....n.
-00004290: 7c17 640f 3700 7d17 7412 7c1c 6413 1700  |.d.7.}.t.|.d...
-000042a0: 7c18 6411 8d02 0100 9001 7142 7c14 7c06  |.d.......qB|.|.
-000042b0: 6414 3c00 7c15 7c06 6415 3c00 7c16 7c06  d.<.|.|.d.<.|.|.
-000042c0: 6416 3c00 7c17 7c06 6417 3c00 7c14 7c15  d.<.|.|.d.<.|.|.
-000042d0: 6b04 9005 7280 7413 a014 7c17 7c14 6702  k...r.t...|.|.g.
-000042e0: 7c15 7c16 6702 6702 a101 7d2a 6e16 7413  |.|.g.g...}*n.t.
-000042f0: a014 7c17 7c15 6702 7c14 7c16 6702 6702  ..|.|.g.|.|.g.g.
-00004300: a101 7d2a 7415 7c2a 6418 6419 8d02 5c02  ..}*t.|*d.d...\.
-00004310: 7d2b 7d2c 7c2b 7c06 641a 3c00 7c2c 7c06  }+},|+|.d.<.|,|.
-00004320: 641b 3c00 7416 6a17 7c06 641c 641d 8d02  d.<.t.j.|.d.d...
-00004330: 5300 291e 61b6 0200 000a 0945 7661 6c75  S.).a......Evalu
-00004340: 6174 6520 6966 2074 776f 2070 6561 6b20  ate if two peak 
-00004350: 7365 7473 2061 7265 2073 6967 6e69 6669  sets are signifi
-00004360: 6361 6e74 6c79 206f 632d 6f63 6375 7272  cantly oc-occurr
-00004370: 6564 206f 7220 6d75 7475 616c 6c79 2065  ed or mutually e
-00004380: 7863 6c75 7369 7665 2e0a 0955 7369 6e67  xclusive...Using
-00004390: 2046 6973 6865 7227 7320 6578 6163 7420   Fisher's exact 
-000043a0: 7465 7374 2e0a 0a09 5061 7261 6d65 7465  test....Paramete
-000043b0: 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09  rs..----------..
-000043c0: 696e 6265 6431 203a 2073 7472 0a09 094e  inbed1 : str...N
-000043d0: 616d 6520 6f66 2061 2042 4544 2066 696c  ame of a BED fil
-000043e0: 652e 0a09 696e 6265 6432 203a 2073 7472  e...inbed2 : str
-000043f0: 0a09 094e 616d 6520 6f66 2061 6e6f 7468  ...Name of anoth
-00004400: 6572 2042 4544 2066 696c 652e 0a09 696e  er BED file...in
-00004410: 6265 645f 6267 203a 2073 7472 0a09 094e  bed_bg : str...N
-00004420: 616d 6520 6f66 2074 6865 2062 6163 6b67  ame of the backg
-00004430: 726f 756e 6420 4245 4420 6669 6c65 2028  round BED file (
-00004440: 652e 672e 2c20 616c 6c20 7072 6f6d 6f74  e.g., all promot
-00004450: 6572 732c 2061 6c6c 2065 6e68 616e 6365  ers, all enhance
-00004460: 7273 292e 0a09 6f75 7466 696c 6520 3a20  rs)...outfile : 
-00004470: 7374 720a 0909 4e61 6d65 206f 6620 7468  str...Name of th
-00004480: 6520 6f75 7470 7574 2066 696c 652e 0a09  e output file...
-00004490: 6e5f 6375 7420 3a20 696e 742c 206f 7074  n_cut : int, opt
-000044a0: 696f 6e61 6c0a 0909 5468 7265 7368 6f6c  ional...Threshol
-000044b0: 6420 6f66 206f 7665 726c 6170 2073 697a  d of overlap siz
-000044c0: 652e 2046 6f72 2065 7861 6d70 6c65 2c20  e. For example, 
-000044d0: 7468 6520 6f76 6572 6c61 7020 7369 7a65  the overlap size
-000044e0: 2069 7320 3230 2066 6f72 2074 6865 7365   is 20 for these
-000044f0: 2074 776f 0a09 0972 6567 696f 6e73 2028   two...regions (
-00004500: 2763 6872 3127 2c20 302c 2031 3030 2920  'chr1', 0, 100) 
-00004510: 616e 6420 2827 6368 7231 272c 2038 302c  and ('chr1', 80,
-00004520: 2032 3530 292e 0a09 0964 6566 6175 6c74   250)....default
-00004530: 203d 2031 0a09 705f 7075 7420 3a20 666c   = 1..p_put : fl
-00004540: 6f61 742c 206f 7074 696f 6e61 6c0a 0909  oat, optional...
-00004550: 5468 7265 7368 6f6c 6420 6f66 206f 7665  Threshold of ove
-00004560: 726c 6170 2070 6572 6365 6e74 6167 652e  rlap percentage.
-00004570: 2049 6e20 7468 6520 6578 616d 706c 6520   In the example 
-00004580: 6162 6f76 652c 2074 6865 206f 7665 726c  above, the overl
-00004590: 6170 2070 6572 6365 6e74 6167 650a 0909  ap percentage...
-000045a0: 666f 7220 2827 6368 7231 272c 2030 2c20  for ('chr1', 0, 
-000045b0: 3130 3029 2069 7320 3230 2f31 3030 203d  100) is 20/100 =
-000045c0: 2030 2e32 2e0a 0909 6465 6661 756c 7420   0.2....default 
-000045d0: 3d20 302e 300a 0952 6574 7572 6e73 0a09  = 0.0..Returns..
-000045e0: 2d2d 2d2d 2d2d 2d0a 094e 6f6e 650a 097a  -------..None..z
-000045f0: 0641 2e6e 616d 657a 0642 2e6e 616d 6572  .A.namez.B.namer
-00004600: 5600 0000 7a07 412e 636f 756e 747a 0742  V...z.A.countz.B
-00004610: 2e63 6f75 6e74 7a28 5265 6164 2061 6e64  .countz(Read and
-00004620: 2075 6e69 6f6e 2062 6163 6b67 726f 756e   union backgroun
-00004630: 6420 4245 4420 6669 6c65 3a20 2225 7322  d BED file: "%s"
-00004640: 7a07 472e 636f 756e 747a 1e42 7569 6c64  z.G.countz.Build
-00004650: 2069 6e74 6572 7661 6c20 7472 6565 2066   interval tree f
-00004660: 6f72 203a 2022 2573 227a 1d42 7569 6c64  or : "%s"z.Build
-00004670: 2069 6e74 6572 7661 6c20 7472 6565 2066   interval tree f
-00004680: 6f72 3a20 2225 7322 7201 0000 0072 6900  or: "%s"r....ri.
-00004690: 0000 726a 0000 0046 5472 0d00 0000 7a08  ..rj...FTr....z.
-000046a0: 0943 6f6f 6363 7572 726b 0000 007a 0809  .Cooccurrk...z..
-000046b0: 2573 5f6f 6e6c 797a 0809 4e65 6974 6865  %s_onlyz..Neithe
-000046c0: 727a 0541 2b2c 422d 7a05 412d 2c42 2b7a  rz.A+,B-z.A-,B+z
-000046d0: 0541 2b2c 422b 7a05 412d 2c42 2dda 0767  .A+,B+z.A-,B-..g
-000046e0: 7265 6174 6572 2901 da0b 616c 7465 726e  reater)...altern
-000046f0: 6174 6976 657a 0a6f 6464 732d 7261 7469  ativez.odds-rati
-00004700: 6f7a 0770 2d76 616c 7565 7a1a 4669 7368  oz.p-valuez.Fish
-00004710: 6572 2773 2065 7861 6374 2074 6573 7420  er's exact test 
-00004720: 7265 7375 6c74 2902 da04 6461 7461 da04  result)...data..
-00004730: 6e61 6d65 2918 7276 0000 0072 7700 0000  name).rv...rw...
-00004740: 7202 0000 0072 1300 0000 7259 0000 0072  r....r....rY...r
-00004750: 2300 0000 7210 0000 0072 0700 0000 725a  #...r....r....rZ
-00004760: 0000 0072 0600 0000 7278 0000 0072 1100  ...r....rx...r..
-00004770: 0000 725b 0000 0072 1a00 0000 7220 0000  ..r[...r....r ..
-00004780: 0072 1f00 0000 7248 0000 0072 4400 0000  .r....rH...rD...
-00004790: 7279 0000 0072 4d00 0000 da05 6172 7261  ry...rM.....arra
-000047a0: 7972 0300 0000 da02 7064 da06 5365 7269  yr......pd..Seri
-000047b0: 6573 292d 7226 0000 0072 2700 0000 da08  es)-r&...r'.....
-000047c0: 696e 6265 645f 6267 da07 6f75 7466 696c  inbed_bg..outfil
-000047d0: 65da 056e 5f63 7574 da05 705f 6375 74da  e..n_cut..p_cut.
-000047e0: 0772 6573 756c 7473 5a0b 696e 6265 6431  .resultsZ.inbed1
-000047f0: 5f6e 616d 655a 0b69 6e62 6564 325f 6e61  _nameZ.inbed2_na
-00004800: 6d65 725c 0000 0072 5d00 0000 5a0a 6261  mer\...r]...Z.ba
-00004810: 636b 6772 6f75 6e64 725e 0000 0072 5f00  ckgroundr^...r_.
-00004820: 0000 7260 0000 0072 6100 0000 7262 0000  ..r`...ra...rb..
-00004830: 0072 6300 0000 7264 0000 0072 6500 0000  .rc...rd...re...
-00004840: 5a09 6265 6431 5f6f 6e6c 795a 0962 6564  Z.bed1_onlyZ.bed
-00004850: 325f 6f6e 6c79 da07 636f 6f63 6375 72da  2_only..cooccur.
-00004860: 076e 6569 7468 6572 da03 4f55 5472 1d00  .neither..OUTr..
-00004870: 0000 7220 0000 0072 1f00 0000 da04 6c69  ..r ...r......li
-00004880: 6e65 5a09 6265 6431 5f66 6c61 675a 0962  neZ.bed1_flagZ.b
-00004890: 6564 325f 666c 6167 5a0d 6265 6432 5f6f  ed2_flagZ.bed2_o
-000048a0: 7665 726c 6170 735a 1062 6564 325f 6f76  verlapsZ.bed2_ov
-000048b0: 6572 6c61 705f 6c73 7472 8000 0000 5a11  erlap_lstr....Z.
-000048c0: 6265 6432 5f6f 7665 726c 6170 5f73 697a  bed2_overlap_siz
-000048d0: 655a 1162 6564 325f 6765 6e6f 6d69 635f  eZ.bed2_genomic_
-000048e0: 7369 7a65 5a12 6265 6432 5f6f 7665 726c  sizeZ.bed2_overl
-000048f0: 6170 5f72 6174 696f 5a0d 6265 6431 5f6f  ap_ratioZ.bed1_o
-00004900: 7665 726c 6170 735a 1062 6564 315f 6f76  verlapsZ.bed1_ov
-00004910: 6572 6c61 705f 6c73 745a 1162 6564 315f  erlap_lstZ.bed1_
-00004920: 6f76 6572 6c61 705f 7369 7a65 5a11 6265  overlap_sizeZ.be
-00004930: 6431 5f67 656e 6f6d 6963 5f73 697a 655a  d1_genomic_sizeZ
-00004940: 1262 6564 315f 6f76 6572 6c61 705f 7261  .bed1_overlap_ra
-00004950: 7469 6fda 0574 6162 6c65 5a05 6f64 6473  tio..tableZ.odds
-00004960: 72da 0170 7221 0000 0072 2100 0000 7222  r..pr!...r!...r"
-00004970: 0000 00da 0c63 6f6f 6363 7572 5f70 6561  .....cooccur_pea
-00004980: 6b9c 0200 0073 0801 0000 001c 0401 0c01  k....s..........
-00004990: 0c01 0801 0801 0e01 0801 0c02 0e01 0801  ................
-000049a0: 0c08 0e01 0801 0c03 0e01 0401 0e01 0801  ................
-000049b0: 0a01 1602 0e01 0401 0e01 0a01 0a01 1603  ................
-000049c0: 0401 0401 0401 0401 0a03 1001 1c01 0401  ................
-000049d0: 0402 1401 0401 1401 1001 0e01 0202 0401  ................
-000049e0: 0801 1801 1201 0801 0201 0c01 0601 0a01  ................
-000049f0: 1401 0801 1401 1001 0e01 0202 0401 0801  ................
-00004a00: 1801 1201 0801 0201 0c01 0601 0a01 1401  ................
-00004a10: 0803 1002 1001 0e01 0e01 0201 0e01 0401  ................
-00004a20: 0801 1801 1201 0801 0201 0c01 0601 0a01  ................
-00004a30: 1401 0801 0e01 0401 0801 1801 1201 0801  ................
-00004a40: 0201 0c01 0601 0a01 1401 0402 0e01 0201  ................
-00004a50: 0e01 0401 0801 1801 1201 0801 0201 0c01  ................
-00004a60: 0601 0a01 1401 0401 0601 0601 0801 1202  ................
-00004a70: 0801 1602 0601 0801 1602 0801 1403 0801  ................
-00004a80: 0801 0801 0803 0a01 1802 1602 1001 0801  ................
-00004a90: 0801 7295 0000 0063 0200 0000 0000 0000  ..r....c........
-00004aa0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-00004ab0: 733c 0000 0074 007c 0164 0183 027d 027c  s<...t.|.d...}.|
-00004ac0: 0044 005d 207d 0374 0164 02a0 0264 0364  .D.] }.t.d...d.d
-00004ad0: 0484 007c 0344 0083 01a1 017c 0264 058d  ...|.D.....|.d..
-00004ae0: 0201 0071 0e7c 02a0 03a1 0001 0064 0653  ...q.|.......d.S
-00004af0: 0029 077a 2520 5361 7665 206c 6973 7420  .).z% Save list 
-00004b00: 6f66 2067 656e 6f6d 6963 2072 6567 696f  of genomic regio
-00004b10: 6e73 2074 6f20 6669 6c65 7269 0000 0072  ns to fileri...r
-00004b20: 6a00 0000 6301 0000 0000 0000 0000 0000  j...c...........
-00004b30: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-00004b40: 0000 6700 7c00 5d0c 7d01 7400 7c01 8301  ..g.|.].}.t.|...
-00004b50: 9102 7104 5300 7221 0000 0072 6f00 0000  ..q.S.r!...ro...
-00004b60: 7270 0000 0072 2100 0000 7221 0000 0072  rp...r!...r!...r
-00004b70: 2200 0000 7273 0000 0061 0300 0073 0400  "...rs...a...s..
-00004b80: 0000 0600 0200 7a1d 6265 6474 6f66 696c  ......z.bedtofil
-00004b90: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00004ba0: 636f 6d70 3e72 6b00 0000 4e29 0472 7800  comp>rk...N).rx.
-00004bb0: 0000 7279 0000 0072 7a00 0000 727b 0000  ..ry...rz...r{..
-00004bc0: 0029 045a 0862 6564 5f6c 6973 745a 0862  .).Z.bed_listZ.b
-00004bd0: 6564 5f66 696c 6572 9100 0000 723f 0000  ed_filer....r?..
-00004be0: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00004bf0: da09 6265 6474 6f66 696c 655d 0300 0073  ..bedtofile]...s
-00004c00: 0800 0000 0002 0a01 0801 1e01 7296 0000  ............r...
-00004c10: 0063 0600 0000 0000 0000 0000 0000 0600  .c..............
-00004c20: 0000 0600 0000 4300 0000 7346 0000 007c  ......C...sF...|
-00004c30: 0164 0117 007d 017c 027d 027c 0464 0117  .d...}.|.}.|.d..
-00004c40: 007d 047c 057d 057c 007c 036b 0372 2464  .}.|.}.|.|.k.r$d
-00004c50: 0253 0074 0074 0174 027c 017c 0483 0274  .S.t.t.t.|.|...t
-00004c60: 037c 027c 0583 0264 0117 0083 0283 0153  .|.|...d.......S
-00004c70: 0064 0353 0029 0461 d801 0000 0a09 4368  .d.S.).a......Ch
-00004c80: 6563 6b20 6966 2074 776f 2072 6567 696f  eck if two regio
-00004c90: 7320 6172 6520 6f76 6572 6c61 702e 0a0a  s are overlap...
-00004ca0: 0950 6172 616d 6574 6572 730a 092d 2d2d  .Parameters..---
-00004cb0: 2d2d 2d2d 2d2d 2d0a 0963 6872 3120 3a20  -------..chr1 : 
-00004cc0: 7374 720a 0909 4368 726f 6d6f 736f 6d65  str...Chromosome
-00004cd0: 2049 4420 6f66 2074 6865 2066 6972 7374   ID of the first
-00004ce0: 2067 656e 6f6d 6963 2072 6567 696f 6e0a   genomic region.
-00004cf0: 0973 7431 203a 2069 6e74 0a09 0953 7461  .st1 : int...Sta
-00004d00: 7274 2063 6f6f 7264 696e 6174 6520 6f66  rt coordinate of
-00004d10: 2074 6865 2066 6972 7374 2067 656e 6f6d   the first genom
-00004d20: 6963 2072 6567 696f 6e0a 0965 6e64 3120  ic region..end1 
-00004d30: 3a20 696e 740a 0909 456e 6420 636f 6f72  : int...End coor
-00004d40: 6469 6e61 7465 206f 6620 7468 6520 6669  dinate of the fi
-00004d50: 7273 7420 6765 6e6f 6d69 6320 7265 6769  rst genomic regi
-00004d60: 6f6e 0a09 6368 7232 203a 2073 7472 0a09  on..chr2 : str..
+00000330: 7d02 7c01 5300 2904 6125 0200 000a 094d  }.|.S.).a%.....M
+00000340: 6572 6765 206f 7220 756e 696f 6e20 6765  erge or union ge
+00000350: 6e6f 6d69 6320 696e 7465 7276 616c 732e  nomic intervals.
+00000360: 204f 6e6c 7920 636f 6e73 6964 6572 2074   Only consider t
+00000370: 6865 2066 6972 7374 2074 6872 6565 2063  he first three c
+00000380: 6f6c 756d 6e73 0a09 2863 6872 6f6d 2c20  olumns..(chrom, 
+00000390: 7374 6172 742c 2065 6e64 292c 206f 7468  start, end), oth
+000003a0: 6572 2063 6f6c 756d 6e73 2077 696c 6c20  er columns will 
+000003b0: 6265 2069 676e 6f72 6564 2e0a 0a09 5061  be ignored....Pa
+000003c0: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+000003d0: 2d2d 2d2d 0a09 696e 6265 6420 3a20 7374  ----..inbed : st
+000003e0: 7220 6f72 206c 6973 740a 0909 4e61 6d65  r or list...Name
+000003f0: 206f 6620 6120 4245 4420 6669 6c65 206f   of a BED file o
+00000400: 7220 6c69 7374 206f 6620 6765 6e6f 6d69  r list of genomi
+00000410: 6320 696e 7465 7276 616c 7320 2866 6f72  c intervals (for
+00000420: 2065 7861 6d70 6c65 2c0a 0909 5b28 6368   example,...[(ch
+00000430: 7231 2031 3030 2032 3030 292c 2028 6368  r1 100 200), (ch
+00000440: 7232 2031 3530 2020 3330 3029 2c20 2863  r2 150  300), (c
+00000450: 6872 3220 3130 3030 2031 3230 3029 5d29  hr2 1000 1200)])
+00000460: 0a0a 0952 6574 7572 6e73 0a09 2d2d 2d2d  ...Returns..----
+00000470: 2d2d 2d0a 0975 6e69 6f6e 6564 5f69 6e74  ---..unioned_int
+00000480: 6572 7661 6c73 203a 206c 6973 740a 0909  ervals : list...
+00000490: 4c69 7374 206f 6620 6765 6e6f 6d69 6320  List of genomic 
+000004a0: 696e 7465 7276 616c 7320 7769 7468 2074  intervals with t
+000004b0: 6865 206f 7665 726c 6170 7065 6420 7265  he overlapped re
+000004c0: 6769 6f6e 7320 6d65 7267 6564 2e0a 0a09  gions merged....
+000004d0: 4578 616d 706c 6573 0a09 2d2d 2d2d 2d2d  Examples..------
+000004e0: 2d2d 0a09 3e3e 3e20 756e 696f 6e5f 6265  --..>>> union_be
+000004f0: 6433 285b 2827 6368 7231 272c 2031 2c20  d3([('chr1', 1, 
+00000500: 3130 292c 2028 2763 6872 3127 2c20 332c  10), ('chr1', 3,
+00000510: 2031 3529 2c20 2827 6368 7231 272c 2032   15), ('chr1', 2
+00000520: 302c 2033 3529 2c20 2827 6368 7231 272c  0, 35), ('chr1',
+00000530: 2032 302c 2035 3029 5d29 0a09 5b28 2763   20, 50)])..[('c
+00000540: 6872 3127 2c20 312c 2031 3529 2c20 2827  hr1', 1, 15), ('
+00000550: 6368 7231 272c 2032 302c 2035 3029 5d0a  chr1', 20, 50)].
+00000560: 0a09 7201 0000 00fa 1169 6e76 616c 6964  ..r......invalid
+00000570: 2069 6e70 7574 3a20 2573 e901 0000 0029   input: %s.....)
+00000580: 11da 0474 7970 65da 046c 6973 74da 036c  ...type..list..l
+00000590: 656e 7205 0000 00da 0373 7472 7204 0000  enr......strr...
+000005a0: 0072 0800 0000 da06 7265 6164 6572 da07  .r......reader..
+000005b0: 6c6f 6767 696e 67da 0565 7272 6f72 da03  logging..error..
+000005c0: 7379 73da 0465 7869 74da 086e 6578 745f  sys..exit..next_
+000005d0: 7365 74da 0473 697a 65da 0a6e 6578 745f  set..size..next_
+000005e0: 636c 6561 72da 0661 7070 656e 64da 0464  clear..append..d
+000005f0: 6963 7429 075a 0569 6e62 6564 5a11 756e  ict).Z.inbedZ.un
+00000600: 696f 6e65 645f 696e 7465 7276 616c 73da  ioned_intervals.
+00000610: 0762 6974 7365 7473 da05 6368 726f 6dda  .bitsets..chrom.
+00000620: 0462 6974 73da 0365 6e64 da05 7374 6172  .bits..end..star
+00000630: 74a9 0072 1f00 0000 fa3f 2f55 7365 7273  t..r.....?/Users
+00000640: 2f6d 3130 3233 3234 2f44 6f63 756d 656e  /m102324/Documen
+00000650: 7473 2f47 6974 4875 622f 636f 6269 6e64  ts/GitHub/cobind
+00000660: 2f6c 6962 2f63 6f62 696e 6461 6269 6c69  /lib/cobindabili
+00000670: 7479 2f42 4544 2e70 79da 0a75 6e69 6f6e  ty/BED.py..union
+00000680: 5f62 6564 3317 0000 0073 2e00 0000 0016  _bed3....s......
+00000690: 0401 0c01 0c01 0402 0a01 0c01 0201 1201  ................
+000006a0: 0601 0e01 1202 0e01 0a02 0801 0801 0402  ................
+000006b0: 0a01 0a00 0201 0a01 1401 0601 7221 0000  ............r!..
+000006c0: 0063 0200 0000 0000 0000 0000 0000 0b00  .c..............
+000006d0: 0000 0700 0000 4300 0000 73b2 0100 0067  ......C...s....g
+000006e0: 007d 0274 007c 0083 0174 016b 0872 2a74  .}.t.|...t.k.r*t
+000006f0: 027c 0083 0164 016b 0272 207c 0253 0074  .|...d.k.r |.S.t
+00000700: 037c 0083 017d 036e 5e74 007c 0083 0174  .|...}.n^t.|...t
+00000710: 046b 0872 707a 1274 0574 06a0 077c 00a1  .k.rpz.t.t...|..
+00000720: 0183 017d 0357 0071 8801 0001 0001 0074  ...}.W.q.......t
+00000730: 08a0 0964 027c 0016 00a1 0101 0074 0aa0  ...d.|.......t..
+00000740: 0b64 03a1 0101 0059 0071 8858 006e 1874  .d.....Y.q.X.n.t
+00000750: 08a0 0964 027c 0016 00a1 0101 0074 0aa0  ...d.|.......t..
+00000760: 0b64 03a1 0101 0074 007c 0183 0174 016b  .d.....t.|...t.k
+00000770: 0872 ae74 027c 0183 0164 016b 0272 a47c  .r.t.|...d.k.r.|
+00000780: 0253 0074 037c 0183 017d 046e 5e74 007c  .S.t.|...}.n^t.|
+00000790: 0183 0174 046b 0872 f47a 1274 0574 06a0  ...t.k.r.z.t.t..
+000007a0: 077c 01a1 0183 017d 0457 006e 2401 0001  .|.....}.W.n$...
+000007b0: 0001 0074 08a0 0964 027c 0116 00a1 0101  ...t...d.|......
+000007c0: 0074 0aa0 0b64 03a1 0101 0059 006e 0258  .t...d.....Y.n.X
+000007d0: 006e 1874 08a0 0964 027c 0116 00a1 0101  .n.t...d.|......
+000007e0: 0074 0aa0 0b64 03a1 0101 0074 0c83 007d  .t...d.....t...}
+000007f0: 057c 0344 005d 2e7d 067c 067c 046b 0690  .|.D.].}.|.|.k..
+00000800: 0172 167c 037c 0619 00a0 0d7c 047c 0619  .r.|.|.....|.|..
+00000810: 00a1 0101 007c 037c 0619 007c 057c 063c  .....|.|...|.|.<
+00000820: 0090 0171 167c 0544 005d 4a7d 077c 057c  ...q.|.D.]J}.|.|
+00000830: 0719 007d 0864 017d 097c 08a0 0e7c 09a1  ...}.d.}.|...|..
+00000840: 017d 0a7c 0a7c 086a 0f6b 0290 0172 7490  .}.|.|.j.k...rt.
+00000850: 0171 4a7c 08a0 107c 0aa1 017d 097c 02a0  .qJ|...|...}.|..
+00000860: 117c 077c 0a7c 0966 03a1 0101 0090 0171  .|.|.|.f.......q
+00000870: 5a90 0171 4a7c 03a0 12a1 0001 007c 04a0  Z..qJ|.......|..
+00000880: 12a1 0001 007c 05a0 12a1 0001 007c 0253  .....|.......|.S
+00000890: 0029 0461 1503 0000 0a09 5265 7475 726e  .).a......Return
+000008a0: 2074 6865 2073 6861 7265 6420 6765 6e6f   the shared geno
+000008b0: 6d69 6320 696e 7465 7276 616c 7320 6265  mic intervals be
+000008c0: 6574 7765 656e 2069 6e62 6564 3120 616e  etween inbed1 an
+000008d0: 6420 696e 6265 6432 2e20 496e 7075 7473  d inbed2. Inputs
+000008e0: 2061 7265 0a09 7477 6f20 4245 4420 6669   are..two BED fi
+000008f0: 6c65 7320 6f72 2074 776f 206c 6973 7473  les or two lists
+00000900: 206f 6620 6765 6e6f 6d69 6320 696e 7465   of genomic inte
+00000910: 7276 616c 732e 2049 6620 696e 7075 7420  rvals. If input 
+00000920: 6973 2061 2042 4544 2066 696c 652c 0a09  is a BED file,..
+00000930: 6f6e 6c79 2063 6f6e 7369 6465 7220 7468  only consider th
+00000940: 6520 6669 7273 7420 7468 7265 6520 636f  e first three co
+00000950: 6c75 6d6e 7320 2863 6872 6f6d 2c20 7374  lumns (chrom, st
+00000960: 6172 742c 2065 6e64 292c 206f 7468 6572  art, end), other
+00000970: 2063 6f6c 756d 6e73 0a09 7769 6c6c 2062   columns..will b
+00000980: 6520 6967 6e6f 7265 642e 0a0a 0950 6172  e ignored....Par
+00000990: 616d 6574 6572 730a 092d 2d2d 2d2d 2d2d  ameters..-------
+000009a0: 2d2d 2d0a 0969 6e62 6564 3120 3a20 7374  ---..inbed1 : st
+000009b0: 7220 6f72 206c 6973 740a 0909 4e61 6d65  r or list...Name
+000009c0: 206f 6620 6120 4245 4420 6669 6c65 206f   of a BED file o
+000009d0: 7220 6c69 7374 206f 6620 6765 6e6f 6d69  r list of genomi
+000009e0: 6320 696e 7465 7276 616c 732c 2066 6f72  c intervals, for
+000009f0: 2065 7861 6d70 6c65 2c0a 0909 5b28 6368   example,...[(ch
+00000a00: 7231 2031 3030 2032 3030 292c 2028 6368  r1 100 200), (ch
+00000a10: 7232 2031 3030 3020 3132 3030 295d 0a09  r2 1000 1200)]..
+00000a20: 696e 6265 6432 203a 2073 7472 206f 7220  inbed2 : str or 
+00000a30: 6c69 7374 0a09 094e 616d 6520 6f66 2061  list...Name of a
+00000a40: 2042 4544 2066 696c 6520 6f72 206c 6973   BED file or lis
+00000a50: 7420 6f66 2067 656e 6f6d 6963 2069 6e74  t of genomic int
+00000a60: 6572 7661 6c73 732c 2066 6f72 2065 7861  ervalss, for exa
+00000a70: 6d70 6c65 2c0a 0909 5b28 6368 7231 2031  mple,...[(chr1 1
+00000a80: 3530 2032 3230 292c 2028 6368 7232 2031  50 220), (chr2 1
+00000a90: 3130 3020 3133 3030 295d 0a0a 0952 6574  100 1300)]...Ret
+00000aa0: 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0973  urns..-------..s
+00000ab0: 6861 7265 645f 696e 7465 7276 616c 7320  hared_intervals 
+00000ac0: 3a20 6c69 7374 0a09 094c 6973 7420 6f66  : list...List of
+00000ad0: 2067 656e 6f6d 6963 2069 6e74 6572 7661   genomic interva
+00000ae0: 6c73 2073 6861 7265 6420 6265 7477 6565  ls shared betwee
+00000af0: 6e20 7468 6520 7477 6f20 696e 7075 7420  n the two input 
+00000b00: 4245 4420 6669 6c65 7320 286f 7220 6c69  BED files (or li
+00000b10: 7374 7329 2e0a 0a09 4578 616d 706c 6573  sts)....Examples
+00000b20: 0a09 2d2d 2d2d 2d2d 2d2d 0a09 3e3e 3e20  ..--------..>>> 
+00000b30: 696e 7465 7273 6563 745f 6265 6433 285b  intersect_bed3([
+00000b40: 2827 6368 7231 272c 2031 2c20 3130 292c  ('chr1', 1, 10),
+00000b50: 2028 2763 6872 3127 2c20 3230 2c20 3335   ('chr1', 20, 35
+00000b60: 295d 2c20 5b28 2763 6872 3127 2c33 2c20  )], [('chr1',3, 
+00000b70: 3135 292c 2028 2763 6872 3127 2c32 302c  15), ('chr1',20,
+00000b80: 2035 3029 5d29 0a09 5b28 2763 6872 3127   50)])..[('chr1'
+00000b90: 2c20 332c 2031 3029 2c20 2827 6368 7231  , 3, 10), ('chr1
+00000ba0: 272c 2032 302c 2033 3529 5d0a 0972 0100  ', 20, 35)]..r..
+00000bb0: 0000 720a 0000 0072 0b00 0000 2913 720c  ..r....r....).r.
+00000bc0: 0000 0072 0d00 0000 720e 0000 0072 0500  ...r....r....r..
+00000bd0: 0000 720f 0000 0072 0400 0000 7208 0000  ..r....r....r...
+00000be0: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000bf0: 7213 0000 0072 1400 0000 7219 0000 00da  r....r....r.....
+00000c00: 0469 616e 6472 1500 0000 7216 0000 0072  .iandr....r....r
+00000c10: 1700 0000 7218 0000 00da 0563 6c65 6172  ....r......clear
+00000c20: 290b da06 696e 6265 6431 da06 696e 6265  )...inbed1..inbe
+00000c30: 6432 5a10 7368 6172 6564 5f69 6e74 6572  d2Z.shared_inter
+00000c40: 7661 6c73 da05 6269 7473 31da 0562 6974  vals..bits1..bit
+00000c50: 7332 721a 0000 00da 036b 6579 721b 0000  s2r......keyr...
+00000c60: 0072 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00000c70: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00000c80: 0e69 6e74 6572 7365 6374 5f62 6564 3349  .intersect_bed3I
+00000c90: 0000 0073 5400 0000 001a 0402 0c01 0c01  ...sT...........
+00000ca0: 0402 0a01 0c01 0201 1201 0601 0e01 1202  ................
+00000cb0: 0e01 0a03 0c01 0c01 0402 0a01 0c01 0201  ................
+00000cc0: 1201 0601 0e01 1202 0e01 0a01 0603 0801  ................
+00000cd0: 0a01 1201 1001 0801 0801 0402 0a01 0c00  ................
+00000ce0: 0401 0a01 1801 0801 0801 0801 7229 0000  ............r)..
+00000cf0: 0063 0200 0000 0000 0000 0000 0000 0a00  .c..............
+00000d00: 0000 0700 0000 4300 0000 73b6 0100 0067  ......C...s....g
+00000d10: 007d 0274 007c 0083 0174 016b 0872 2a74  .}.t.|...t.k.r*t
+00000d20: 027c 0083 0164 016b 0272 207c 0253 0074  .|...d.k.r |.S.t
+00000d30: 037c 0083 017d 036e 5e74 007c 0083 0174  .|...}.n^t.|...t
+00000d40: 046b 0872 707a 1274 0574 06a0 077c 00a1  .k.rpz.t.t...|..
+00000d50: 0183 017d 0357 0071 8801 0001 0001 0074  ...}.W.q.......t
+00000d60: 08a0 0964 027c 0016 00a1 0101 0074 0aa0  ...d.|.......t..
+00000d70: 0b64 03a1 0101 0059 0071 8858 006e 1874  .d.....Y.q.X.n.t
+00000d80: 08a0 0964 027c 0016 00a1 0101 0074 0aa0  ...d.|.......t..
+00000d90: 0b64 03a1 0101 0074 007c 0183 0174 016b  .d.....t.|...t.k
+00000da0: 0872 c474 027c 0183 0164 016b 0272 ba74  .r.t.|...d.k.r.t
+00000db0: 007c 0083 0174 016b 0872 b07c 0053 0074  .|...t.k.r.|.S.t
+00000dc0: 0c7c 0083 0153 006e 0874 037c 0183 017d  .|...S.n.t.|...}
+00000dd0: 046e 6074 007c 0183 0174 046b 0890 0172  .n`t.|...t.k...r
+00000de0: 0c7a 1274 0574 06a0 077c 01a1 0183 017d  .z.t.t...|.....}
+00000df0: 0457 006e 2401 0001 0001 0074 08a0 0964  .W.n$......t...d
+00000e00: 027c 0116 00a1 0101 0074 0aa0 0b64 03a1  .|.......t...d..
+00000e10: 0101 0059 006e 0258 006e 1874 08a0 0964  ...Y.n.X.n.t...d
+00000e20: 027c 0116 00a1 0101 0074 0aa0 0b64 03a1  .|.......t...d..
+00000e30: 0101 007c 0344 005d 7c7d 057c 057c 036b  ...|.D.]|}.|.|.k
+00000e40: 0790 0172 3a90 0171 287c 037c 0519 007d  ...r:..q(|.|...}
+00000e50: 067c 057c 046b 0690 0172 667c 047c 0519  .|.|.k...rf|.|..
+00000e60: 007d 077c 07a0 0da1 0001 007c 06a0 0e7c  .}.|.......|...|
+00000e70: 07a1 0101 0064 017d 087c 06a0 0f7c 08a1  .....d.}.|...|..
+00000e80: 017d 097c 097c 066a 106b 0290 0172 8490  .}.|.|.j.k...r..
+00000e90: 0171 287c 06a0 117c 09a1 017d 087c 02a0  .q(|...|...}.|..
+00000ea0: 127c 057c 097c 0866 03a1 0101 0090 0171  .|.|.|.f.......q
+00000eb0: 6a90 0171 2874 1383 007d 0374 1383 007d  j..q(t...}.t...}
+00000ec0: 047c 0253 0029 0461 4602 0000 0a09 5375  .|.S.).aF.....Su
+00000ed0: 6274 7261 6374 2069 6e62 6564 3220 6672  btract inbed2 fr
+00000ee0: 6f6d 2069 6e62 6564 3120 2869 6e62 6564  om inbed1 (inbed
+00000ef0: 3120 2d20 696e 6265 6432 290a 0a09 5061  1 - inbed2)...Pa
+00000f00: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+00000f10: 2d2d 2d2d 0a09 696e 6265 6431 203a 2073  ----..inbed1 : s
+00000f20: 7472 206f 7220 6c69 7374 0a09 094e 616d  tr or list...Nam
+00000f30: 6520 6f66 2061 2042 4544 2066 696c 6520  e of a BED file 
+00000f40: 6f72 206c 6973 7420 6f66 2067 656e 6f6d  or list of genom
+00000f50: 6963 2069 6e74 6572 7661 6c73 2c20 666f  ic intervals, fo
+00000f60: 7220 6578 616d 706c 652c 0a09 095b 2863  r example,...[(c
+00000f70: 6872 3120 3130 3020 3230 3029 2c20 2863  hr1 100 200), (c
+00000f80: 6872 3220 3130 3030 2031 3230 3029 5d0a  hr2 1000 1200)].
+00000f90: 0969 6e62 6564 3220 3a20 7374 7220 6f72  .inbed2 : str or
+00000fa0: 206c 6973 740a 0909 4e61 6d65 206f 6620   list...Name of 
+00000fb0: 6120 4245 4420 6669 6c65 206f 7220 6c69  a BED file or li
+00000fc0: 7374 206f 6620 6765 6e6f 6d69 6320 696e  st of genomic in
+00000fd0: 7465 7276 616c 732c 2066 6f72 2065 7861  tervals, for exa
+00000fe0: 6d70 6c65 2c0a 0909 5b28 6368 7231 2031  mple,...[(chr1 1
+00000ff0: 3530 2032 3230 292c 2028 6368 7232 2031  50 220), (chr2 1
+00001000: 3130 3020 3133 3030 295d 0a0a 0952 6574  100 1300)]...Ret
+00001010: 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0972  urns..-------..r
+00001020: 656d 6169 6e5f 696e 7465 7276 616c 7320  emain_intervals 
+00001030: 3a20 6c69 7374 0a09 094c 6973 7420 6f66  : list...List of
+00001040: 2067 656e 6f6d 6963 2069 6e74 6572 7661   genomic interva
+00001050: 6c73 2066 726f 6d20 696e 6265 6431 2077  ls from inbed1 w
+00001060: 6974 6820 7468 6f73 6520 7368 6172 6564  ith those shared
+00001070: 2072 6567 696f 6e73 2077 6974 6820 696e   regions with in
+00001080: 6265 6432 2072 656d 6f76 6564 2e0a 0a09  bed2 removed....
+00001090: 4578 616d 706c 6573 0a09 2d2d 2d2d 2d2d  Examples..------
+000010a0: 2d2d 0a09 3e3e 3e20 7375 6274 7261 6374  --..>>> subtract
+000010b0: 5f62 6564 3328 5b28 2763 6872 3127 2c20  _bed3([('chr1', 
+000010c0: 312c 2031 3029 2c20 2827 6368 7231 272c  1, 10), ('chr1',
+000010d0: 2032 302c 2033 3529 5d2c 205b 2827 6368   20, 35)], [('ch
+000010e0: 7231 272c 332c 2031 3529 2c20 2827 6368  r1',3, 15), ('ch
+000010f0: 7231 272c 3230 2c20 3530 295d 290a 095b  r1',20, 50)])..[
+00001100: 2827 6368 7231 272c 2031 2c20 3329 5d0a  ('chr1', 1, 3)].
+00001110: 0a09 7201 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00001120: 0029 1472 0c00 0000 720d 0000 0072 0e00  .).r....r....r..
+00001130: 0000 7205 0000 0072 0f00 0000 7204 0000  ..r....r....r...
+00001140: 0072 0800 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001150: 7212 0000 0072 1300 0000 7214 0000 00da  r....r....r.....
+00001160: 0b62 6564 5f74 6f5f 6c69 7374 da06 696e  .bed_to_list..in
+00001170: 7665 7274 7222 0000 0072 1500 0000 7216  vertr"...r....r.
+00001180: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00001190: 0000 290a 7224 0000 0072 2500 0000 5a10  ..).r$...r%...Z.
+000011a0: 7265 6d61 696e 5f69 6e74 6572 7661 6c73  remain_intervals
+000011b0: 5a08 6269 7473 6574 7331 5a08 6269 7473  Z.bitsets1Z.bits
+000011c0: 6574 7332 721b 0000 0072 2600 0000 7227  ets2r....r&...r'
+000011d0: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+000011e0: 0000 721f 0000 0072 2000 0000 da0d 7375  ..r....r .....su
+000011f0: 6274 7261 6374 5f62 6564 3398 0000 0073  btract_bed3....s
+00001200: 5800 0000 0018 0402 0c01 0c01 0402 0a01  X...............
+00001210: 0c01 0201 1201 0601 0e01 1202 0e01 0a02  ................
+00001220: 0c01 0c01 0c01 0402 0a02 0a01 0e01 0201  ................
+00001230: 1201 0601 0e01 1202 0e01 0a01 0801 0a01  ................
+00001240: 0401 0801 0a01 0801 0801 0a01 0402 0a01  ................
+00001250: 0c00 0401 0a01 1801 0601 0601 722c 0000  ............r,..
+00001260: 0063 0000 0000 0000 0000 0000 0000 0a00  .c..............
+00001270: 0000 0600 0000 4700 0000 73c8 0000 0067  ......G...s....g
+00001280: 007d 017c 0044 005d ba7d 0264 017d 0374  .}.|.D.].}.d.}.t
+00001290: 007c 0283 0174 016b 0872 427c 0244 005d  .|...t.k.rB|.D.]
+000012a0: 1e5c 037d 047d 057d 067c 0374 027c 0683  .\.}.}.}.|.t.|..
+000012b0: 0174 027c 0583 0118 0037 007d 0371 206e  .t.|.....7.}.q n
+000012c0: 7674 007c 0283 0174 036b 0872 b874 04a0  vt.|...t.k.r.t..
+000012d0: 057c 02a1 0144 005d 5e7d 077c 07a0 0664  .|...D.]^}.|...d
+000012e0: 02a1 0172 6871 587c 07a0 07a1 007d 0874  ...rhqX|.....}.t
+000012f0: 087c 0883 0164 036b 0072 8c74 09a0 0a64  .|...d.k.r.t...d
+00001300: 047c 0716 00a1 0101 0071 5874 027c 0864  .|.......qXt.|.d
+00001310: 0519 0083 0174 027c 0864 0619 0083 0118  .....t.|.d......
+00001320: 007d 097c 0964 016b 0172 ae71 587c 037c  .}.|.d.k.r.qX|.|
+00001330: 0937 007d 0371 587c 01a0 0b7c 03a1 0101  .7.}.qX|...|....
+00001340: 0071 087c 0153 0029 0761 3202 0000 0a09  .q.|.S.).a2.....
+00001350: 4361 6c63 756c 6174 6520 7468 6520 6167  Calculate the ag
+00001360: 6772 6567 6174 6564 2073 697a 6520 6f66  gregated size of
+00001370: 2067 656e 6f6d 6963 2069 6e74 6572 7661   genomic interva
+00001380: 6c73 2e0a 0a09 5061 7261 6d65 7465 7273  ls....Parameters
+00001390: 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09 6172  ..----------..ar
+000013a0: 6776 203a 206c 6973 7420 6f66 2067 656e  gv : list of gen
+000013b0: 6f6d 6963 2072 6567 696f 6e73 2e0a 0909  omic regions....
+000013c0: 4561 6368 2061 7267 756d 656e 7420 6361  Each argument ca
+000013d0: 6e20 6265 2061 206c 6973 742c 2042 4544  n be a list, BED
+000013e0: 2d6c 696b 6520 6669 6c65 2c20 6f72 2061  -like file, or a
+000013f0: 2062 6967 4265 6420 6669 6c65 2e20 4245   bigBed file. BE
+00001400: 4420 6669 6c65 0a09 0963 616e 2062 6520  D file...can be 
+00001410: 7265 6775 6c61 722c 2063 6f6d 7072 6573  regular, compres
+00001420: 7365 642c 206f 7220 7265 6d6f 7465 2066  sed, or remote f
+00001430: 696c 652e 2054 6865 2073 7566 6669 7820  ile. The suffix 
+00001440: 6f66 2062 6967 4265 6420 6669 6c65 0a09  of bigBed file..
+00001450: 096d 7573 7420 6265 206f 6e65 206f 6620  .must be one of 
+00001460: 2827 2e62 6227 2c27 2e62 6967 6265 6427  ('.bb','.bigbed'
+00001470: 2c27 2e62 6967 4265 6427 2c27 2e42 6967  ,'.bigBed','.Big
+00001480: 4265 6427 2c20 272e 4242 272c 2720 4249  Bed', '.BB',' BI
+00001490: 4742 4544 2729 2e0a 0a09 5265 7475 726e  GBED')....Return
+000014a0: 730a 092d 2d2d 2d2d 2d2d 0a09 4c69 7374  s..-------..List
+000014b0: 206f 6620 6167 6772 6567 6174 6564 2073   of aggregated s
+000014c0: 697a 652e 0a0a 0945 7861 6d70 6c65 730a  ize....Examples.
+000014d0: 092d 2d2d 2d2d 2d2d 2d0a 093e 3e3e 2069  .--------..>>> i
+000014e0: 6e74 6572 7661 6c73 5f31 203d 205b 2827  ntervals_1 = [('
+000014f0: 6368 7231 272c 2031 2c20 3130 292c 2028  chr1', 1, 10), (
+00001500: 2763 6872 3127 2c20 3230 2c20 3335 295d  'chr1', 20, 35)]
+00001510: 0a09 3e3e 3e20 696e 7465 7276 616c 735f  ..>>> intervals_
+00001520: 3220 3d20 5b28 2763 6872 3127 2c33 2c20  2 = [('chr1',3, 
+00001530: 3135 292c 2028 2763 6872 3127 2c32 302c  15), ('chr1',20,
+00001540: 2035 3029 5d0a 093e 3e3e 2062 6564 5f61   50)]..>>> bed_a
+00001550: 6374 7561 6c5f 7369 7a65 2869 6e74 6572  ctual_size(inter
+00001560: 7661 6c73 5f31 2c20 696e 7465 7276 616c  vals_1, interval
+00001570: 735f 3229 0a09 5b32 342c 2034 325d 0a09  s_2)..[24, 42]..
+00001580: 7201 0000 00a9 03da 0762 726f 7773 6572  r........browser
+00001590: fa01 23da 0574 7261 636b e903 0000 00fa  ..#..track......
+000015a0: 1469 6e76 616c 6964 2042 4544 206c 696e  .invalid BED lin
+000015b0: 653a 2025 73e9 0200 0000 720b 0000 0029  e: %s.....r....)
+000015c0: 0c72 0c00 0000 720d 0000 00da 0369 6e74  .r....r......int
+000015d0: 720f 0000 0072 0800 0000 7210 0000 00da  r....r....r.....
+000015e0: 0a73 7461 7274 7377 6974 68da 0573 706c  .startswith..spl
+000015f0: 6974 720e 0000 0072 1100 0000 da07 7761  itr....r......wa
+00001600: 726e 696e 6772 1800 0000 290a da04 6172  rningr....)...ar
+00001610: 6776 da05 7369 7a65 73da 0361 7267 7216  gv..sizes..argr.
+00001620: 0000 0072 1b00 0000 721e 0000 0072 1d00  ...r....r....r..
+00001630: 0000 da01 6cda 0166 da03 746d 7072 1f00  ....l..f..tmpr..
+00001640: 0000 721f 0000 0072 2000 0000 da0f 6265  ..r....r .....be
+00001650: 645f 6163 7475 616c 5f73 697a 65e4 0000  d_actual_size...
+00001660: 0073 2800 0000 0016 0401 0801 0401 0c01  .s(.............
+00001670: 0e01 1801 0c01 0e01 0a00 0201 0801 0c01  ................
+00001680: 0e01 0201 1801 0801 0201 0a01 0c01 723e  ..............r>
+00001690: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+000016a0: 0600 0000 0600 0000 4700 0000 738a 0000  ........G...s...
+000016b0: 0067 007d 017c 0044 005d 7c7d 0264 017d  .g.}.|.D.]|}.d.}
+000016c0: 0374 007c 0283 0174 016b 0872 2674 027c  .t.|...t.k.r&t.|
+000016d0: 0283 017d 036e 5474 007c 0283 0174 036b  ...}.nTt.|...t.k
+000016e0: 0872 7a74 04a0 057c 02a1 0144 005d 3c7d  .rzt...|...D.]<}
+000016f0: 047c 04a0 0664 02a1 0172 4c71 3c7c 04a0  .|...d...rLq<|..
+00001700: 07a1 007d 0574 027c 0583 0164 036b 0072  ...}.t.|...d.k.r
+00001710: 7074 08a0 0964 047c 0416 00a1 0101 0071  pt...d.|.......q
+00001720: 3c7c 0364 0537 007d 0371 3c7c 01a0 0a7c  <|.d.7.}.q<|...|
+00001730: 03a1 0101 0071 087c 0153 0029 0661 2502  .....q.|.S.).a%.
+00001740: 0000 0a09 4361 6c63 756c 6174 6520 7468  ....Calculate th
+00001750: 6520 6e75 6d62 6572 206f 6620 6765 6e6f  e number of geno
+00001760: 6d69 6320 696e 7465 7276 616c 7320 696e  mic intervals in
+00001770: 2042 4544 2066 696c 652e 0a0a 0a09 5061   BED file.....Pa
+00001780: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+00001790: 2d2d 2d2d 0a09 6172 6776 203a 206c 6973  ----..argv : lis
+000017a0: 7420 6f66 2067 656e 6f6d 6963 2072 6567  t of genomic reg
+000017b0: 696f 6e73 2e0a 0909 4561 6368 2061 7267  ions....Each arg
+000017c0: 756d 656e 7420 6361 6e20 6265 2061 206c  ument can be a l
+000017d0: 6973 742c 2042 4544 2d6c 696b 6520 6669  ist, BED-like fi
+000017e0: 6c65 2c20 6f72 2061 2062 6967 4265 6420  le, or a bigBed 
+000017f0: 6669 6c65 2e20 4245 4420 6669 6c65 0a09  file. BED file..
+00001800: 0963 616e 2062 6520 7265 6775 6c61 722c  .can be regular,
+00001810: 2063 6f6d 7072 6573 7365 642c 206f 7220   compressed, or 
+00001820: 7265 6d6f 7465 2066 696c 652e 2054 6865  remote file. The
+00001830: 2073 7566 6669 7820 6f66 2062 6967 4265   suffix of bigBe
+00001840: 6420 6669 6c65 0a09 096d 7573 7420 6265  d file...must be
+00001850: 206f 6e65 206f 6620 2827 2e62 6227 2c27   one of ('.bb','
+00001860: 2e62 6967 6265 6427 2c27 2e62 6967 4265  .bigbed','.bigBe
+00001870: 6427 2c27 2e42 6967 4265 6427 2c20 272e  d','.BigBed', '.
+00001880: 4242 272c 2720 4249 4742 4544 2729 2e0a  BB',' BIGBED')..
+00001890: 0a09 5265 7475 726e 730a 092d 2d2d 2d2d  ..Returns..-----
+000018a0: 2d2d 0a09 4c69 7374 206f 6620 6167 6772  --..List of aggr
+000018b0: 6567 6174 6564 2073 697a 652e 0a0a 0945  egated size....E
+000018c0: 7861 6d70 6c65 730a 092d 2d2d 2d2d 2d2d  xamples..-------
+000018d0: 2d0a 093e 3e3e 2062 6564 3120 3d20 5b28  -..>>> bed1 = [(
+000018e0: 2763 6872 3127 2c20 312c 2031 3029 2c20  'chr1', 1, 10), 
+000018f0: 2827 6368 7231 272c 2032 302c 2033 3529  ('chr1', 20, 35)
+00001900: 5d0a 093e 3e3e 2062 6564 3220 3d20 5b28  ]..>>> bed2 = [(
+00001910: 2763 6872 3127 2c33 2c20 3135 292c 2028  'chr1',3, 15), (
+00001920: 2763 6872 3127 2c32 302c 2035 3029 2c20  'chr1',20, 50), 
+00001930: 2827 6368 7232 272c 3130 302c 3230 3029  ('chr2',100,200)
+00001940: 5d0a 093e 3e3e 2062 6564 5f63 6f75 6e74  ]..>>> bed_count
+00001950: 7328 6265 6431 2c20 6265 6432 290a 095b  s(bed1, bed2)..[
+00001960: 322c 2033 5d0a 0972 0100 0000 722d 0000  2, 3]..r....r-..
+00001970: 0072 3100 0000 7232 0000 0072 0b00 0000  .r1...r2...r....
+00001980: 290b 720c 0000 0072 0d00 0000 720e 0000  ).r....r....r...
+00001990: 0072 0f00 0000 7208 0000 0072 1000 0000  .r....r....r....
+000019a0: 7235 0000 0072 3600 0000 7211 0000 0072  r5...r6...r....r
+000019b0: 3700 0000 7218 0000 0029 0672 3800 0000  7...r....).r8...
+000019c0: da0a 6265 645f 636f 756e 7473 723a 0000  ..bed_countsr:..
+000019d0: 00da 0563 6f75 6e74 723b 0000 0072 3c00  ...countr;...r<.
+000019e0: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+000019f0: 0072 3f00 0000 0f01 0000 7320 0000 0000  .r?.......s ....
+00001a00: 1704 0108 0104 010c 010a 010c 010e 010a  ................
+00001a10: 0002 0108 010c 010e 0102 010a 010c 0172  ...............r
+00001a20: 3f00 0000 6300 0000 0000 0000 0000 0000  ?...c...........
+00001a30: 0009 0000 0008 0000 0047 0000 0073 d800  .........G...s..
+00001a40: 0000 6700 7d01 7c00 4400 5dca 7d02 7400  ..g.}.|.D.].}.t.
+00001a50: 7c02 8301 7401 6b08 7222 7402 7c02 8301  |...t.k.r"t.|...
+00001a60: 7d03 6e5e 7400 7c02 8301 7403 6b08 7268  }.n^t.|...t.k.rh
+00001a70: 7a12 7404 7405 a006 7c02 a101 8301 7d03  z.t.t...|.....}.
+00001a80: 5700 7180 0100 0100 0100 7407 a008 6401  W.q.......t...d.
+00001a90: 7c02 1600 a101 0100 7409 a00a 6402 a101  |.......t...d...
+00001aa0: 0100 5900 7180 5800 6e18 7407 a008 6401  ..Y.q.X.n.t...d.
+00001ab0: 7c02 1600 a101 0100 7409 a00a 6402 a101  |.......t...d...
+00001ac0: 0100 6403 7d04 7c03 4400 5d3e 7d05 7c03  ..d.}.|.D.]>}.|.
+00001ad0: 7c05 1900 7d06 6403 7d07 7c06 a00b 7c07  |...}.d.}.|...|.
+00001ae0: a101 7d08 7c08 7c06 6a0c 6b02 72ae 7188  ..}.|.|.j.k.r.q.
+00001af0: 7c06 a00d 7c08 a101 7d07 7c04 7c07 7c08  |...|...}.|.|.|.
+00001b00: 1800 3700 7d04 7198 7188 7c01 a00e 7c04  ..7.}.q.q.|...|.
+00001b10: a101 0100 7108 7c01 5300 2904 61c8 0200  ....q.|.S.).a...
+00001b20: 000a 0943 616c 6375 6c61 7465 2074 6865  ...Calculate the
+00001b30: 202a 6765 6e6f 6d69 632f 756e 6971 7565   *genomic/unique
+00001b40: 2073 697a 652a 206f 6620 4245 4420 6669   size* of BED fi
+00001b50: 6c65 7320 286f 7220 6c69 7374 7320 6f66  les (or lists of
+00001b60: 2067 656e 6f6d 6963 2069 6e74 6572 7661   genomic interva
+00001b70: 6c73 292e 0a09 4e6f 7465 2c20 6765 6e6f  ls)...Note, geno
+00001b80: 6d69 635f 7369 7a65 203c 3d20 6163 7475  mic_size <= actu
+00001b90: 616c 5f73 697a 652e 0a0a 0950 6172 616d  al_size....Param
+00001ba0: 6574 6572 730a 092d 2d2d 2d2d 2d2d 2d2d  eters..---------
+00001bb0: 2d0a 0961 7267 7620 3a20 6c69 7374 206f  -..argv : list o
+00001bc0: 6620 6765 6e6f 6d69 6320 7265 6769 6f6e  f genomic region
+00001bd0: 732e 0a09 0945 6163 6820 6172 6775 6d65  s....Each argume
+00001be0: 6e74 2063 616e 2062 6520 6120 6c69 7374  nt can be a list
+00001bf0: 2c20 4245 442d 6c69 6b65 2066 696c 652c  , BED-like file,
+00001c00: 206f 7220 6120 6269 6742 6564 2066 696c   or a bigBed fil
+00001c10: 652e 2042 4544 2066 696c 650a 0909 6361  e. BED file...ca
+00001c20: 6e20 6265 2072 6567 756c 6172 2c20 636f  n be regular, co
+00001c30: 6d70 7265 7373 6564 2c20 6f72 2072 656d  mpressed, or rem
+00001c40: 6f74 6520 6669 6c65 2e20 5468 6520 7375  ote file. The su
+00001c50: 6666 6978 206f 6620 6269 6742 6564 2066  ffix of bigBed f
+00001c60: 696c 650a 0909 6d75 7374 2062 6520 6f6e  ile...must be on
+00001c70: 6520 6f66 2028 272e 6262 272c 272e 6269  e of ('.bb','.bi
+00001c80: 6762 6564 272c 272e 6269 6742 6564 272c  gbed','.bigBed',
+00001c90: 272e 4269 6742 6564 272c 2027 2e42 4227  '.BigBed', '.BB'
+00001ca0: 2c27 2042 4947 4245 4427 292e 0a0a 0952  ,' BIGBED')....R
+00001cb0: 6574 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a  eturns..-------.
+00001cc0: 094c 6973 7420 6f66 2067 656e 6f6d 6963  .List of genomic
+00001cd0: 2073 697a 652e 0a0a 0945 7861 6d70 6c65   size....Example
+00001ce0: 0a09 2d2d 2d2d 2d2d 2d0a 093e 3e3e 2062  ..-------..>>> b
+00001cf0: 6564 3120 3d20 5b28 2763 6872 3127 2c20  ed1 = [('chr1', 
+00001d00: 302c 2031 3030 292c 2028 2763 6872 3127  0, 100), ('chr1'
+00001d10: 2c20 3530 2c20 3135 3029 2c20 2827 6368  , 50, 150), ('ch
+00001d20: 7231 272c 2038 302c 2031 3830 295d 0a09  r1', 80, 180)]..
+00001d30: 3e3e 3e20 6265 645f 6765 6e6f 6d69 635f  >>> bed_genomic_
+00001d40: 7369 7a65 2862 6564 3129 0a09 5b31 3830  size(bed1)..[180
+00001d50: 5d0a 093e 3e3e 2062 6564 3220 3d20 5b28  ]..>>> bed2 = [(
+00001d60: 2763 6872 3127 2c20 302c 2031 3030 292c  'chr1', 0, 100),
+00001d70: 2028 2763 6872 3227 2c20 3530 2c20 3135   ('chr2', 50, 15
+00001d80: 3029 2c20 2827 6368 7233 272c 2038 302c  0), ('chr3', 80,
+00001d90: 2031 3830 295d 0a09 3e3e 3e20 6265 645f   180)]..>>> bed_
+00001da0: 6765 6e6f 6d69 635f 7369 7a65 2862 6564  genomic_size(bed
+00001db0: 3229 0a09 5b33 3030 5d0a 093e 3e3e 2062  2)..[300]..>>> b
+00001dc0: 6564 5f67 656e 6f6d 6963 5f73 697a 6528  ed_genomic_size(
+00001dd0: 6265 6431 2c20 6265 6432 290a 095b 3138  bed1, bed2)..[18
+00001de0: 302c 2033 3030 5d0a 097a 1149 6e76 616c  0, 300]..z.Inval
+00001df0: 6964 2069 6e70 7574 3a20 2573 720b 0000  id input: %sr...
+00001e00: 0072 0100 0000 290f 720c 0000 0072 0d00  .r....).r....r..
+00001e10: 0000 7205 0000 0072 0f00 0000 7204 0000  ..r....r....r...
+00001e20: 0072 0800 0000 7210 0000 0072 1100 0000  .r....r....r....
+00001e30: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00001e40: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
+00001e50: 0000 0029 0972 3800 0000 5a0b 756e 696f  ...).r8...Z.unio
+00001e60: 6e5f 7369 7a65 7372 3a00 0000 721a 0000  n_sizesr:...r...
+00001e70: 00da 0a75 6e69 6f6e 5f73 697a 6572 1b00  ...union_sizer..
+00001e80: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00001e90: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00001ea0: da10 6265 645f 6765 6e6f 6d69 635f 7369  ..bed_genomic_si
+00001eb0: 7a65 3701 0000 732e 0000 0000 1b04 0108  ze7...s.........
+00001ec0: 010c 010a 010c 0102 0112 0106 010e 0112  ................
+00001ed0: 020e 010a 0104 0108 0108 0104 020a 010a  ................
+00001ee0: 0002 010a 0110 010c 0172 4200 0000 6302  .........rB...c.
+00001ef0: 0000 0000 0000 0000 0000 000b 0000 0005  ................
+00001f00: 0000 0043 0000 0073 ca00 0000 6401 7d02  ...C...s....d.}.
+00001f10: 7400 7c00 8301 7401 6b08 721a 7402 7c00  t.|...t.k.r.t.|.
+00001f20: 8301 7d03 6e0e 7403 7404 a005 7c00 a101  ..}.n.t.t...|...
+00001f30: 8301 7d03 7400 7c01 8301 7401 6b08 723e  ..}.t.|...t.k.r>
+00001f40: 7402 7c01 8301 7d04 6e0e 7403 7404 a005  t.|...}.n.t.t...
+00001f50: 7c01 a101 8301 7d04 7406 8300 7d05 7c03  |.....}.t...}.|.
+00001f60: 4400 5d2a 7d06 7c06 7c04 6b06 7256 7c03  D.]*}.|.|.k.rV|.
+00001f70: 7c06 1900 a007 7c04 7c06 1900 a101 0100  |.....|.|.......
+00001f80: 7c03 7c06 1900 7c05 7c06 3c00 7156 7c05  |.|...|.|.<.qV|.
+00001f90: 4400 5d3e 7d07 7c05 7c07 1900 7d08 6401  D.]>}.|.|...}.d.
+00001fa0: 7d09 7c08 a008 7c09 a101 7d0a 7c0a 7c08  }.|...|...}.|.|.
+00001fb0: 6a09 6b02 72ac 7186 7c08 a00a 7c0a a101  j.k.r.q.|...|...
+00001fc0: 7d09 7c02 7c09 7c0a 1800 3700 7d02 7196  }.|.|.|...7.}.q.
+00001fd0: 7186 7c02 5300 2902 6178 0200 000a 0943  q.|.S.).ax.....C
+00001fe0: 616c 6375 6c61 7465 2074 6865 2074 6f74  alculate the tot
+00001ff0: 616c 206e 756d 6265 7220 6f66 202a 6261  al number of *ba
+00002000: 7365 732a 206f 7665 726c 6170 7065 6420  ses* overlapped 
+00002010: 6265 7477 6565 6e20 7477 6f20 6265 6420  between two bed 
+00002020: 6669 6c65 7320 6f72 0a09 7477 6f20 6c69  files or..two li
+00002030: 7374 7320 6f66 2067 656e 6f6d 6963 2069  sts of genomic i
+00002040: 6e74 6572 7661 6c73 2e0a 0a09 5061 7261  ntervals....Para
+00002050: 6d65 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d  meters..--------
+00002060: 2d2d 0a09 6265 6431 203a 2073 7472 206f  --..bed1 : str o
+00002070: 7220 6c69 7374 0a09 0946 696c 6520 6e61  r list...File na
+00002080: 6d65 206f 6620 7468 6520 6669 7273 7420  me of the first 
+00002090: 4245 4420 6669 6c65 2e20 4361 6e20 616c  BED file. Can al
+000020a0: 736f 2062 6520 6120 6c69 7374 2c20 7375  so be a list, su
+000020b0: 6368 2061 730a 0909 5b28 6368 7231 2031  ch as...[(chr1 1
+000020c0: 3030 2032 3030 292c 2028 6368 7232 2031  00 200), (chr2 1
+000020d0: 3530 2020 3330 3029 2c20 2863 6872 3220  50  300), (chr2 
+000020e0: 3130 3030 2031 3230 3029 5d0a 0962 6564  1000 1200)]..bed
+000020f0: 3220 3a20 7374 7220 6f72 206c 6973 740a  2 : str or list.
+00002100: 0909 4669 6c65 206e 616d 6520 6f66 2074  ..File name of t
+00002110: 6865 2073 6563 6f6e 6420 4245 4420 6669  he second BED fi
+00002120: 6c65 2e20 4361 6e20 616c 736f 2062 6520  le. Can also be 
+00002130: 6120 6c69 7374 2c20 7375 6368 2061 730a  a list, such as.
+00002140: 0909 5b28 6368 7231 2031 3030 2032 3030  ..[(chr1 100 200
+00002150: 292c 2028 6368 7232 2031 3530 2020 3330  ), (chr2 150  30
+00002160: 3029 2c20 2863 6872 3220 3130 3030 2031  0), (chr2 1000 1
+00002170: 3230 3029 5d0a 0a09 4578 616d 706c 650a  200)]...Example.
+00002180: 092d 2d2d 2d2d 2d2d 0a09 3e3e 3e20 696e  .-------..>>> in
+00002190: 7075 745f 6461 7461 3120 3d20 5b28 2763  put_data1 = [('c
+000021a0: 6872 3127 2c20 312c 2031 3029 2c20 2827  hr1', 1, 10), ('
+000021b0: 6368 7231 272c 2032 302c 2033 3529 5d0a  chr1', 20, 35)].
+000021c0: 093e 3e3e 2069 6e70 7574 5f64 6174 6132  .>>> input_data2
+000021d0: 203d 205b 2827 6368 7231 272c 332c 2031   = [('chr1',3, 1
+000021e0: 3529 2c20 2827 6368 7231 272c 3230 2c20  5), ('chr1',20, 
+000021f0: 3530 295d 0a09 3e3e 3e20 6265 645f 6f76  50)]..>>> bed_ov
+00002200: 6572 6c61 705f 7369 7a65 2869 6e70 7574  erlap_size(input
+00002210: 5f64 6174 6131 2c20 696e 7075 745f 6461  _data1, input_da
+00002220: 7461 3229 0a09 3232 0a0a 0952 6574 7572  ta2)..22...Retur
+00002230: 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0949 6e74  ns..-------..Int
+00002240: 2e20 4f76 6572 6c61 7070 6564 2073 697a  . Overlapped siz
+00002250: 652e 0a0a 0972 0100 0000 290b 720c 0000  e....r....).r...
+00002260: 0072 0d00 0000 7205 0000 0072 0400 0000  .r....r....r....
+00002270: 7208 0000 0072 1000 0000 7219 0000 0072  r....r....r....r
+00002280: 2200 0000 7215 0000 0072 1600 0000 7217  "...r....r....r.
+00002290: 0000 0029 0b5a 0462 6564 315a 0462 6564  ...).Z.bed1Z.bed
+000022a0: 32da 0c6f 7665 726c 6170 5f73 697a 6572  2..overlap_sizer
+000022b0: 2600 0000 7227 0000 0072 1a00 0000 7228  &...r'...r....r(
+000022c0: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
+000022d0: 0000 721e 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+000022e0: 0072 2000 0000 da10 6265 645f 6f76 6572  .r .....bed_over
+000022f0: 6c61 705f 7369 7a65 6b01 0000 732a 0000  lap_sizek...s*..
+00002300: 0000 1a04 010c 010a 020e 010c 010a 020e  ................
+00002310: 0106 0108 0108 0112 010e 0108 0108 0104  ................
+00002320: 020a 010a 0002 010a 0110 0172 4400 0000  ...........rD...
+00002330: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+00002340: 0005 0000 0043 0000 0073 3e01 0000 7400  .....C...s>...t.
+00002350: a001 6401 7c00 1600 a101 0100 6900 7d01  ..d.|.......i.}.
+00002360: 7402 7c00 8301 7c01 6402 3c00 7403 7c00  t.|...|.d.<.t.|.
+00002370: 8301 6403 1900 7c01 6404 3c00 6403 7c01  ..d...|.d.<.d.|.
+00002380: 6405 3c00 6403 7c01 6406 3c00 6403 7d02  d.<.d.|.d.<.d.}.
+00002390: 6700 7d03 7404 a005 7c00 a101 4400 5d9e  g.}.t...|...D.].
+000023a0: 7d04 7c04 a006 6407 a101 7260 7150 7c04  }.|...d...r`qP|.
+000023b0: a007 a100 7d05 7408 7c05 8301 6408 6b00  ....}.t.|...d.k.
+000023c0: 7282 7400 a009 6409 7c04 1600 a101 0100  r.t...d.|.......
+000023d0: 740a 7c05 640a 1900 8301 740a 7c05 640b  t.|.d.....t.|.d.
+000023e0: 1900 8301 1800 6403 6b00 72ac 7400 a009  ......d.k.r.t...
+000023f0: 6409 7c04 1600 a101 0100 7c01 6406 0500  d.|.......|.d...
+00002400: 1900 640b 3700 0300 3c00 740a 7c05 640a  ..d.7...<.t.|.d.
+00002410: 1900 8301 740a 7c05 640b 1900 8301 1800  ....t.|.d.......
+00002420: 7d02 7c01 6405 0500 1900 7c02 3700 0300  }.|.d.....|.7...
+00002430: 3c00 7c03 a00b 7c02 a101 0100 7150 740c  <.|...|.....qPt.
+00002440: a00d 7c03 a101 7c01 640c 3c00 740c a00e  ..|...|.d.<.t...
+00002450: 7c03 a101 7c01 640d 3c00 740c a00f 7c03  |...|.d.<.t...|.
+00002460: a101 7c01 640e 3c00 740c a010 7c03 a101  ..|.d.<.t...|...
+00002470: 7c01 640f 3c00 740c 6a11 7c03 640b 6410  |.d.<.t.j.|.d.d.
+00002480: 8d02 7c01 6411 3c00 7c01 5300 2912 7a2b  ..|.d.<.|.S.).z+
+00002490: 0a09 4261 7369 6320 696e 666f 726d 6174  ..Basic informat
+000024a0: 696f 6e20 6f66 2067 656e 6f6d 6963 2069  ion of genomic i
+000024b0: 6e74 6572 7661 6c73 2e0a 097a 2e47 6174  ntervals...z.Gat
+000024c0: 6865 7269 6e67 2074 6568 2062 6173 6963  hering teh basic
+000024d0: 2073 7461 7469 7374 6963 7320 6f66 2042   statistics of B
+000024e0: 4544 2066 696c 653a 2025 73da 044e 616d  ED file: %s..Nam
+000024f0: 6572 0100 0000 5a0c 4765 6e6f 6d69 635f  er....Z.Genomic_
+00002500: 7369 7a65 5a0a 546f 7461 6c5f 7369 7a65  sizeZ.Total_size
+00002510: 5a05 436f 756e 7472 2d00 0000 7231 0000  Z.Countr-...r1..
+00002520: 0072 3200 0000 7233 0000 0072 0b00 0000  .r2...r3...r....
+00002530: 5a09 4d65 616e 5f73 697a 655a 0b4d 6564  Z.Mean_sizeZ.Med
+00002540: 6961 6e5f 7369 7a65 5a08 4d69 6e5f 7369  ian_sizeZ.Min_si
+00002550: 7a65 5a08 4d61 785f 7369 7a65 2901 5a04  zeZ.Max_size).Z.
+00002560: 6464 6f66 5a03 5354 4429 1272 1100 0000  ddofZ.STD).r....
+00002570: da05 6465 6275 6772 0200 0000 7242 0000  ..debugr....rB..
+00002580: 0072 0800 0000 7210 0000 0072 3500 0000  .r....r....r5...
+00002590: 7236 0000 0072 0e00 0000 7212 0000 0072  r6...r....r....r
+000025a0: 3400 0000 7218 0000 00da 026e 705a 046d  4...r......npZ.m
+000025b0: 6561 6e5a 066d 6564 6961 6eda 036d 696e  eanZ.median..min
+000025c0: da03 6d61 785a 0373 7464 2906 da06 696e  ..maxZ.std)...in
+000025d0: 6669 6c65 5a09 6265 645f 696e 666f 7272  fileZ.bed_inforr
+000025e0: 1600 0000 7239 0000 0072 3b00 0000 723c  ....r9...r;...r<
+000025f0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00002600: 0000 da08 6265 645f 696e 666f 9d01 0000  ....bed_info....
+00002610: 7334 0000 0000 040e 0104 010c 0110 0108  s4..............
+00002620: 0108 0104 0104 010e 010a 0102 0108 010c  ................
+00002630: 010e 011c 010e 0110 0118 0110 010c 010e  ................
+00002640: 010e 010e 010e 0112 0272 4b00 0000 6301  .........rK...c.
+00002650: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00002660: 0000 0043 0000 0073 c400 0000 6700 7d01  ...C...s....g.}.
+00002670: 7400 a001 7c00 a101 4400 5db0 7d02 7c02  t...|...D.].}.|.
+00002680: a002 a100 7d02 7c02 a003 6401 a101 730e  ....}.|...d...s.
+00002690: 7c02 a003 6402 a101 730e 7c02 a003 6403  |...d...s.|...d.
+000026a0: a101 723a 710e 7c02 a004 a100 7d03 7405  ..r:q.|.....}.t.
+000026b0: 7c03 8301 6404 6b00 7266 7406 a007 6405  |...d.k.rft...d.
+000026c0: 7c02 1600 a101 0100 7408 a009 6406 a101  |.......t...d...
+000026d0: 0100 740a 7c03 6407 1900 8301 740a 7c03  ..t.|.d.....t.|.
+000026e0: 6406 1900 8301 1800 6408 6b00 729a 7406  d.......d.k.r.t.
+000026f0: a007 6405 7c02 1600 a101 0100 7408 a009  ..d.|.......t...
+00002700: 6406 a101 0100 7c01 a00b 7c03 6408 1900  d.....|...|.d...
+00002710: 740a 7c03 6406 1900 8301 740a 7c03 6407  t.|.d.....t.|.d.
+00002720: 1900 8301 6603 a101 0100 710e 7c01 5300  ....f.....q.|.S.
+00002730: 2909 7a21 0a09 436f 6e76 6572 7420 4245  ).z!..Convert BE
+00002740: 4420 6669 6c65 2069 6e74 6f20 6120 6c69  D file into a li
+00002750: 7374 2e0a 0972 2e00 0000 722f 0000 0072  st...r....r/...r
+00002760: 3000 0000 7231 0000 0072 3200 0000 720b  0...r1...r2...r.
+00002770: 0000 0072 3300 0000 7201 0000 0029 0c72  ...r3...r....).r
+00002780: 0800 0000 7210 0000 00da 0573 7472 6970  ....r......strip
+00002790: 7235 0000 0072 3600 0000 720e 0000 0072  r5...r6...r....r
+000027a0: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
+000027b0: 0000 0072 3400 0000 7218 0000 0029 045a  ...r4...r....).Z
+000027c0: 0762 6564 6669 6c65 5a07 7265 6769 6f6e  .bedfileZ.region
+000027d0: 7372 3b00 0000 723c 0000 0072 1f00 0000  sr;...r<...r....
+000027e0: 721f 0000 0072 2000 0000 722a 0000 00be  r....r ...r*....
+000027f0: 0100 0073 1c00 0000 0004 0402 0e01 0801  ...s............
+00002800: 1e01 0201 0801 0c01 0e01 0a01 1c01 0e01  ................
+00002810: 0a01 2601 722a 0000 0063 0200 0000 0000  ..&.r*...c......
+00002820: 0000 0000 0000 1300 0000 0600 0000 4300  ..............C.
+00002830: 0000 7364 0200 0074 00a0 0164 017c 0016  ..sd...t...d.|..
+00002840: 00a1 0101 0074 027c 0083 017d 0274 00a0  .....t.|...}.t..
+00002850: 0164 027c 0074 037c 0283 0166 0216 00a1  .d.|.t.|...f....
+00002860: 0101 0074 00a0 0164 017c 0116 00a1 0101  ...t...d.|......
+00002870: 0074 027c 0183 017d 0374 00a0 0164 027c  .t.|...}.t...d.|
+00002880: 0174 037c 0383 0166 0216 00a1 0101 0074  .t.|...f.......t
+00002890: 00a0 0164 037c 007c 0166 0216 00a1 0101  ...d.|.|.f......
+000028a0: 0074 027c 027c 0317 0083 017d 0474 00a0  .t.|.|.....}.t..
+000028b0: 0164 0474 037c 0483 0116 00a1 0101 0074  .d.t.|.........t
+000028c0: 00a0 0164 057c 0016 00a1 0101 0069 007d  ...d.|.......i.}
+000028d0: 057c 0244 005d 305c 037d 067d 077d 087c  .|.D.]0\.}.}.}.|
+000028e0: 067c 056b 0772 ba74 0483 007c 057c 063c  .|.k.r.t...|.|.<
+000028f0: 007c 057c 0619 00a0 0574 067c 077c 0883  .|.|.....t.|.|..
+00002900: 02a1 0101 0071 9e74 00a0 0164 057c 0116  .....q.t...d.|..
+00002910: 00a1 0101 0069 007d 097c 0344 005d 325c  .....i.}.|.D.]2\
+00002920: 037d 0a7d 0b7d 0c7c 0a7c 096b 0790 0172  .}.}.}.|.|.k...r
+00002930: 0474 0483 007c 097c 0a3c 007c 097c 0a19  .t...|.|.<.|.|..
+00002940: 00a0 0574 067c 0b7c 0c83 02a1 0101 0071  ...t.|.|.......q
+00002950: e674 00a0 0164 06a1 0101 0067 007d 0d67  .t...d.....g.}.g
+00002960: 007d 0e67 007d 0f7c 0444 005d e65c 037d  .}.g.}.|.D.].\.}
+00002970: 107d 117d 127c 107c 056b 0690 0172 dc7c  .}.}.|.|.k...r.|
+00002980: 107c 096b 0690 0172 dc74 037c 057c 1019  .|.k...r.t.|.|..
+00002990: 00a0 077c 117c 12a1 0283 0164 076b 0490  ...|.|.....d.k..
+000029a0: 0172 aa74 037c 097c 1019 00a0 077c 117c  .r.t.|.|.....|.|
+000029b0: 12a1 0283 0164 076b 0490 0172 987c 0fa0  .....d.k...r.|..
+000029c0: 087c 107c 117c 1266 03a1 0101 006e 107c  .|.|.|.f.....n.|
+000029d0: 0da0 087c 107c 117c 1266 03a1 0101 006e  ...|.|.|.f.....n
+000029e0: 3074 037c 097c 1019 00a0 077c 117c 12a1  0t.|.|.....|.|..
+000029f0: 0283 0164 076b 0490 0172 347c 0ea0 087c  ...d.k...r4|...|
+00002a00: 107c 117c 1266 03a1 0101 006e 0490 0171  .|.|.f.....n...q
+00002a10: 346e 3c7c 107c 056b 0690 0172 f87c 0da0  4n<|.|.k...r.|..
+00002a20: 087c 107c 117c 1266 03a1 0101 006e 207c  .|.|.|.f.....n |
+00002a30: 107c 096b 0690 0172 347c 0ea0 087c 107c  .|.k...r4|...|.|
+00002a40: 117c 1266 03a1 0101 006e 0490 0171 3490  .|.f.....n...q4.
+00002a50: 0171 3474 00a0 0164 087c 0074 037c 0d83  .q4t...d.|.t.|..
+00002a60: 0166 0216 00a1 0101 0074 00a0 0164 087c  .f.......t...d.|
+00002a70: 0174 037c 0e83 0166 0216 00a1 0101 0074  .t.|...f.......t
+00002a80: 00a0 0164 0974 037c 0f83 0116 00a1 0101  ...d.t.|........
+00002a90: 007c 0d7c 0e7c 0f66 0353 0029 0a61 d703  .|.|.|.f.S.).a..
+00002aa0: 0000 0a09 436f 6d70 6172 6520 7477 6f20  ....Compare two 
+00002ab0: 4245 4420 6669 6c65 7320 286f 7220 6c69  BED files (or li
+00002ac0: 7374 7329 2e20 5468 6973 2066 756e 6374  sts). This funct
+00002ad0: 696f 6e20 6973 2073 696d 696c 6172 2074  ion is similar t
+00002ae0: 6f20 4c69 6e75 7820 2263 6f6d 6d22 2063  o Linux "comm" c
+00002af0: 6f6d 6d61 6e64 2e0a 0a09 5061 7261 6d65  ommand....Parame
+00002b00: 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d  ters..----------
+00002b10: 0a09 696e 6265 6431 203a 2073 7472 206f  ..inbed1 : str o
+00002b20: 7220 6c69 7374 0a09 094e 616d 6520 6f66  r list...Name of
+00002b30: 2061 2042 4544 2066 696c 6520 6f72 206c   a BED file or l
+00002b40: 6973 7420 6f66 2042 4544 2072 6567 696f  ist of BED regio
+00002b50: 6e73 2c20 666f 7220 6578 616d 706c 652c  ns, for example,
+00002b60: 0a09 095b 2863 6872 3120 3130 3020 3230  ...[(chr1 100 20
+00002b70: 3029 2c20 2863 6872 3220 3135 3020 2033  0), (chr2 150  3
+00002b80: 3030 292c 2028 6368 7232 2031 3030 3020  00), (chr2 1000 
+00002b90: 3132 3030 295d 0a09 696e 6265 6432 203a  1200)]..inbed2 :
+00002ba0: 2073 7472 206f 7220 6c69 7374 0a09 094e   str or list...N
+00002bb0: 616d 6520 6f66 2061 2042 4544 2066 696c  ame of a BED fil
+00002bc0: 6520 6f72 206c 6973 7420 6f66 2042 4544  e or list of BED
+00002bd0: 2072 6567 696f 6e73 2c20 666f 7220 6578   regions, for ex
+00002be0: 616d 706c 652c 0a09 095b 2863 6872 3120  ample,...[(chr1 
+00002bf0: 3130 3020 3230 3029 2c20 2863 6872 3220  100 200), (chr2 
+00002c00: 3135 3020 2033 3030 292c 2028 6368 7232  150  300), (chr2
+00002c10: 2031 3030 3020 3132 3030 295d 0a0a 0952   1000 1200)]...R
+00002c20: 6574 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a  eturns..-------.
+00002c30: 0962 6564 315f 756e 6971 203a 206c 6973  .bed1_uniq : lis
+00002c40: 740a 0909 4765 6e6f 6d69 6320 7265 6769  t...Genomic regi
+00002c50: 6f6e 7320 7468 6174 2061 7265 2069 6e62  ons that are inb
+00002c60: 6564 3120 756e 6971 7565 2028 692e 652e  ed1 unique (i.e.
+00002c70: 2c20 7265 6769 6f6e 7320 6f6e 6c79 2070  , regions only p
+00002c80: 7265 7365 6e74 2069 6e20 696e 6265 6431  resent in inbed1
+00002c90: 2062 7574 0a09 0964 6f20 6e6f 7420 6f76   but...do not ov
+00002ca0: 6572 6c61 7020 7769 7468 2061 6e79 2072  erlap with any r
+00002cb0: 6567 696f 6e73 2069 6e20 696e 6265 6432  egions in inbed2
+00002cc0: 292e 0a09 6265 6432 5f75 6e69 7120 3a20  )...bed2_uniq : 
+00002cd0: 6c69 7374 0a09 0947 656e 6f6d 6963 2072  list...Genomic r
+00002ce0: 6567 696f 6e73 2074 6861 7420 6172 6520  egions that are 
+00002cf0: 696e 6265 6432 2075 6e69 7175 6520 2869  inbed2 unique (i
+00002d00: 2e65 2e2c 2072 6567 696f 6e73 206f 6e6c  .e., regions onl
+00002d10: 7920 7072 6573 656e 7420 696e 2069 6e62  y present in inb
+00002d20: 6564 3220 6275 740a 0909 646f 206e 6f74  ed2 but...do not
+00002d30: 206f 7665 726c 6170 2077 6974 6820 616e   overlap with an
+00002d40: 7920 7265 6769 6f6e 7320 696e 2069 6e62  y regions in inb
+00002d50: 6564 3129 2e0a 0963 6f6d 6d6f 6e20 3a20  ed1)...common : 
+00002d60: 6c69 7374 0a09 0947 656e 6f6d 6963 2072  list...Genomic r
+00002d70: 6567 696f 6e73 206f 7665 726c 6170 7065  egions overlappe
+00002d80: 6420 6265 7477 6565 6e20 696e 6265 6431  d between inbed1
+00002d90: 2061 6e64 2069 6e62 6564 322e 204e 6f74   and inbed2. Not
+00002da0: 652c 2074 6865 0a09 096f 7665 726c 6170  e, the...overlap
+00002db0: 7065 6420 7265 6769 6f6e 7320 7765 7265  ped regions were
+00002dc0: 206d 6572 6765 642e 2046 6f72 2065 7861   merged. For exa
+00002dd0: 6d70 6c65 2c20 2863 6872 3120 3120 3130  mple, (chr1 1 10
+00002de0: 2920 616e 6420 2863 6872 3120 3520 3135  ) and (chr1 5 15
+00002df0: 290a 0909 7769 6c6c 2062 6520 6d65 7267  )...will be merg
+00002e00: 6564 2061 7320 2863 6872 3120 3120 3135  ed as (chr1 1 15
+00002e10: 292e 0a0a 094e 6f74 650a 092d 2d2d 2d0a  )....Note..----.
+00002e20: 094f 7665 726c 6170 7065 6420 7265 6769  .Overlapped regi
+00002e30: 6f6e 7320 2a77 6974 6869 6e2a 2069 6e70  ons *within* inp
+00002e40: 7574 2042 4544 2066 696c 6573 2028 6f72  ut BED files (or
+00002e50: 206c 6973 7473 2920 6172 6520 6d65 7267   lists) are merg
+00002e60: 6564 2062 6566 6f72 650a 0963 6f6d 7061  ed before..compa
+00002e70: 7269 736f 6e2e 0a0a 09fa 1d52 6561 6420  rison......Read 
+00002e80: 616e 6420 756e 696f 6e20 4245 4420 6669  and union BED fi
+00002e90: 6c65 3a20 2225 7322 fa1c 556e 696f 6e65  le: "%s"..Unione
+00002ea0: 6420 7265 6769 6f6e 7320 6f66 2022 2573  d regions of "%s
+00002eb0: 2220 3a20 2564 7a1d 4d65 7267 6520 4245  " : %dz.Merge BE
+00002ec0: 4420 6669 6c65 7320 2225 7322 2061 6e64  D files "%s" and
+00002ed0: 2022 2573 227a 2555 6e69 6f6e 6564 2072   "%s"z%Unioned r
+00002ee0: 6567 696f 6e73 206f 6620 7477 6f20 4245  egions of two BE
+00002ef0: 4420 6669 6c65 7320 3a20 2564 fa2e 4275  D files : %d..Bu
+00002f00: 696c 6420 696e 7465 7276 616c 2074 7265  ild interval tre
+00002f10: 6520 666f 7220 756e 696f 6e65 6420 4245  e for unioned BE
+00002f20: 4420 6669 6c65 3a20 2225 7322 7a24 4669  D file: "%s"z$Fi
+00002f30: 6e64 2063 6f6d 6d6f 6e20 616e 6420 7370  nd common and sp
+00002f40: 6563 6966 6963 2072 6567 696f 6e73 202e  ecific regions .
+00002f50: 2e2e 7201 0000 007a 1722 2573 2220 756e  ..r....z."%s" un
+00002f60: 6971 7565 2072 6567 696f 6e73 3a20 2564  ique regions: %d
+00002f70: 7a1f 436f 6d6d 6f6e 2028 6f76 6572 6c61  z.Common (overla
+00002f80: 7070 6564 2920 7265 6769 6f6e 733a 2025  pped) regions: %
+00002f90: 6429 0972 1100 0000 da04 696e 666f 7221  d).r......infor!
+00002fa0: 0000 0072 0e00 0000 7207 0000 00da 0c61  ...r....r......a
+00002fb0: 6464 5f69 6e74 6572 7661 6c72 0600 0000  dd_intervalr....
+00002fc0: da04 6669 6e64 7218 0000 0029 1372 2400  ..findr....).r$.
+00002fd0: 0000 7225 0000 00da 0a62 6564 315f 756e  ..r%.....bed1_un
+00002fe0: 696f 6eda 0a62 6564 325f 756e 696f 6e5a  ion..bed2_unionZ
+00002ff0: 0b62 6564 3132 5f75 6e69 6f6e da05 6d61  .bed12_union..ma
+00003000: 7073 31da 0569 6368 7231 da07 6973 7461  ps1..ichr1..ista
+00003010: 7274 31da 0569 656e 6431 da05 6d61 7073  rt1..iend1..maps
+00003020: 32da 0569 6368 7232 da07 6973 7461 7274  2..ichr2..istart
+00003030: 32da 0569 656e 6432 5a09 6265 6431 5f75  2..iend2Z.bed1_u
+00003040: 6e69 715a 0962 6564 325f 756e 6971 da06  niqZ.bed2_uniq..
+00003050: 636f 6d6d 6f6e 721b 0000 0072 1e00 0000  commonr....r....
+00003060: 721d 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00003070: 2000 0000 da0b 636f 6d70 6172 655f 6265   .....compare_be
+00003080: 64d3 0100 0073 5600 0000 0022 0e01 0802  d....sV...."....
+00003090: 1602 0e01 0802 1602 1201 0c01 1203 0e01  ................
+000030a0: 0401 0e01 0801 0a01 1602 0e01 0401 0e01  ................
+000030b0: 0a01 0a01 1602 0a01 0401 0401 0401 0e01  ................
+000030c0: 1402 1a02 1a01 1203 1204 1a01 1203 0601  ................
+000030d0: 0a01 1201 0a01 1202 0801 1601 1601 1201  ................
+000030e0: 725e 0000 00da 024e 4163 0500 0000 0000  r^.....NAc......
+000030f0: 0000 0000 0000 2000 0000 1100 0000 4300  ...... .......C.
+00003100: 0000 73b4 0400 0074 00a0 0164 017c 0016  ..s....t...d.|..
+00003110: 00a1 0101 0074 027c 0083 017d 0574 00a0  .....t.|...}.t..
+00003120: 0164 027c 0074 037c 0583 0166 0216 00a1  .d.|.t.|...f....
+00003130: 0101 0074 00a0 0164 017c 0116 00a1 0101  ...t...d.|......
+00003140: 0074 027c 0183 017d 0674 00a0 0164 027c  .t.|...}.t...d.|
+00003150: 0174 037c 0683 0166 0216 00a1 0101 0074  .t.|...f.......t
+00003160: 00a0 0164 037c 0016 00a1 0101 0069 007d  ...d.|.......i.}
+00003170: 077c 0544 005d 305c 037d 087d 097d 0a7c  .|.D.]0\.}.}.}.|
+00003180: 087c 076b 0772 8a74 0483 007c 077c 083c  .|.k.r.t...|.|.<
+00003190: 007c 077c 0819 00a0 0574 067c 097c 0a83  .|.|.....t.|.|..
+000031a0: 02a1 0101 0071 6e74 00a0 0164 037c 0116  .....qnt...d.|..
+000031b0: 00a1 0101 0069 007d 0b7c 0644 005d 305c  .....i.}.|.D.]0\
+000031c0: 037d 0c7d 0d7d 0e7c 0c7c 0b6b 0772 d274  .}.}.}.|.|.k.r.t
+000031d0: 0483 007c 0b7c 0c3c 007c 0b7c 0c19 00a0  ...|.|.<.|.|....
+000031e0: 0574 067c 0d7c 0e83 02a1 0101 0071 b674  .t.|.|.......q.t
+000031f0: 00a0 0164 047c 0016 00a1 0101 0074 076a  ...d.|.......t.j
+00003200: 08a0 097c 00a1 0164 0517 007d 0f74 0a7c  ...|...d...}.t.|
+00003210: 0f64 0683 027d 1074 0b64 07a0 0c64 0864  .d...}.t.d...d.d
+00003220: 0964 0a64 0b64 0c64 0d64 0e64 0f64 1067  .d.d.d.d.d.d.d.g
+00003230: 09a1 017c 1064 118d 0201 007c 0544 0090  ...|.d.....|.D..
+00003240: 015d 825c 037d 117d 127d 1390 017a 387c  .].\.}.}.}...z8|
+00003250: 137c 1218 007d 147c 1464 126b 0190 0172  .|...}.|.d.k...r
+00003260: 8074 00a0 0d64 137c 1164 1417 0074 0e7c  .t...d.|.d...t.|
+00003270: 1283 0117 0064 1517 0074 0e7c 1383 0117  .....d...t.|....
+00003280: 0016 00a1 0101 007c 117c 127c 1366 0367  .......|.|.|.f.g
+00003290: 017d 1564 127d 1667 007d 177c 0b7c 1119  .}.d.}.g.}.|.|..
+000032a0: 00a0 0f7c 127c 13a1 027d 1874 037c 1883  ...|.|...}.t.|..
+000032b0: 0164 126b 0290 0172 e274 0b64 07a0 0c64  .d.k...r.t.d...d
+000032c0: 1664 1784 007c 117c 127c 137c 147c 047c  .d...|.|.|.|.|.|
+000032d0: 047c 047c 047c 0466 0944 0083 01a1 017c  .|.|.|.f.D.....|
+000032e0: 1064 118d 0201 006e 9a7c 1844 005d 2a7d  .d.....n.|.D.]*}
+000032f0: 197c 167c 196a 107c 196a 1118 0037 007d  .|.|.j.|.j...7.}
+00003300: 167c 17a0 127c 117c 196a 117c 196a 1066  .|...|.|.j.|.j.f
+00003310: 03a1 0101 0090 0171 e674 137c 157c 1783  .......q.t.|.|..
+00003320: 027d 1a74 147c 157c 1717 0083 0164 1219  .}.t.|.|.....d..
+00003330: 007d 1b7c 027c 147c 167c 1a7c 0383 047d  .}.|.|.|.|.|...}
+00003340: 1c64 18a0 0c64 1964 1784 007c 1744 0083  .d...d.d...|.D..
+00003350: 01a1 017d 1d74 0b64 07a0 0c64 1a64 1784  ...}.t.d...d.d..
+00003360: 007c 117c 127c 137c 147c 167c 1a7c 1b7c  .|.|.|.|.|.|.|.|
+00003370: 1d7c 1c66 0944 0083 01a1 017c 1064 118d  .|.f.D.....|.d..
+00003380: 0201 0057 006e 3a01 0001 0001 0074 0b64  ...W.n:......t.d
+00003390: 07a0 0c64 1b64 1784 007c 117c 127c 137c  ...d.d...|.|.|.|
+000033a0: 147c 047c 047c 047c 047c 0466 0944 0083  .|.|.|.|.|.f.D..
+000033b0: 01a1 017c 1064 118d 0201 0059 006e 0258  ...|.d.....Y.n.X
+000033c0: 0090 0171 387c 10a0 15a1 0001 0074 00a0  ...q8|.......t..
+000033d0: 0164 1c7c 0f16 00a1 0101 0074 00a0 0164  .d.|.......t...d
+000033e0: 047c 0116 00a1 0101 0074 076a 08a0 097c  .|.......t.j...|
+000033f0: 01a1 0164 0517 007d 1e74 0a7c 1e64 0683  ...d...}.t.|.d..
+00003400: 027d 1f74 0b64 07a0 0c64 0864 0964 0a64  .}.t.d...d.d.d.d
+00003410: 0b64 0c64 0d64 0e64 0f64 1067 09a1 017c  .d.d.d.d.d.g...|
+00003420: 1f64 118d 0201 007c 0644 0090 015d 725c  .d.....|.D...]r\
+00003430: 037d 117d 127d 1390 017a 287c 137c 1218  .}.}.}...z(|.|..
+00003440: 007d 167c 1664 126b 0190 0372 6c74 00a0  .}.|.d.k...rlt..
+00003450: 0d64 137c 1164 1417 0074 0e7c 1283 0117  .d.|.d...t.|....
+00003460: 0064 1517 0074 0e7c 1383 0117 0016 00a1  .d...t.|........
+00003470: 0101 007c 117c 127c 1366 0367 017d 1764  ...|.|.|.f.g.}.d
+00003480: 127d 1467 007d 157c 077c 1119 00a0 0f7c  .}.g.}.|.|.....|
+00003490: 127c 13a1 027d 1874 037c 1883 0164 126b  .|...}.t.|...d.k
+000034a0: 0290 0372 ce74 0b64 07a0 0c64 1d64 1784  ...r.t.d...d.d..
+000034b0: 007c 117c 127c 137c 147c 047c 047c 047c  .|.|.|.|.|.|.|.|
+000034c0: 047c 0466 0944 0083 01a1 017c 1f64 118d  .|.f.D.....|.d..
+000034d0: 0201 006e 8a7c 1844 005d 2a7d 197c 147c  ...n.|.D.]*}.|.|
+000034e0: 196a 107c 196a 1118 0037 007d 147c 15a0  .j.|.j...7.}.|..
+000034f0: 127c 117c 196a 117c 196a 1066 03a1 0101  .|.|.j.|.j.f....
+00003500: 0090 0371 d274 137c 177c 1583 027d 1a7c  ...q.t.|.|...}.|
+00003510: 027c 147c 167c 1a7c 0383 047d 1c64 18a0  .|.|.|.|...}.d..
+00003520: 0c64 1e64 1784 007c 1544 0083 01a1 017d  .d.d...|.D.....}
+00003530: 1d74 0b64 07a0 0c64 1f64 1784 007c 117c  .t.d...d.d...|.|
+00003540: 127c 137c 147c 167c 1a7c 1b7c 1d7c 1c66  .|.|.|.|.|.|.|.f
+00003550: 0944 0083 01a1 017c 1f64 118d 0201 0057  .D.....|.d.....W
+00003560: 006e 3a01 0001 0001 0074 0b64 07a0 0c64  .n:......t.d...d
+00003570: 2064 1784 007c 117c 127c 137c 147c 047c   d...|.|.|.|.|.|
+00003580: 047c 047c 047c 0466 0944 0083 01a1 017c  .|.|.|.f.D.....|
+00003590: 1f64 118d 0201 0059 006e 0258 0090 0371  .d.....Y.n.X...q
+000035a0: 247c 1fa0 15a1 0001 0074 00a0 0164 1c7c  $|.......t...d.|
+000035b0: 1e16 00a1 0101 0064 2153 0029 2261 7601  .......d!S.)"av.
+000035c0: 0000 0a09 4361 6c63 756c 6174 6573 2070  ....Calculates p
+000035d0: 6561 6b2d 7769 7365 206f 7665 726c 6170  eak-wise overlap
+000035e0: 202e 0a0a 0950 6172 616d 6574 6572 730a   ....Parameters.
+000035f0: 092d 2d2d 2d2d 2d2d 2d2d 2d0a 0969 6e62  .----------..inb
+00003600: 6564 3120 3a20 7374 720a 0909 4e61 6d65  ed1 : str...Name
+00003610: 206f 6620 6120 4245 4420 6669 6c65 2e0a   of a BED file..
+00003620: 0969 6e62 6564 3220 3a20 7374 720a 0909  .inbed2 : str...
+00003630: 4e61 6d65 206f 6620 616e 6f74 6865 7220  Name of another 
+00003640: 4245 4420 6669 6c65 2e0a 0973 636f 7265  BED file...score
+00003650: 5f66 756e 6320 3a20 6675 6e63 7469 6f6e  _func : function
+00003660: 0a09 0946 756e 6374 696f 6e20 746f 2063  ...Function to c
+00003670: 616c 6375 6c61 7465 206f 7665 726c 6170  alculate overlap
+00003680: 2069 6e64 6578 2e20 496e 636c 7564 6520   index. Include 
+00003690: 6f76 5f63 6f65 662c 206f 765f 6a61 6363  ov_coef, ov_jacc
+000036a0: 6172 642c 206f 765f 7373 2c20 6f76 5f73  ard, ov_ss, ov_s
+000036b0: 642e 0a09 6720 3a20 696e 740a 0909 5369  d...g : int...Si
+000036c0: 7a65 206f 6620 7468 6520 6765 6e6f 6d69  ze of the genomi
+000036d0: 6320 6261 636b 6772 6f75 6e64 2e0a 096e  c background...n
+000036e0: 615f 6c61 6265 6c20 3a20 7374 720a 0909  a_label : str...
+000036f0: 5374 7269 6e67 206c 6162 656c 2075 7365  String label use
+00003700: 6420 746f 2072 6570 7265 7365 6e74 206d  d to represent m
+00003710: 6973 7369 6e67 2076 616c 7565 2e0a 0a09  issing value....
+00003720: 5265 7475 726e 730a 092d 2d2d 2d2d 2d2d  Returns..-------
+00003730: 0a09 4e6f 6e65 0a09 724d 0000 0072 4e00  ..None..rM...rN.
+00003740: 0000 724f 0000 007a 4243 616c 6375 6c61  ..rO...zBCalcula
+00003750: 7465 2074 6865 206f 7665 726c 6170 2063  te the overlap c
+00003760: 6f65 6666 6963 6965 6e74 206f 6620 6561  oefficient of ea
+00003770: 6368 2067 656e 6f6d 6963 2072 6567 696f  ch genomic regio
+00003780: 6e20 696e 2025 7320 2e2e 2e7a 145f 7065  n in %s ...z._pe
+00003790: 616b 7769 7365 5f73 636f 7265 732e 7473  akwise_scores.ts
+000037a0: 76da 0177 fa01 0972 1b00 0000 721e 0000  v..w...r....r...
+000037b0: 0072 1d00 0000 7a06 412e 7369 7a65 7a06  .r....z.A.sizez.
+000037c0: 422e 7369 7a65 7505 0000 0041 e288 a942  B.sizeu....A...B
+000037d0: 7505 0000 0041 e288 aa42 7a06 422e 6c69  u....A...Bz.B.li
+000037e0: 7374 5a05 5363 6f72 65a9 01da 0466 696c  stZ.Score....fil
+000037f0: 6572 0100 0000 7a07 536b 6970 2025 73fa  er....z.Skip %s.
+00003800: 013a fa01 2d63 0100 0000 0000 0000 0000  .:..-c..........
+00003810: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
+00003820: 0000 0067 007c 005d 0c7d 0174 007c 0183  ...g.|.].}.t.|..
+00003830: 0191 0271 0453 0072 1f00 0000 a901 720f  ...q.S.r......r.
+00003840: 0000 00a9 02da 022e 30da 0169 721f 0000  ........0..ir...
+00003850: 0072 1f00 0000 7220 0000 00da 0a3c 6c69  .r....r .....<li
+00003860: 7374 636f 6d70 3e76 0200 0073 0400 0000  stcomp>v...s....
+00003870: 0600 0200 7a23 7065 616b 7769 7365 5f6f  ....z#peakwise_o
+00003880: 7663 6f65 662e 3c6c 6f63 616c 733e 2e3c  vcoef.<locals>.<
+00003890: 6c69 7374 636f 6d70 3efa 012c 6301 0000  listcomp>..,c...
+000038a0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
+000038b0: 0053 0000 0073 3400 0000 6700 7c00 5d2c  .S...s4...g.|.],
+000038c0: 7d01 7c01 6400 1900 6401 1700 7400 7c01  }.|.d...d...t.|.
+000038d0: 6402 1900 8301 1700 6403 1700 7400 7c01  d.......d...t.|.
+000038e0: 6404 1900 8301 1700 9102 7104 5300 a905  d.........q.S...
+000038f0: 7201 0000 0072 6400 0000 720b 0000 0072  r....rd...r....r
+00003900: 6500 0000 7233 0000 0072 6600 0000 7267  e...r3...rf...rg
+00003910: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00003920: 0000 726a 0000 007e 0200 0073 0400 0000  ..rj...~...s....
+00003930: 0600 0200 6301 0000 0000 0000 0000 0000  ....c...........
+00003940: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+00003950: 0000 6700 7c00 5d0c 7d01 7400 7c01 8301  ..g.|.].}.t.|...
+00003960: 9102 7104 5300 721f 0000 0072 6600 0000  ..q.S.r....rf...
+00003970: 7267 0000 0072 1f00 0000 721f 0000 0072  rg...r....r....r
+00003980: 2000 0000 726a 0000 007f 0200 0073 0400   ...rj.......s..
+00003990: 0000 0600 0200 6301 0000 0000 0000 0000  ......c.........
+000039a0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+000039b0: 1400 0000 6700 7c00 5d0c 7d01 7400 7c01  ....g.|.].}.t.|.
+000039c0: 8301 9102 7104 5300 721f 0000 0072 6600  ....q.S.r....rf.
+000039d0: 0000 7267 0000 0072 1f00 0000 721f 0000  ..rg...r....r...
+000039e0: 0072 2000 0000 726a 0000 0081 0200 0073  .r ...rj.......s
+000039f0: 0400 0000 0600 0200 7a1e 5361 7665 2070  ........z.Save p
+00003a00: 6561 6b77 6973 6520 7363 6f72 6573 2074  eakwise scores t
+00003a10: 6f20 2573 202e 2e2e 6301 0000 0000 0000  o %s ...c.......
+00003a20: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00003a30: 0073 1400 0000 6700 7c00 5d0c 7d01 7400  .s....g.|.].}.t.
+00003a40: 7c01 8301 9102 7104 5300 721f 0000 0072  |.....q.S.r....r
+00003a50: 6600 0000 7267 0000 0072 1f00 0000 721f  f...rg...r....r.
+00003a60: 0000 0072 2000 0000 726a 0000 0095 0200  ...r ...rj......
+00003a70: 0073 0400 0000 0600 0200 6301 0000 0000  .s........c.....
+00003a80: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00003a90: 0000 0073 3400 0000 6700 7c00 5d2c 7d01  ...s4...g.|.],}.
+00003aa0: 7c01 6400 1900 6401 1700 7400 7c01 6402  |.d...d...t.|.d.
+00003ab0: 1900 8301 1700 6403 1700 7400 7c01 6404  ......d...t.|.d.
+00003ac0: 1900 8301 1700 9102 7104 5300 726c 0000  ........q.S.rl..
+00003ad0: 0072 6600 0000 7267 0000 0072 1f00 0000  .rf...rg...r....
+00003ae0: 721f 0000 0072 2000 0000 726a 0000 009c  r....r ...rj....
+00003af0: 0200 0073 0400 0000 0600 0200 6301 0000  ...s........c...
+00003b00: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00003b10: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+00003b20: 7d01 7400 7c01 8301 9102 7104 5300 721f  }.t.|.....q.S.r.
+00003b30: 0000 0072 6600 0000 7267 0000 0072 1f00  ...rf...rg...r..
+00003b40: 0000 721f 0000 0072 2000 0000 726a 0000  ..r....r ...rj..
+00003b50: 009d 0200 0073 0400 0000 0600 0200 6301  .....s........c.
+00003b60: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00003b70: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
+00003b80: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
+00003b90: 721f 0000 0072 6600 0000 7267 0000 0072  r....rf...rg...r
+00003ba0: 1f00 0000 721f 0000 0072 2000 0000 726a  ....r....r ...rj
+00003bb0: 0000 009f 0200 0073 0400 0000 0600 0200  .......s........
+00003bc0: 4e29 1672 1100 0000 7250 0000 0072 2100  N).r....rP...r!.
+00003bd0: 0000 720e 0000 0072 0700 0000 7251 0000  ..r....r....rQ..
+00003be0: 0072 0600 0000 da02 6f73 da04 7061 7468  .r......os..path
+00003bf0: 7202 0000 00da 046f 7065 6eda 0570 7269  r......open..pri
+00003c00: 6e74 da04 6a6f 696e 7246 0000 0072 0f00  nt..joinrF...r..
+00003c10: 0000 7252 0000 0072 1d00 0000 721e 0000  ..rR...r....r...
+00003c20: 0072 1800 0000 7244 0000 0072 4200 0000  .r....rD...rB...
+00003c30: da05 636c 6f73 6529 2072 2400 0000 7225  ..close) r$...r%
+00003c40: 0000 005a 0a73 636f 7265 5f66 756e 63da  ...Z.score_func.
+00003c50: 0167 5a08 6e61 5f6c 6162 656c 7253 0000  .gZ.na_labelrS..
+00003c60: 0072 5400 0000 7255 0000 0072 5600 0000  .rT...rU...rV...
+00003c70: 7257 0000 0072 5800 0000 7259 0000 0072  rW...rX...rY...r
+00003c80: 5a00 0000 725b 0000 0072 5c00 0000 5a0d  Z...r[...r\...Z.
+00003c90: 6f75 7466 696c 655f 6e61 6d65 315a 0742  outfile_name1Z.B
+00003ca0: 4544 314f 5554 721b 0000 0072 1e00 0000  ED1OUTr....r....
+00003cb0: 721d 0000 005a 0a62 6564 5f31 5f73 697a  r....Z.bed_1_siz
+00003cc0: 655a 0962 6564 5f31 5f6c 7374 5a0a 6265  eZ.bed_1_lstZ.be
+00003cd0: 645f 325f 7369 7a65 5a09 6265 645f 325f  d_2_sizeZ.bed_2_
+00003ce0: 6c73 74da 086f 7665 726c 6170 73da 016f  lst..overlaps..o
+00003cf0: 7243 0000 0072 4100 0000 5a0c 7065 616b  rC...rA...Z.peak
+00003d00: 5f6f 765f 636f 6566 5a0b 7461 7267 6574  _ov_coefZ.target
+00003d10: 5f6c 6973 745a 0d6f 7574 6669 6c65 5f6e  _listZ.outfile_n
+00003d20: 616d 6532 5a07 4245 4432 4f55 5472 1f00  ame2Z.BED2OUTr..
+00003d30: 0000 721f 0000 0072 2000 0000 da0f 7065  ..r....r .....pe
+00003d40: 616b 7769 7365 5f6f 7663 6f65 6634 0200  akwise_ovcoef4..
+00003d50: 0073 8e00 0000 0017 0e01 0801 1602 0e01  .s..............
+00003d60: 0801 1606 0e01 0401 0e01 0801 0a01 1602  ................
+00003d70: 0e01 0401 0e01 0801 0a01 1603 0e01 1001  ................
+00003d80: 0a01 2401 1001 0401 0801 0a01 2601 0c01  ..$.........&...
+00003d90: 0401 0402 1002 0e01 3002 0801 1001 1801  ........0.......
+00003da0: 0a01 1001 0e01 1401 3201 0601 3801 0801  ........2...8...
+00003db0: 0e03 0e01 1001 0a01 2401 1001 0401 0801  ........$.......
+00003dc0: 0a01 2601 0c01 0401 0402 1001 0e01 3002  ..&...........0.
+00003dd0: 0801 1001 1801 0a01 0e01 1401 3201 0601  ............2...
+00003de0: 3801 0801 7276 0000 0072 0b00 0000 e700  8...rv...r......
+00003df0: 0000 0000 0000 0063 0600 0000 0000 0000  .......c........
+00003e00: 0000 0000 2d00 0000 0700 0000 4300 0000  ....-.......C...
+00003e10: 73c4 0500 0069 007d 0674 006a 01a0 027c  s....i.}.t.j...|
+00003e20: 00a1 017d 0774 006a 01a0 027c 01a1 017d  ...}.t.j...|...}
+00003e30: 087c 077c 0664 013c 007c 087c 0664 023c  .|.|.d.<.|.|.d.<
+00003e40: 0074 03a0 0464 037c 0016 00a1 0101 0074  .t...d.|.......t
+00003e50: 057c 0083 017d 0974 067c 0983 017c 0664  .|...}.t.|...|.d
+00003e60: 043c 0074 03a0 0464 037c 0116 00a1 0101  .<.t...d.|......
+00003e70: 0074 057c 0183 017d 0a74 067c 0a83 017c  .t.|...}.t.|...|
+00003e80: 0664 053c 0074 03a0 0464 067c 0216 00a1  .d.<.t...d.|....
+00003e90: 0101 0074 057c 0283 017d 0b74 067c 0b83  ...t.|...}.t.|..
+00003ea0: 017c 0664 073c 0074 03a0 0464 087c 0016  .|.d.<.t...d.|..
+00003eb0: 00a1 0101 0069 007d 0c7c 0944 005d 305c  .....i.}.|.D.]0\
+00003ec0: 037d 0d7d 0e7d 0f7c 0d7c 0c6b 0772 c474  .}.}.}.|.|.k.r.t
+00003ed0: 0783 007c 0c7c 0d3c 007c 0c7c 0d19 00a0  ...|.|.<.|.|....
+00003ee0: 0874 097c 0e7c 0f83 02a1 0101 0071 a874  .t.|.|.......q.t
+00003ef0: 03a0 0464 097c 0116 00a1 0101 0069 007d  ...d.|.......i.}
+00003f00: 107c 0a44 005d 325c 037d 117d 127d 137c  .|.D.]2\.}.}.}.|
+00003f10: 117c 106b 0790 0172 0e74 0783 007c 107c  .|.k...r.t...|.|
+00003f20: 113c 007c 107c 1119 00a0 0874 097c 127c  .<.|.|.....t.|.|
+00003f30: 1383 02a1 0101 0071 f064 0a7d 1464 0a7d  .......q.d.}.d.}
+00003f40: 1564 0a7d 1664 0a7d 1774 0a7c 0364 0b83  .d.}.d.}.t.|.d..
+00003f50: 027d 187c 0b44 0090 035d f85c 037d 197d  .}.|.D...].\.}.}
+00003f60: 1a7d 1b7c 1964 0c17 0074 0b7c 1a83 0117  .}.|.d...t.|....
+00003f70: 0064 0c17 0074 0b7c 1b83 0117 007d 1c64  .d...t.|.....}.d
+00003f80: 0d7d 1d64 0d7d 1e7c 197c 0c6b 0790 0172  .}.d.}.|.|.k...r
+00003f90: 8a7c 197c 106b 0790 0172 8a90 036e 307c  .|.|.k...r...n0|
+00003fa0: 197c 0c6b 0790 0272 367c 197c 106b 0690  .|.k...r6|.|.k..
+00003fb0: 0272 367c 107c 1919 00a0 0c7c 1a7c 1ba1  .r6|.|.....|.|..
+00003fc0: 027d 1f74 067c 1f83 0164 0a6b 0290 0172  .}.t.|...d.k...r
+00003fd0: be6e 7467 007d 207c 1f44 005d 1a7d 217c  .ntg.} |.D.].}!|
+00003fe0: 20a0 0d7c 197c 216a 0e7c 216a 0f66 03a1   ..|.|!j.|!j.f..
+00003ff0: 0101 0090 0171 c674 107c 197c 1a7c 1b66  .....q.t.|.|.|.f
+00004000: 0367 017c 2083 027d 2274 117c 2083 017d  .g.| ..}"t.| ..}
+00004010: 237a 0c7c 227c 231b 007d 2457 006e 1001  #z.|"|#..}$W.n..
+00004020: 0001 0001 0064 0a7d 2459 006e 0258 007c  .....d.}$Y.n.X.|
+00004030: 227c 046b 0590 0472 ba7c 247c 056b 0590  "|.k...r.|$|.k..
+00004040: 0472 ba64 0e7d 1e90 026e 847c 197c 0c6b  .r.d.}...n.|.|.k
+00004050: 0690 0272 e27c 197c 106b 0790 0272 e27c  ...r.|.|.k...r.|
+00004060: 0c7c 1919 00a0 0c7c 1a7c 1ba1 027d 2574  .|.....|.|...}%t
+00004070: 067c 1f83 0164 0a6b 0290 0272 6a6e 7467  .|...d.k...rjntg
+00004080: 007d 267c 2544 005d 1a7d 217c 26a0 0d7c  .}&|%D.].}!|&..|
+00004090: 197c 216a 0e7c 216a 0f66 03a1 0101 0090  .|!j.|!j.f......
+000040a0: 0271 7274 107c 197c 1a7c 1b66 0367 017c  .qrt.|.|.|.f.g.|
+000040b0: 2683 027d 2774 117c 2683 017d 287a 0c7c  &..}'t.|&..}(z.|
+000040c0: 277c 281b 007d 2957 006e 1001 0001 0001  '|(..})W.n......
+000040d0: 0064 0a7d 2959 006e 0258 007c 277c 046b  .d.})Y.n.X.|'|.k
+000040e0: 0590 0472 ba7c 297c 056b 0590 0472 ba64  ...r.|)|.k...r.d
+000040f0: 0e7d 1d90 016e d87c 0c7c 1919 00a0 0c7c  .}...n.|.|.....|
+00004100: 1a7c 1ba1 027d 257c 107c 1919 00a0 0c7c  .|...}%|.|.....|
+00004110: 1a7c 1ba1 027d 1f74 067c 2583 0164 0a6b  .|...}.t.|%..d.k
+00004120: 0290 0372 a674 067c 1f83 0164 0a6b 0290  ...r.t.|...d.k..
+00004130: 0372 206e 8274 067c 1f83 0164 0a6b 0490  .r n.t.|...d.k..
+00004140: 0472 ba67 007d 207c 1f44 005d 1a7d 217c  .r.g.} |.D.].}!|
+00004150: 20a0 0d7c 197c 216a 0e7c 216a 0f66 03a1   ..|.|!j.|!j.f..
+00004160: 0101 0090 0371 3674 107c 197c 1a7c 1b66  .....q6t.|.|.|.f
+00004170: 0367 017c 2083 027d 2274 117c 2083 017d  .g.| ..}"t.| ..}
+00004180: 237a 0c7c 227c 231b 007d 2457 006e 1001  #z.|"|#..}$W.n..
+00004190: 0001 0001 0064 0a7d 2459 006e 0258 007c  .....d.}$Y.n.X.|
+000041a0: 227c 046b 0590 0472 ba7c 247c 056b 0590  "|.k...r.|$|.k..
+000041b0: 0472 ba64 0e7d 1e90 016e 1474 067c 2583  .r.d.}...n.t.|%.
+000041c0: 0164 0a6b 0490 0472 ba67 007d 267c 2544  .d.k...r.g.}&|%D
+000041d0: 005d 1a7d 217c 26a0 0d7c 197c 216a 0e7c  .].}!|&..|.|!j.|
+000041e0: 216a 0f66 03a1 0101 0090 0371 bc74 107c  !j.f.......q.t.|
+000041f0: 197c 1a7c 1b66 0367 017c 2683 027d 2774  .|.|.f.g.|&..}'t
+00004200: 117c 2683 017d 287a 0c7c 277c 281b 007d  .|&..}(z.|'|(..}
+00004210: 2957 006e 1001 0001 0001 0064 0a7d 2959  )W.n.......d.})Y
+00004220: 006e 0258 007c 277c 046b 0590 0472 287c  .n.X.|'|.k...r(|
+00004230: 297c 056b 0590 0472 2864 0e7d 1d74 067c  )|.k...r(d.}.t.|
+00004240: 1f83 0164 0a6b 0290 0472 386e 8274 067c  ...d.k...r8n.t.|
+00004250: 1f83 0164 0a6b 0490 0472 ba67 007d 207c  ...d.k...r.g.} |
+00004260: 1f44 005d 1a7d 217c 20a0 0d7c 197c 216a  .D.].}!| ..|.|!j
+00004270: 0e7c 216a 0f66 03a1 0101 0090 0471 4e74  .|!j.f.......qNt
+00004280: 107c 197c 1a7c 1b66 0367 017c 2083 027d  .|.|.|.f.g.| ..}
+00004290: 2274 117c 2083 017d 237a 0c7c 227c 231b  "t.| ..}#z.|"|#.
+000042a0: 007d 2457 006e 1001 0001 0001 0064 0a7d  .}$W.n.......d.}
+000042b0: 2459 006e 0258 007c 227c 046b 0590 0472  $Y.n.X.|"|.k...r
+000042c0: ba7c 247c 056b 0590 0472 ba64 0e7d 1e7c  .|$|.k...r.d.}.|
+000042d0: 1d90 0472 fe7c 1e90 0472 e07c 1664 0f37  ...r.|...r.|.d.7
+000042e0: 007d 1674 127c 1c64 1017 007c 1864 118d  .}.t.|.d...|.d..
+000042f0: 0201 006e 1c7c 1464 0f37 007d 1474 127c  ...n.|.d.7.}.t.|
+00004300: 1c64 127c 0716 0017 007c 1864 118d 0201  .d.|.....|.d....
+00004310: 006e 3c7c 1e90 0572 227c 1564 0f37 007d  .n<|...r"|.d.7.}
+00004320: 1574 127c 1c64 127c 0816 0017 007c 1864  .t.|.d.|.....|.d
+00004330: 118d 0201 006e 187c 1764 0f37 007d 1774  .....n.|.d.7.}.t
+00004340: 127c 1c64 1317 007c 1864 118d 0201 0090  .|.d...|.d......
+00004350: 0171 427c 147c 0664 143c 007c 157c 0664  .qB|.|.d.<.|.|.d
+00004360: 153c 007c 167c 0664 163c 007c 177c 0664  .<.|.|.d.<.|.|.d
+00004370: 173c 007c 147c 156b 0490 0572 8074 13a0  .<.|.|.k...r.t..
+00004380: 147c 177c 1467 027c 157c 1667 0267 02a1  .|.|.g.|.|.g.g..
+00004390: 017d 2a6e 1674 13a0 147c 177c 1567 027c  .}*n.t...|.|.g.|
+000043a0: 147c 1667 0267 02a1 017d 2a74 157c 2a64  .|.g.g...}*t.|*d
+000043b0: 1864 198d 025c 027d 2b7d 2c7c 2b7c 0664  .d...\.}+},|+|.d
+000043c0: 1a3c 007c 2c7c 0664 1b3c 0074 166a 177c  .<.|,|.d.<.t.j.|
+000043d0: 0664 1c64 1d8d 0253 0029 1e61 b602 0000  .d.d...S.).a....
+000043e0: 0a09 4576 616c 7561 7465 2069 6620 7477  ..Evaluate if tw
+000043f0: 6f20 7065 616b 2073 6574 7320 6172 6520  o peak sets are 
+00004400: 7369 676e 6966 6963 616e 746c 7920 6f63  significantly oc
+00004410: 2d6f 6363 7572 7265 6420 6f72 206d 7574  -occurred or mut
+00004420: 7561 6c6c 7920 6578 636c 7573 6976 652e  ually exclusive.
+00004430: 0a09 5573 696e 6720 4669 7368 6572 2773  ..Using Fisher's
+00004440: 2065 7861 6374 2074 6573 742e 0a0a 0950   exact test....P
+00004450: 6172 616d 6574 6572 730a 092d 2d2d 2d2d  arameters..-----
+00004460: 2d2d 2d2d 2d0a 0969 6e62 6564 3120 3a20  -----..inbed1 : 
+00004470: 7374 720a 0909 4e61 6d65 206f 6620 6120  str...Name of a 
+00004480: 4245 4420 6669 6c65 2e0a 0969 6e62 6564  BED file...inbed
+00004490: 3220 3a20 7374 720a 0909 4e61 6d65 206f  2 : str...Name o
+000044a0: 6620 616e 6f74 6865 7220 4245 4420 6669  f another BED fi
+000044b0: 6c65 2e0a 0969 6e62 6564 5f62 6720 3a20  le...inbed_bg : 
+000044c0: 7374 720a 0909 4e61 6d65 206f 6620 7468  str...Name of th
+000044d0: 6520 6261 636b 6772 6f75 6e64 2042 4544  e background BED
+000044e0: 2066 696c 6520 2865 2e67 2e2c 2061 6c6c   file (e.g., all
+000044f0: 2070 726f 6d6f 7465 7273 2c20 616c 6c20   promoters, all 
+00004500: 656e 6861 6e63 6572 7329 2e0a 096f 7574  enhancers)...out
+00004510: 6669 6c65 203a 2073 7472 0a09 094e 616d  file : str...Nam
+00004520: 6520 6f66 2074 6865 206f 7574 7075 7420  e of the output 
+00004530: 6669 6c65 2e0a 096e 5f63 7574 203a 2069  file...n_cut : i
+00004540: 6e74 2c20 6f70 7469 6f6e 616c 0a09 0954  nt, optional...T
+00004550: 6872 6573 686f 6c64 206f 6620 6f76 6572  hreshold of over
+00004560: 6c61 7020 7369 7a65 2e20 466f 7220 6578  lap size. For ex
+00004570: 616d 706c 652c 2074 6865 206f 7665 726c  ample, the overl
+00004580: 6170 2073 697a 6520 6973 2032 3020 666f  ap size is 20 fo
+00004590: 7220 7468 6573 6520 7477 6f0a 0909 7265  r these two...re
+000045a0: 6769 6f6e 7320 2827 6368 7231 272c 2030  gions ('chr1', 0
+000045b0: 2c20 3130 3029 2061 6e64 2028 2763 6872  , 100) and ('chr
+000045c0: 3127 2c20 3830 2c20 3235 3029 2e0a 0909  1', 80, 250)....
+000045d0: 6465 6661 756c 7420 3d20 310a 0970 5f70  default = 1..p_p
+000045e0: 7574 203a 2066 6c6f 6174 2c20 6f70 7469  ut : float, opti
+000045f0: 6f6e 616c 0a09 0954 6872 6573 686f 6c64  onal...Threshold
+00004600: 206f 6620 6f76 6572 6c61 7020 7065 7263   of overlap perc
+00004610: 656e 7461 6765 2e20 496e 2074 6865 2065  entage. In the e
+00004620: 7861 6d70 6c65 2061 626f 7665 2c20 7468  xample above, th
+00004630: 6520 6f76 6572 6c61 7020 7065 7263 656e  e overlap percen
+00004640: 7461 6765 0a09 0966 6f72 2028 2763 6872  tage...for ('chr
+00004650: 3127 2c20 302c 2031 3030 2920 6973 2032  1', 0, 100) is 2
+00004660: 302f 3130 3020 3d20 302e 322e 0a09 0964  0/100 = 0.2....d
+00004670: 6566 6175 6c74 203d 2030 2e30 0a09 5265  efault = 0.0..Re
+00004680: 7475 726e 730a 092d 2d2d 2d2d 2d2d 0a09  turns..-------..
+00004690: 4e6f 6e65 0a09 7a06 412e 6e61 6d65 7a06  None..z.A.namez.
+000046a0: 422e 6e61 6d65 724d 0000 007a 0741 2e63  B.namerM...z.A.c
+000046b0: 6f75 6e74 7a07 422e 636f 756e 747a 2852  ountz.B.countz(R
+000046c0: 6561 6420 616e 6420 756e 696f 6e20 6261  ead and union ba
+000046d0: 636b 6772 6f75 6e64 2042 4544 2066 696c  ckground BED fil
+000046e0: 653a 2022 2573 227a 0747 2e63 6f75 6e74  e: "%s"z.G.count
+000046f0: 7a1e 4275 696c 6420 696e 7465 7276 616c  z.Build interval
+00004700: 2074 7265 6520 666f 7220 3a20 2225 7322   tree for : "%s"
+00004710: 7a1d 4275 696c 6420 696e 7465 7276 616c  z.Build interval
+00004720: 2074 7265 6520 666f 723a 2022 2573 2272   tree for: "%s"r
+00004730: 0100 0000 7260 0000 0072 6100 0000 4654  ....r`...ra...FT
+00004740: 720b 0000 007a 0809 436f 6f63 6375 7272  r....z..Cooccurr
+00004750: 6200 0000 7a08 0925 735f 6f6e 6c79 7a08  b...z..%s_onlyz.
+00004760: 094e 6569 7468 6572 7a05 412b 2c42 2d7a  .Neitherz.A+,B-z
+00004770: 0541 2d2c 422b 7a05 412b 2c42 2b7a 0541  .A-,B+z.A+,B+z.A
+00004780: 2d2c 422d 5a07 6772 6561 7465 7229 015a  -,B-Z.greater).Z
+00004790: 0b61 6c74 6572 6e61 7469 7665 7a0a 6f64  .alternativez.od
+000047a0: 6473 2d72 6174 696f 7a07 702d 7661 6c75  ds-ratioz.p-valu
+000047b0: 657a 1a46 6973 6865 7227 7320 6578 6163  ez.Fisher's exac
+000047c0: 7420 7465 7374 2072 6573 756c 7429 02da  t test result)..
+000047d0: 0464 6174 61da 046e 616d 6529 1872 6d00  .data..name).rm.
+000047e0: 0000 726e 0000 0072 0200 0000 7211 0000  ..rn...r....r...
+000047f0: 0072 5000 0000 7221 0000 0072 0e00 0000  .rP...r!...r....
+00004800: 7207 0000 0072 5100 0000 7206 0000 0072  r....rQ...r....r
+00004810: 6f00 0000 720f 0000 0072 5200 0000 7218  o...r....rR...r.
+00004820: 0000 0072 1e00 0000 721d 0000 0072 4400  ...r....r....rD.
+00004830: 0000 7242 0000 0072 7000 0000 7247 0000  ..rB...rp...rG..
+00004840: 005a 0561 7272 6179 7203 0000 00da 0270  .Z.arrayr......p
+00004850: 64da 0653 6572 6965 7329 2d72 2400 0000  d..Series)-r$...
+00004860: 7225 0000 005a 0869 6e62 6564 5f62 67da  r%...Z.inbed_bg.
+00004870: 076f 7574 6669 6c65 5a05 6e5f 6375 745a  .outfileZ.n_cutZ
+00004880: 0570 5f63 7574 da07 7265 7375 6c74 735a  .p_cut..resultsZ
+00004890: 0b69 6e62 6564 315f 6e61 6d65 5a0b 696e  .inbed1_nameZ.in
+000048a0: 6265 6432 5f6e 616d 6572 5300 0000 7254  bed2_namerS...rT
+000048b0: 0000 005a 0a62 6163 6b67 726f 756e 6472  ...Z.backgroundr
+000048c0: 5500 0000 7256 0000 0072 5700 0000 7258  U...rV...rW...rX
+000048d0: 0000 0072 5900 0000 725a 0000 0072 5b00  ...rY...rZ...r[.
+000048e0: 0000 725c 0000 005a 0962 6564 315f 6f6e  ..r\...Z.bed1_on
+000048f0: 6c79 5a09 6265 6432 5f6f 6e6c 795a 0763  lyZ.bed2_onlyZ.c
+00004900: 6f6f 6363 7572 5a07 6e65 6974 6865 72da  ooccurZ.neither.
+00004910: 034f 5554 721b 0000 0072 1e00 0000 721d  .OUTr....r....r.
+00004920: 0000 00da 046c 696e 655a 0962 6564 315f  .....lineZ.bed1_
+00004930: 666c 6167 5a09 6265 6432 5f66 6c61 675a  flagZ.bed2_flagZ
+00004940: 0d62 6564 325f 6f76 6572 6c61 7073 5a10  .bed2_overlapsZ.
+00004950: 6265 6432 5f6f 7665 726c 6170 5f6c 7374  bed2_overlap_lst
+00004960: 7275 0000 005a 1162 6564 325f 6f76 6572  ru...Z.bed2_over
+00004970: 6c61 705f 7369 7a65 5a11 6265 6432 5f67  lap_sizeZ.bed2_g
+00004980: 656e 6f6d 6963 5f73 697a 655a 1262 6564  enomic_sizeZ.bed
+00004990: 325f 6f76 6572 6c61 705f 7261 7469 6f5a  2_overlap_ratioZ
+000049a0: 0d62 6564 315f 6f76 6572 6c61 7073 5a10  .bed1_overlapsZ.
+000049b0: 6265 6431 5f6f 7665 726c 6170 5f6c 7374  bed1_overlap_lst
+000049c0: 5a11 6265 6431 5f6f 7665 726c 6170 5f73  Z.bed1_overlap_s
+000049d0: 697a 655a 1162 6564 315f 6765 6e6f 6d69  izeZ.bed1_genomi
+000049e0: 635f 7369 7a65 5a12 6265 6431 5f6f 7665  c_sizeZ.bed1_ove
+000049f0: 726c 6170 5f72 6174 696f da05 7461 626c  rlap_ratio..tabl
+00004a00: 655a 056f 6464 7372 da01 7072 1f00 0000  eZ.oddsr..pr....
+00004a10: 721f 0000 0072 2000 0000 da0c 636f 6f63  r....r .....cooc
+00004a20: 6375 725f 7065 616b a302 0000 7308 0100  cur_peak....s...
+00004a30: 0000 1c04 010c 010c 0108 0108 010e 0108  ................
+00004a40: 010c 020e 0108 010c 080e 0108 010c 030e  ................
+00004a50: 0104 010e 0108 010a 0116 020e 0104 010e  ................
+00004a60: 010a 010a 0116 0304 0104 0104 0104 010a  ................
+00004a70: 0310 011c 0104 0104 0214 0104 0114 0110  ................
+00004a80: 010e 0102 0204 0108 0118 0112 0108 0102  ................
+00004a90: 010c 0106 010a 0114 0108 0114 0110 010e  ................
+00004aa0: 0102 0204 0108 0118 0112 0108 0102 010c  ................
+00004ab0: 0106 010a 0114 0108 0310 0210 010e 010e  ................
+00004ac0: 0102 010e 0104 0108 0118 0112 0108 0102  ................
+00004ad0: 010c 0106 010a 0114 0108 010e 0104 0108  ................
+00004ae0: 0118 0112 0108 0102 010c 0106 010a 0114  ................
+00004af0: 0104 020e 0102 010e 0104 0108 0118 0112  ................
+00004b00: 0108 0102 010c 0106 010a 0114 0104 0106  ................
+00004b10: 0106 0108 0112 0208 0116 0206 0108 0116  ................
+00004b20: 0208 0114 0308 0108 0108 0108 030a 0118  ................
+00004b30: 0216 0210 0108 0108 0172 8200 0000 6302  .........r....c.
+00004b40: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00004b50: 0000 0043 0000 0073 3c00 0000 7400 7c01  ...C...s<...t.|.
+00004b60: 6401 8302 7d02 7c00 4400 5d20 7d03 7401  d...}.|.D.] }.t.
+00004b70: 6402 a002 6403 6404 8400 7c03 4400 8301  d...d.d...|.D...
+00004b80: a101 7c02 6405 8d02 0100 710e 7c02 a003  ..|.d.....q.|...
+00004b90: a100 0100 6406 5300 2907 7a25 2053 6176  ....d.S.).z% Sav
+00004ba0: 6520 6c69 7374 206f 6620 6765 6e6f 6d69  e list of genomi
+00004bb0: 6320 7265 6769 6f6e 7320 746f 2066 696c  c regions to fil
+00004bc0: 6572 6000 0000 7261 0000 0063 0100 0000  er`...ra...c....
+00004bd0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00004be0: 5300 0000 7314 0000 0067 007c 005d 0c7d  S...s....g.|.].}
+00004bf0: 0174 007c 0183 0191 0271 0453 0072 1f00  .t.|.....q.S.r..
+00004c00: 0000 7266 0000 0072 6700 0000 721f 0000  ..rf...rg...r...
+00004c10: 0072 1f00 0000 7220 0000 0072 6a00 0000  .r....r ...rj...
+00004c20: 6803 0000 7304 0000 0006 0002 007a 1f62  h...s........z.b
+00004c30: 6564 5f74 6f5f 6669 6c65 2e3c 6c6f 6361  ed_to_file.<loca
+00004c40: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7262  ls>.<listcomp>rb
+00004c50: 0000 004e 2904 726f 0000 0072 7000 0000  ...N).ro...rp...
+00004c60: 7271 0000 0072 7200 0000 2904 5a08 6265  rq...rr...).Z.be
+00004c70: 645f 6c69 7374 5a08 6265 645f 6669 6c65  d_listZ.bed_file
+00004c80: 727e 0000 0072 3d00 0000 721f 0000 0072  r~...r=...r....r
+00004c90: 1f00 0000 7220 0000 00da 0b62 6564 5f74  ....r .....bed_t
+00004ca0: 6f5f 6669 6c65 6403 0000 7308 0000 0000  o_filed...s.....
+00004cb0: 020a 0108 011e 0172 8300 0000 6306 0000  .......r....c...
+00004cc0: 0000 0000 0000 0000 0006 0000 0006 0000  ................
+00004cd0: 0043 0000 0073 4600 0000 7c01 6401 1700  .C...sF...|.d...
+00004ce0: 7d01 7c02 7d02 7c04 6401 1700 7d04 7c05  }.|.}.|.d...}.|.
+00004cf0: 7d05 7c00 7c03 6b03 7224 6402 5300 7400  }.|.|.k.r$d.S.t.
+00004d00: 7401 7402 7c01 7c04 8302 7403 7c02 7c05  t.t.|.|...t.|.|.
+00004d10: 8302 6401 1700 8302 8301 5300 6403 5300  ..d.......S.d.S.
+00004d20: 2904 61d8 0100 000a 0943 6865 636b 2069  ).a......Check i
+00004d30: 6620 7477 6f20 7265 6769 6f73 2061 7265  f two regios are
+00004d40: 206f 7665 726c 6170 2e0a 0a09 5061 7261   overlap....Para
+00004d50: 6d65 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d  meters..--------
+00004d60: 2d2d 0a09 6368 7231 203a 2073 7472 0a09  --..chr1 : str..
 00004d70: 0943 6872 6f6d 6f73 6f6d 6520 4944 206f  .Chromosome ID o
-00004d80: 6620 7468 6520 7365 636f 6e64 2067 656e  f the second gen
-00004d90: 6f6d 6963 2072 6567 696f 6e0a 0973 7432  omic region..st2
-00004da0: 203a 2069 6e74 0a09 0953 7461 7274 2063   : int...Start c
-00004db0: 6f6f 7264 696e 6174 6520 6f66 2074 6865  oordinate of the
-00004dc0: 2073 6563 6f6e 6420 6765 6e6f 6d69 6320   second genomic 
-00004dd0: 7265 6769 6f6e 0a09 656e 6432 203a 2069  region..end2 : i
-00004de0: 6e74 0a09 0945 6e64 2063 6f6f 7264 696e  nt...End coordin
-00004df0: 6174 6520 6f66 2074 6865 2073 6563 6f6e  ate of the secon
-00004e00: 6420 6765 6e6f 6d69 6320 7265 6769 6f6e  d genomic region
-00004e10: 0a09 5265 7475 726e 0a09 2d2d 2d2d 2d2d  ..Return..------
-00004e20: 0a09 0930 3a20 6e6f 6e20 6f76 6572 6c61  ...0: non overla
-00004e30: 700a 0909 706f 7369 7469 7665 2069 6e74  p...positive int
-00004e40: 6567 6572 205b 312c 293a 206f 7665 726c  eger [1,): overl
-00004e50: 6170 0a09 720d 0000 0072 0100 0000 4e29  ap..r....r....N)
-00004e60: 0472 1000 0000 da05 7261 6e67 6572 5100  .r......rangerQ.
-00004e70: 0000 7250 0000 0029 065a 0463 6872 315a  ..rP...).Z.chr1Z
-00004e80: 0373 7431 5a04 656e 6431 5a04 6368 7232  .st1Z.end1Z.chr2
-00004e90: 5a03 7374 325a 0465 6e64 3272 2100 0000  Z.st2Z.end2r!...
-00004ea0: 7221 0000 0072 2200 0000 da0a 6973 5f6f  r!...r".....is_o
-00004eb0: 7665 726c 6170 6503 0000 730e 0000 0000  verlape...s.....
-00004ec0: 1808 0104 0108 0104 0108 0104 0272 9800  .............r..
-00004ed0: 0000 6302 0000 0000 0000 0000 0000 000a  ..c.............
-00004ee0: 0000 0007 0000 0043 0000 0073 5e01 0000  .......C...s^...
-00004ef0: 6401 7d02 7a44 7c00 6402 1900 7d03 7400  d.}.zD|.d...}.t.
-00004f00: 7c00 6403 1900 8301 7d04 7400 7c00 6404  |.d.....}.t.|.d.
-00004f10: 1900 8301 7d05 7c01 6402 1900 7d06 7400  ....}.|.d...}.t.
-00004f20: 7c01 6403 1900 8301 7d07 7400 7c01 6404  |.d.....}.t.|.d.
-00004f30: 1900 8301 7d08 5700 6e14 0100 0100 0100  ....}.W.n.......
-00004f40: 6405 7d02 7c02 0600 5900 5300 5800 7401  d.}.|...Y.S.X.t.
-00004f50: 7c03 7c04 7c05 7c06 7c07 7c08 8306 7d09  |.|.|.|.|.|...}.
-00004f60: 7c09 6402 6b02 72a2 7c03 7c06 6b03 7286  |.d.k.r.|.|.k.r.
-00004f70: 6406 7d02 6e1a 7c04 7c08 6b02 7396 7c05  d.}.n.|.|.k.s.|.
-00004f80: 7c07 6b02 729c 6407 7d02 6e04 6406 7d02  |.k.r.d.}.n.d.}.
-00004f90: 6eb8 7c09 6402 6b04 9001 725a 7c04 7c07  n.|.d.k...rZ|.|.
-00004fa0: 6b02 72c2 7c05 7c08 6b02 72c2 6408 7d02  k.r.|.|.k.r.d.}.
-00004fb0: 6e98 7c04 7c07 6b05 72d8 7c05 7c08 6b00  n.|.|.k.r.|.|.k.
-00004fc0: 72d8 6409 7d02 6e82 7c04 7c07 6b04 72ee  r.d.}.n.|.|.k.r.
-00004fd0: 7c05 7c08 6b01 72ee 6409 7d02 6e6c 7c04  |.|.k.r.d.}.nl|.
-00004fe0: 7c07 6b04 9001 7208 7c05 7c08 6b00 9001  |.k...r.|.|.k...
-00004ff0: 7208 6409 7d02 6e52 7c04 7c07 6b01 9001  r.d.}.nR|.|.k...
-00005000: 7222 7c05 7c08 6b04 9001 7222 640a 7d02  r"|.|.k...r"d.}.
-00005010: 6e38 7c04 7c07 6b00 9001 723c 7c05 7c08  n8|.|.k...r<|.|.
-00005020: 6b05 9001 723c 640a 7d02 6e1e 7c04 7c07  k...r<d.}.n.|.|.
-00005030: 6b00 9001 7256 7c05 7c08 6b04 9001 7256  k...rV|.|.k...rV
-00005040: 640a 7d02 6e04 640b 7d02 7c02 5300 290c  d.}.n.d.}.|.S.).
-00005050: 614f 0100 000a 0944 6574 6572 6d69 6e65  aO.....Determine
-00005060: 2074 6865 2073 7061 7469 616c 2072 656c   the spatial rel
-00005070: 6174 696f 6e73 206f 6620 6765 6e6f 6d69  ations of genomi
-00005080: 6320 7265 6769 6f6e 7320 2853 524f 4729  c regions (SROG)
-00005090: 0a0a 0950 6172 616d 6574 6572 730a 092d  ...Parameters..-
-000050a0: 2d2d 2d2d 2d2d 2d2d 2d0a 096c 7374 3120  ---------..lst1 
-000050b0: 3a20 7475 706c 650a 0909 4120 7475 706c  : tuple...A tupl
-000050c0: 6520 6f66 2067 656e 6f6d 6963 2069 6e74  e of genomic int
-000050d0: 6572 7661 6c2e 2045 672e 2028 2763 6872  erval. Eg. ('chr
-000050e0: 3127 2c20 312c 2031 3030 292e 0a09 6c73  1', 1, 100)...ls
-000050f0: 7432 203a 2074 7570 6c65 0a09 0941 2074  t2 : tuple...A t
-00005100: 7570 6c65 206f 6620 6765 6e6f 6d69 6320  uple of genomic 
-00005110: 696e 7465 7276 616c 2e20 4567 2e20 2827  interval. Eg. ('
-00005120: 6368 7231 272c 2031 352c 2036 3029 2e2e  chr1', 15, 60)..
-00005130: 0a0a 0952 6574 7572 6e73 0a09 2d2d 2d2d  ...Returns..----
-00005140: 2d2d 2d0a 0972 6574 7572 6e5f 636f 6465  ---..return_code
-00005150: 203a 2073 7472 0a09 0952 6574 7572 6e20   : str...Return 
-00005160: 6f6e 6520 6f66 2028 2764 6973 6a6f 696e  one of ('disjoin
-00005170: 7427 2c27 746f 7563 6827 2c27 6571 7561  t','touch','equa
-00005180: 6c27 2c27 6f76 6572 6c61 7027 2c27 636f  l','overlap','co
-00005190: 6e74 6169 6e27 2c27 7769 7468 696e 2729  ntain','within')
-000051a0: 2e0a 0a09 da00 7201 0000 0072 0d00 0000  ......r....r....
-000051b0: 7235 0000 00da 0775 6e6b 6e6f 776e da08  r5.....unknown..
-000051c0: 6469 736a 6f69 6e74 da05 746f 7563 68da  disjoint..touch.
-000051d0: 0565 7175 616c da06 7769 7468 696e da07  .equal..within..
-000051e0: 636f 6e74 6169 6eda 076f 7665 726c 6170  contain..overlap
-000051f0: 2902 7236 0000 0072 9800 0000 290a 5a04  ).r6...r....).Z.
-00005200: 6c73 7431 5a04 6c73 7432 5a0b 7265 7475  lst1Z.lst2Z.retu
-00005210: 726e 5f63 6f64 655a 0763 6872 6f6d 5f31  rn_codeZ.chrom_1
-00005220: 5a07 7374 6172 745f 315a 0565 6e64 5f31  Z.start_1Z.end_1
-00005230: 5a07 6368 726f 6d5f 325a 0773 7461 7274  Z.chrom_2Z.start
-00005240: 5f32 5a05 656e 645f 325a 076f 765f 7369  _2Z.end_2Z.ov_si
-00005250: 7a65 7221 0000 0072 2100 0000 7222 0000  zer!...r!...r"..
-00005260: 00da 0873 726f 6763 6f64 6586 0300 0073  ...srogcode....s
-00005270: 4600 0000 0011 0401 0201 0801 0c01 0c01  F...............
-00005280: 0801 0c01 1001 0601 0401 0a01 1201 0801  ................
-00005290: 0801 0602 1001 0602 0601 0a01 1001 0601  ................
-000052a0: 1001 0601 1001 0601 1401 0601 1401 0601  ................
-000052b0: 1401 0601 1401 0602 0401 72a1 0000 00e9  ..........r.....
-000052c0: 80b2 e60e 6306 0000 0000 0000 0000 0000  ....c...........
-000052d0: 001a 0000 0009 0000 0043 0000 0073 ea03  .........C...s..
-000052e0: 0000 6900 7d06 7400 7c02 6401 8302 7d07  ..i.}.t.|.d...}.
-000052f0: 6402 6402 6402 6402 6402 6402 6402 6403  d.d.d.d.d.d.d.d.
-00005300: 9c07 7d08 7401 a002 6404 7c01 1600 a101  ..}.t...d.|.....
-00005310: 0100 7403 a004 7c01 a101 4400 9001 5d02  ..t...|...D...].
-00005320: 7d09 7c09 a005 6405 a101 724c 713a 7c09  }.|...d...rLq:|.
-00005330: a006 a100 7d0a 7407 7c0a 8301 6406 6b00  ....}.t.|...d.k.
-00005340: 7270 7401 a008 6407 7c09 1600 a101 0100  rpt...d.|.......
-00005350: 713a 7c0a 6402 1900 7409 7c0a 6408 1900  q:|.d...t.|.d...
-00005360: 8301 7409 7c0a 6409 1900 8301 0300 0200  ..t.|.d.........
-00005370: 7d0b 7d0c 7d0d 7c0c 7c0d 6b04 72ac 7401  }.}.}.|.|.k.r.t.
-00005380: a008 640a 7c09 1600 a101 0100 713a 7a0c  ..d.|.......q:z.
-00005390: 7c0a 6406 1900 7d0e 5700 6e2c 0100 0100  |.d...}.W.n,....
-000053a0: 0100 7c0a 6402 1900 640b 1700 7c0a 6408  ..|.d...d...|.d.
-000053b0: 1900 1700 640c 1700 7c0a 6409 1900 1700  ....d...|.d.....
-000053c0: 7d0e 5900 6e02 5800 7a18 7c0a 640d 1900  }.Y.n.X.z.|.d...
-000053d0: 7d0f 7c0f 640e 6b07 72fc 640f 7d0f 5700  }.|.d.k.r.d.}.W.
-000053e0: 6e10 0100 0100 0100 640f 7d0f 5900 6e02  n.......d.}.Y.n.
-000053f0: 5800 7c0b 7c06 6b07 9001 7224 740a 8300  X.|.|.k...r$t...
-00005400: 7c06 7c0b 3c00 7c06 7c0b 1900 a00b 740c  |.|.<.|.|.....t.
-00005410: 7c0c 7c0d 7c0e 7c0f 6410 8d04 a101 0100  |.|.|.|.d.......
-00005420: 713a 7401 a002 6411 7c00 1600 a101 0100  q:t...d.|.......
-00005430: 7403 a004 7c00 a101 4400 9002 5d82 7d09  t...|...D...].}.
-00005440: 7c09 a005 6405 a101 9001 726e 9001 7158  |...d.....rn..qX
-00005450: 7c09 a006 a100 7d0a 7407 7c0a 8301 6406  |.....}.t.|...d.
-00005460: 6b00 9001 7296 7401 a008 6407 7c09 1600  k...r.t...d.|...
-00005470: a101 0100 9001 7158 7c0a 6402 1900 7409  ......qX|.d...t.
-00005480: 7c0a 6408 1900 8301 7409 7c0a 6409 1900  |.d.....t.|.d...
-00005490: 8301 0300 0200 7d0b 7d0c 7d0d 7c0c 7c0d  ......}.}.}.|.|.
-000054a0: 6b04 9001 72d6 7401 a008 6412 7c09 1600  k...r.t...d.|...
-000054b0: a101 0100 9001 7158 7a0c 7c0a 6406 1900  ......qXz.|.d...
-000054c0: 7d0e 5700 6e2c 0100 0100 0100 7c0a 6402  }.W.n,......|.d.
-000054d0: 1900 640b 1700 7c0a 6408 1900 1700 640c  ..d...|.d.....d.
-000054e0: 1700 7c0a 6409 1900 1700 7d0e 5900 6e02  ..|.d.....}.Y.n.
-000054f0: 5800 7a1a 7c0a 640d 1900 7d0f 7c0f 640e  X.z.|.d...}.|.d.
-00005500: 6b07 9002 7228 640f 7d0f 5700 6e10 0100  k...r(d.}.W.n...
-00005510: 0100 0100 640f 7d0f 5900 6e02 5800 7c0b  ....d.}.Y.n.X.|.
-00005520: 7c06 6b07 9002 7276 7c08 6413 0500 1900  |.k...rv|.d.....
-00005530: 6408 3700 0300 3c00 740d 7c09 6414 1700  d.7...<.t.|.d...
-00005540: 6415 1700 6414 1700 6415 1700 7c07 6416  d...d...d...|.d.
-00005550: 8d02 0100 9001 7158 7c06 7c0b 1900 a00e  ......qX|.|.....
-00005560: 7c0c 7c0d a102 7d10 7407 7c10 8301 6402  |.|...}.t.|...d.
-00005570: 6b02 9003 7252 7c08 6413 0500 1900 6408  k...rR|.d.....d.
-00005580: 3700 0300 3c00 7c06 7c0b 1900 6a0f 740c  7...<.|.|...j.t.
-00005590: 7c0c 7c0d 7c0f 6417 8d03 7c03 7c05 6418  |.|.|.d...|.|.d.
-000055a0: 8d03 7d11 7c06 7c0b 1900 6a10 740c 7c0c  ..}.|.|...j.t.|.
-000055b0: 7c0d 7c0f 6417 8d03 7c04 7c05 6418 8d03  |.|.d...|.|.d...
-000055c0: 7d12 7407 7c11 8301 6402 6b02 9002 72f4  }.t.|...d.k...r.
-000055d0: 6415 7d13 6e0e 7411 7c11 6402 1900 6a12  d.}.n.t.|.d...j.
-000055e0: 8301 7d13 7407 7c12 8301 6402 6b02 9003  ..}.t.|...d.k...
-000055f0: 7216 6415 7d14 6e0e 7411 7c12 6402 1900  r.d.}.n.t.|.d...
-00005600: 6a12 8301 7d14 740d 7c09 6414 1700 6413  j...}.t.|.d...d.
-00005610: 1700 6414 1700 6419 1700 7c13 1700 641a  ..d...d...|...d.
-00005620: 1700 641b 1700 7c14 1700 7c07 6416 8d02  ..d...|...|.d...
-00005630: 0100 6e88 6700 7d15 6700 7d16 7c10 4400  ..n.g.}.g.}.|.D.
-00005640: 5d36 7d17 7413 7c0b 7c0c 7c0d 6603 7c0b  ]6}.t.|.|.|.f.|.
-00005650: 7c17 6a14 7c17 6a15 6603 8302 7d18 7c15  |.j.|.j.f...}.|.
-00005660: a016 7c18 a101 0100 7c16 a016 7c17 6a12  ..|.....|...|.j.
-00005670: a101 0100 9003 715e 740d 7c09 6414 1700  ......q^t.|.d...
-00005680: 641a a017 7c15 a101 1700 6414 1700 641a  d...|.....d...d.
-00005690: a017 7c16 a101 1700 7c07 6416 8d02 0100  ..|.....|.d.....
-000056a0: 7c15 4400 5d16 7d19 7c08 7c19 0500 1900  |.D.].}.|.|.....
-000056b0: 6408 3700 0300 3c00 9003 71c2 9001 7158  d.7...<...q...qX
-000056c0: 7418 6a19 7c08 641c 8d01 5300 291d 7add  t.j.|.d...S.).z.
-000056d0: 0a09 4361 6c63 756c 6174 6573 2053 524f  ..Calculates SRO
-000056e0: 4720 636f 6465 2066 6f72 2065 6163 6820  G code for each 
-000056f0: 7265 6769 6f6e 2069 6e20 696e 6265 6431  region in inbed1
-00005700: 0a0a 0950 6172 616d 6574 6572 730a 092d  ...Parameters..-
-00005710: 2d2d 2d2d 2d2d 2d2d 2d0a 0969 6e62 6564  ---------..inbed
-00005720: 3120 3a20 7374 720a 0909 4e61 6d65 206f  1 : str...Name o
-00005730: 6620 6120 4245 4420 6669 6c65 2e0a 0969  f a BED file...i
-00005740: 6e62 6564 3220 3a20 7374 720a 0909 4e61  nbed2 : str...Na
-00005750: 6d65 206f 6620 616e 6f74 6865 7220 4245  me of another BE
-00005760: 4420 6669 6c65 2e0a 096f 7574 6669 6c65  D file...outfile
-00005770: 203a 2073 7472 0a09 094e 616d 6520 6f66   : str...Name of
-00005780: 206f 7574 7075 7420 6669 6c65 2e0a 0a09   output file....
-00005790: 5265 7475 726e 730a 092d 2d2d 2d2d 2d2d  Returns..-------
-000057a0: 0a09 7064 2053 6572 6965 730a 0972 6900  ..pd Series..ri.
-000057b0: 0000 7201 0000 0029 0772 9b00 0000 72a0  ..r....).r....r.
-000057c0: 0000 0072 9f00 0000 729e 0000 0072 9c00  ...r....r....r..
-000057d0: 0000 729d 0000 00da 056f 7468 6572 7a23  ..r......otherz#
-000057e0: 4275 696c 6420 696e 7465 7276 616c 2074  Build interval t
-000057f0: 7265 6520 6672 6f6d 2066 696c 653a 2022  ree from file: "
-00005800: 2573 2272 2f00 0000 7233 0000 007a 4549  %s"r/...r3...zEI
-00005810: 6e76 616c 6964 2042 4544 206c 696e 6520  nvalid BED line 
-00005820: 2852 6571 7569 7265 7320 6174 206c 6561  (Requires at lea
-00005830: 7374 2033 2063 6f6c 756d 6e73 3a20 6368  st 3 columns: ch
-00005840: 726f 6d2c 2073 7461 7274 2c20 656e 6429  rom, start, end)
-00005850: 3a20 2573 720d 0000 0072 3500 0000 7a22  : %sr....r5...z"
-00005860: 696e 7661 6c69 6420 4245 4420 6c69 6e65  invalid BED line
-00005870: 2028 7374 6172 7420 3e20 656e 6429 3a20   (start > end): 
-00005880: 2573 726d 0000 0072 6e00 0000 e905 0000  %srm...rn.......
-00005890: 0029 02fa 012b 726e 0000 0072 a500 0000  .)...+rn...r....
-000058a0: 2902 da05 7661 6c75 65da 0673 7472 616e  )...value..stran
-000058b0: 647a 1652 6561 6469 6e67 2042 4544 2066  dz.Reading BED f
-000058c0: 696c 653a 2022 2573 227a 2249 6e76 616c  ile: "%s"z"Inval
-000058d0: 6964 2042 4544 206c 696e 6520 2873 7461  id BED line (sta
-000058e0: 7274 203e 2065 6e64 293a 2025 7372 9b00  rt > end): %sr..
-000058f0: 0000 726a 0000 0072 6800 0000 726b 0000  ..rj...rh...rk..
-00005900: 0029 0172 a700 0000 2902 5a0d 6e75 6d5f  .).r....).Z.num_
-00005910: 696e 7465 7276 616c 73da 086d 6178 5f64  intervals..max_d
-00005920: 6973 747a 0b55 7049 6e74 6572 7661 6c3d  istz.UpInterval=
-00005930: 7274 0000 007a 0d44 6f77 6e49 6e74 6572  rt...z.DownInter
-00005940: 7661 6c3d 2901 7285 0000 0029 1a72 7800  val=).r....).rx.
-00005950: 0000 7213 0000 0072 5900 0000 7208 0000  ..r....rY...r...
-00005960: 0072 1200 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-00005970: 7210 0000 0072 3900 0000 7236 0000 0072  r....r9...r6...r
-00005980: 0700 0000 725a 0000 0072 0600 0000 7279  ....rZ...r....ry
-00005990: 0000 0072 5b00 0000 5a14 7570 7374 7265  ...r[...Z.upstre
-000059a0: 616d 5f6f 665f 696e 7465 7276 616c 5a16  am_of_intervalZ.
-000059b0: 646f 776e 7374 7265 616d 5f6f 665f 696e  downstream_of_in
-000059c0: 7465 7276 616c 7211 0000 0072 a600 0000  tervalr....r....
-000059d0: 72a1 0000 0072 2000 0000 721f 0000 0072  r....r ...r....r
-000059e0: 1a00 0000 727a 0000 0072 8800 0000 7289  ....rz...r....r.
-000059f0: 0000 0029 1a72 2600 0000 7227 0000 0072  ...).r&...r'...r
-00005a00: 8b00 0000 5a04 6e5f 7570 5a06 6e5f 646f  ....Z.n_upZ.n_do
-00005a10: 776e 72a8 0000 00da 046d 6170 735a 064f  wnr......mapsZ.O
-00005a20: 5554 5055 545a 0c73 726f 675f 7375 6d6d  UTPUTZ.srog_summ
-00005a30: 6172 7972 3d00 0000 723e 0000 0072 1d00  aryr=...r>...r..
-00005a40: 0000 7220 0000 0072 1f00 0000 7286 0000  ..r ...r....r...
-00005a50: 005a 0a73 7472 616e 646e 6573 7372 7f00  .Z.strandnessr..
-00005a60: 0000 5a0b 7570 5f69 6e74 6572 7661 6c5a  ..Z.up_intervalZ
-00005a70: 0d64 6f77 6e5f 696e 7465 7276 616c 5a10  .down_intervalZ.
-00005a80: 7570 5f69 6e74 6572 7661 6c5f 6e61 6d65  up_interval_name
-00005a90: 5a12 646f 776e 5f69 6e74 6572 7661 6c5f  Z.down_interval_
-00005aa0: 6e61 6d65 5a0a 7372 6f67 5f63 6f64 6573  nameZ.srog_codes
-00005ab0: 5a0c 7461 7267 6574 5f6e 616d 6573 7280  Z.target_namesr.
-00005ac0: 0000 0072 3f00 0000 da04 636f 6465 7221  ...r?.....coder!
-00005ad0: 0000 0072 2100 0000 7222 0000 00da 0973  ...r!...r".....s
-00005ae0: 726f 675f 7065 616b bf03 0000 7398 0000  rog_peak....s...
-00005af0: 0000 1304 010a 0114 010e 0110 010a 0002  ................
-00005b00: 0108 010c 010e 0102 0124 0108 010e 0102  .........$......
-00005b10: 0302 010c 0106 0126 0302 0108 0108 0108  .......&........
-00005b20: 0106 010a 020a 010a 011c 020e 0110 010c  ................
-00005b30: 0004 0108 010e 010e 0104 0124 010a 010e  ...........$....
-00005b40: 0104 0302 010c 0106 0126 0302 0108 010a  .........&......
-00005b50: 0108 0106 010a 020a 0110 011c 0104 0210  ................
-00005b60: 010e 0110 011e 011e 010e 0106 020e 010e  ................
-00005b70: 0106 020e 012e 0204 0104 0108 011a 010a  ................
-00005b80: 0110 0128 0108 0118 0172 ab00 0000 da08  ...(.....r......
-00005b90: 5f5f 6d61 696e 5f5f 7235 0000 0072 3300  __main__r5...r3.
-00005ba0: 0000 2901 7268 0000 0029 0272 0d00 0000  ..).rh...).r....
-00005bb0: 7282 0000 0029 0372 0d00 0000 720d 0000  r....).r....r...
-00005bc0: 0072 a200 0000 2930 7215 0000 0072 7600  .r....)0r....rv.
-00005bd0: 0000 7213 0000 00da 056e 756d 7079 724d  ..r......numpyrM
-00005be0: 0000 00da 0670 616e 6461 7372 8800 0000  .....pandasr....
-00005bf0: da07 6f73 2e70 6174 6872 0200 0000 da0b  ..os.pathr......
-00005c00: 7363 6970 792e 7374 6174 7372 0300 0000  scipy.statsr....
-00005c10: 5a12 6278 2e62 6974 7365 745f 6275 696c  Z.bx.bitset_buil
-00005c20: 6465 7273 7204 0000 0072 0500 0000 5a19  dersr....r....Z.
-00005c30: 6278 2e69 6e74 6572 7661 6c73 2e69 6e74  bx.intervals.int
-00005c40: 6572 7365 6374 696f 6e72 0600 0000 7207  ersectionr....r.
-00005c50: 0000 00da 0d63 6f62 696e 6461 6269 6c69  .....cobindabili
-00005c60: 7479 7208 0000 0072 0900 0000 da0a 5f5f  tyr....r......__
-00005c70: 6175 7468 6f72 5f5f da0d 5f5f 636f 7079  author__..__copy
-00005c80: 7269 6768 745f 5fda 0b5f 5f63 7265 6469  right__..__credi
-00005c90: 7473 5f5f da0b 5f5f 6c69 6365 6e73 655f  ts__..__license_
-00005ca0: 5fda 0b5f 5f76 6572 7369 6f6e 5f5f da0e  _..__version__..
-00005cb0: 5f5f 6d61 696e 7461 696e 6572 5f5f da09  __maintainer__..
-00005cc0: 5f5f 656d 6169 6c5f 5fda 0a5f 5f73 7461  __email__..__sta
-00005cd0: 7475 735f 5f72 2300 0000 722b 0000 0072  tus__r#...r+...r
-00005ce0: 2e00 0000 7240 0000 0072 4100 0000 7244  ....r@...rA...rD
-00005cf0: 0000 0072 4800 0000 7254 0000 0072 2c00  ...rH...rT...r,.
-00005d00: 0000 7267 0000 0072 8100 0000 7295 0000  ..rg...r....r...
-00005d10: 0072 9600 0000 7298 0000 0072 a100 0000  .r....r....r....
-00005d20: 72ab 0000 00da 085f 5f6e 616d 655f 5f72  r......__name__r
-00005d30: 3a00 0000 da01 6172 7900 0000 7221 0000  :.....ary...r!..
-00005d40: 0072 2100 0000 7221 0000 0072 2200 0000  .r!...r!...r"...
-00005d50: da08 3c6d 6f64 756c 653e 0300 0000 7348  ..<module>....sH
-00005d60: 0000 0010 0108 0108 0108 010c 010c 0110  ................
-00005d70: 0110 0110 0204 0104 0104 0104 0106 0104  ................
-00005d80: 0104 0104 0308 3208 4f08 4c08 2b08 2808  ......2.O.L.+.(.
-00005d90: 3408 2b08 2108 1508 610a 6f0a 7f00 4208  4.+.!...a.o...B.
-00005da0: 0808 2108 390a 6e0a 051e 01              ..!.9.n....
+00004d80: 6620 7468 6520 6669 7273 7420 6765 6e6f  f the first geno
+00004d90: 6d69 6320 7265 6769 6f6e 0a09 7374 3120  mic region..st1 
+00004da0: 3a20 696e 740a 0909 5374 6172 7420 636f  : int...Start co
+00004db0: 6f72 6469 6e61 7465 206f 6620 7468 6520  ordinate of the 
+00004dc0: 6669 7273 7420 6765 6e6f 6d69 6320 7265  first genomic re
+00004dd0: 6769 6f6e 0a09 656e 6431 203a 2069 6e74  gion..end1 : int
+00004de0: 0a09 0945 6e64 2063 6f6f 7264 696e 6174  ...End coordinat
+00004df0: 6520 6f66 2074 6865 2066 6972 7374 2067  e of the first g
+00004e00: 656e 6f6d 6963 2072 6567 696f 6e0a 0963  enomic region..c
+00004e10: 6872 3220 3a20 7374 720a 0909 4368 726f  hr2 : str...Chro
+00004e20: 6d6f 736f 6d65 2049 4420 6f66 2074 6865  mosome ID of the
+00004e30: 2073 6563 6f6e 6420 6765 6e6f 6d69 6320   second genomic 
+00004e40: 7265 6769 6f6e 0a09 7374 3220 3a20 696e  region..st2 : in
+00004e50: 740a 0909 5374 6172 7420 636f 6f72 6469  t...Start coordi
+00004e60: 6e61 7465 206f 6620 7468 6520 7365 636f  nate of the seco
+00004e70: 6e64 2067 656e 6f6d 6963 2072 6567 696f  nd genomic regio
+00004e80: 6e0a 0965 6e64 3220 3a20 696e 740a 0909  n..end2 : int...
+00004e90: 456e 6420 636f 6f72 6469 6e61 7465 206f  End coordinate o
+00004ea0: 6620 7468 6520 7365 636f 6e64 2067 656e  f the second gen
+00004eb0: 6f6d 6963 2072 6567 696f 6e0a 0952 6574  omic region..Ret
+00004ec0: 7572 6e0a 092d 2d2d 2d2d 2d0a 0909 303a  urn..------...0:
+00004ed0: 206e 6f6e 206f 7665 726c 6170 0a09 0970   non overlap...p
+00004ee0: 6f73 6974 6976 6520 696e 7465 6765 7220  ositive integer 
+00004ef0: 5b31 2c29 3a20 6f76 6572 6c61 700a 0972  [1,): overlap..r
+00004f00: 0b00 0000 7201 0000 004e 2904 720e 0000  ....r....N).r...
+00004f10: 00da 0572 616e 6765 7249 0000 0072 4800  ...rangerI...rH.
+00004f20: 0000 2906 da04 6368 7231 5a03 7374 315a  ..)...chr1Z.st1Z
+00004f30: 0465 6e64 31da 0463 6872 325a 0373 7432  .end1..chr2Z.st2
+00004f40: 5a04 656e 6432 721f 0000 0072 1f00 0000  Z.end2r....r....
+00004f50: 7220 0000 00da 0a69 735f 6f76 6572 6c61  r .....is_overla
+00004f60: 706c 0300 0073 0e00 0000 0018 0801 0401  pl...s..........
+00004f70: 0801 0401 0801 0402 7287 0000 0063 0200  ........r....c..
+00004f80: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
+00004f90: 0000 4300 0000 735e 0100 0064 017d 027a  ..C...s^...d.}.z
+00004fa0: 447c 0064 0219 007d 0374 007c 0064 0319  D|.d...}.t.|.d..
+00004fb0: 0083 017d 0474 007c 0064 0419 0083 017d  ...}.t.|.d.....}
+00004fc0: 057c 0164 0219 007d 0674 007c 0164 0319  .|.d...}.t.|.d..
+00004fd0: 0083 017d 0774 007c 0164 0419 0083 017d  ...}.t.|.d.....}
+00004fe0: 0857 006e 1401 0001 0001 0064 057d 027c  .W.n.......d.}.|
+00004ff0: 0206 0059 0053 0058 0074 017c 037c 047c  ...Y.S.X.t.|.|.|
+00005000: 057c 067c 077c 0883 067d 097c 0964 026b  .|.|.|...}.|.d.k
+00005010: 0272 a27c 037c 066b 0372 8664 067d 026e  .r.|.|.k.r.d.}.n
+00005020: 1a7c 047c 086b 0273 967c 057c 076b 0272  .|.|.k.s.|.|.k.r
+00005030: 9c64 077d 026e 0464 067d 026e b87c 0964  .d.}.n.d.}.n.|.d
+00005040: 026b 0490 0172 5a7c 047c 076b 0272 c27c  .k...rZ|.|.k.r.|
+00005050: 057c 086b 0272 c264 087d 026e 987c 047c  .|.k.r.d.}.n.|.|
+00005060: 076b 0572 d87c 057c 086b 0072 d864 097d  .k.r.|.|.k.r.d.}
+00005070: 026e 827c 047c 076b 0472 ee7c 057c 086b  .n.|.|.k.r.|.|.k
+00005080: 0172 ee64 097d 026e 6c7c 047c 076b 0490  .r.d.}.nl|.|.k..
+00005090: 0172 087c 057c 086b 0090 0172 0864 097d  .r.|.|.k...r.d.}
+000050a0: 026e 527c 047c 076b 0190 0172 227c 057c  .nR|.|.k...r"|.|
+000050b0: 086b 0490 0172 2264 0a7d 026e 387c 047c  .k...r"d.}.n8|.|
+000050c0: 076b 0090 0172 3c7c 057c 086b 0590 0172  .k...r<|.|.k...r
+000050d0: 3c64 0a7d 026e 1e7c 047c 076b 0090 0172  <d.}.n.|.|.k...r
+000050e0: 567c 057c 086b 0490 0172 5664 0a7d 026e  V|.|.k...rVd.}.n
+000050f0: 0464 0b7d 027c 0253 0029 0c61 4f01 0000  .d.}.|.S.).aO...
+00005100: 0a09 4465 7465 726d 696e 6520 7468 6520  ..Determine the 
+00005110: 7370 6174 6961 6c20 7265 6c61 7469 6f6e  spatial relation
+00005120: 7320 6f66 2067 656e 6f6d 6963 2072 6567  s of genomic reg
+00005130: 696f 6e73 2028 5352 4f47 290a 0a09 5061  ions (SROG)...Pa
+00005140: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+00005150: 2d2d 2d2d 0a09 6c73 7431 203a 2074 7570  ----..lst1 : tup
+00005160: 6c65 0a09 0941 2074 7570 6c65 206f 6620  le...A tuple of 
+00005170: 6765 6e6f 6d69 6320 696e 7465 7276 616c  genomic interval
+00005180: 2e20 4567 2e20 2827 6368 7231 272c 2031  . Eg. ('chr1', 1
+00005190: 2c20 3130 3029 2e0a 096c 7374 3220 3a20  , 100)...lst2 : 
+000051a0: 7475 706c 650a 0909 4120 7475 706c 6520  tuple...A tuple 
+000051b0: 6f66 2067 656e 6f6d 6963 2069 6e74 6572  of genomic inter
+000051c0: 7661 6c2e 2045 672e 2028 2763 6872 3127  val. Eg. ('chr1'
+000051d0: 2c20 3135 2c20 3630 292e 2e0a 0a09 5265  , 15, 60).....Re
+000051e0: 7475 726e 730a 092d 2d2d 2d2d 2d2d 0a09  turns..-------..
+000051f0: 7265 7475 726e 5f63 6f64 6520 3a20 7374  return_code : st
+00005200: 720a 0909 5265 7475 726e 206f 6e65 206f  r...Return one o
+00005210: 6620 2827 6469 736a 6f69 6e74 272c 2774  f ('disjoint','t
+00005220: 6f75 6368 272c 2765 7175 616c 272c 276f  ouch','equal','o
+00005230: 7665 726c 6170 272c 2763 6f6e 7461 696e  verlap','contain
+00005240: 272c 2777 6974 6869 6e27 292e 0a0a 09da  ','within').....
+00005250: 0072 0100 0000 720b 0000 0072 3300 0000  .r....r....r3...
+00005260: da07 756e 6b6e 6f77 6eda 0864 6973 6a6f  ..unknown..disjo
+00005270: 696e 74da 0574 6f75 6368 da05 6571 7561  int..touch..equa
+00005280: 6cda 0677 6974 6869 6eda 0763 6f6e 7461  l..within..conta
+00005290: 696e da07 6f76 6572 6c61 7029 0272 3400  in..overlap).r4.
+000052a0: 0000 7287 0000 0029 0a5a 046c 7374 315a  ..r....).Z.lst1Z
+000052b0: 046c 7374 325a 0b72 6574 7572 6e5f 636f  .lst2Z.return_co
+000052c0: 6465 5a07 6368 726f 6d5f 315a 0773 7461  deZ.chrom_1Z.sta
+000052d0: 7274 5f31 5a05 656e 645f 315a 0763 6872  rt_1Z.end_1Z.chr
+000052e0: 6f6d 5f32 5a07 7374 6172 745f 325a 0565  om_2Z.start_2Z.e
+000052f0: 6e64 5f32 5a07 6f76 5f73 697a 6572 1f00  nd_2Z.ov_sizer..
+00005300: 0000 721f 0000 0072 2000 0000 da08 7372  ..r....r .....sr
+00005310: 6f67 636f 6465 8d03 0000 7346 0000 0000  ogcode....sF....
+00005320: 1104 0102 0108 010c 010c 0108 010c 0110  ................
+00005330: 0106 0104 010a 0112 0108 0108 0106 0210  ................
+00005340: 0106 0206 010a 0110 0106 0110 0106 0110  ................
+00005350: 0106 0114 0106 0114 0106 0114 0106 0114  ................
+00005360: 0106 0204 0172 9000 0000 e980 b2e6 0e63  .....r.........c
+00005370: 0600 0000 0000 0000 0000 0000 1a00 0000  ................
+00005380: 0900 0000 4300 0000 73ea 0300 0069 007d  ....C...s....i.}
+00005390: 0674 007c 0264 0183 027d 0764 0264 0264  .t.|.d...}.d.d.d
+000053a0: 0264 0264 0264 0264 0264 039c 077d 0874  .d.d.d.d.d...}.t
+000053b0: 01a0 0264 047c 0116 00a1 0101 0074 03a0  ...d.|.......t..
+000053c0: 047c 01a1 0144 0090 015d 027d 097c 09a0  .|...D...].}.|..
+000053d0: 0564 05a1 0172 4c71 3a7c 09a0 06a1 007d  .d...rLq:|.....}
+000053e0: 0a74 077c 0a83 0164 066b 0072 7074 01a0  .t.|...d.k.rpt..
+000053f0: 0864 077c 0916 00a1 0101 0071 3a7c 0a64  .d.|.......q:|.d
+00005400: 0219 0074 097c 0a64 0819 0083 0174 097c  ...t.|.d.....t.|
+00005410: 0a64 0919 0083 0103 0002 007d 0b7d 0c7d  .d.........}.}.}
+00005420: 0d7c 0c7c 0d6b 0472 ac74 01a0 0864 0a7c  .|.|.k.r.t...d.|
+00005430: 0916 00a1 0101 0071 3a7a 0c7c 0a64 0619  .......q:z.|.d..
+00005440: 007d 0e57 006e 2c01 0001 0001 007c 0a64  .}.W.n,......|.d
+00005450: 0219 0064 0b17 007c 0a64 0819 0017 0064  ...d...|.d.....d
+00005460: 0c17 007c 0a64 0919 0017 007d 0e59 006e  ...|.d.....}.Y.n
+00005470: 0258 007a 187c 0a64 0d19 007d 0f7c 0f64  .X.z.|.d...}.|.d
+00005480: 0e6b 0772 fc64 0f7d 0f57 006e 1001 0001  .k.r.d.}.W.n....
+00005490: 0001 0064 0f7d 0f59 006e 0258 007c 0b7c  ...d.}.Y.n.X.|.|
+000054a0: 066b 0790 0172 2474 0a83 007c 067c 0b3c  .k...r$t...|.|.<
+000054b0: 007c 067c 0b19 00a0 0b74 0c7c 0c7c 0d7c  .|.|.....t.|.|.|
+000054c0: 0e7c 0f64 108d 04a1 0101 0071 3a74 01a0  .|.d.......q:t..
+000054d0: 0264 117c 0016 00a1 0101 0074 03a0 047c  .d.|.......t...|
+000054e0: 00a1 0144 0090 025d 827d 097c 09a0 0564  ...D...].}.|...d
+000054f0: 05a1 0190 0172 6e90 0171 587c 09a0 06a1  .....rn..qX|....
+00005500: 007d 0a74 077c 0a83 0164 066b 0090 0172  .}.t.|...d.k...r
+00005510: 9674 01a0 0864 077c 0916 00a1 0101 0090  .t...d.|........
+00005520: 0171 587c 0a64 0219 0074 097c 0a64 0819  .qX|.d...t.|.d..
+00005530: 0083 0174 097c 0a64 0919 0083 0103 0002  ...t.|.d........
+00005540: 007d 0b7d 0c7d 0d7c 0c7c 0d6b 0490 0172  .}.}.}.|.|.k...r
+00005550: d674 01a0 0864 127c 0916 00a1 0101 0090  .t...d.|........
+00005560: 0171 587a 0c7c 0a64 0619 007d 0e57 006e  .qXz.|.d...}.W.n
+00005570: 2c01 0001 0001 007c 0a64 0219 0064 0b17  ,......|.d...d..
+00005580: 007c 0a64 0819 0017 0064 0c17 007c 0a64  .|.d.....d...|.d
+00005590: 0919 0017 007d 0e59 006e 0258 007a 1a7c  .....}.Y.n.X.z.|
+000055a0: 0a64 0d19 007d 0f7c 0f64 0e6b 0790 0272  .d...}.|.d.k...r
+000055b0: 2864 0f7d 0f57 006e 1001 0001 0001 0064  (d.}.W.n.......d
+000055c0: 0f7d 0f59 006e 0258 007c 0b7c 066b 0790  .}.Y.n.X.|.|.k..
+000055d0: 0272 767c 0864 1305 0019 0064 0837 0003  .rv|.d.....d.7..
+000055e0: 003c 0074 0d7c 0964 1417 0064 1517 0064  .<.t.|.d...d...d
+000055f0: 1417 0064 1517 007c 0764 168d 0201 0090  ...d...|.d......
+00005600: 0171 587c 067c 0b19 00a0 0e7c 0c7c 0da1  .qX|.|.....|.|..
+00005610: 027d 1074 077c 1083 0164 026b 0290 0372  .}.t.|...d.k...r
+00005620: 527c 0864 1305 0019 0064 0837 0003 003c  R|.d.....d.7...<
+00005630: 007c 067c 0b19 006a 0f74 0c7c 0c7c 0d7c  .|.|...j.t.|.|.|
+00005640: 0f64 178d 037c 037c 0564 188d 037d 117c  .d...|.|.d...}.|
+00005650: 067c 0b19 006a 1074 0c7c 0c7c 0d7c 0f64  .|...j.t.|.|.|.d
+00005660: 178d 037c 047c 0564 188d 037d 1274 077c  ...|.|.d...}.t.|
+00005670: 1183 0164 026b 0290 0272 f464 157d 136e  ...d.k...r.d.}.n
+00005680: 0e74 117c 1164 0219 006a 1283 017d 1374  .t.|.d...j...}.t
+00005690: 077c 1283 0164 026b 0290 0372 1664 157d  .|...d.k...r.d.}
+000056a0: 146e 0e74 117c 1264 0219 006a 1283 017d  .n.t.|.d...j...}
+000056b0: 1474 0d7c 0964 1417 0064 1317 0064 1417  .t.|.d...d...d..
+000056c0: 0064 1917 007c 1317 0064 1a17 0064 1b17  .d...|...d...d..
+000056d0: 007c 1417 007c 0764 168d 0201 006e 8867  .|...|.d.....n.g
+000056e0: 007d 1567 007d 167c 1044 005d 367d 1774  .}.g.}.|.D.]6}.t
+000056f0: 137c 0b7c 0c7c 0d66 037c 0b7c 176a 147c  .|.|.|.f.|.|.j.|
+00005700: 176a 1566 0383 027d 187c 15a0 167c 18a1  .j.f...}.|...|..
+00005710: 0101 007c 16a0 167c 176a 12a1 0101 0090  ...|...|.j......
+00005720: 0371 5e74 0d7c 0964 1417 0064 1aa0 177c  .q^t.|.d...d...|
+00005730: 15a1 0117 0064 1417 0064 1aa0 177c 16a1  .....d...d...|..
+00005740: 0117 007c 0764 168d 0201 007c 1544 005d  ...|.d.....|.D.]
+00005750: 167d 197c 087c 1905 0019 0064 0837 0003  .}.|.|.....d.7..
+00005760: 003c 0090 0371 c290 0171 5874 186a 197c  .<...q...qXt.j.|
+00005770: 0864 1c8d 0153 0029 1d7a dd0a 0943 616c  .d...S.).z...Cal
+00005780: 6375 6c61 7465 7320 5352 4f47 2063 6f64  culates SROG cod
+00005790: 6520 666f 7220 6561 6368 2072 6567 696f  e for each regio
+000057a0: 6e20 696e 2069 6e62 6564 310a 0a09 5061  n in inbed1...Pa
+000057b0: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+000057c0: 2d2d 2d2d 0a09 696e 6265 6431 203a 2073  ----..inbed1 : s
+000057d0: 7472 0a09 094e 616d 6520 6f66 2061 2042  tr...Name of a B
+000057e0: 4544 2066 696c 652e 0a09 696e 6265 6432  ED file...inbed2
+000057f0: 203a 2073 7472 0a09 094e 616d 6520 6f66   : str...Name of
+00005800: 2061 6e6f 7468 6572 2042 4544 2066 696c   another BED fil
+00005810: 652e 0a09 6f75 7466 696c 6520 3a20 7374  e...outfile : st
+00005820: 720a 0909 4e61 6d65 206f 6620 6f75 7470  r...Name of outp
+00005830: 7574 2066 696c 652e 0a0a 0952 6574 7572  ut file....Retur
+00005840: 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0970 6420  ns..-------..pd 
+00005850: 5365 7269 6573 0a09 7260 0000 0072 0100  Series..r`...r..
+00005860: 0000 2907 728a 0000 0072 8f00 0000 728e  ..).r....r....r.
+00005870: 0000 0072 8d00 0000 728b 0000 0072 8c00  ...r....r....r..
+00005880: 0000 da05 6f74 6865 727a 2342 7569 6c64  ....otherz#Build
+00005890: 2069 6e74 6572 7661 6c20 7472 6565 2066   interval tree f
+000058a0: 726f 6d20 6669 6c65 3a20 2225 7322 722d  rom file: "%s"r-
+000058b0: 0000 0072 3100 0000 7a45 496e 7661 6c69  ...r1...zEInvali
+000058c0: 6420 4245 4420 6c69 6e65 2028 5265 7175  d BED line (Requ
+000058d0: 6972 6573 2061 7420 6c65 6173 7420 3320  ires at least 3 
+000058e0: 636f 6c75 6d6e 733a 2063 6872 6f6d 2c20  columns: chrom, 
+000058f0: 7374 6172 742c 2065 6e64 293a 2025 7372  start, end): %sr
+00005900: 0b00 0000 7233 0000 007a 2269 6e76 616c  ....r3...z"inval
+00005910: 6964 2042 4544 206c 696e 6520 2873 7461  id BED line (sta
+00005920: 7274 203e 2065 6e64 293a 2025 7372 6400  rt > end): %srd.
+00005930: 0000 7265 0000 00e9 0500 0000 2902 fa01  ..re........)...
+00005940: 2b72 6500 0000 7294 0000 0029 02da 0576  +re...r....)...v
+00005950: 616c 7565 da06 7374 7261 6e64 7a16 5265  alue..strandz.Re
+00005960: 6164 696e 6720 4245 4420 6669 6c65 3a20  ading BED file: 
+00005970: 2225 7322 7a22 496e 7661 6c69 6420 4245  "%s"z"Invalid BE
+00005980: 4420 6c69 6e65 2028 7374 6172 7420 3e20  D line (start > 
+00005990: 656e 6429 3a20 2573 728a 0000 0072 6100  end): %sr....ra.
+000059a0: 0000 725f 0000 0072 6200 0000 2901 7296  ..r_...rb...).r.
+000059b0: 0000 0029 025a 0d6e 756d 5f69 6e74 6572  ...).Z.num_inter
+000059c0: 7661 6c73 da08 6d61 785f 6469 7374 7a0b  vals..max_distz.
+000059d0: 5570 496e 7465 7276 616c 3d72 6b00 0000  UpInterval=rk...
+000059e0: 7a0d 446f 776e 496e 7465 7276 616c 3d29  z.DownInterval=)
+000059f0: 0172 7800 0000 291a 726f 0000 0072 1100  .rx...).ro...r..
+00005a00: 0000 7250 0000 0072 0800 0000 7210 0000  ..rP...r....r...
+00005a10: 0072 3500 0000 7236 0000 0072 0e00 0000  .r5...r6...r....
+00005a20: 7237 0000 0072 3400 0000 7207 0000 0072  r7...r4...r....r
+00005a30: 5100 0000 7206 0000 0072 7000 0000 7252  Q...r....rp...rR
+00005a40: 0000 005a 1475 7073 7472 6561 6d5f 6f66  ...Z.upstream_of
+00005a50: 5f69 6e74 6572 7661 6c5a 1664 6f77 6e73  _intervalZ.downs
+00005a60: 7472 6561 6d5f 6f66 5f69 6e74 6572 7661  tream_of_interva
+00005a70: 6c72 0f00 0000 7295 0000 0072 9000 0000  lr....r....r....
+00005a80: 721e 0000 0072 1d00 0000 7218 0000 0072  r....r....r....r
+00005a90: 7100 0000 727a 0000 0072 7b00 0000 291a  q...rz...r{...).
+00005aa0: 7224 0000 0072 2500 0000 727c 0000 005a  r$...r%...r|...Z
+00005ab0: 046e 5f75 705a 066e 5f64 6f77 6e72 9700  .n_upZ.n_downr..
+00005ac0: 0000 da04 6d61 7073 5a06 4f55 5450 5554  ....mapsZ.OUTPUT
+00005ad0: 5a0c 7372 6f67 5f73 756d 6d61 7279 723b  Z.srog_summaryr;
+00005ae0: 0000 0072 3c00 0000 721b 0000 0072 1e00  ...r<...r....r..
+00005af0: 0000 721d 0000 0072 7900 0000 5a0a 7374  ..r....ry...Z.st
+00005b00: 7261 6e64 6e65 7373 7274 0000 005a 0b75  randnessrt...Z.u
+00005b10: 705f 696e 7465 7276 616c 5a0d 646f 776e  p_intervalZ.down
+00005b20: 5f69 6e74 6572 7661 6c5a 1075 705f 696e  _intervalZ.up_in
+00005b30: 7465 7276 616c 5f6e 616d 655a 1264 6f77  terval_nameZ.dow
+00005b40: 6e5f 696e 7465 7276 616c 5f6e 616d 655a  n_interval_nameZ
+00005b50: 0a73 726f 675f 636f 6465 735a 0c74 6172  .srog_codesZ.tar
+00005b60: 6765 745f 6e61 6d65 7372 7500 0000 723d  get_namesru...r=
+00005b70: 0000 00da 0463 6f64 6572 1f00 0000 721f  .....coder....r.
+00005b80: 0000 0072 2000 0000 da09 7372 6f67 5f70  ...r .....srog_p
+00005b90: 6561 6bc6 0300 0073 9800 0000 0013 0401  eak....s........
+00005ba0: 0a01 1401 0e01 1001 0a00 0201 0801 0c01  ................
+00005bb0: 0e01 0201 2401 0801 0e01 0203 0201 0c01  ....$...........
+00005bc0: 0601 2603 0201 0801 0801 0801 0601 0a02  ..&.............
+00005bd0: 0a01 0a01 1c02 0e01 1001 0c00 0401 0801  ................
+00005be0: 0e01 0e01 0401 2401 0a01 0e01 0403 0201  ......$.........
+00005bf0: 0c01 0601 2603 0201 0801 0a01 0801 0601  ....&...........
+00005c00: 0a02 0a01 1001 1c01 0402 1001 0e01 1001  ................
+00005c10: 1e01 1e01 0e01 0602 0e01 0e01 0602 0e01  ................
+00005c20: 2e02 0401 0401 0801 1a01 0a01 1001 2801  ..............(.
+00005c30: 0801 1801 729a 0000 00da 085f 5f6d 6169  ....r......__mai
+00005c40: 6e5f 5f72 3300 0000 7231 0000 0029 0172  n__r3...r1...).r
+00005c50: 5f00 0000 2902 720b 0000 0072 7700 0000  _...).r....rw...
+00005c60: 2903 720b 0000 0072 0b00 0000 7291 0000  ).r....r....r...
+00005c70: 0029 3072 1300 0000 726d 0000 0072 1100  .)0r....rm...r..
+00005c80: 0000 5a05 6e75 6d70 7972 4700 0000 5a06  ..Z.numpyrG...Z.
+00005c90: 7061 6e64 6173 727a 0000 00da 076f 732e  pandasrz.....os.
+00005ca0: 7061 7468 7202 0000 005a 0b73 6369 7079  pathr....Z.scipy
+00005cb0: 2e73 7461 7473 7203 0000 005a 1262 782e  .statsr....Z.bx.
+00005cc0: 6269 7473 6574 5f62 7569 6c64 6572 7372  bitset_buildersr
+00005cd0: 0400 0000 7205 0000 005a 1962 782e 696e  ....r....Z.bx.in
+00005ce0: 7465 7276 616c 732e 696e 7465 7273 6563  tervals.intersec
+00005cf0: 7469 6f6e 7206 0000 0072 0700 0000 5a0d  tionr....r....Z.
+00005d00: 636f 6269 6e64 6162 696c 6974 7972 0800  cobindabilityr..
+00005d10: 0000 7209 0000 00da 0a5f 5f61 7574 686f  ..r......__autho
+00005d20: 725f 5f5a 0d5f 5f63 6f70 7972 6967 6874  r__Z.__copyright
+00005d30: 5f5f da0b 5f5f 6372 6564 6974 735f 5f5a  __..__credits__Z
+00005d40: 0b5f 5f6c 6963 656e 7365 5f5f da0b 5f5f  .__license__..__
+00005d50: 7665 7273 696f 6e5f 5f5a 0e5f 5f6d 6169  version__Z.__mai
+00005d60: 6e74 6169 6e65 725f 5f5a 095f 5f65 6d61  ntainer__Z.__ema
+00005d70: 696c 5f5f da0a 5f5f 7374 6174 7573 5f5f  il__..__status__
+00005d80: 7221 0000 0072 2900 0000 722c 0000 0072  r!...r)...r,...r
+00005d90: 3e00 0000 723f 0000 0072 4200 0000 7244  >...r?...rB...rD
+00005da0: 0000 0072 4b00 0000 722a 0000 0072 5e00  ...rK...r*...r^.
+00005db0: 0000 7276 0000 0072 8200 0000 7283 0000  ..rv...r....r...
+00005dc0: 0072 8700 0000 7290 0000 0072 9a00 0000  .r....r....r....
+00005dd0: da08 5f5f 6e61 6d65 5f5f 7238 0000 00da  ..__name__r8....
+00005de0: 0161 7270 0000 0072 1f00 0000 721f 0000  .arp...r....r...
+00005df0: 0072 1f00 0000 7220 0000 00da 083c 6d6f  .r....r .....<mo
+00005e00: 6475 6c65 3e03 0000 0073 4800 0000 1001  dule>....sH.....
+00005e10: 0801 0801 0801 0c01 0c01 1001 1001 1002  ................
+00005e20: 0401 0401 0401 0401 0601 0401 0401 0403  ................
+00005e30: 0832 084f 084c 082b 0828 0834 0832 0821  .2.O.L.+.(.4.2.!
+00005e40: 0815 0861 0a6f 0a7f 0042 0808 0821 0839  ...a.o...B...!.9
+00005e50: 0a6e 0a05 1e01                           .n....
```

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/bbreader.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/bbreader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/bw.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/bw.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/coefcal.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/coefcal.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jan 16 03:53:00 2022 UTC, .py size: 4069 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 9c96 e361 e50f 0000  U..........a....
+00000000: 550d 0d0a 0000 0000 3e4a 7962 ee0f 0000  U.......>Jyb....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6404 5a07 6405 5a08 6700  m.Z...d.Z.d.Z.g.
 00000060: 5a09 6406 5a0a 6506 6a06 5a0b 6404 5a0c  Z.d.Z.e.j.Z.d.Z.
 00000070: 6407 5a0d 6408 5a0e 6409 640a 8400 5a0f  d.Z.d.Z.d.d...Z.
@@ -21,243 +21,244 @@
 00000140: 0000 0400 0000 0500 0000 4300 0000 7366  ..........C...sf
 00000150: 0000 007c 027c 006b 0473 107c 027c 016b  ...|.|.k.s.|.|.k
 00000160: 0472 1a74 00a0 0164 01a1 0101 0074 027c  .r.t...d.....t.|
 00000170: 007c 017c 0283 0364 026b 0072 3474 00a0  .|.|...d.k.r4t..
 00000180: 0164 01a1 0101 007c 0064 026b 0273 4c7c  .d.....|.d.k.sL|
 00000190: 0164 026b 0273 4c7c 0264 026b 0272 5064  .d.k.sL|.d.k.rPd
 000001a0: 0253 007c 0274 03a0 047c 007c 0114 00a1  .S.|.t...|.|....
-000001b0: 011b 0053 0064 0353 0029 0461 0401 0000  ...S.d.S.).a....
+000001b0: 011b 0053 0064 0353 0029 0461 0c01 0000  ...S.d.S.).a....
 000001c0: 0a09 4361 6c63 756c 6174 6520 7468 6520  ..Calculate the 
-000001d0: 6f76 6572 6c61 7020 636f 6566 6669 6369  overlap coeffici
-000001e0: 656e 742e 0a0a 0950 6172 616d 6574 6572  ent....Parameter
-000001f0: 730a 092d 2d2d 2d2d 2d2d 2d2d 2d0a 0978  s..----------..x
-00000200: 203a 2069 6e74 0a09 0954 6865 2063 6172   : int...The car
-00000210: 6469 6e61 6c69 7479 206f 6620 412e 0a09  dinality of A...
-00000220: 7920 3a20 696e 740a 0909 5468 6520 6361  y : int...The ca
-00000230: 7264 696e 616c 6974 7920 6f66 2042 2e0a  rdinality of B..
-00000240: 0978 7920 3a20 696e 740a 0909 5468 6520  .xy : int...The 
-00000250: 6361 7264 696e 616c 6974 7920 6f66 2041  cardinality of A
-00000260: 2041 4e44 2042 2e0a 0967 203a 2069 6e74   AND B...g : int
-00000270: 0a09 0954 6865 2063 6172 6469 6e61 6c69  ...The cardinali
-00000280: 7479 206f 6620 6261 636b 6772 6f75 6e64  ty of background
-00000290: 2e0a 0a09 5265 7475 726e 730a 092d 2d2d  ....Returns..---
-000002a0: 2d2d 2d2d 0a09 666c 6f61 740a 0909 4f76  ----..float...Ov
-000002b0: 6572 6c61 7020 636f 6566 6669 6369 656e  erlap coefficien
-000002c0: 742e 0a09 fa13 496e 7661 6c69 6420 7061  t.....Invalid pa
-000002d0: 7261 6d65 7465 7273 2e72 0100 0000 4e29  rameters.r....N)
-000002e0: 05da 076c 6f67 6769 6e67 da05 6572 726f  ...logging..erro
-000002f0: 72da 036d 696e da04 6d61 7468 da04 7371  r..min..math..sq
-00000300: 7274 a904 da01 78da 0179 da02 7879 da01  rt....x..y..xy..
-00000310: 67a9 0072 1100 0000 fa43 2f55 7365 7273  g..r.....C/Users
-00000320: 2f6d 3130 3233 3234 2f44 6f63 756d 656e  /m102324/Documen
-00000330: 7473 2f47 6974 4875 622f 636f 6269 6e64  ts/GitHub/cobind
-00000340: 2f6c 6962 2f63 6f62 696e 6461 6269 6c69  /lib/cobindabili
-00000350: 7479 2f63 6f65 6663 616c 2e70 79da 076f  ty/coefcal.py..o
-00000360: 765f 636f 6566 1700 0000 730e 0000 0000  v_coef....s.....
-00000370: 1410 010a 0110 010a 0118 0104 0272 1300  .............r..
-00000380: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
-00000390: 0000 0004 0000 0043 0000 0073 5c00 0000  .......C...s\...
-000003a0: 7c02 7c00 6b04 7310 7c02 7c01 6b04 721a  |.|.k.s.|.|.k.r.
-000003b0: 7400 a001 6401 a101 0100 7402 7c00 7c01  t...d.....t.|.|.
-000003c0: 7c02 8303 6402 6b00 7234 7400 a001 6401  |...d.k.r4t...d.
-000003d0: a101 0100 7c00 6402 6b02 7344 7c01 6402  ....|.d.k.sD|.d.
-000003e0: 6b02 7248 6402 5300 7c02 7c00 7c01 1700  k.rHd.S.|.|.|...
-000003f0: 7c02 1800 1b00 5300 6403 5300 2904 6134  |.....S.d.S.).a4
-00000400: 0100 000a 0943 616c 6375 6c61 7465 2074  .....Calculate t
-00000410: 6865 204a 6163 6361 7264 2773 2063 6f65  he Jaccard's coe
-00000420: 6666 6963 6965 6e74 2028 6874 7470 733a  fficient (https:
-00000430: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00000440: 7267 2f77 696b 692f 4a61 6363 6172 645f  rg/wiki/Jaccard_
-00000450: 696e 6465 7829 2e0a 0a09 5061 7261 6d65  index)....Parame
-00000460: 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d  ters..----------
-00000470: 0a09 7820 3a20 696e 740a 0909 5468 6520  ..x : int...The 
-00000480: 6361 7264 696e 616c 6974 7920 6f66 2041  cardinality of A
-00000490: 2e0a 0979 203a 2069 6e74 0a09 0954 6865  ...y : int...The
-000004a0: 2063 6172 6469 6e61 6c69 7479 206f 6620   cardinality of 
-000004b0: 422e 0a09 7879 203a 2069 6e74 0a09 0954  B...xy : int...T
-000004c0: 6865 2063 6172 6469 6e61 6c69 7479 206f  he cardinality o
-000004d0: 6620 4120 414e 4420 422e 0a09 6720 3a20  f A AND B...g : 
-000004e0: 696e 740a 0909 5468 6520 6361 7264 696e  int...The cardin
-000004f0: 616c 6974 7920 6f66 2062 6163 6b67 726f  ality of backgro
-00000500: 756e 642e 0a0a 0952 6574 7572 6e73 0a09  und....Returns..
-00000510: 2d2d 2d2d 2d2d 2d0a 0966 6c6f 6174 0a09  -------..float..
-00000520: 094f 7665 726c 6170 2063 6f65 6666 6963  .Overlap coeffic
-00000530: 6965 6e74 2e0a 0972 0600 0000 7201 0000  ient...r....r...
-00000540: 004e a903 7207 0000 0072 0800 0000 7209  .N..r....r....r.
-00000550: 0000 0072 0c00 0000 7211 0000 0072 1100  ...r....r....r..
-00000560: 0000 7212 0000 00da 0a6f 765f 6a61 6363  ..r......ov_jacc
-00000570: 6172 6434 0000 0073 0e00 0000 0014 1001  ard4...s........
-00000580: 0a01 1001 0a01 1001 0402 7215 0000 0063  ..........r....c
-00000590: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-000005a0: 0400 0000 4300 0000 735a 0000 007c 027c  ....C...sZ...|.|
-000005b0: 006b 0473 107c 027c 016b 0472 1a74 00a0  .k.s.|.|.k.r.t..
-000005c0: 0164 01a1 0101 0074 027c 007c 017c 0283  .d.....t.|.|.|..
-000005d0: 0364 026b 0072 3474 00a0 0164 01a1 0101  .d.k.r4t...d....
-000005e0: 007c 0064 026b 0273 447c 0164 026b 0272  .|.d.k.sD|.d.k.r
-000005f0: 4864 0253 007c 0274 027c 007c 0183 021b  Hd.S.|.t.|.|....
-00000600: 0053 0064 0353 0029 0475 5501 0000 0a09  .S.d.S.).uU.....
-00000610: 4361 6c63 756c 6174 6520 7468 6520 537a  Calculate the Sz
-00000620: 796d 6b69 6577 6963 7ae2 8093 5369 6d70  ymkiewicz...Simp
-00000630: 736f 6e20 636f 6566 6669 6369 656e 742c  son coefficient,
-00000640: 2028 6874 7470 733a 2f2f 656e 2e77 696b   (https://en.wik
-00000650: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
-00000660: 4f76 6572 6c61 705f 636f 6566 6669 6369  Overlap_coeffici
-00000670: 656e 7429 2e0a 0a09 5061 7261 6d65 7465  ent)....Paramete
-00000680: 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09  rs..----------..
-00000690: 7820 3a20 696e 740a 0909 5468 6520 6361  x : int...The ca
-000006a0: 7264 696e 616c 6974 7920 6f66 2041 2e0a  rdinality of A..
-000006b0: 0979 203a 2069 6e74 0a09 0954 6865 2063  .y : int...The c
-000006c0: 6172 6469 6e61 6c69 7479 206f 6620 422e  ardinality of B.
-000006d0: 0a09 7879 203a 2069 6e74 0a09 0954 6865  ..xy : int...The
-000006e0: 2063 6172 6469 6e61 6c69 7479 206f 6620   cardinality of 
-000006f0: 4120 414e 4420 422e 0a09 6720 3a20 696e  A AND B...g : in
-00000700: 740a 0909 5468 6520 6361 7264 696e 616c  t...The cardinal
-00000710: 6974 7920 6f66 2062 6163 6b67 726f 756e  ity of backgroun
-00000720: 642e 0a0a 0952 6574 7572 6e73 0a09 2d2d  d....Returns..--
-00000730: 2d2d 2d2d 2d0a 0966 6c6f 6174 0a09 0953  -----..float...S
-00000740: 7a79 6d6b 6965 7769 637a e280 9353 696d  zymkiewicz...Sim
-00000750: 7073 6f6e 2063 6f65 6666 6963 6965 6e74  pson coefficient
-00000760: 2e0a 0972 0600 0000 7201 0000 004e 7214  ...r....r....Nr.
-00000770: 0000 0072 0c00 0000 7211 0000 0072 1100  ...r....r....r..
-00000780: 0000 7212 0000 00da 056f 765f 7373 5100  ..r......ov_ssQ.
-00000790: 0000 730e 0000 0000 1410 010a 0110 010a  ..s.............
-000007a0: 0110 0104 0272 1600 0000 6304 0000 0000  .....r....c.....
-000007b0: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-000007c0: 0000 0073 5c00 0000 7c02 7c00 6b04 7310  ...s\...|.|.k.s.
-000007d0: 7c02 7c01 6b04 721a 7400 a001 6401 a101  |.|.k.r.t...d...
-000007e0: 0100 7402 7c00 7c01 7c02 8303 6402 6b00  ..t.|.|.|...d.k.
-000007f0: 7234 7400 a001 6401 a101 0100 7c00 6402  r4t...d.....|.d.
-00000800: 6b02 7344 7c01 6402 6b02 7248 6402 5300  k.sD|.d.k.rHd.S.
-00000810: 6403 7c02 1400 7c00 7c01 1700 1b00 5300  d.|...|.|.....S.
-00000820: 6404 5300 2905 75b9 0100 000a 0943 616c  d.S.).u......Cal
-00000830: 6375 6c61 7465 2074 6865 2053 c3b8 7265  culate the S..re
-00000840: 6e73 656e e280 9344 6963 6520 636f 6566  nsen...Dice coef
-00000850: 6669 6369 656e 7420 2868 7474 7073 3a2f  ficient (https:/
-00000860: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00000870: 672f 7769 6b69 2f53 c3b8 7265 6e73 656e  g/wiki/S..rensen
-00000880: e280 9344 6963 655f 636f 6566 6669 6369  ...Dice_coeffici
-00000890: 656e 7429 2e0a 0953 c3b8 7265 6e73 656e  ent)...S..rensen
-000008a0: e280 9344 6963 6520 636f 6566 6669 6369  ...Dice coeffici
-000008b0: 656e 7420 616c 736f 2063 616c 6c65 6420  ent also called 
-000008c0: 2253 c3b8 7265 6e73 656e e280 9344 6963  "S..rensen...Dic
-000008d0: 6520 696e 6465 7822 2c20 2253 c3b8 7265  e index", "S..re
-000008e0: 6e73 656e 2069 6e64 6578 2220 6f72 2022  nsen index" or "
-000008f0: 4469 6365 2773 2063 6f65 6666 6963 6965  Dice's coefficie
-00000900: 6e74 222e 0a0a 0950 6172 616d 6574 6572  nt"....Parameter
-00000910: 730a 092d 2d2d 2d2d 2d2d 2d2d 2d0a 0978  s..----------..x
-00000920: 203a 2069 6e74 0a09 0954 6865 2063 6172   : int...The car
-00000930: 6469 6e61 6c69 7479 206f 6620 412e 0a09  dinality of A...
-00000940: 7920 3a20 696e 740a 0909 5468 6520 6361  y : int...The ca
-00000950: 7264 696e 616c 6974 7920 6f66 2042 2e0a  rdinality of B..
-00000960: 0978 7920 3a20 696e 740a 0909 5468 6520  .xy : int...The 
-00000970: 6361 7264 696e 616c 6974 7920 6f66 2041  cardinality of A
-00000980: 2041 4e44 2042 2e0a 0967 203a 2069 6e74   AND B...g : int
-00000990: 0a09 0954 6865 2063 6172 6469 6e61 6c69  ...The cardinali
-000009a0: 7479 206f 6620 6261 636b 6772 6f75 6e64  ty of background
-000009b0: 2e0a 0a09 5265 7475 726e 730a 092d 2d2d  ....Returns..---
-000009c0: 2d2d 2d2d 0a09 666c 6f61 740a 0909 4f76  ----..float...Ov
-000009d0: 6572 6c61 7020 636f 6566 6669 6369 656e  erlap coefficien
-000009e0: 742e 0a09 7206 0000 0072 0100 0000 e902  t...r....r......
-000009f0: 0000 004e 7214 0000 0072 0c00 0000 7211  ...Nr....r....r.
-00000a00: 0000 0072 1100 0000 7212 0000 00da 056f  ...r....r......o
-00000a10: 765f 7364 6e00 0000 730e 0000 0000 1510  v_sdn...s.......
-00000a20: 010a 0110 010a 0110 0104 0272 1800 0000  ...........r....
-00000a30: 6304 0000 0000 0000 0000 0000 0007 0000  c...............
-00000a40: 0004 0000 0043 0000 0073 aa00 0000 7c03  .....C...s....|.
-00000a50: 6401 6b01 7212 7400 a001 6402 a101 0100  d.k.r.t...d.....
-00000a60: 7c02 7c00 6b04 7322 7c02 7c01 6b04 722c  |.|.k.s"|.|.k.r,
-00000a70: 7400 a001 6403 a101 0100 7c00 7c03 6b04  t...d.....|.|.k.
-00000a80: 733c 7c01 7c03 6b04 7246 7400 a001 6403  s<|.|.k.rFt...d.
-00000a90: a101 0100 7402 7c00 7c01 7c02 8303 6401  ....t.|.|.|...d.
-00000aa0: 6b00 7260 7400 a001 6403 a101 0100 7c00  k.r`t...d.....|.
-00000ab0: 7c03 1b00 7d04 7c01 7c03 1b00 7d05 7c02  |...}.|.|...}.|.
-00000ac0: 7c03 1b00 7d06 7c06 6401 6b02 7288 7403  |...}.|.d.k.r.t.
-00000ad0: 6a04 0b00 5300 7403 a005 7c06 a101 7403  j...S.t...|...t.
-00000ae0: a005 7c04 a101 1800 7403 a005 7c05 a101  ..|.....t...|...
-00000af0: 1800 5300 6404 5300 2905 611d 0100 000a  ..S.d.S.).a.....
-00000b00: 0943 616c 6375 6c61 7465 2074 6865 2070  .Calculate the p
-00000b10: 6f69 6e74 7769 7365 206d 7574 7561 6c20  ointwise mutual 
-00000b20: 696e 666f 726d 6174 696f 6e20 2850 4d49  information (PMI
-00000b30: 292e 0a0a 0950 6172 616d 6574 6572 730a  )....Parameters.
-00000b40: 092d 2d2d 2d2d 2d2d 2d2d 2d0a 0978 203a  .----------..x :
-00000b50: 2069 6e74 0a09 0954 6865 2063 6172 6469   int...The cardi
-00000b60: 6e61 6c69 7479 206f 6620 412e 0a09 7920  nality of A...y 
-00000b70: 3a20 696e 740a 0909 5468 6520 6361 7264  : int...The card
-00000b80: 696e 616c 6974 7920 6f66 2042 2e0a 0978  inality of B...x
-00000b90: 7920 3a20 696e 740a 0909 5468 6520 6361  y : int...The ca
-00000ba0: 7264 696e 616c 6974 7920 6f66 2041 2041  rdinality of A A
-00000bb0: 4e44 2042 2e0a 0967 203a 2069 6e74 0a09  ND B...g : int..
-00000bc0: 0954 6865 2063 6172 6469 6e61 6c69 7479  .The cardinality
-00000bd0: 206f 6620 6261 636b 6772 6f75 6e64 2e0a   of background..
-00000be0: 0a09 5265 7475 726e 730a 092d 2d2d 2d2d  ..Returns..-----
-00000bf0: 2d2d 0a09 666c 6f61 740a 0909 506f 696e  --..float...Poin
-00000c00: 7477 6973 6520 6d75 7475 7461 6c20 696e  twise mututal in
-00000c10: 666f 726d 6174 696f 6e2e 0a09 7201 0000  formation...r...
-00000c20: 00fa 3854 6865 2063 6172 6469 6e61 6c69  ..8The cardinali
-00000c30: 7479 206f 6620 6261 636b 6772 6f75 6e64  ty of background
-00000c40: 206d 7573 7420 6265 2061 2070 6f73 7469   must be a posti
-00000c50: 7665 2069 6e74 6567 6572 2e72 0600 0000  ve integer.r....
-00000c60: 4e29 0672 0700 0000 7208 0000 0072 0900  N).r....r....r..
-00000c70: 0000 da02 6e70 da03 696e 66da 036c 6f67  ....np..inf..log
-00000c80: a907 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000c90: 0072 1000 0000 da02 7078 da02 7079 5a03  .r......px..pyZ.
-00000ca0: 7078 7972 1100 0000 7211 0000 0072 1200  pxyr....r....r..
-00000cb0: 0000 da09 706d 695f 7661 6c75 658d 0000  ....pmi_value...
-00000cc0: 0073 1c00 0000 0014 0801 0a01 1001 0a01  .s..............
-00000cd0: 1001 0a01 1001 0a01 0801 0801 0801 0801  ................
-00000ce0: 0802 7220 0000 0063 0400 0000 0000 0000  ..r ...c........
-00000cf0: 0000 0000 0700 0000 0400 0000 4300 0000  ............C...
-00000d00: 73a4 0000 007c 0364 016b 0172 1274 00a0  s....|.d.k.r.t..
-00000d10: 0164 02a1 0101 007c 027c 006b 0473 227c  .d.....|.|.k.s"|
-00000d20: 027c 016b 0472 2c74 00a0 0164 03a1 0101  .|.k.r,t...d....
-00000d30: 007c 007c 036b 0473 3c7c 017c 036b 0472  .|.|.k.s<|.|.k.r
-00000d40: 4674 00a0 0164 03a1 0101 0074 027c 007c  Ft...d.....t.|.|
-00000d50: 017c 0283 0364 016b 0072 6074 00a0 0164  .|...d.k.r`t...d
-00000d60: 03a1 0101 007c 007c 031b 007d 047c 017c  .....|.|...}.|.|
-00000d70: 031b 007d 057c 027c 031b 007d 067c 0664  ...}.|.|...}.|.d
-00000d80: 016b 0272 8464 0453 0074 03a0 047c 047c  .k.r.d.S.t...|.|
-00000d90: 0514 00a1 0174 03a0 047c 06a1 011b 0064  .....t...|.....d
-00000da0: 0518 0053 0064 0653 0029 0761 3301 0000  ...S.d.S.).a3...
-00000db0: 0a09 4361 6c63 756c 6174 6520 7468 6520  ..Calculate the 
-00000dc0: 6e6f 726d 616c 697a 6564 2070 6f69 6e74  normalized point
-00000dd0: 7769 7365 206d 7574 7561 6c20 696e 666f  wise mutual info
-00000de0: 726d 6174 696f 6e20 284e 504d 4929 2e0a  rmation (NPMI)..
-00000df0: 0a09 5061 7261 6d65 7465 7273 0a09 2d2d  ..Parameters..--
-00000e00: 2d2d 2d2d 2d2d 2d2d 0a09 7820 3a20 696e  --------..x : in
-00000e10: 740a 0909 5468 6520 6361 7264 696e 616c  t...The cardinal
-00000e20: 6974 7920 6f66 2041 2e0a 0979 203a 2069  ity of A...y : i
-00000e30: 6e74 0a09 0954 6865 2063 6172 6469 6e61  nt...The cardina
-00000e40: 6c69 7479 206f 6620 422e 0a09 7879 203a  lity of B...xy :
-00000e50: 2069 6e74 0a09 0954 6865 2063 6172 6469   int...The cardi
-00000e60: 6e61 6c69 7479 206f 6620 4120 414e 4420  nality of A AND 
-00000e70: 422e 0a09 6720 3a20 696e 740a 0909 5468  B...g : int...Th
-00000e80: 6520 6361 7264 696e 616c 6974 7920 6f66  e cardinality of
-00000e90: 2062 6163 6b67 726f 756e 642e 0a0a 0952   background....R
-00000ea0: 6574 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a  eturns..-------.
-00000eb0: 0966 6c6f 6174 0a09 094e 6f72 6d61 6c69  .float...Normali
-00000ec0: 7a65 6420 706f 696e 7477 6973 6520 6d75  zed pointwise mu
-00000ed0: 7475 616c 2069 6e66 6f72 6d61 7469 6f6e  tual information
-00000ee0: 2e0a 0972 0100 0000 7219 0000 0072 0600  ...r....r....r..
-00000ef0: 0000 e9ff ffff ffe9 0100 0000 4e29 0572  ............N).r
-00000f00: 0700 0000 7208 0000 0072 0900 0000 721a  ....r....r....r.
-00000f10: 0000 0072 1c00 0000 721d 0000 0072 1100  ...r....r....r..
-00000f20: 0000 7211 0000 0072 1200 0000 da0a 6e70  ..r....r......np
-00000f30: 6d69 5f76 616c 7565 b100 0000 731c 0000  mi_value....s...
-00000f40: 0000 1408 010a 0110 010a 0110 010a 0110  ................
-00000f50: 010a 0108 0108 0108 0108 0104 0272 2300  .............r#.
-00000f60: 0000 2915 da07 5f5f 646f 635f 5f72 0a00  ..)...__doc__r..
-00000f70: 0000 7207 0000 00da 056e 756d 7079 721a  ..r......numpyr.
-00000f80: 0000 00da 0d63 6f62 696e 6461 6269 6c69  .....cobindabili
-00000f90: 7479 7202 0000 00da 0a5f 5f61 7574 686f  tyr......__autho
-00000fa0: 725f 5fda 0d5f 5f63 6f70 7972 6967 6874  r__..__copyright
-00000fb0: 5f5f da0b 5f5f 6372 6564 6974 735f 5fda  __..__credits__.
-00000fc0: 0b5f 5f6c 6963 656e 7365 5f5f da0b 5f5f  .__license__..__
-00000fd0: 7665 7273 696f 6e5f 5fda 0e5f 5f6d 6169  version__..__mai
-00000fe0: 6e74 6169 6e65 725f 5fda 095f 5f65 6d61  ntainer__..__ema
-00000ff0: 696c 5f5f da0a 5f5f 7374 6174 7573 5f5f  il__..__status__
-00001000: 7213 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00001010: 1800 0000 7220 0000 0072 2300 0000 7211  ....r ...r#...r.
-00001020: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001030: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
-00001040: 7324 0000 0004 0508 0108 0108 010c 0304  s$..............
-00001050: 0104 0104 0104 0106 0104 0104 0104 0208  ................
-00001060: 1d08 1d08 1d08 1f08 24                   ........$
+000001d0: 636f 6c6c 6f63 6174 696f 6e20 636f 6566  collocation coef
+000001e0: 6669 6369 656e 742e 0a0a 0950 6172 616d  ficient....Param
+000001f0: 6574 6572 730a 092d 2d2d 2d2d 2d2d 2d2d  eters..---------
+00000200: 2d0a 0978 203a 2069 6e74 0a09 0954 6865  -..x : int...The
+00000210: 2063 6172 6469 6e61 6c69 7479 206f 6620   cardinality of 
+00000220: 412e 0a09 7920 3a20 696e 740a 0909 5468  A...y : int...Th
+00000230: 6520 6361 7264 696e 616c 6974 7920 6f66  e cardinality of
+00000240: 2042 2e0a 0978 7920 3a20 696e 740a 0909   B...xy : int...
+00000250: 5468 6520 6361 7264 696e 616c 6974 7920  The cardinality 
+00000260: 6f66 2041 2041 4e44 2042 2e0a 0967 203a  of A AND B...g :
+00000270: 2069 6e74 0a09 0954 6865 2063 6172 6469   int...The cardi
+00000280: 6e61 6c69 7479 206f 6620 6261 636b 6772  nality of backgr
+00000290: 6f75 6e64 2e0a 0a09 5265 7475 726e 730a  ound....Returns.
+000002a0: 092d 2d2d 2d2d 2d2d 0a09 666c 6f61 740a  .-------..float.
+000002b0: 0909 436f 6c6c 6f63 6174 696f 6e20 636f  ..Collocation co
+000002c0: 6566 6669 6369 656e 742e 0a09 fa13 496e  efficient.....In
+000002d0: 7661 6c69 6420 7061 7261 6d65 7465 7273  valid parameters
+000002e0: 2e72 0100 0000 4e29 05da 076c 6f67 6769  .r....N)...loggi
+000002f0: 6e67 da05 6572 726f 72da 036d 696e da04  ng..error..min..
+00000300: 6d61 7468 da04 7371 7274 a904 da01 78da  math..sqrt....x.
+00000310: 0179 da02 7879 da01 67a9 0072 1100 0000  .y..xy..g..r....
+00000320: fa43 2f55 7365 7273 2f6d 3130 3233 3234  .C/Users/m102324
+00000330: 2f44 6f63 756d 656e 7473 2f47 6974 4875  /Documents/GitHu
+00000340: 622f 636f 6269 6e64 2f6c 6962 2f63 6f62  b/cobind/lib/cob
+00000350: 696e 6461 6269 6c69 7479 2f63 6f65 6663  indability/coefc
+00000360: 616c 2e70 79da 076f 765f 636f 6566 1700  al.py..ov_coef..
+00000370: 0000 730e 0000 0000 1410 010a 0110 010a  ..s.............
+00000380: 0118 0104 0272 1300 0000 6304 0000 0000  .....r....c.....
+00000390: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
+000003a0: 0000 0073 5c00 0000 7c02 7c00 6b04 7310  ...s\...|.|.k.s.
+000003b0: 7c02 7c01 6b04 721a 7400 a001 6401 a101  |.|.k.r.t...d...
+000003c0: 0100 7402 7c00 7c01 7c02 8303 6402 6b00  ..t.|.|.|...d.k.
+000003d0: 7234 7400 a001 6401 a101 0100 7c00 6402  r4t...d.....|.d.
+000003e0: 6b02 7344 7c01 6402 6b02 7248 6402 5300  k.sD|.d.k.rHd.S.
+000003f0: 7c02 7c00 7c01 1700 7c02 1800 1b00 5300  |.|.|...|.....S.
+00000400: 6403 5300 2904 6134 0100 000a 0943 616c  d.S.).a4.....Cal
+00000410: 6375 6c61 7465 2074 6865 204a 6163 6361  culate the Jacca
+00000420: 7264 2773 2063 6f65 6666 6963 6965 6e74  rd's coefficient
+00000430: 2028 6874 7470 733a 2f2f 656e 2e77 696b   (https://en.wik
+00000440: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+00000450: 4a61 6363 6172 645f 696e 6465 7829 2e0a  Jaccard_index)..
+00000460: 0a09 5061 7261 6d65 7465 7273 0a09 2d2d  ..Parameters..--
+00000470: 2d2d 2d2d 2d2d 2d2d 0a09 7820 3a20 696e  --------..x : in
+00000480: 740a 0909 5468 6520 6361 7264 696e 616c  t...The cardinal
+00000490: 6974 7920 6f66 2041 2e0a 0979 203a 2069  ity of A...y : i
+000004a0: 6e74 0a09 0954 6865 2063 6172 6469 6e61  nt...The cardina
+000004b0: 6c69 7479 206f 6620 422e 0a09 7879 203a  lity of B...xy :
+000004c0: 2069 6e74 0a09 0954 6865 2063 6172 6469   int...The cardi
+000004d0: 6e61 6c69 7479 206f 6620 4120 414e 4420  nality of A AND 
+000004e0: 422e 0a09 6720 3a20 696e 740a 0909 5468  B...g : int...Th
+000004f0: 6520 6361 7264 696e 616c 6974 7920 6f66  e cardinality of
+00000500: 2062 6163 6b67 726f 756e 642e 0a0a 0952   background....R
+00000510: 6574 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a  eturns..-------.
+00000520: 0966 6c6f 6174 0a09 094f 7665 726c 6170  .float...Overlap
+00000530: 2063 6f65 6666 6963 6965 6e74 2e0a 0972   coefficient...r
+00000540: 0600 0000 7201 0000 004e a903 7207 0000  ....r....N..r...
+00000550: 0072 0800 0000 7209 0000 0072 0c00 0000  .r....r....r....
+00000560: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000570: 0a6f 765f 6a61 6363 6172 6434 0000 0073  .ov_jaccard4...s
+00000580: 0e00 0000 0014 1001 0a01 1001 0a01 1001  ................
+00000590: 0402 7215 0000 0063 0400 0000 0000 0000  ..r....c........
+000005a0: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+000005b0: 735a 0000 007c 027c 006b 0473 107c 027c  sZ...|.|.k.s.|.|
+000005c0: 016b 0472 1a74 00a0 0164 01a1 0101 0074  .k.r.t...d.....t
+000005d0: 027c 007c 017c 0283 0364 026b 0072 3474  .|.|.|...d.k.r4t
+000005e0: 00a0 0164 01a1 0101 007c 0064 026b 0273  ...d.....|.d.k.s
+000005f0: 447c 0164 026b 0272 4864 0253 007c 0274  D|.d.k.rHd.S.|.t
+00000600: 027c 007c 0183 021b 0053 0064 0353 0029  .|.|.....S.d.S.)
+00000610: 0475 5501 0000 0a09 4361 6c63 756c 6174  .uU.....Calculat
+00000620: 6520 7468 6520 537a 796d 6b69 6577 6963  e the Szymkiewic
+00000630: 7ae2 8093 5369 6d70 736f 6e20 636f 6566  z...Simpson coef
+00000640: 6669 6369 656e 742c 2028 6874 7470 733a  ficient, (https:
+00000650: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00000660: 7267 2f77 696b 692f 4f76 6572 6c61 705f  rg/wiki/Overlap_
+00000670: 636f 6566 6669 6369 656e 7429 2e0a 0a09  coefficient)....
+00000680: 5061 7261 6d65 7465 7273 0a09 2d2d 2d2d  Parameters..----
+00000690: 2d2d 2d2d 2d2d 0a09 7820 3a20 696e 740a  ------..x : int.
+000006a0: 0909 5468 6520 6361 7264 696e 616c 6974  ..The cardinalit
+000006b0: 7920 6f66 2041 2e0a 0979 203a 2069 6e74  y of A...y : int
+000006c0: 0a09 0954 6865 2063 6172 6469 6e61 6c69  ...The cardinali
+000006d0: 7479 206f 6620 422e 0a09 7879 203a 2069  ty of B...xy : i
+000006e0: 6e74 0a09 0954 6865 2063 6172 6469 6e61  nt...The cardina
+000006f0: 6c69 7479 206f 6620 4120 414e 4420 422e  lity of A AND B.
+00000700: 0a09 6720 3a20 696e 740a 0909 5468 6520  ..g : int...The 
+00000710: 6361 7264 696e 616c 6974 7920 6f66 2062  cardinality of b
+00000720: 6163 6b67 726f 756e 642e 0a0a 0952 6574  ackground....Ret
+00000730: 7572 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0966  urns..-------..f
+00000740: 6c6f 6174 0a09 0953 7a79 6d6b 6965 7769  loat...Szymkiewi
+00000750: 637a e280 9353 696d 7073 6f6e 2063 6f65  cz...Simpson coe
+00000760: 6666 6963 6965 6e74 2e0a 0972 0600 0000  fficient...r....
+00000770: 7201 0000 004e 7214 0000 0072 0c00 0000  r....Nr....r....
+00000780: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000790: 056f 765f 7373 5100 0000 730e 0000 0000  .ov_ssQ...s.....
+000007a0: 1410 010a 0110 010a 0110 0104 0272 1600  .............r..
+000007b0: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
+000007c0: 0000 0004 0000 0043 0000 0073 5c00 0000  .......C...s\...
+000007d0: 7c02 7c00 6b04 7310 7c02 7c01 6b04 721a  |.|.k.s.|.|.k.r.
+000007e0: 7400 a001 6401 a101 0100 7402 7c00 7c01  t...d.....t.|.|.
+000007f0: 7c02 8303 6402 6b00 7234 7400 a001 6401  |...d.k.r4t...d.
+00000800: a101 0100 7c00 6402 6b02 7344 7c01 6402  ....|.d.k.sD|.d.
+00000810: 6b02 7248 6402 5300 6403 7c02 1400 7c00  k.rHd.S.d.|...|.
+00000820: 7c01 1700 1b00 5300 6404 5300 2905 75b9  |.....S.d.S.).u.
+00000830: 0100 000a 0943 616c 6375 6c61 7465 2074  .....Calculate t
+00000840: 6865 2053 c3b8 7265 6e73 656e e280 9344  he S..rensen...D
+00000850: 6963 6520 636f 6566 6669 6369 656e 7420  ice coefficient 
+00000860: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+00000870: 7065 6469 612e 6f72 672f 7769 6b69 2f53  pedia.org/wiki/S
+00000880: c3b8 7265 6e73 656e e280 9344 6963 655f  ..rensen...Dice_
+00000890: 636f 6566 6669 6369 656e 7429 2e0a 0953  coefficient)...S
+000008a0: c3b8 7265 6e73 656e e280 9344 6963 6520  ..rensen...Dice 
+000008b0: 636f 6566 6669 6369 656e 7420 616c 736f  coefficient also
+000008c0: 2063 616c 6c65 6420 2253 c3b8 7265 6e73   called "S..rens
+000008d0: 656e e280 9344 6963 6520 696e 6465 7822  en...Dice index"
+000008e0: 2c20 2253 c3b8 7265 6e73 656e 2069 6e64  , "S..rensen ind
+000008f0: 6578 2220 6f72 2022 4469 6365 2773 2063  ex" or "Dice's c
+00000900: 6f65 6666 6963 6965 6e74 222e 0a0a 0950  oefficient"....P
+00000910: 6172 616d 6574 6572 730a 092d 2d2d 2d2d  arameters..-----
+00000920: 2d2d 2d2d 2d0a 0978 203a 2069 6e74 0a09  -----..x : int..
+00000930: 0954 6865 2063 6172 6469 6e61 6c69 7479  .The cardinality
+00000940: 206f 6620 412e 0a09 7920 3a20 696e 740a   of A...y : int.
+00000950: 0909 5468 6520 6361 7264 696e 616c 6974  ..The cardinalit
+00000960: 7920 6f66 2042 2e0a 0978 7920 3a20 696e  y of B...xy : in
+00000970: 740a 0909 5468 6520 6361 7264 696e 616c  t...The cardinal
+00000980: 6974 7920 6f66 2041 2041 4e44 2042 2e0a  ity of A AND B..
+00000990: 0967 203a 2069 6e74 0a09 0954 6865 2063  .g : int...The c
+000009a0: 6172 6469 6e61 6c69 7479 206f 6620 6261  ardinality of ba
+000009b0: 636b 6772 6f75 6e64 2e0a 0a09 5265 7475  ckground....Retu
+000009c0: 726e 730a 092d 2d2d 2d2d 2d2d 0a09 666c  rns..-------..fl
+000009d0: 6f61 740a 0909 4f76 6572 6c61 7020 636f  oat...Overlap co
+000009e0: 6566 6669 6369 656e 742e 0a09 7206 0000  efficient...r...
+000009f0: 0072 0100 0000 e902 0000 004e 7214 0000  .r.........Nr...
+00000a00: 0072 0c00 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000a10: 7212 0000 00da 056f 765f 7364 6e00 0000  r......ov_sdn...
+00000a20: 730e 0000 0000 1510 010a 0110 010a 0110  s...............
+00000a30: 0104 0272 1800 0000 6304 0000 0000 0000  ...r....c.......
+00000a40: 0000 0000 0007 0000 0004 0000 0043 0000  .............C..
+00000a50: 0073 aa00 0000 7c03 6401 6b01 7212 7400  .s....|.d.k.r.t.
+00000a60: a001 6402 a101 0100 7c02 7c00 6b04 7322  ..d.....|.|.k.s"
+00000a70: 7c02 7c01 6b04 722c 7400 a001 6403 a101  |.|.k.r,t...d...
+00000a80: 0100 7c00 7c03 6b04 733c 7c01 7c03 6b04  ..|.|.k.s<|.|.k.
+00000a90: 7246 7400 a001 6403 a101 0100 7402 7c00  rFt...d.....t.|.
+00000aa0: 7c01 7c02 8303 6401 6b00 7260 7400 a001  |.|...d.k.r`t...
+00000ab0: 6403 a101 0100 7c00 7c03 1b00 7d04 7c01  d.....|.|...}.|.
+00000ac0: 7c03 1b00 7d05 7c02 7c03 1b00 7d06 7c06  |...}.|.|...}.|.
+00000ad0: 6401 6b02 7288 7403 6a04 0b00 5300 7403  d.k.r.t.j...S.t.
+00000ae0: a005 7c06 a101 7403 a005 7c04 a101 1800  ..|...t...|.....
+00000af0: 7403 a005 7c05 a101 1800 5300 6404 5300  t...|.....S.d.S.
+00000b00: 2905 611d 0100 000a 0943 616c 6375 6c61  ).a......Calcula
+00000b10: 7465 2074 6865 2070 6f69 6e74 7769 7365  te the pointwise
+00000b20: 206d 7574 7561 6c20 696e 666f 726d 6174   mutual informat
+00000b30: 696f 6e20 2850 4d49 292e 0a0a 0950 6172  ion (PMI)....Par
+00000b40: 616d 6574 6572 730a 092d 2d2d 2d2d 2d2d  ameters..-------
+00000b50: 2d2d 2d0a 0978 203a 2069 6e74 0a09 0954  ---..x : int...T
+00000b60: 6865 2063 6172 6469 6e61 6c69 7479 206f  he cardinality o
+00000b70: 6620 412e 0a09 7920 3a20 696e 740a 0909  f A...y : int...
+00000b80: 5468 6520 6361 7264 696e 616c 6974 7920  The cardinality 
+00000b90: 6f66 2042 2e0a 0978 7920 3a20 696e 740a  of B...xy : int.
+00000ba0: 0909 5468 6520 6361 7264 696e 616c 6974  ..The cardinalit
+00000bb0: 7920 6f66 2041 2041 4e44 2042 2e0a 0967  y of A AND B...g
+00000bc0: 203a 2069 6e74 0a09 0954 6865 2063 6172   : int...The car
+00000bd0: 6469 6e61 6c69 7479 206f 6620 6261 636b  dinality of back
+00000be0: 6772 6f75 6e64 2e0a 0a09 5265 7475 726e  ground....Return
+00000bf0: 730a 092d 2d2d 2d2d 2d2d 0a09 666c 6f61  s..-------..floa
+00000c00: 740a 0909 506f 696e 7477 6973 6520 6d75  t...Pointwise mu
+00000c10: 7475 7461 6c20 696e 666f 726d 6174 696f  tutal informatio
+00000c20: 6e2e 0a09 7201 0000 00fa 3854 6865 2063  n...r.....8The c
+00000c30: 6172 6469 6e61 6c69 7479 206f 6620 6261  ardinality of ba
+00000c40: 636b 6772 6f75 6e64 206d 7573 7420 6265  ckground must be
+00000c50: 2061 2070 6f73 7469 7665 2069 6e74 6567   a postive integ
+00000c60: 6572 2e72 0600 0000 4e29 0672 0700 0000  er.r....N).r....
+00000c70: 7208 0000 0072 0900 0000 da02 6e70 da03  r....r......np..
+00000c80: 696e 66da 036c 6f67 a907 720d 0000 0072  inf..log..r....r
+00000c90: 0e00 0000 720f 0000 0072 1000 0000 da02  ....r....r......
+00000ca0: 7078 da02 7079 5a03 7078 7972 1100 0000  px..pyZ.pxyr....
+00000cb0: 7211 0000 0072 1200 0000 da09 706d 695f  r....r......pmi_
+00000cc0: 7661 6c75 658d 0000 0073 1c00 0000 0014  value....s......
+00000cd0: 0801 0a01 1001 0a01 1001 0a01 1001 0a01  ................
+00000ce0: 0801 0801 0801 0801 0802 7220 0000 0063  ..........r ...c
+00000cf0: 0400 0000 0000 0000 0000 0000 0700 0000  ................
+00000d00: 0400 0000 4300 0000 73a4 0000 007c 0364  ....C...s....|.d
+00000d10: 016b 0172 1274 00a0 0164 02a1 0101 007c  .k.r.t...d.....|
+00000d20: 027c 006b 0473 227c 027c 016b 0472 2c74  .|.k.s"|.|.k.r,t
+00000d30: 00a0 0164 03a1 0101 007c 007c 036b 0473  ...d.....|.|.k.s
+00000d40: 3c7c 017c 036b 0472 4674 00a0 0164 03a1  <|.|.k.rFt...d..
+00000d50: 0101 0074 027c 007c 017c 0283 0364 016b  ...t.|.|.|...d.k
+00000d60: 0072 6074 00a0 0164 03a1 0101 007c 007c  .r`t...d.....|.|
+00000d70: 031b 007d 047c 017c 031b 007d 057c 027c  ...}.|.|...}.|.|
+00000d80: 031b 007d 067c 0664 016b 0272 8464 0453  ...}.|.d.k.r.d.S
+00000d90: 0074 03a0 047c 047c 0514 00a1 0174 03a0  .t...|.|.....t..
+00000da0: 047c 06a1 011b 0064 0518 0053 0064 0653  .|.....d...S.d.S
+00000db0: 0029 0761 3301 0000 0a09 4361 6c63 756c  .).a3.....Calcul
+00000dc0: 6174 6520 7468 6520 6e6f 726d 616c 697a  ate the normaliz
+00000dd0: 6564 2070 6f69 6e74 7769 7365 206d 7574  ed pointwise mut
+00000de0: 7561 6c20 696e 666f 726d 6174 696f 6e20  ual information 
+00000df0: 284e 504d 4929 2e0a 0a09 5061 7261 6d65  (NPMI)....Parame
+00000e00: 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d  ters..----------
+00000e10: 0a09 7820 3a20 696e 740a 0909 5468 6520  ..x : int...The 
+00000e20: 6361 7264 696e 616c 6974 7920 6f66 2041  cardinality of A
+00000e30: 2e0a 0979 203a 2069 6e74 0a09 0954 6865  ...y : int...The
+00000e40: 2063 6172 6469 6e61 6c69 7479 206f 6620   cardinality of 
+00000e50: 422e 0a09 7879 203a 2069 6e74 0a09 0954  B...xy : int...T
+00000e60: 6865 2063 6172 6469 6e61 6c69 7479 206f  he cardinality o
+00000e70: 6620 4120 414e 4420 422e 0a09 6720 3a20  f A AND B...g : 
+00000e80: 696e 740a 0909 5468 6520 6361 7264 696e  int...The cardin
+00000e90: 616c 6974 7920 6f66 2062 6163 6b67 726f  ality of backgro
+00000ea0: 756e 642e 0a0a 0952 6574 7572 6e73 0a09  und....Returns..
+00000eb0: 2d2d 2d2d 2d2d 2d0a 0966 6c6f 6174 0a09  -------..float..
+00000ec0: 094e 6f72 6d61 6c69 7a65 6420 706f 696e  .Normalized poin
+00000ed0: 7477 6973 6520 6d75 7475 616c 2069 6e66  twise mutual inf
+00000ee0: 6f72 6d61 7469 6f6e 2e0a 0972 0100 0000  ormation...r....
+00000ef0: 7219 0000 0072 0600 0000 e9ff ffff ffe9  r....r..........
+00000f00: 0100 0000 4e29 0572 0700 0000 7208 0000  ....N).r....r...
+00000f10: 0072 0900 0000 721a 0000 0072 1c00 0000  .r....r....r....
+00000f20: 721d 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000f30: 1200 0000 da0a 6e70 6d69 5f76 616c 7565  ......npmi_value
+00000f40: b100 0000 731c 0000 0000 1408 010a 0110  ....s...........
+00000f50: 010a 0110 010a 0110 010a 0108 0108 0108  ................
+00000f60: 0108 0104 0272 2300 0000 2915 da07 5f5f  .....r#...)...__
+00000f70: 646f 635f 5f72 0a00 0000 7207 0000 00da  doc__r....r.....
+00000f80: 056e 756d 7079 721a 0000 00da 0d63 6f62  .numpyr......cob
+00000f90: 696e 6461 6269 6c69 7479 7202 0000 00da  indabilityr.....
+00000fa0: 0a5f 5f61 7574 686f 725f 5fda 0d5f 5f63  .__author__..__c
+00000fb0: 6f70 7972 6967 6874 5f5f da0b 5f5f 6372  opyright__..__cr
+00000fc0: 6564 6974 735f 5fda 0b5f 5f6c 6963 656e  edits__..__licen
+00000fd0: 7365 5f5f da0b 5f5f 7665 7273 696f 6e5f  se__..__version_
+00000fe0: 5fda 0e5f 5f6d 6169 6e74 6169 6e65 725f  _..__maintainer_
+00000ff0: 5fda 095f 5f65 6d61 696c 5f5f da0a 5f5f  _..__email__..__
+00001000: 7374 6174 7573 5f5f 7213 0000 0072 1500  status__r....r..
+00001010: 0000 7216 0000 0072 1800 0000 7220 0000  ..r....r....r ..
+00001020: 0072 2300 0000 7211 0000 0072 1100 0000  .r#...r....r....
+00001030: 7211 0000 0072 1200 0000 da08 3c6d 6f64  r....r......<mod
+00001040: 756c 653e 0300 0000 7324 0000 0004 0508  ule>....s$......
+00001050: 0108 0108 010c 0304 0104 0104 0104 0106  ................
+00001060: 0104 0104 0104 0208 1d08 1d08 1d08 1f08  ................
+00001070: 24                                       $
```

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ireader.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ireader.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ovbootstrap.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ovbootstrap.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sun Jan 16 16:58:13 2022 UTC, .py size: 9343 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a54e e461 7f24 0000  U........N.a.$..
+00000000: 550d 0d0a 0000 0000 e7db 7b62 0b25 0000  U.........{b.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6401 6404 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6402 6c09 5a09 6401 6402 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -13,454 +13,462 @@
 000000c0: 8401 5a1b 6402 5300 2915 7a37 0a43 7265  ..Z.d.S.).z7.Cre
 000000d0: 6174 6564 206f 6e20 5765 6420 4a61 6e20  ated on Wed Jan 
 000000e0: 2035 2031 333a 3036 3a32 3220 3230 3232   5 13:06:22 2022
 000000f0: 0a0a 4061 7574 686f 723a 206d 3130 3233  ..@author: m1023
 00000100: 3234 0ae9 0000 0000 4e29 04da 1062 6564  24......N)...bed
 00000110: 5f67 656e 6f6d 6963 5f73 697a 65da 1062  _genomic_size..b
 00000120: 6564 5f6f 7665 726c 6170 5f73 697a 65da  ed_overlap_size.
-00000130: 0962 6564 746f 6c69 7374 da0a 6265 645f  .bedtolist..bed_
-00000140: 636f 756e 7473 2901 da08 6261 7365 6e61  counts)...basena
-00000150: 6d65 2901 da06 7361 6d70 6c65 2901 da07  me)...sample)...
-00000160: 7665 7273 696f 6e7a 0a4c 6967 756f 2057  versionz.Liguo W
-00000170: 616e 67da 0843 6f70 796c 6566 74da 034d  ang..Copyleft..M
-00000180: 4954 7a13 7761 6e67 2e6c 6967 756f 406d  ITz.wang.liguo@m
-00000190: 6179 6f2e 6564 75da 0b44 6576 656c 6f70  ayo.edu..Develop
-000001a0: 6d65 6e74 e914 0000 00e7 0000 0000 0000  ment............
-000001b0: e83f e700 0000 8093 dcd4 4163 0700 0000  .?........Ac....
-000001c0: 0000 0000 0000 0000 1d00 0000 0600 0000  ................
-000001d0: 4300 0000 73ec 0100 0069 007d 0774 007c  C...s....i.}.t.|
-000001e0: 0083 017d 0874 007c 0183 017d 0974 017c  ...}.t.|...}.t.|
-000001f0: 0083 017c 0764 013c 0074 017c 0183 017c  ...|.d.<.t.|...|
-00000200: 0764 023c 0074 02a0 0364 03a1 0101 0074  .d.<.t...d.....t
-00000210: 047c 007c 0183 025c 027d 0a7d 0b7c 0a7c  .|.|...\.}.}.|.|
-00000220: 0764 043c 007c 0b7c 0764 053c 0074 057c  .d.<.|.|.d.<.t.|
-00000230: 087c 0983 025c 027d 0c7d 0d74 067c 087c  .|...\.}.}.t.|.|
-00000240: 0983 027d 0e7c 0c7c 0d14 007c 061b 007d  ...}.|.|...|...}
-00000250: 0f74 057c 087c 0917 0083 015c 017d 107c  .t.|.|.....\.}.|
-00000260: 0c7c 0764 063c 007c 0d7c 0764 073c 007c  .|.d.<.|.|.d.<.|
-00000270: 107c 0764 083c 007c 0e7c 0764 093c 007c  .|.d.<.|.|.d.<.|
-00000280: 027c 0c7c 0d7c 0e7c 0683 047c 0764 0a3c  .|.|.|.|...|.d.<
-00000290: 007c 027c 0c7c 0d7c 0f7c 0683 047c 0764  .|.|.|.|.|...|.d
-000002a0: 0b3c 007c 0464 0c6b 0490 0172 ce7c 0564  .<.|.d.k...r.|.d
-000002b0: 0c6b 0472 fe7c 0564 0d6b 0072 fe74 077c  .k.r.|.d.k.r.t.|
-000002c0: 0a7c 0514 0083 017d 1174 077c 0b7c 0514  .|.....}.t.|.|..
-000002d0: 0083 017d 126e 1474 02a0 0864 0ea1 0101  ...}.n.t...d....
-000002e0: 0074 09a0 0a64 0ca1 0101 0074 02a0 0364  .t...d.....t...d
-000002f0: 0f7c 0416 00a1 0101 0067 007d 1374 0b7c  .|.......g.}.t.|
-00000300: 0483 0144 005d 6a7d 1474 02a0 0364 107c  ...D.]j}.t...d.|
-00000310: 1416 00a1 0101 0074 0c7c 087c 1183 027d  .......t.|.|...}
-00000320: 1574 0c7c 097c 1283 027d 1674 067c 157c  .t.|.|...}.t.|.|
-00000330: 1683 027d 177c 0364 0d6b 0390 0172 6e7c  ...}.|.d.k...rn|
-00000340: 177c 0314 007d 1774 057c 157c 1683 025c  .|...}.t.|.|...\
-00000350: 027d 187d 197c 027c 187c 197c 177c 0683  .}.}.|.|.|.|.|..
-00000360: 047d 1a7c 13a0 0d7c 1aa1 0101 0090 0171  .}.|...|.......q
-00000370: 2c74 0ea0 0f74 0ea0 107c 13a1 0164 11a1  ,t...t...|...d..
-00000380: 027d 1b74 0ea0 0f74 0ea0 107c 13a1 0164  .}.t...t...|...d
-00000390: 12a1 027d 1c64 137c 1b7c 1c66 0216 007c  ...}.d.|.|.f...|
-000003a0: 0764 143c 006e 1274 02a0 1164 15a1 0101  .d.<.n.t...d....
-000003b0: 0064 167c 0764 143c 0074 126a 137c 0764  .d.|.d.<.t.j.|.d
-000003c0: 178d 0153 0029 1875 1d09 0000 0a09 4361  ...S.).u......Ca
-000003d0: 6c63 756c 6174 6520 7468 6520 666f 6c6c  lculate the foll
-000003e0: 6f77 696e 6720 696e 6469 6365 733a 0a09  owing indices:..
-000003f0: 2d20 6f76 6572 6c61 7020 636f 6566 6669  - overlap coeffi
-00000400: 6369 656e 742c 0a09 2d20 4a61 6363 6172  cient,..- Jaccar
-00000410: 6427 7320 636f 6566 6669 6369 656e 7420  d's coefficient 
-00000420: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
-00000430: 7065 6469 612e 6f72 672f 7769 6b69 2f4a  pedia.org/wiki/J
-00000440: 6163 6361 7264 5f69 6e64 6578 292c 0a09  accard_index),..
-00000450: 2d20 537a 796d 6b69 6577 6963 7ae2 8093  - Szymkiewicz...
-00000460: 5369 6d70 736f 6e20 636f 6566 6669 6369  Simpson coeffici
-00000470: 656e 742c 2028 6874 7470 733a 2f2f 656e  ent, (https://en
-00000480: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
-00000490: 696b 692f 4f76 6572 6c61 705f 636f 6566  iki/Overlap_coef
-000004a0: 6669 6369 656e 7429 2c0a 092d 2053 c3b8  ficient),..- S..
-000004b0: 7265 6e73 656e e280 9344 6963 6520 636f  rensen...Dice co
-000004c0: 6566 6669 6369 656e 7420 2868 7474 7073  efficient (https
-000004d0: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-000004e0: 6f72 672f 7769 6b69 2f53 c3b8 7265 6e73  org/wiki/S..rens
-000004f0: 656e e280 9344 6963 655f 636f 6566 6669  en...Dice_coeffi
-00000500: 6369 656e 7429 2c0a 092d 2050 6f69 6e74  cient),..- Point
-00000510: 7769 7365 206d 7574 7561 6c20 696e 666f  wise mutual info
-00000520: 726d 6174 696f 6e20 2868 7474 7073 3a2f  rmation (https:/
-00000530: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00000540: 672f 7769 6b69 2f50 6f69 6e74 7769 7365  g/wiki/Pointwise
-00000550: 5f6d 7574 7561 6c5f 696e 666f 726d 6174  _mutual_informat
-00000560: 696f 6e29 2c0a 0a09 5061 7261 6d65 7465  ion),...Paramete
-00000570: 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09  rs..----------..
-00000580: 6669 6c65 3120 3a20 7374 720a 0909 4765  file1 : str...Ge
-00000590: 6e6f 6d69 6320 7265 6769 6f6e 7320 696e  nomic regions in
-000005a0: 2042 4544 2028 4272 6f77 7365 7220 4578   BED (Browser Ex
-000005b0: 7465 6e73 6962 6c65 2044 6174 612c 2068  tensible Data, h
-000005c0: 7474 7073 3a2f 2f67 656e 6f6d 652e 7563  ttps://genome.uc
-000005d0: 7363 2e65 6475 2f46 4151 2f46 4151 666f  sc.edu/FAQ/FAQfo
-000005e0: 726d 6174 2e68 746d 6c23 666f 726d 6174  rmat.html#format
-000005f0: 3129 2c20 4245 442d 6c69 6b65 206f 7220  1), BED-like or 
-00000600: 4269 6742 6564 2066 6f72 6d61 742e 0a09  BigBed format...
-00000610: 0954 6865 2042 4544 2d6c 696b 6520 666f  .The BED-like fo
-00000620: 726d 6174 2069 6e63 6c75 6465 7320 2762  rmat includes 'b
-00000630: 6564 3327 2c27 6265 6434 272c 2762 6564  ed3','bed4','bed
-00000640: 3627 2c27 6265 6431 3227 2c27 6265 6467  6','bed12','bedg
-00000650: 7261 7068 272c 276e 6172 726f 7770 6561  raph','narrowpea
-00000660: 6b27 2c20 2762 726f 6164 7065 616b 272c  k', 'broadpeak',
-00000670: 2767 6170 7065 6470 6561 6b27 2e20 4245  'gappedpeak'. BE
-00000680: 4420 616e 6420 4245 442d 6c69 6b65 0a09  D and BED-like..
-00000690: 0966 6f72 6d61 7420 6361 6e20 6265 2070  .format can be p
-000006a0: 6c61 696e 2074 6578 742c 2063 6f6d 7072  lain text, compr
-000006b0: 6573 7365 6420 282e 677a 2c20 2e7a 2c20  essed (.gz, .z, 
-000006c0: 2e62 7a2c 202e 627a 322c 202e 627a 6970  .bz, .bz2, .bzip
-000006d0: 3229 206f 7220 7265 6d6f 7465 2028 6874  2) or remote (ht
-000006e0: 7470 3a2f 2f2c 2068 7474 7073 3a2f 2f2c  tp://, https://,
-000006f0: 2066 7470 3a2f 2f29 2066 696c 6573 2e20   ftp://) files. 
-00000700: 446f 206e 6f74 2063 6f6d 7072 6573 730a  Do not compress.
-00000710: 0909 4269 6742 6564 2066 6f72 616d 742e  ..BigBed foramt.
-00000720: 2042 6967 4265 6420 6669 6c65 2063 616e   BigBed file can
-00000730: 2061 6c73 6f20 6265 2061 2072 656d 6f74   also be a remot
-00000740: 6520 6669 6c65 2e0a 0966 696c 6532 203a  e file...file2 :
-00000750: 2073 7472 0a09 0947 656e 6f6d 6963 2072   str...Genomic r
-00000760: 6567 696f 6e73 2069 6e20 4245 4420 2842  egions in BED (B
-00000770: 726f 7773 6572 2045 7874 656e 7369 626c  rowser Extensibl
-00000780: 6520 4461 7461 2c20 6874 7470 733a 2f2f  e Data, https://
-00000790: 6765 6e6f 6d65 2e75 6373 632e 6564 752f  genome.ucsc.edu/
-000007a0: 4641 512f 4641 5166 6f72 6d61 742e 6874  FAQ/FAQformat.ht
-000007b0: 6d6c 2366 6f72 6d61 7431 292c 2042 4544  ml#format1), BED
-000007c0: 2d6c 696b 6520 6f72 2042 6967 4265 6420  -like or BigBed 
-000007d0: 666f 726d 6174 2e0a 0909 5468 6520 4245  format....The BE
-000007e0: 442d 6c69 6b65 2066 6f72 6d61 7420 696e  D-like format in
-000007f0: 636c 7564 6573 2027 6265 6433 272c 2762  cludes 'bed3','b
-00000800: 6564 3427 2c27 6265 6436 272c 2762 6564  ed4','bed6','bed
-00000810: 3132 272c 2762 6564 6772 6170 6827 2c27  12','bedgraph','
-00000820: 6e61 7272 6f77 7065 616b 272c 2027 6272  narrowpeak', 'br
-00000830: 6f61 6470 6561 6b27 2c27 6761 7070 6564  oadpeak','gapped
-00000840: 7065 616b 272e 2042 4544 2061 6e64 2042  peak'. BED and B
-00000850: 4544 2d6c 696b 650a 0909 666f 726d 6174  ED-like...format
-00000860: 2063 616e 2062 6520 706c 6169 6e20 7465   can be plain te
-00000870: 7874 2c20 636f 6d70 7265 7373 6564 2028  xt, compressed (
-00000880: 2e67 7a2c 202e 7a2c 202e 627a 2c20 2e62  .gz, .z, .bz, .b
-00000890: 7a32 2c20 2e62 7a69 7032 2920 6f72 2072  z2, .bzip2) or r
-000008a0: 656d 6f74 6520 2868 7474 703a 2f2f 2c20  emote (http://, 
-000008b0: 6874 7470 733a 2f2f 2c20 6674 703a 2f2f  https://, ftp://
-000008c0: 2920 6669 6c65 732e 2044 6f20 6e6f 7420  ) files. Do not 
-000008d0: 636f 6d70 7265 7373 0a09 0942 6967 4265  compress...BigBe
-000008e0: 6420 666f 7261 6d74 2e20 4269 6742 6564  d foramt. BigBed
-000008f0: 2066 696c 6520 6361 6e20 616c 736f 2062   file can also b
-00000900: 6520 6120 7265 6d6f 7465 2066 696c 652e  e a remote file.
-00000910: 0a09 7363 6f72 655f 6675 6e63 203a 2066  ..score_func : f
-00000920: 756e 6374 696f 6e0a 0909 4675 6e63 7469  unction...Functi
-00000930: 6f6e 2074 6f20 6361 6c63 756c 6174 6520  on to calculate 
-00000940: 6f76 6572 6c61 7020 696e 6465 782e 2049  overlap index. I
-00000950: 6e63 6c75 6465 206f 765f 636f 6566 2c20  nclude ov_coef, 
-00000960: 6f76 5f6a 6163 6361 7264 2c20 6f76 5f73  ov_jaccard, ov_s
-00000970: 732c 206f 765f 7364 2c20 706d 695f 7661  s, ov_sd, pmi_va
-00000980: 6c75 652c 206e 706d 695f 7661 6c75 650a  lue, npmi_value.
-00000990: 096e 5f64 7261 7773 203a 2069 6e74 0a09  .n_draws : int..
-000009a0: 0954 696d 6573 206f 6620 6472 6177 696e  .Times of drawin
-000009b0: 6720 7361 6d70 6c65 7320 7769 7468 2072  g samples with r
-000009c0: 6570 6c61 6365 6d65 6e74 2e20 5365 7420  eplacement. Set 
-000009d0: 746f 2027 3027 2074 6f20 7475 726e 206f  to '0' to turn o
-000009e0: 6666 2062 6f6f 7473 7472 6170 696e 672e  ff bootstraping.
-000009f0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-00000a00: 2032 302e 0a09 6672 6163 7469 6f6e 203a   20...fraction :
-00000a10: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00000a20: 0a09 0954 6865 2066 7261 6374 696f 6e20  ...The fraction 
-00000a30: 6f66 2073 7562 7361 6d70 6c65 2e20 5468  of subsample. Th
-00000a40: 6520 6465 6661 756c 7420 6973 2030 2e37  e default is 0.7
-00000a50: 3520 2837 3525 206f 6620 7468 6520 6f72  5 (75% of the or
-00000a60: 6967 6e61 6c20 6765 6e6f 6d69 6320 7265  ignal genomic re
-00000a70: 6769 6e6f 7320 7769 6c6c 2062 6520 7365  ginos will be se
-00000a80: 6c65 6374 6564 292e 0a09 6267 5f73 697a  lected)...bg_siz
-00000a90: 6520 3a20 696e 742c 206f 7074 696f 6e61  e : int, optiona
-00000aa0: 6c0a 0909 5468 6520 6566 6665 6374 6976  l...The effectiv
-00000ab0: 6520 6261 636b 6772 6f75 6e64 2067 656e  e background gen
-00000ac0: 6f6d 6520 7369 7a65 2e20 4162 6f75 7420  ome size. About 
-00000ad0: 312e 3447 6220 6f66 2074 6865 2068 756d  1.4Gb of the hum
-00000ae0: 616e 2067 656e 6f6d 6520 6172 652e 2054  an genome are. T
-00000af0: 6865 2064 6566 6175 6c74 2069 7320 312e  he default is 1.
-00000b00: 3465 392e 0a0a 0952 6574 7572 6e73 0a09  4e9....Returns..
-00000b10: 2d2d 2d2d 2d2d 2d0a 0970 616e 6461 732e  -------..pandas.
-00000b20: 5365 7269 6573 0a09 0950 616e 6461 7320  Series...Pandas 
-00000b30: 5365 7269 6573 206f 6620 2763 6f65 665f  Series of 'coef_
-00000b40: 6f62 7327 2c20 2763 6f65 665f 6578 7027  obs', 'coef_exp'
-00000b50: 2c27 636f 6566 5f72 6174 696f 272c 2027  ,'coef_ratio', '
-00000b60: 636f 6566 5f72 6174 696f 5f6c 6f77 272c  coef_ratio_low',
-00000b70: 2027 636f 6566 5f72 6174 696f 5f68 6967   'coef_ratio_hig
-00000b80: 6827 2e0a 0909 2763 6f65 665f 6f62 7327  h'....'coef_obs'
-00000b90: 203a 204f 6273 6572 7665 6420 6f76 6572   : Observed over
-00000ba0: 6c61 7020 636f 6566 6669 6369 656e 7420  lap coefficient 
-00000bb0: 6265 7477 6565 6e20 7477 6f20 4245 4420  between two BED 
-00000bc0: 6669 6c65 732e 0a09 0927 636f 6566 5f65  files....'coef_e
-00000bd0: 7870 2720 3a20 4578 7065 6374 6564 206f  xp' : Expected o
-00000be0: 7665 726c 6170 2063 6f65 6666 6963 6965  verlap coefficie
-00000bf0: 6e74 2062 6574 7765 656e 2074 776f 2042  nt between two B
-00000c00: 4544 2066 696c 6573 2e0a 0909 2763 6f65  ED files....'coe
-00000c10: 665f 7261 7469 6f27 203a 2052 6174 696f  f_ratio' : Ratio
-00000c20: 2062 6574 7765 656e 2027 636f 6566 5f6f   between 'coef_o
-00000c30: 6273 2720 616e 6420 2763 6f65 665f 6578  bs' and 'coef_ex
-00000c40: 7027 2e0a 0909 2763 6f65 665f 7261 7469  p'....'coef_rati
-00000c50: 6f5f 6c6f 7727 203a 2054 6865 206c 6f77  o_low' : The low
-00000c60: 6572 2062 6f75 6e64 206f 6620 3935 2520  er bound of 95% 
-00000c70: 636f 6e66 6964 656e 6365 2069 6e74 6572  confidence inter
-00000c80: 7661 6c20 6f66 2027 636f 6566 5f72 6174  val of 'coef_rat
-00000c90: 696f 272e 0a09 0927 636f 6566 5f72 6174  io'....'coef_rat
-00000ca0: 696f 5f68 6967 6827 203a 2054 6865 2075  io_high' : The u
-00000cb0: 7070 6572 2062 6f75 6e64 206f 6620 3935  pper bound of 95
-00000cc0: 2520 636f 6e66 6964 656e 6365 2069 6e74  % confidence int
-00000cd0: 6572 7661 6c20 6f66 2027 636f 6566 5f72  erval of 'coef_r
-00000ce0: 6174 696f 272e 0a0a 09fa 0641 2e6e 616d  atio'......A.nam
-00000cf0: 65fa 0642 2e6e 616d 65fa 1a43 616c 6375  e..B.name..Calcu
-00000d00: 6c61 7469 6e67 2062 6564 2063 6f75 6e74  lating bed count
-00000d10: 7320 2e2e 2efa 1041 2e69 6e74 6572 7661  s .....A.interva
-00000d20: 6c5f 636f 756e 74fa 1042 2e69 6e74 6572  l_count..B.inter
-00000d30: 7661 6c5f 636f 756e 74fa 0641 2e73 697a  val_count..A.siz
-00000d40: 65fa 0642 2e73 697a 65fa 0b41 5f6f 725f  e..B.size..A_or_
-00000d50: 422e 7369 7a65 fa0c 415f 616e 645f 422e  B.size..A_and_B.
-00000d60: 7369 7a65 da04 436f 6566 fa0e 436f 6566  size..Coef..Coef
-00000d70: 2865 7870 6563 7465 6429 7201 0000 00e9  (expected)r.....
-00000d80: 0100 0000 fa1d 4672 6163 7469 6f6e 206d  ......Fraction m
-00000d90: 7573 7420 6265 203e 2030 2061 6e64 203c  ust be > 0 and <
-00000da0: 2031 2efa 2642 6f6f 7473 7472 6170 696e   1..&Bootstrapin
-00000db0: 6720 6973 206f 6e2e 2049 7465 7261 7465  g is on. Iterate
-00000dc0: 2025 6420 7469 6d65 732e 20fa 1b42 6f6f   %d times. ..Boo
-00000dd0: 7473 7472 6170 2072 6573 616d 706c 696e  tstrap resamplin
-00000de0: 6720 2564 202e 2e2e e700 0000 0000 0004  g %d ...........
-00000df0: 40e7 0000 0000 0060 5840 fa0b 5b25 2e34  @......`X@..[%.4
-00000e00: 662c 252e 3466 5dfa 0c43 6f65 6628 3935  f,%.4f]..Coef(95
-00000e10: 2520 4349 29fa 1742 6f6f 7473 7472 6170  % CI)..Bootstrap
-00000e20: 696e 6720 6973 206f 6666 202e 2e2e fa07  ing is off .....
-00000e30: 5b4e 412c 4e41 5da9 01da 0464 6174 61a9  [NA,NA]....data.
-00000e40: 1472 0400 0000 7206 0000 00da 076c 6f67  .r....r......log
-00000e50: 6769 6e67 da05 6465 6275 6772 0500 0000  ging..debugr....
-00000e60: 7202 0000 0072 0300 0000 da03 696e 74da  r....r......int.
-00000e70: 0565 7272 6f72 da03 7379 73da 0465 7869  .error..sys..exi
-00000e80: 74da 0572 616e 6765 7207 0000 00da 0661  t..ranger......a
-00000e90: 7070 656e 64da 026e 70da 0a70 6572 6365  ppend..np..perce
-00000ea0: 6e74 696c 65da 0561 7272 6179 da04 696e  ntile..array..in
-00000eb0: 666f da02 7064 da06 5365 7269 6573 a91d  fo..pd..Series..
-00000ec0: da05 6669 6c65 31da 0566 696c 6532 da0a  ..file1..file2..
-00000ed0: 7363 6f72 655f 6675 6e63 da0b 7369 7a65  score_func..size
-00000ee0: 5f66 6163 746f 72da 076e 5f64 7261 7773  _factor..n_draws
-00000ef0: da08 6672 6163 7469 6f6e da07 6267 5f73  ..fraction..bg_s
-00000f00: 697a 65da 0772 6573 756c 7473 da09 6669  ize..results..fi
-00000f10: 6c65 315f 6c73 74da 0966 696c 6532 5f6c  le1_lst..file2_l
-00000f20: 7374 5a0b 746f 7461 6c43 6f75 6e74 315a  stZ.totalCount1Z
-00000f30: 0b74 6f74 616c 436f 756e 7432 da09 756e  .totalCount2..un
-00000f40: 6971 4261 7365 31da 0975 6e69 7142 6173  iqBase1..uniqBas
-00000f50: 6532 da0c 6f76 6572 6c61 7042 6173 6573  e2..overlapBases
-00000f60: 5a10 6f76 6572 6c61 7042 6173 6573 5f65  Z.overlapBases_e
-00000f70: 7870 5a0a 756e 696f 6e42 6173 6573 5a0e  xpZ.unionBasesZ.
-00000f80: 7265 7361 6d70 6c65 5f73 697a 6531 5a0e  resample_size1Z.
-00000f90: 7265 7361 6d70 6c65 5f73 697a 6532 da03  resample_size2..
-00000fa0: 746d 70da 0169 5a08 7361 6d70 6c65 5f31  tmp..iZ.sample_1
-00000fb0: 5a08 7361 6d70 6c65 5f32 5a13 7361 6d70  Z.sample_2Z.samp
-00000fc0: 6c65 5f6f 7665 726c 6170 4261 7365 735a  le_overlapBasesZ
-00000fd0: 0c73 616d 706c 6531 5f73 697a 655a 0c73  .sample1_sizeZ.s
-00000fe0: 616d 706c 6532 5f73 697a 655a 0d73 616d  ample2_sizeZ.sam
-00000ff0: 706c 655f 6f76 636f 6566 5a08 6369 5f6c  ple_ovcoefZ.ci_l
-00001000: 6f77 6572 5a08 6369 5f75 7070 6572 a900  owerZ.ci_upper..
-00001010: 7245 0000 00fa 472f 5573 6572 732f 6d31  rE....G/Users/m1
-00001020: 3032 3332 342f 446f 6375 6d65 6e74 732f  02324/Documents/
-00001030: 4769 7448 7562 2f63 6f62 696e 642f 6c69  GitHub/cobind/li
-00001040: 622f 636f 6269 6e64 6162 696c 6974 792f  b/cobindability/
-00001050: 6f76 626f 6f74 7374 7261 702e 7079 da0e  ovbootstrap.py..
-00001060: 626f 6f74 7374 7261 705f 636f 6566 1e00  bootstrap_coef..
-00001070: 0000 7356 0000 0000 2a04 0208 0108 020c  ..sV....*.......
-00001080: 010c 030a 010e 0108 0108 050e 030a 010c  ................
-00001090: 010e 0208 0108 0108 0108 0112 0112 020a  ................
-000010a0: 0110 010c 010e 020a 010a 010e 0104 010c  ................
-000010b0: 010e 010a 010a 020a 010a 0108 010e 010e  ................
-000010c0: 010e 0112 0112 0112 020a 0108 0272 4700  .............rG.
-000010d0: 0000 6307 0000 0000 0000 0000 0000 001d  ..c.............
-000010e0: 0000 0007 0000 0043 0000 0073 f001 0000  .......C...s....
-000010f0: 6900 7d07 7400 7c00 8301 7d08 7400 7c01  i.}.t.|...}.t.|.
-00001100: 8301 7d09 7401 7c00 8301 7c07 6401 3c00  ..}.t.|...|.d.<.
-00001110: 7401 7c01 8301 7c07 6402 3c00 7402 a003  t.|...|.d.<.t...
-00001120: 6403 a101 0100 7404 7c00 7c01 8302 5c02  d.....t.|.|...\.
-00001130: 7d0a 7d0b 7c0a 7c07 6404 3c00 7c0b 7c07  }.}.|.|.d.<.|.|.
-00001140: 6405 3c00 7405 7c08 7c09 8302 5c02 7d0c  d.<.t.|.|...\.}.
-00001150: 7d0d 7406 7c08 7c09 8302 7d0e 7c0c 7c0d  }.t.|.|...}.|.|.
-00001160: 1400 7c06 1b00 7d0f 7405 7c08 7c09 1700  ..|...}.t.|.|...
-00001170: 8301 5c01 7d10 7c0c 7c07 6406 3c00 7c0d  ..\.}.|.|.d.<.|.
-00001180: 7c07 6407 3c00 7c10 7c07 6408 3c00 7c0e  |.d.<.|.|.d.<.|.
-00001190: 7c07 6409 3c00 7c02 7c0c 7c0d 7c0e 7c06  |.d.<.|.|.|.|.|.
-000011a0: 8304 7c07 640a 3c00 7c02 7c0c 7c0d 7c0f  ..|.d.<.|.|.|.|.
-000011b0: 7c06 8304 7c07 640b 3c00 7c04 640c 6b04  |...|.d.<.|.d.k.
-000011c0: 9001 72d2 7c05 640c 6b04 72fe 7c05 640d  ..r.|.d.k.r.|.d.
-000011d0: 6b00 72fe 7407 7c0a 7c05 1400 8301 7d11  k.r.t.|.|.....}.
-000011e0: 7407 7c0b 7c05 1400 8301 7d12 6e14 7402  t.|.|.....}.n.t.
-000011f0: a008 640e a101 0100 7409 a00a 640c a101  ..d.....t...d...
-00001200: 0100 7402 a003 640f 7c04 1600 a101 0100  ..t...d.|.......
-00001210: 6700 7d13 740b 7c04 8301 4400 5d6e 7d14  g.}.t.|...D.]n}.
-00001220: 7402 a003 6410 7c14 1600 a101 0100 740c  t...d.|.......t.
-00001230: 7c08 7c11 8302 7d15 740c 7c09 7c12 8302  |.|...}.t.|.|...
-00001240: 7d16 7406 7c15 7c16 8302 7d17 7c03 640d  }.t.|.|...}.|.d.
-00001250: 6b03 9001 726e 7c17 7c03 1400 7d17 7405  k...rn|.|...}.t.
-00001260: 7c15 7c16 8302 5c02 7d18 7d19 7c02 7c18  |.|...\.}.}.|.|.
-00001270: 7c19 7c17 7c06 7c05 1400 8304 7d1a 7c13  |.|.|.|.....}.|.
-00001280: a00d 7c1a a101 0100 9001 712c 740e a00f  ..|.......q,t...
-00001290: 740e a010 7c13 a101 6411 a102 7d1b 740e  t...|...d...}.t.
-000012a0: a00f 740e a010 7c13 a101 6412 a102 7d1c  ..t...|...d...}.
-000012b0: 6413 7c1b 7c1c 6602 1600 7c07 6414 3c00  d.|.|.f...|.d.<.
-000012c0: 6e12 7402 a011 6415 a101 0100 6416 7c07  n.t...d.....d.|.
-000012d0: 6414 3c00 7412 6a13 7c07 6417 8d01 5300  d.<.t.j.|.d...S.
-000012e0: 2918 61d2 0700 000a 0943 616c 6375 6c61  ).a......Calcula
-000012f0: 7465 2074 6865 2066 6f6c 6c6f 7769 6e67  te the following
-00001300: 2069 6e64 6963 6573 3a0a 092d 204e 6f72   indices:..- Nor
-00001310: 6d61 6c69 7a65 6420 706f 696e 7477 6973  malized pointwis
-00001320: 6520 6d75 7475 616c 2069 6e66 6f72 6d61  e mutual informa
-00001330: 7469 6f6e 2e0a 0a09 5061 7261 6d65 7465  tion....Paramete
-00001340: 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d 0a09  rs..----------..
-00001350: 6669 6c65 3120 3a20 7374 720a 0909 4765  file1 : str...Ge
-00001360: 6e6f 6d69 6320 7265 6769 6f6e 7320 696e  nomic regions in
-00001370: 2042 4544 2028 4272 6f77 7365 7220 4578   BED (Browser Ex
-00001380: 7465 6e73 6962 6c65 2044 6174 612c 2068  tensible Data, h
-00001390: 7474 7073 3a2f 2f67 656e 6f6d 652e 7563  ttps://genome.uc
-000013a0: 7363 2e65 6475 2f46 4151 2f46 4151 666f  sc.edu/FAQ/FAQfo
-000013b0: 726d 6174 2e68 746d 6c23 666f 726d 6174  rmat.html#format
-000013c0: 3129 2c20 4245 442d 6c69 6b65 206f 7220  1), BED-like or 
-000013d0: 4269 6742 6564 2066 6f72 6d61 742e 0a09  BigBed format...
-000013e0: 0954 6865 2042 4544 2d6c 696b 6520 666f  .The BED-like fo
-000013f0: 726d 6174 2069 6e63 6c75 6465 7320 2762  rmat includes 'b
-00001400: 6564 3327 2c27 6265 6434 272c 2762 6564  ed3','bed4','bed
-00001410: 3627 2c27 6265 6431 3227 2c27 6265 6467  6','bed12','bedg
-00001420: 7261 7068 272c 276e 6172 726f 7770 6561  raph','narrowpea
-00001430: 6b27 2c20 2762 726f 6164 7065 616b 272c  k', 'broadpeak',
-00001440: 2767 6170 7065 6470 6561 6b27 2e20 4245  'gappedpeak'. BE
-00001450: 4420 616e 6420 4245 442d 6c69 6b65 0a09  D and BED-like..
-00001460: 0966 6f72 6d61 7420 6361 6e20 6265 2070  .format can be p
-00001470: 6c61 696e 2074 6578 742c 2063 6f6d 7072  lain text, compr
-00001480: 6573 7365 6420 282e 677a 2c20 2e7a 2c20  essed (.gz, .z, 
-00001490: 2e62 7a2c 202e 627a 322c 202e 627a 6970  .bz, .bz2, .bzip
-000014a0: 3229 206f 7220 7265 6d6f 7465 2028 6874  2) or remote (ht
-000014b0: 7470 3a2f 2f2c 2068 7474 7073 3a2f 2f2c  tp://, https://,
-000014c0: 2066 7470 3a2f 2f29 2066 696c 6573 2e20   ftp://) files. 
-000014d0: 446f 206e 6f74 2063 6f6d 7072 6573 730a  Do not compress.
-000014e0: 0909 4269 6742 6564 2066 6f72 616d 742e  ..BigBed foramt.
-000014f0: 2042 6967 4265 6420 6669 6c65 2063 616e   BigBed file can
-00001500: 2061 6c73 6f20 6265 2061 2072 656d 6f74   also be a remot
-00001510: 6520 6669 6c65 2e0a 0966 696c 6532 203a  e file...file2 :
-00001520: 2073 7472 0a09 0947 656e 6f6d 6963 2072   str...Genomic r
-00001530: 6567 696f 6e73 2069 6e20 4245 4420 2842  egions in BED (B
-00001540: 726f 7773 6572 2045 7874 656e 7369 626c  rowser Extensibl
-00001550: 6520 4461 7461 2c20 6874 7470 733a 2f2f  e Data, https://
-00001560: 6765 6e6f 6d65 2e75 6373 632e 6564 752f  genome.ucsc.edu/
-00001570: 4641 512f 4641 5166 6f72 6d61 742e 6874  FAQ/FAQformat.ht
-00001580: 6d6c 2366 6f72 6d61 7431 292c 2042 4544  ml#format1), BED
-00001590: 2d6c 696b 6520 6f72 2042 6967 4265 6420  -like or BigBed 
-000015a0: 666f 726d 6174 2e0a 0909 5468 6520 4245  format....The BE
-000015b0: 442d 6c69 6b65 2066 6f72 6d61 7420 696e  D-like format in
-000015c0: 636c 7564 6573 2027 6265 6433 272c 2762  cludes 'bed3','b
-000015d0: 6564 3427 2c27 6265 6436 272c 2762 6564  ed4','bed6','bed
-000015e0: 3132 272c 2762 6564 6772 6170 6827 2c27  12','bedgraph','
-000015f0: 6e61 7272 6f77 7065 616b 272c 2027 6272  narrowpeak', 'br
-00001600: 6f61 6470 6561 6b27 2c27 6761 7070 6564  oadpeak','gapped
-00001610: 7065 616b 272e 2042 4544 2061 6e64 2042  peak'. BED and B
-00001620: 4544 2d6c 696b 650a 0909 666f 726d 6174  ED-like...format
-00001630: 2063 616e 2062 6520 706c 6169 6e20 7465   can be plain te
-00001640: 7874 2c20 636f 6d70 7265 7373 6564 2028  xt, compressed (
-00001650: 2e67 7a2c 202e 7a2c 202e 627a 2c20 2e62  .gz, .z, .bz, .b
-00001660: 7a32 2c20 2e62 7a69 7032 2920 6f72 2072  z2, .bzip2) or r
-00001670: 656d 6f74 6520 2868 7474 703a 2f2f 2c20  emote (http://, 
-00001680: 6874 7470 733a 2f2f 2c20 6674 703a 2f2f  https://, ftp://
-00001690: 2920 6669 6c65 732e 2044 6f20 6e6f 7420  ) files. Do not 
-000016a0: 636f 6d70 7265 7373 0a09 0942 6967 4265  compress...BigBe
-000016b0: 6420 666f 7261 6d74 2e20 4269 6742 6564  d foramt. BigBed
-000016c0: 2066 696c 6520 6361 6e20 616c 736f 2062   file can also b
-000016d0: 6520 6120 7265 6d6f 7465 2066 696c 652e  e a remote file.
-000016e0: 0a09 7363 6f72 655f 6675 6e63 203a 2066  ..score_func : f
-000016f0: 756e 6374 696f 6e0a 0909 4675 6e63 7469  unction...Functi
-00001700: 6f6e 2074 6f20 6361 6c63 756c 6174 6520  on to calculate 
-00001710: 6f76 6572 6c61 7020 696e 6465 782e 2049  overlap index. I
-00001720: 6e63 6c75 6465 206f 765f 636f 6566 2c20  nclude ov_coef, 
-00001730: 6f76 5f6a 6163 6361 7264 2c20 6f76 5f73  ov_jaccard, ov_s
-00001740: 732c 206f 765f 7364 2c20 706d 695f 7661  s, ov_sd, pmi_va
-00001750: 6c75 652c 206e 706d 695f 7661 6c75 650a  lue, npmi_value.
-00001760: 096e 5f64 7261 7773 203a 2069 6e74 0a09  .n_draws : int..
-00001770: 0954 696d 6573 206f 6620 6472 6177 696e  .Times of drawin
-00001780: 6720 7361 6d70 6c65 7320 7769 7468 2072  g samples with r
-00001790: 6570 6c61 6365 6d65 6e74 2e20 5365 7420  eplacement. Set 
-000017a0: 746f 2027 3027 2074 6f20 7475 726e 206f  to '0' to turn o
-000017b0: 6666 2062 6f6f 7473 7472 6170 696e 672e  ff bootstraping.
-000017c0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-000017d0: 2032 302e 0a09 6672 6163 7469 6f6e 203a   20...fraction :
-000017e0: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-000017f0: 0a09 0954 6865 2066 7261 6374 696f 6e20  ...The fraction 
-00001800: 6f66 2073 7562 7361 6d70 6c65 2e20 5468  of subsample. Th
-00001810: 6520 6465 6661 756c 7420 6973 2030 2e37  e default is 0.7
-00001820: 3520 2837 3525 206f 6620 7468 6520 6f72  5 (75% of the or
-00001830: 6967 6e61 6c20 6765 6e6f 6d69 6320 7265  ignal genomic re
-00001840: 6769 6e6f 7320 7769 6c6c 2062 6520 7365  ginos will be se
-00001850: 6c65 6374 6564 292e 0a09 6267 5f73 697a  lected)...bg_siz
-00001860: 6520 3a20 696e 742c 206f 7074 696f 6e61  e : int, optiona
-00001870: 6c0a 0909 5468 6520 6566 6665 6374 6976  l...The effectiv
-00001880: 6520 6261 636b 6772 6f75 6e64 2067 656e  e background gen
-00001890: 6f6d 6520 7369 7a65 2e20 4162 6f75 7420  ome size. About 
-000018a0: 312e 3447 6220 6f66 2074 6865 2068 756d  1.4Gb of the hum
-000018b0: 616e 2067 656e 6f6d 6520 6172 652e 2054  an genome are. T
-000018c0: 6865 2064 6566 6175 6c74 2069 7320 312e  he default is 1.
-000018d0: 3465 392e 0a0a 0952 6574 7572 6e73 0a09  4e9....Returns..
-000018e0: 2d2d 2d2d 2d2d 2d0a 0970 616e 6461 732e  -------..pandas.
-000018f0: 5365 7269 6573 0a09 0950 616e 6461 7320  Series...Pandas 
-00001900: 5365 7269 6573 206f 6620 2763 6f65 665f  Series of 'coef_
-00001910: 6f62 7327 2c20 2763 6f65 665f 6578 7027  obs', 'coef_exp'
-00001920: 2c27 636f 6566 5f72 6174 696f 272c 2027  ,'coef_ratio', '
-00001930: 636f 6566 5f72 6174 696f 5f6c 6f77 272c  coef_ratio_low',
-00001940: 2027 636f 6566 5f72 6174 696f 5f68 6967   'coef_ratio_hig
-00001950: 6827 2e0a 0909 2763 6f65 665f 6f62 7327  h'....'coef_obs'
-00001960: 203a 204f 6273 6572 7665 6420 6f76 6572   : Observed over
-00001970: 6c61 7020 636f 6566 6669 6369 656e 7420  lap coefficient 
-00001980: 6265 7477 6565 6e20 7477 6f20 4245 4420  between two BED 
-00001990: 6669 6c65 732e 0a09 0927 636f 6566 5f65  files....'coef_e
-000019a0: 7870 2720 3a20 4578 7065 6374 6564 206f  xp' : Expected o
-000019b0: 7665 726c 6170 2063 6f65 6666 6963 6965  verlap coefficie
-000019c0: 6e74 2062 6574 7765 656e 2074 776f 2042  nt between two B
-000019d0: 4544 2066 696c 6573 2e0a 0909 2763 6f65  ED files....'coe
-000019e0: 665f 7261 7469 6f27 203a 2052 6174 696f  f_ratio' : Ratio
-000019f0: 2062 6574 7765 656e 2027 636f 6566 5f6f   between 'coef_o
-00001a00: 6273 2720 616e 6420 2763 6f65 665f 6578  bs' and 'coef_ex
-00001a10: 7027 2e0a 0909 2763 6f65 665f 7261 7469  p'....'coef_rati
-00001a20: 6f5f 6c6f 7727 203a 2054 6865 206c 6f77  o_low' : The low
-00001a30: 6572 2062 6f75 6e64 206f 6620 3935 2520  er bound of 95% 
-00001a40: 636f 6e66 6964 656e 6365 2069 6e74 6572  confidence inter
-00001a50: 7661 6c20 6f66 2027 636f 6566 5f72 6174  val of 'coef_rat
-00001a60: 696f 272e 0a09 0927 636f 6566 5f72 6174  io'....'coef_rat
-00001a70: 696f 5f68 6967 6827 203a 2054 6865 2075  io_high' : The u
-00001a80: 7070 6572 2062 6f75 6e64 206f 6620 3935  pper bound of 95
-00001a90: 2520 636f 6e66 6964 656e 6365 2069 6e74  % confidence int
-00001aa0: 6572 7661 6c20 6f66 2027 636f 6566 5f72  erval of 'coef_r
-00001ab0: 6174 696f 272e 0a0a 0972 0f00 0000 7210  atio'....r....r.
-00001ac0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00001ad0: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001ae0: 0072 1700 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001af0: 7201 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00001b00: 1c00 0000 721d 0000 0072 1e00 0000 721f  ....r....r....r.
-00001b10: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
-00001b20: 0000 7223 0000 0072 2400 0000 7226 0000  ..r#...r$...r&..
-00001b30: 0072 3500 0000 7245 0000 0072 4500 0000  .r5...rE...rE...
-00001b40: 7246 0000 00da 0e62 6f6f 7473 7472 6170  rF.....bootstrap
-00001b50: 5f6e 706d 6985 0000 0073 5600 0000 0026  _npmi....sV....&
-00001b60: 0402 0801 0802 0c01 0c03 0a01 0e01 0801  ................
-00001b70: 0805 0e03 0a01 0c01 0e02 0801 0801 0801  ................
-00001b80: 0801 1201 1202 0a01 1001 0c01 0e02 0a01  ................
-00001b90: 0a01 0e01 0401 0c01 0e01 0a01 0a02 0a01  ................
-00001ba0: 0a01 0801 0e01 1201 0e01 1201 1201 1202  ................
-00001bb0: 0a01 0802 7248 0000 0029 0372 0c00 0000  ....rH...).r....
-00001bc0: 720d 0000 0072 0e00 0000 2903 720c 0000  r....r....).r...
-00001bd0: 0072 0d00 0000 720e 0000 0029 1cda 075f  .r....r....)..._
-00001be0: 5f64 6f63 5f5f 722b 0000 00da 1163 6f62  _doc__r+.....cob
-00001bf0: 696e 6461 6269 6c69 7479 2e42 4544 7202  indability.BEDr.
-00001c00: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
-00001c10: 0000 da07 6f73 2e70 6174 6872 0600 0000  ....os.pathr....
-00001c20: 7227 0000 00da 056e 756d 7079 722f 0000  r'.....numpyr/..
-00001c30: 00da 0670 616e 6461 7372 3300 0000 da06  ...pandasr3.....
-00001c40: 7261 6e64 6f6d 7207 0000 00da 0d63 6f62  randomr......cob
-00001c50: 696e 6461 6269 6c69 7479 7208 0000 00da  indabilityr.....
-00001c60: 0a5f 5f61 7574 686f 725f 5fda 0d5f 5f63  .__author__..__c
-00001c70: 6f70 7972 6967 6874 5f5f da0b 5f5f 6372  opyright__..__cr
-00001c80: 6564 6974 735f 5fda 0b5f 5f6c 6963 656e  edits__..__licen
-00001c90: 7365 5f5f da0b 5f5f 7665 7273 696f 6e5f  se__..__version_
-00001ca0: 5fda 0e5f 5f6d 6169 6e74 6169 6e65 725f  _..__maintainer_
-00001cb0: 5fda 095f 5f65 6d61 696c 5f5f da0a 5f5f  _..__email__..__
-00001cc0: 7374 6174 7573 5f5f 7247 0000 0072 4800  status__rG...rH.
-00001cd0: 0000 7245 0000 0072 4500 0000 7245 0000  ..rE...rE...rE..
-00001ce0: 0072 4600 0000 da08 3c6d 6f64 756c 653e  .rF.....<module>
-00001cf0: 0300 0000 7324 0000 0004 0608 0118 020c  ....s$..........
-00001d00: 0108 0108 0108 010c 010c 0304 0104 0104  ................
-00001d10: 0104 0106 0104 0104 0104 030a 67         ............g
+00000130: 0b62 6564 5f74 6f5f 6c69 7374 da0a 6265  .bed_to_list..be
+00000140: 645f 636f 756e 7473 2901 da08 6261 7365  d_counts)...base
+00000150: 6e61 6d65 2901 da06 7361 6d70 6c65 2901  name)...sample).
+00000160: da07 7665 7273 696f 6e7a 0a4c 6967 756f  ..versionz.Liguo
+00000170: 2057 616e 67da 0843 6f70 796c 6566 74da   Wang..Copyleft.
+00000180: 034d 4954 7a13 7761 6e67 2e6c 6967 756f  .MITz.wang.liguo
+00000190: 406d 6179 6f2e 6564 75da 0b44 6576 656c  @mayo.edu..Devel
+000001a0: 6f70 6d65 6e74 e914 0000 00e7 0000 0000  opment..........
+000001b0: 0000 e83f e700 0000 8093 dcd4 4163 0700  ...?........Ac..
+000001c0: 0000 0000 0000 0000 0000 1d00 0000 0600  ................
+000001d0: 0000 4300 0000 73ec 0100 0069 007d 0774  ..C...s....i.}.t
+000001e0: 007c 0083 017d 0874 007c 0183 017d 0974  .|...}.t.|...}.t
+000001f0: 017c 0083 017c 0764 013c 0074 017c 0183  .|...|.d.<.t.|..
+00000200: 017c 0764 023c 0074 02a0 0364 03a1 0101  .|.d.<.t...d....
+00000210: 0074 047c 007c 0183 025c 027d 0a7d 0b7c  .t.|.|...\.}.}.|
+00000220: 0a7c 0764 043c 007c 0b7c 0764 053c 0074  .|.d.<.|.|.d.<.t
+00000230: 057c 087c 0983 025c 027d 0c7d 0d74 067c  .|.|...\.}.}.t.|
+00000240: 087c 0983 027d 0e7c 0c7c 0d14 007c 061b  .|...}.|.|...|..
+00000250: 007d 0f74 057c 087c 0917 0083 015c 017d  .}.t.|.|.....\.}
+00000260: 107c 0c7c 0764 063c 007c 0d7c 0764 073c  .|.|.d.<.|.|.d.<
+00000270: 007c 107c 0764 083c 007c 0e7c 0764 093c  .|.|.d.<.|.|.d.<
+00000280: 007c 027c 0c7c 0d7c 0e7c 0683 047c 0764  .|.|.|.|.|...|.d
+00000290: 0a3c 007c 027c 0c7c 0d7c 0f7c 0683 047c  .<.|.|.|.|.|...|
+000002a0: 0764 0b3c 007c 0464 0c6b 0490 0172 ce7c  .d.<.|.d.k...r.|
+000002b0: 0564 0c6b 0472 fe7c 0564 0d6b 0072 fe74  .d.k.r.|.d.k.r.t
+000002c0: 077c 0a7c 0514 0083 017d 1174 077c 0b7c  .|.|.....}.t.|.|
+000002d0: 0514 0083 017d 126e 1474 02a0 0864 0ea1  .....}.n.t...d..
+000002e0: 0101 0074 09a0 0a64 0ca1 0101 0074 02a0  ...t...d.....t..
+000002f0: 0364 0f7c 0416 00a1 0101 0067 007d 1374  .d.|.......g.}.t
+00000300: 0b7c 0483 0144 005d 6a7d 1474 02a0 0364  .|...D.]j}.t...d
+00000310: 107c 1416 00a1 0101 0074 0c7c 087c 1183  .|.......t.|.|..
+00000320: 027d 1574 0c7c 097c 1283 027d 1674 067c  .}.t.|.|...}.t.|
+00000330: 157c 1683 027d 177c 0364 0d6b 0390 0172  .|...}.|.d.k...r
+00000340: 6e7c 177c 0314 007d 1774 057c 157c 1683  n|.|...}.t.|.|..
+00000350: 025c 027d 187d 197c 027c 187c 197c 177c  .\.}.}.|.|.|.|.|
+00000360: 0683 047d 1a7c 13a0 0d7c 1aa1 0101 0090  ...}.|...|......
+00000370: 0171 2c74 0ea0 0f74 0ea0 107c 13a1 0164  .q,t...t...|...d
+00000380: 11a1 027d 1b74 0ea0 0f74 0ea0 107c 13a1  ...}.t...t...|..
+00000390: 0164 12a1 027d 1c64 137c 1b7c 1c66 0216  .d...}.d.|.|.f..
+000003a0: 007c 0764 143c 006e 1274 02a0 1164 15a1  .|.d.<.n.t...d..
+000003b0: 0101 0064 167c 0764 143c 0074 126a 137c  ...d.|.d.<.t.j.|
+000003c0: 0764 178d 0153 0029 1875 9e09 0000 0a09  .d...S.).u......
+000003d0: 4361 6c63 756c 6174 6520 7468 6520 666f  Calculate the fo
+000003e0: 6c6c 6f77 696e 6720 696e 6469 6365 733a  llowing indices:
+000003f0: 0a09 2d20 436f 6c6c 6f63 6174 696f 6e20  ..- Collocation 
+00000400: 636f 6566 6669 6369 656e 742c 0a09 2d20  coefficient,..- 
+00000410: 4a61 6363 6172 6427 7320 636f 6566 6669  Jaccard's coeffi
+00000420: 6369 656e 7420 2868 7474 7073 3a2f 2f65  cient (https://e
+00000430: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00000440: 7769 6b69 2f4a 6163 6361 7264 5f69 6e64  wiki/Jaccard_ind
+00000450: 6578 292c 0a09 2d20 537a 796d 6b69 6577  ex),..- Szymkiew
+00000460: 6963 7ae2 8093 5369 6d70 736f 6e20 636f  icz...Simpson co
+00000470: 6566 6669 6369 656e 742c 2028 6874 7470  efficient, (http
+00000480: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
+00000490: 2e6f 7267 2f77 696b 692f 4f76 6572 6c61  .org/wiki/Overla
+000004a0: 705f 636f 6566 6669 6369 656e 7429 2c0a  p_coefficient),.
+000004b0: 092d 2053 c3b8 7265 6e73 656e e280 9344  .- S..rensen...D
+000004c0: 6963 6520 636f 6566 6669 6369 656e 7420  ice coefficient 
+000004d0: 2868 7474 7073 3a2f 2f65 6e2e 7769 6b69  (https://en.wiki
+000004e0: 7065 6469 612e 6f72 672f 7769 6b69 2f53  pedia.org/wiki/S
+000004f0: c3b8 7265 6e73 656e e280 9344 6963 655f  ..rensen...Dice_
+00000500: 636f 6566 6669 6369 656e 7429 2c0a 092d  coefficient),..-
+00000510: 2050 6f69 6e74 7769 7365 206d 7574 7561   Pointwise mutua
+00000520: 6c20 696e 666f 726d 6174 696f 6e20 2868  l information (h
+00000530: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00000540: 6469 612e 6f72 672f 7769 6b69 2f50 6f69  dia.org/wiki/Poi
+00000550: 6e74 7769 7365 5f6d 7574 7561 6c5f 696e  ntwise_mutual_in
+00000560: 666f 726d 6174 696f 6e29 2c0a 0a09 5061  formation),...Pa
+00000570: 7261 6d65 7465 7273 0a09 2d2d 2d2d 2d2d  rameters..------
+00000580: 2d2d 2d2d 0a09 6669 6c65 3120 3a20 7374  ----..file1 : st
+00000590: 720a 0909 4765 6e6f 6d69 6320 7265 6769  r...Genomic regi
+000005a0: 6f6e 7320 696e 2042 4544 2028 4272 6f77  ons in BED (Brow
+000005b0: 7365 7220 4578 7465 6e73 6962 6c65 2044  ser Extensible D
+000005c0: 6174 612c 2068 7474 7073 3a2f 2f67 656e  ata, https://gen
+000005d0: 6f6d 652e 7563 7363 2e65 6475 2f46 4151  ome.ucsc.edu/FAQ
+000005e0: 2f46 4151 666f 726d 6174 2e68 746d 6c23  /FAQformat.html#
+000005f0: 666f 726d 6174 3129 2c20 4245 442d 6c69  format1), BED-li
+00000600: 6b65 206f 7220 4269 6742 6564 2066 6f72  ke or BigBed for
+00000610: 6d61 742e 0a09 0954 6865 2042 4544 2d6c  mat....The BED-l
+00000620: 696b 6520 666f 726d 6174 2069 6e63 6c75  ike format inclu
+00000630: 6465 7320 2762 6564 3327 2c27 6265 6434  des 'bed3','bed4
+00000640: 272c 2762 6564 3627 2c27 6265 6431 3227  ','bed6','bed12'
+00000650: 2c27 6265 6467 7261 7068 272c 276e 6172  ,'bedgraph','nar
+00000660: 726f 7770 6561 6b27 2c20 2762 726f 6164  rowpeak', 'broad
+00000670: 7065 616b 272c 2767 6170 7065 6470 6561  peak','gappedpea
+00000680: 6b27 2e20 4245 4420 616e 6420 4245 442d  k'. BED and BED-
+00000690: 6c69 6b65 0a09 0966 6f72 6d61 7420 6361  like...format ca
+000006a0: 6e20 6265 2070 6c61 696e 2074 6578 742c  n be plain text,
+000006b0: 2063 6f6d 7072 6573 7365 6420 282e 677a   compressed (.gz
+000006c0: 2c20 2e7a 2c20 2e62 7a2c 202e 627a 322c  , .z, .bz, .bz2,
+000006d0: 202e 627a 6970 3229 206f 7220 7265 6d6f   .bzip2) or remo
+000006e0: 7465 2028 6874 7470 3a2f 2f2c 2068 7474  te (http://, htt
+000006f0: 7073 3a2f 2f2c 2066 7470 3a2f 2f29 2066  ps://, ftp://) f
+00000700: 696c 6573 2e20 446f 206e 6f74 2063 6f6d  iles. Do not com
+00000710: 7072 6573 730a 0909 4269 6742 6564 2066  press...BigBed f
+00000720: 6f72 616d 742e 2042 6967 4265 6420 6669  oramt. BigBed fi
+00000730: 6c65 2063 616e 2061 6c73 6f20 6265 2061  le can also be a
+00000740: 2072 656d 6f74 6520 6669 6c65 2e0a 0966   remote file...f
+00000750: 696c 6532 203a 2073 7472 0a09 0947 656e  ile2 : str...Gen
+00000760: 6f6d 6963 2072 6567 696f 6e73 2069 6e20  omic regions in 
+00000770: 4245 4420 2842 726f 7773 6572 2045 7874  BED (Browser Ext
+00000780: 656e 7369 626c 6520 4461 7461 2c20 6874  ensible Data, ht
+00000790: 7470 733a 2f2f 6765 6e6f 6d65 2e75 6373  tps://genome.ucs
+000007a0: 632e 6564 752f 4641 512f 4641 5166 6f72  c.edu/FAQ/FAQfor
+000007b0: 6d61 742e 6874 6d6c 2366 6f72 6d61 7431  mat.html#format1
+000007c0: 292c 2042 4544 2d6c 696b 6520 6f72 2042  ), BED-like or B
+000007d0: 6967 4265 6420 666f 726d 6174 2e0a 0909  igBed format....
+000007e0: 5468 6520 4245 442d 6c69 6b65 2066 6f72  The BED-like for
+000007f0: 6d61 7420 696e 636c 7564 6573 2027 6265  mat includes 'be
+00000800: 6433 272c 2762 6564 3427 2c27 6265 6436  d3','bed4','bed6
+00000810: 272c 2762 6564 3132 272c 2762 6564 6772  ','bed12','bedgr
+00000820: 6170 6827 2c27 6e61 7272 6f77 7065 616b  aph','narrowpeak
+00000830: 272c 2027 6272 6f61 6470 6561 6b27 2c27  ', 'broadpeak','
+00000840: 6761 7070 6564 7065 616b 272e 2042 4544  gappedpeak'. BED
+00000850: 2061 6e64 2042 4544 2d6c 696b 650a 0909   and BED-like...
+00000860: 666f 726d 6174 2063 616e 2062 6520 706c  format can be pl
+00000870: 6169 6e20 7465 7874 2c20 636f 6d70 7265  ain text, compre
+00000880: 7373 6564 2028 2e67 7a2c 202e 7a2c 202e  ssed (.gz, .z, .
+00000890: 627a 2c20 2e62 7a32 2c20 2e62 7a69 7032  bz, .bz2, .bzip2
+000008a0: 2920 6f72 2072 656d 6f74 6520 2868 7474  ) or remote (htt
+000008b0: 703a 2f2f 2c20 6874 7470 733a 2f2f 2c20  p://, https://, 
+000008c0: 6674 703a 2f2f 2920 6669 6c65 732e 2044  ftp://) files. D
+000008d0: 6f20 6e6f 7420 636f 6d70 7265 7373 0a09  o not compress..
+000008e0: 0942 6967 4265 6420 666f 7261 6d74 2e20  .BigBed foramt. 
+000008f0: 4269 6742 6564 2066 696c 6520 6361 6e20  BigBed file can 
+00000900: 616c 736f 2062 6520 6120 7265 6d6f 7465  also be a remote
+00000910: 2066 696c 652e 0a09 7363 6f72 655f 6675   file...score_fu
+00000920: 6e63 203a 2066 756e 6374 696f 6e0a 0909  nc : function...
+00000930: 4675 6e63 7469 6f6e 2074 6f20 6361 6c63  Function to calc
+00000940: 756c 6174 6520 6f76 6572 6c61 7020 696e  ulate overlap in
+00000950: 6465 782e 2049 6e63 6c75 6465 206f 765f  dex. Include ov_
+00000960: 636f 6566 2c20 6f76 5f6a 6163 6361 7264  coef, ov_jaccard
+00000970: 2c20 6f76 5f73 732c 206f 765f 7364 2c20  , ov_ss, ov_sd, 
+00000980: 706d 695f 7661 6c75 652c 206e 706d 695f  pmi_value, npmi_
+00000990: 7661 6c75 650a 096e 5f64 7261 7773 203a  value..n_draws :
+000009a0: 2069 6e74 0a09 0954 696d 6573 206f 6620   int...Times of 
+000009b0: 6472 6177 696e 6720 7361 6d70 6c65 7320  drawing samples 
+000009c0: 7769 7468 2072 6570 6c61 6365 6d65 6e74  with replacement
+000009d0: 2e20 5365 7420 746f 2027 3027 2074 6f20  . Set to '0' to 
+000009e0: 7475 726e 206f 6666 2062 6f6f 7473 7472  turn off bootstr
+000009f0: 6170 696e 672e 2020 5468 6520 6465 6661  aping.  The defa
+00000a00: 756c 7420 6973 2032 302e 0a09 6672 6163  ult is 20...frac
+00000a10: 7469 6f6e 203a 2066 6c6f 6174 2c20 6f70  tion : float, op
+00000a20: 7469 6f6e 616c 0a09 0954 6865 2066 7261  tional...The fra
+00000a30: 6374 696f 6e20 6f66 2073 7562 7361 6d70  ction of subsamp
+00000a40: 6c65 2e20 5468 6520 6465 6661 756c 7420  le. The default 
+00000a50: 6973 2030 2e37 3520 2837 3525 206f 6620  is 0.75 (75% of 
+00000a60: 7468 6520 6f72 6967 6e61 6c20 6765 6e6f  the orignal geno
+00000a70: 6d69 6320 7265 6769 6e6f 7320 7769 6c6c  mic reginos will
+00000a80: 2062 6520 7365 6c65 6374 6564 292e 0a09   be selected)...
+00000a90: 6267 5f73 697a 6520 3a20 696e 742c 206f  bg_size : int, o
+00000aa0: 7074 696f 6e61 6c0a 0909 5468 6520 6566  ptional...The ef
+00000ab0: 6665 6374 6976 6520 6261 636b 6772 6f75  fective backgrou
+00000ac0: 6e64 2067 656e 6f6d 6520 7369 7a65 2e20  nd genome size. 
+00000ad0: 4162 6f75 7420 312e 3447 6220 6f66 2074  About 1.4Gb of t
+00000ae0: 6865 2068 756d 616e 2067 656e 6f6d 6520  he human genome 
+00000af0: 6172 652e 2054 6865 2064 6566 6175 6c74  are. The default
+00000b00: 2069 7320 312e 3465 392e 0a09 0a09 4e6f   is 1.4e9.....No
+00000b10: 7465 0a09 2d2d 2d2d 0a09 0946 6f72 2074  te..----...For t
+00000b20: 6865 2062 6f6f 7473 7472 6170 2070 726f  he bootstrap pro
+00000b30: 6365 7373 2077 6f72 6b73 2070 726f 7065  cess works prope
+00000b40: 726c 792c 2074 6865 206f 7665 726c 6170  rly, the overlap
+00000b50: 7065 6420 6765 6e6f 6d69 6320 696e 7465  ped genomic inte
+00000b60: 7276 616c 7320 696e 2066 696c 6531 2061  rvals in file1 a
+00000b70: 6e64 2066 696c 6532 206d 7573 7420 6265  nd file2 must be
+00000b80: 206d 6572 6765 642e 0a09 5265 7475 726e   merged...Return
+00000b90: 730a 092d 2d2d 2d2d 2d2d 0a09 7061 6e64  s..-------..pand
+00000ba0: 6173 2e53 6572 6965 730a 0909 5061 6e64  as.Series...Pand
+00000bb0: 6173 2053 6572 6965 7320 6f66 2027 636f  as Series of 'co
+00000bc0: 6566 5f6f 6273 272c 2027 636f 6566 5f65  ef_obs', 'coef_e
+00000bd0: 7870 272c 2763 6f65 665f 7261 7469 6f27  xp','coef_ratio'
+00000be0: 2c20 2763 6f65 665f 7261 7469 6f5f 6c6f  , 'coef_ratio_lo
+00000bf0: 7727 2c20 2763 6f65 665f 7261 7469 6f5f  w', 'coef_ratio_
+00000c00: 6869 6768 272e 0a09 0927 636f 6566 5f6f  high'....'coef_o
+00000c10: 6273 2720 3a20 4f62 7365 7276 6564 206f  bs' : Observed o
+00000c20: 7665 726c 6170 2063 6f65 6666 6963 6965  verlap coefficie
+00000c30: 6e74 2062 6574 7765 656e 2074 776f 2042  nt between two B
+00000c40: 4544 2066 696c 6573 2e0a 0909 2763 6f65  ED files....'coe
+00000c50: 665f 6578 7027 203a 2045 7870 6563 7465  f_exp' : Expecte
+00000c60: 6420 6f76 6572 6c61 7020 636f 6566 6669  d overlap coeffi
+00000c70: 6369 656e 7420 6265 7477 6565 6e20 7477  cient between tw
+00000c80: 6f20 4245 4420 6669 6c65 732e 0a09 0927  o BED files....'
+00000c90: 636f 6566 5f72 6174 696f 2720 3a20 5261  coef_ratio' : Ra
+00000ca0: 7469 6f20 6265 7477 6565 6e20 2763 6f65  tio between 'coe
+00000cb0: 665f 6f62 7327 2061 6e64 2027 636f 6566  f_obs' and 'coef
+00000cc0: 5f65 7870 272e 0a09 0927 636f 6566 5f72  _exp'....'coef_r
+00000cd0: 6174 696f 5f6c 6f77 2720 3a20 5468 6520  atio_low' : The 
+00000ce0: 6c6f 7765 7220 626f 756e 6420 6f66 2039  lower bound of 9
+00000cf0: 3525 2063 6f6e 6669 6465 6e63 6520 696e  5% confidence in
+00000d00: 7465 7276 616c 206f 6620 2763 6f65 665f  terval of 'coef_
+00000d10: 7261 7469 6f27 2e0a 0909 2763 6f65 665f  ratio'....'coef_
+00000d20: 7261 7469 6f5f 6869 6768 2720 3a20 5468  ratio_high' : Th
+00000d30: 6520 7570 7065 7220 626f 756e 6420 6f66  e upper bound of
+00000d40: 2039 3525 2063 6f6e 6669 6465 6e63 6520   95% confidence 
+00000d50: 696e 7465 7276 616c 206f 6620 2763 6f65  interval of 'coe
+00000d60: 665f 7261 7469 6f27 2e0a 0a09 fa06 412e  f_ratio'......A.
+00000d70: 6e61 6d65 fa06 422e 6e61 6d65 fa1a 4361  name..B.name..Ca
+00000d80: 6c63 756c 6174 696e 6720 6265 6420 636f  lculating bed co
+00000d90: 756e 7473 202e 2e2e fa10 412e 696e 7465  unts .....A.inte
+00000da0: 7276 616c 5f63 6f75 6e74 fa10 422e 696e  rval_count..B.in
+00000db0: 7465 7276 616c 5f63 6f75 6e74 fa06 412e  terval_count..A.
+00000dc0: 7369 7a65 fa06 422e 7369 7a65 fa0b 415f  size..B.size..A_
+00000dd0: 6f72 5f42 2e73 697a 65fa 0c41 5f61 6e64  or_B.size..A_and
+00000de0: 5f42 2e73 697a 65da 0443 6f65 66fa 0e43  _B.size..Coef..C
+00000df0: 6f65 6628 6578 7065 6374 6564 2972 0100  oef(expected)r..
+00000e00: 0000 e901 0000 00fa 1d46 7261 6374 696f  .........Fractio
+00000e10: 6e20 6d75 7374 2062 6520 3e20 3020 616e  n must be > 0 an
+00000e20: 6420 3c20 312e fa26 426f 6f74 7374 7261  d < 1..&Bootstra
+00000e30: 7069 6e67 2069 7320 6f6e 2e20 4974 6572  ping is on. Iter
+00000e40: 6174 6520 2564 2074 696d 6573 2e20 fa1b  ate %d times. ..
+00000e50: 426f 6f74 7374 7261 7020 7265 7361 6d70  Bootstrap resamp
+00000e60: 6c69 6e67 2025 6420 2e2e 2ee7 0000 0000  ling %d ........
+00000e70: 0000 0440 e700 0000 0000 6058 40fa 0b5b  ...@......`X@..[
+00000e80: 252e 3466 2c25 2e34 665d fa0c 436f 6566  %.4f,%.4f]..Coef
+00000e90: 2839 3525 2043 4929 fa17 426f 6f74 7374  (95% CI)..Bootst
+00000ea0: 7261 7069 6e67 2069 7320 6f66 6620 2e2e  raping is off ..
+00000eb0: 2efa 075b 4e41 2c4e 415d a901 da04 6461  ...[NA,NA]....da
+00000ec0: 7461 a914 7204 0000 0072 0600 0000 da07  ta..r....r......
+00000ed0: 6c6f 6767 696e 67da 0564 6562 7567 7205  logging..debugr.
+00000ee0: 0000 0072 0200 0000 7203 0000 00da 0369  ...r....r......i
+00000ef0: 6e74 da05 6572 726f 72da 0373 7973 da04  nt..error..sys..
+00000f00: 6578 6974 da05 7261 6e67 6572 0700 0000  exit..ranger....
+00000f10: da06 6170 7065 6e64 da02 6e70 da0a 7065  ..append..np..pe
+00000f20: 7263 656e 7469 6c65 da05 6172 7261 79da  rcentile..array.
+00000f30: 0469 6e66 6fda 0270 64da 0653 6572 6965  .info..pd..Serie
+00000f40: 73a9 1dda 0566 696c 6531 da05 6669 6c65  s....file1..file
+00000f50: 32da 0a73 636f 7265 5f66 756e 63da 0b73  2..score_func..s
+00000f60: 697a 655f 6661 6374 6f72 da07 6e5f 6472  ize_factor..n_dr
+00000f70: 6177 73da 0866 7261 6374 696f 6eda 0762  aws..fraction..b
+00000f80: 675f 7369 7a65 da07 7265 7375 6c74 73da  g_size..results.
+00000f90: 0966 696c 6531 5f6c 7374 da09 6669 6c65  .file1_lst..file
+00000fa0: 325f 6c73 745a 0b74 6f74 616c 436f 756e  2_lstZ.totalCoun
+00000fb0: 7431 5a0b 746f 7461 6c43 6f75 6e74 32da  t1Z.totalCount2.
+00000fc0: 0975 6e69 7142 6173 6531 da09 756e 6971  .uniqBase1..uniq
+00000fd0: 4261 7365 32da 0c6f 7665 726c 6170 4261  Base2..overlapBa
+00000fe0: 7365 735a 106f 7665 726c 6170 4261 7365  sesZ.overlapBase
+00000ff0: 735f 6578 705a 0a75 6e69 6f6e 4261 7365  s_expZ.unionBase
+00001000: 735a 0e72 6573 616d 706c 655f 7369 7a65  sZ.resample_size
+00001010: 315a 0e72 6573 616d 706c 655f 7369 7a65  1Z.resample_size
+00001020: 32da 0374 6d70 da01 695a 0873 616d 706c  2..tmp..iZ.sampl
+00001030: 655f 315a 0873 616d 706c 655f 325a 1373  e_1Z.sample_2Z.s
+00001040: 616d 706c 655f 6f76 6572 6c61 7042 6173  ample_overlapBas
+00001050: 6573 5a0c 7361 6d70 6c65 315f 7369 7a65  esZ.sample1_size
+00001060: 5a0c 7361 6d70 6c65 325f 7369 7a65 5a0d  Z.sample2_sizeZ.
+00001070: 7361 6d70 6c65 5f6f 7663 6f65 665a 0863  sample_ovcoefZ.c
+00001080: 695f 6c6f 7765 725a 0863 695f 7570 7065  i_lowerZ.ci_uppe
+00001090: 72a9 0072 4500 0000 fa47 2f55 7365 7273  r..rE....G/Users
+000010a0: 2f6d 3130 3233 3234 2f44 6f63 756d 656e  /m102324/Documen
+000010b0: 7473 2f47 6974 4875 622f 636f 6269 6e64  ts/GitHub/cobind
+000010c0: 2f6c 6962 2f63 6f62 696e 6461 6269 6c69  /lib/cobindabili
+000010d0: 7479 2f6f 7662 6f6f 7473 7472 6170 2e70  ty/ovbootstrap.p
+000010e0: 79da 0e62 6f6f 7473 7472 6170 5f63 6f65  y..bootstrap_coe
+000010f0: 661e 0000 0073 5600 0000 002d 0402 0801  f....sV....-....
+00001100: 0802 0c01 0c03 0a01 0e01 0801 0805 0e03  ................
+00001110: 0a01 0c01 0e02 0801 0801 0801 0801 1201  ................
+00001120: 1202 0a01 1001 0c01 0e02 0a01 0a01 0e01  ................
+00001130: 0401 0c01 0e01 0a01 0a02 0a01 0a01 0801  ................
+00001140: 0e01 0e01 0e01 1201 1201 1202 0a01 0802  ................
+00001150: 7247 0000 0063 0700 0000 0000 0000 0000  rG...c..........
+00001160: 0000 1d00 0000 0700 0000 4300 0000 73f0  ..........C...s.
+00001170: 0100 0069 007d 0774 007c 0083 017d 0874  ...i.}.t.|...}.t
+00001180: 007c 0183 017d 0974 017c 0083 017c 0764  .|...}.t.|...|.d
+00001190: 013c 0074 017c 0183 017c 0764 023c 0074  .<.t.|...|.d.<.t
+000011a0: 02a0 0364 03a1 0101 0074 047c 007c 0183  ...d.....t.|.|..
+000011b0: 025c 027d 0a7d 0b7c 0a7c 0764 043c 007c  .\.}.}.|.|.d.<.|
+000011c0: 0b7c 0764 053c 0074 057c 087c 0983 025c  .|.d.<.t.|.|...\
+000011d0: 027d 0c7d 0d74 067c 087c 0983 027d 0e7c  .}.}.t.|.|...}.|
+000011e0: 0c7c 0d14 007c 061b 007d 0f74 057c 087c  .|...|...}.t.|.|
+000011f0: 0917 0083 015c 017d 107c 0c7c 0764 063c  .....\.}.|.|.d.<
+00001200: 007c 0d7c 0764 073c 007c 107c 0764 083c  .|.|.d.<.|.|.d.<
+00001210: 007c 0e7c 0764 093c 007c 027c 0c7c 0d7c  .|.|.d.<.|.|.|.|
+00001220: 0e7c 0683 047c 0764 0a3c 007c 027c 0c7c  .|...|.d.<.|.|.|
+00001230: 0d7c 0f7c 0683 047c 0764 0b3c 007c 0464  .|.|...|.d.<.|.d
+00001240: 0c6b 0490 0172 d27c 0564 0c6b 0472 fe7c  .k...r.|.d.k.r.|
+00001250: 0564 0d6b 0072 fe74 077c 0a7c 0514 0083  .d.k.r.t.|.|....
+00001260: 017d 1174 077c 0b7c 0514 0083 017d 126e  .}.t.|.|.....}.n
+00001270: 1474 02a0 0864 0ea1 0101 0074 09a0 0a64  .t...d.....t...d
+00001280: 0ca1 0101 0074 02a0 0364 0f7c 0416 00a1  .....t...d.|....
+00001290: 0101 0067 007d 1374 0b7c 0483 0144 005d  ...g.}.t.|...D.]
+000012a0: 6e7d 1474 02a0 0364 107c 1416 00a1 0101  n}.t...d.|......
+000012b0: 0074 0c7c 087c 1183 027d 1574 0c7c 097c  .t.|.|...}.t.|.|
+000012c0: 1283 027d 1674 067c 157c 1683 027d 177c  ...}.t.|.|...}.|
+000012d0: 0364 0d6b 0390 0172 6e7c 177c 0314 007d  .d.k...rn|.|...}
+000012e0: 1774 057c 157c 1683 025c 027d 187d 197c  .t.|.|...\.}.}.|
+000012f0: 027c 187c 197c 177c 067c 0514 0083 047d  .|.|.|.|.|.....}
+00001300: 1a7c 13a0 0d7c 1aa1 0101 0090 0171 2c74  .|...|.......q,t
+00001310: 0ea0 0f74 0ea0 107c 13a1 0164 11a1 027d  ...t...|...d...}
+00001320: 1b74 0ea0 0f74 0ea0 107c 13a1 0164 12a1  .t...t...|...d..
+00001330: 027d 1c64 137c 1b7c 1c66 0216 007c 0764  .}.d.|.|.f...|.d
+00001340: 143c 006e 1274 02a0 1164 15a1 0101 0064  .<.n.t...d.....d
+00001350: 167c 0764 143c 0074 126a 137c 0764 178d  .|.d.<.t.j.|.d..
+00001360: 0153 0029 1861 d207 0000 0a09 4361 6c63  .S.).a......Calc
+00001370: 756c 6174 6520 7468 6520 666f 6c6c 6f77  ulate the follow
+00001380: 696e 6720 696e 6469 6365 733a 0a09 2d20  ing indices:..- 
+00001390: 4e6f 726d 616c 697a 6564 2070 6f69 6e74  Normalized point
+000013a0: 7769 7365 206d 7574 7561 6c20 696e 666f  wise mutual info
+000013b0: 726d 6174 696f 6e2e 0a0a 0950 6172 616d  rmation....Param
+000013c0: 6574 6572 730a 092d 2d2d 2d2d 2d2d 2d2d  eters..---------
+000013d0: 2d0a 0966 696c 6531 203a 2073 7472 0a09  -..file1 : str..
+000013e0: 0947 656e 6f6d 6963 2072 6567 696f 6e73  .Genomic regions
+000013f0: 2069 6e20 4245 4420 2842 726f 7773 6572   in BED (Browser
+00001400: 2045 7874 656e 7369 626c 6520 4461 7461   Extensible Data
+00001410: 2c20 6874 7470 733a 2f2f 6765 6e6f 6d65  , https://genome
+00001420: 2e75 6373 632e 6564 752f 4641 512f 4641  .ucsc.edu/FAQ/FA
+00001430: 5166 6f72 6d61 742e 6874 6d6c 2366 6f72  Qformat.html#for
+00001440: 6d61 7431 292c 2042 4544 2d6c 696b 6520  mat1), BED-like 
+00001450: 6f72 2042 6967 4265 6420 666f 726d 6174  or BigBed format
+00001460: 2e0a 0909 5468 6520 4245 442d 6c69 6b65  ....The BED-like
+00001470: 2066 6f72 6d61 7420 696e 636c 7564 6573   format includes
+00001480: 2027 6265 6433 272c 2762 6564 3427 2c27   'bed3','bed4','
+00001490: 6265 6436 272c 2762 6564 3132 272c 2762  bed6','bed12','b
+000014a0: 6564 6772 6170 6827 2c27 6e61 7272 6f77  edgraph','narrow
+000014b0: 7065 616b 272c 2027 6272 6f61 6470 6561  peak', 'broadpea
+000014c0: 6b27 2c27 6761 7070 6564 7065 616b 272e  k','gappedpeak'.
+000014d0: 2042 4544 2061 6e64 2042 4544 2d6c 696b   BED and BED-lik
+000014e0: 650a 0909 666f 726d 6174 2063 616e 2062  e...format can b
+000014f0: 6520 706c 6169 6e20 7465 7874 2c20 636f  e plain text, co
+00001500: 6d70 7265 7373 6564 2028 2e67 7a2c 202e  mpressed (.gz, .
+00001510: 7a2c 202e 627a 2c20 2e62 7a32 2c20 2e62  z, .bz, .bz2, .b
+00001520: 7a69 7032 2920 6f72 2072 656d 6f74 6520  zip2) or remote 
+00001530: 2868 7474 703a 2f2f 2c20 6874 7470 733a  (http://, https:
+00001540: 2f2f 2c20 6674 703a 2f2f 2920 6669 6c65  //, ftp://) file
+00001550: 732e 2044 6f20 6e6f 7420 636f 6d70 7265  s. Do not compre
+00001560: 7373 0a09 0942 6967 4265 6420 666f 7261  ss...BigBed fora
+00001570: 6d74 2e20 4269 6742 6564 2066 696c 6520  mt. BigBed file 
+00001580: 6361 6e20 616c 736f 2062 6520 6120 7265  can also be a re
+00001590: 6d6f 7465 2066 696c 652e 0a09 6669 6c65  mote file...file
+000015a0: 3220 3a20 7374 720a 0909 4765 6e6f 6d69  2 : str...Genomi
+000015b0: 6320 7265 6769 6f6e 7320 696e 2042 4544  c regions in BED
+000015c0: 2028 4272 6f77 7365 7220 4578 7465 6e73   (Browser Extens
+000015d0: 6962 6c65 2044 6174 612c 2068 7474 7073  ible Data, https
+000015e0: 3a2f 2f67 656e 6f6d 652e 7563 7363 2e65  ://genome.ucsc.e
+000015f0: 6475 2f46 4151 2f46 4151 666f 726d 6174  du/FAQ/FAQformat
+00001600: 2e68 746d 6c23 666f 726d 6174 3129 2c20  .html#format1), 
+00001610: 4245 442d 6c69 6b65 206f 7220 4269 6742  BED-like or BigB
+00001620: 6564 2066 6f72 6d61 742e 0a09 0954 6865  ed format....The
+00001630: 2042 4544 2d6c 696b 6520 666f 726d 6174   BED-like format
+00001640: 2069 6e63 6c75 6465 7320 2762 6564 3327   includes 'bed3'
+00001650: 2c27 6265 6434 272c 2762 6564 3627 2c27  ,'bed4','bed6','
+00001660: 6265 6431 3227 2c27 6265 6467 7261 7068  bed12','bedgraph
+00001670: 272c 276e 6172 726f 7770 6561 6b27 2c20  ','narrowpeak', 
+00001680: 2762 726f 6164 7065 616b 272c 2767 6170  'broadpeak','gap
+00001690: 7065 6470 6561 6b27 2e20 4245 4420 616e  pedpeak'. BED an
+000016a0: 6420 4245 442d 6c69 6b65 0a09 0966 6f72  d BED-like...for
+000016b0: 6d61 7420 6361 6e20 6265 2070 6c61 696e  mat can be plain
+000016c0: 2074 6578 742c 2063 6f6d 7072 6573 7365   text, compresse
+000016d0: 6420 282e 677a 2c20 2e7a 2c20 2e62 7a2c  d (.gz, .z, .bz,
+000016e0: 202e 627a 322c 202e 627a 6970 3229 206f   .bz2, .bzip2) o
+000016f0: 7220 7265 6d6f 7465 2028 6874 7470 3a2f  r remote (http:/
+00001700: 2f2c 2068 7474 7073 3a2f 2f2c 2066 7470  /, https://, ftp
+00001710: 3a2f 2f29 2066 696c 6573 2e20 446f 206e  ://) files. Do n
+00001720: 6f74 2063 6f6d 7072 6573 730a 0909 4269  ot compress...Bi
+00001730: 6742 6564 2066 6f72 616d 742e 2042 6967  gBed foramt. Big
+00001740: 4265 6420 6669 6c65 2063 616e 2061 6c73  Bed file can als
+00001750: 6f20 6265 2061 2072 656d 6f74 6520 6669  o be a remote fi
+00001760: 6c65 2e0a 0973 636f 7265 5f66 756e 6320  le...score_func 
+00001770: 3a20 6675 6e63 7469 6f6e 0a09 0946 756e  : function...Fun
+00001780: 6374 696f 6e20 746f 2063 616c 6375 6c61  ction to calcula
+00001790: 7465 206f 7665 726c 6170 2069 6e64 6578  te overlap index
+000017a0: 2e20 496e 636c 7564 6520 6f76 5f63 6f65  . Include ov_coe
+000017b0: 662c 206f 765f 6a61 6363 6172 642c 206f  f, ov_jaccard, o
+000017c0: 765f 7373 2c20 6f76 5f73 642c 2070 6d69  v_ss, ov_sd, pmi
+000017d0: 5f76 616c 7565 2c20 6e70 6d69 5f76 616c  _value, npmi_val
+000017e0: 7565 0a09 6e5f 6472 6177 7320 3a20 696e  ue..n_draws : in
+000017f0: 740a 0909 5469 6d65 7320 6f66 2064 7261  t...Times of dra
+00001800: 7769 6e67 2073 616d 706c 6573 2077 6974  wing samples wit
+00001810: 6820 7265 706c 6163 656d 656e 742e 2053  h replacement. S
+00001820: 6574 2074 6f20 2730 2720 746f 2074 7572  et to '0' to tur
+00001830: 6e20 6f66 6620 626f 6f74 7374 7261 7069  n off bootstrapi
+00001840: 6e67 2e20 2054 6865 2064 6566 6175 6c74  ng.  The default
+00001850: 2069 7320 3230 2e0a 0966 7261 6374 696f   is 20...fractio
+00001860: 6e20 3a20 666c 6f61 742c 206f 7074 696f  n : float, optio
+00001870: 6e61 6c0a 0909 5468 6520 6672 6163 7469  nal...The fracti
+00001880: 6f6e 206f 6620 7375 6273 616d 706c 652e  on of subsample.
+00001890: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
+000018a0: 302e 3735 2028 3735 2520 6f66 2074 6865  0.75 (75% of the
+000018b0: 206f 7269 676e 616c 2067 656e 6f6d 6963   orignal genomic
+000018c0: 2072 6567 696e 6f73 2077 696c 6c20 6265   reginos will be
+000018d0: 2073 656c 6563 7465 6429 2e0a 0962 675f   selected)...bg_
+000018e0: 7369 7a65 203a 2069 6e74 2c20 6f70 7469  size : int, opti
+000018f0: 6f6e 616c 0a09 0954 6865 2065 6666 6563  onal...The effec
+00001900: 7469 7665 2062 6163 6b67 726f 756e 6420  tive background 
+00001910: 6765 6e6f 6d65 2073 697a 652e 2041 626f  genome size. Abo
+00001920: 7574 2031 2e34 4762 206f 6620 7468 6520  ut 1.4Gb of the 
+00001930: 6875 6d61 6e20 6765 6e6f 6d65 2061 7265  human genome are
+00001940: 2e20 5468 6520 6465 6661 756c 7420 6973  . The default is
+00001950: 2031 2e34 6539 2e0a 0a09 5265 7475 726e   1.4e9....Return
+00001960: 730a 092d 2d2d 2d2d 2d2d 0a09 7061 6e64  s..-------..pand
+00001970: 6173 2e53 6572 6965 730a 0909 5061 6e64  as.Series...Pand
+00001980: 6173 2053 6572 6965 7320 6f66 2027 636f  as Series of 'co
+00001990: 6566 5f6f 6273 272c 2027 636f 6566 5f65  ef_obs', 'coef_e
+000019a0: 7870 272c 2763 6f65 665f 7261 7469 6f27  xp','coef_ratio'
+000019b0: 2c20 2763 6f65 665f 7261 7469 6f5f 6c6f  , 'coef_ratio_lo
+000019c0: 7727 2c20 2763 6f65 665f 7261 7469 6f5f  w', 'coef_ratio_
+000019d0: 6869 6768 272e 0a09 0927 636f 6566 5f6f  high'....'coef_o
+000019e0: 6273 2720 3a20 4f62 7365 7276 6564 206f  bs' : Observed o
+000019f0: 7665 726c 6170 2063 6f65 6666 6963 6965  verlap coefficie
+00001a00: 6e74 2062 6574 7765 656e 2074 776f 2042  nt between two B
+00001a10: 4544 2066 696c 6573 2e0a 0909 2763 6f65  ED files....'coe
+00001a20: 665f 6578 7027 203a 2045 7870 6563 7465  f_exp' : Expecte
+00001a30: 6420 6f76 6572 6c61 7020 636f 6566 6669  d overlap coeffi
+00001a40: 6369 656e 7420 6265 7477 6565 6e20 7477  cient between tw
+00001a50: 6f20 4245 4420 6669 6c65 732e 0a09 0927  o BED files....'
+00001a60: 636f 6566 5f72 6174 696f 2720 3a20 5261  coef_ratio' : Ra
+00001a70: 7469 6f20 6265 7477 6565 6e20 2763 6f65  tio between 'coe
+00001a80: 665f 6f62 7327 2061 6e64 2027 636f 6566  f_obs' and 'coef
+00001a90: 5f65 7870 272e 0a09 0927 636f 6566 5f72  _exp'....'coef_r
+00001aa0: 6174 696f 5f6c 6f77 2720 3a20 5468 6520  atio_low' : The 
+00001ab0: 6c6f 7765 7220 626f 756e 6420 6f66 2039  lower bound of 9
+00001ac0: 3525 2063 6f6e 6669 6465 6e63 6520 696e  5% confidence in
+00001ad0: 7465 7276 616c 206f 6620 2763 6f65 665f  terval of 'coef_
+00001ae0: 7261 7469 6f27 2e0a 0909 2763 6f65 665f  ratio'....'coef_
+00001af0: 7261 7469 6f5f 6869 6768 2720 3a20 5468  ratio_high' : Th
+00001b00: 6520 7570 7065 7220 626f 756e 6420 6f66  e upper bound of
+00001b10: 2039 3525 2063 6f6e 6669 6465 6e63 6520   95% confidence 
+00001b20: 696e 7465 7276 616c 206f 6620 2763 6f65  interval of 'coe
+00001b30: 665f 7261 7469 6f27 2e0a 0a09 720f 0000  f_ratio'....r...
+00001b40: 0072 1000 0000 7211 0000 0072 1200 0000  .r....r....r....
+00001b50: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00001b60: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00001b70: 0000 0072 0100 0000 721a 0000 0072 1b00  ...r....r....r..
+00001b80: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00001b90: 0072 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00001ba0: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00001bb0: 2600 0000 7235 0000 0072 4500 0000 7245  &...r5...rE...rE
+00001bc0: 0000 0072 4600 0000 da0e 626f 6f74 7374  ...rF.....bootst
+00001bd0: 7261 705f 6e70 6d69 8800 0000 7356 0000  rap_npmi....sV..
+00001be0: 0000 2604 0208 0108 020c 010c 030a 010e  ..&.............
+00001bf0: 0108 0108 050e 030a 010c 010e 0208 0108  ................
+00001c00: 0108 0108 0112 0112 020a 0110 010c 010e  ................
+00001c10: 020a 010a 010e 0104 010c 010e 010a 010a  ................
+00001c20: 020a 010a 0108 010e 0112 010e 0112 0112  ................
+00001c30: 0112 020a 0108 0272 4800 0000 2903 720c  .......rH...).r.
+00001c40: 0000 0072 0d00 0000 720e 0000 0029 0372  ...r....r....).r
+00001c50: 0c00 0000 720d 0000 0072 0e00 0000 291c  ....r....r....).
+00001c60: da07 5f5f 646f 635f 5f72 2b00 0000 da11  ..__doc__r+.....
+00001c70: 636f 6269 6e64 6162 696c 6974 792e 4245  cobindability.BE
+00001c80: 4472 0200 0000 7203 0000 0072 0400 0000  Dr....r....r....
+00001c90: 7205 0000 00da 076f 732e 7061 7468 7206  r......os.pathr.
+00001ca0: 0000 0072 2700 0000 da05 6e75 6d70 7972  ...r'.....numpyr
+00001cb0: 2f00 0000 da06 7061 6e64 6173 7233 0000  /.....pandasr3..
+00001cc0: 00da 0672 616e 646f 6d72 0700 0000 da0d  ...randomr......
+00001cd0: 636f 6269 6e64 6162 696c 6974 7972 0800  cobindabilityr..
+00001ce0: 0000 da0a 5f5f 6175 7468 6f72 5f5f da0d  ....__author__..
+00001cf0: 5f5f 636f 7079 7269 6768 745f 5fda 0b5f  __copyright__.._
+00001d00: 5f63 7265 6469 7473 5f5f da0b 5f5f 6c69  _credits__..__li
+00001d10: 6365 6e73 655f 5fda 0b5f 5f76 6572 7369  cense__..__versi
+00001d20: 6f6e 5f5f da0e 5f5f 6d61 696e 7461 696e  on__..__maintain
+00001d30: 6572 5f5f da09 5f5f 656d 6169 6c5f 5fda  er__..__email__.
+00001d40: 0a5f 5f73 7461 7475 735f 5f72 4700 0000  .__status__rG...
+00001d50: 7248 0000 0072 4500 0000 7245 0000 0072  rH...rE...rE...r
+00001d60: 4500 0000 7246 0000 00da 083c 6d6f 6475  E...rF.....<modu
+00001d70: 6c65 3e03 0000 0073 2400 0000 0406 0801  le>....s$.......
+00001d80: 1802 0c01 0801 0801 0801 0c01 0c03 0401  ................
+00001d90: 0401 0401 0401 0601 0401 0401 0403 0a6a  ...............j
```

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ovcoef.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ovcoef.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ovjaccard.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ovjaccard.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ovpmi.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ovpmi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/__pycache__/ovstat.cpython-38.pyc` & `cobind-1.0.1/lib/cobindability/__pycache__/ovstat.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jan 15 03:58:05 2022 UTC, .py size: 4963 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 4d46 e261 6313 0000  U.......MF.ac...
+00000000: 550d 0d0a 0000 0000 e893 c962 7c13 0000  U..........b|...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100 6401  m.Z.m.Z.m.Z...d.
@@ -14,264 +14,265 @@
 000000d0: 6501 6a1d 6412 1900 6501 6a1d 6413 1900  e.j.d...e.j.d...
 000000e0: 8302 5a1e 651f 651e 8301 0100 6402 5300  ..Z.e.e.....d.S.
 000000f0: 2915 7a37 0a43 7265 6174 6564 206f 6e20  ).z7.Created on 
 00000100: 5475 6520 4a61 6e20 3131 2031 343a 3137  Tue Jan 11 14:17
 00000110: 3a35 3020 3230 3232 0a0a 4061 7574 686f  :50 2022..@autho
 00000120: 723a 206d 3130 3233 3234 0ae9 0000 0000  r: m102324......
 00000130: 4e29 03da 1062 6564 5f6f 7665 726c 6170  N)...bed_overlap
-00000140: 5f73 697a 65da 0962 6564 746f 6c69 7374  _size..bedtolist
-00000150: da07 6265 6469 6e66 6f29 06da 076f 765f  ..bedinfo)...ov_
-00000160: 636f 6566 da0a 6f76 5f6a 6163 6361 7264  coef..ov_jaccard
-00000170: da05 6f76 5f73 73da 056f 765f 7364 da09  ..ov_ss..ov_sd..
-00000180: 706d 695f 7661 6c75 65da 0a6e 706d 695f  pmi_value..npmi_
-00000190: 7661 6c75 6529 01da 0776 6572 7369 6f6e  value)...version
-000001a0: 7a0a 4c69 6775 6f20 5761 6e67 da08 436f  z.Liguo Wang..Co
-000001b0: 7079 6c65 6674 da03 4d49 547a 1377 616e  pyleft..MITz.wan
-000001c0: 672e 6c69 6775 6f40 6d61 796f 2e65 6475  g.liguo@mayo.edu
-000001d0: da0b 4465 7665 6c6f 706d 656e 74e9 004e  ..Development..N
-000001e0: 7253 6303 0000 0000 0000 0000 0000 000b  rSc.............
-000001f0: 0000 0005 0000 0043 0000 0073 2002 0000  .......C...s ...
-00000200: 6900 7d03 7400 7c00 8301 7d04 7400 7c01  i.}.t.|...}.t.|.
-00000210: 8301 7d05 7401 a002 6401 7c00 1600 a101  ..}.t...d.|.....
-00000220: 0100 7403 7c00 8301 7d06 7c06 6402 1900  ..t.|...}.|.d...
-00000230: 7c03 6403 3c00 7c06 6404 1900 7c03 6405  |.d.<.|.d...|.d.
-00000240: 3c00 7c06 6406 1900 7c03 6407 3c00 7c06  <.|.d...|.d.<.|.
-00000250: 6408 1900 7c03 6409 3c00 7c06 640a 1900  d...|.d.<.|.d...
-00000260: 7c03 640b 3c00 7c06 640c 1900 7c03 640d  |.d.<.|.d...|.d.
-00000270: 3c00 7c06 640e 1900 7c03 640f 3c00 7c06  <.|.d...|.d.<.|.
-00000280: 6410 1900 7c03 6411 3c00 7c06 6412 1900  d...|.d.<.|.d...
-00000290: 7d07 7401 a002 6401 7c01 1600 a101 0100  }.t...d.|.......
-000002a0: 7403 7c01 8301 7d08 7c08 6402 1900 7c03  t.|...}.|.d...|.
-000002b0: 6413 3c00 7c08 6404 1900 7c03 6414 3c00  d.<.|.d...|.d.<.
-000002c0: 7c08 6406 1900 7c03 6415 3c00 7c08 6408  |.d...|.d.<.|.d.
-000002d0: 1900 7c03 6416 3c00 7c08 640a 1900 7c03  ..|.d.<.|.d...|.
-000002e0: 6417 3c00 7c08 640c 1900 7c03 6418 3c00  d.<.|.d...|.d.<.
-000002f0: 7c08 640e 1900 7c03 6419 3c00 7c08 6410  |.d...|.d.<.|.d.
-00000300: 1900 7c03 641a 3c00 7c08 6412 1900 7d09  ..|.d.<.|.d...}.
-00000310: 7401 a004 641b a101 0100 7405 7c04 7c05  t...d.....t.|.|.
-00000320: 8302 7d0a 7c02 7c03 641c 3c00 7c07 7c03  ..}.|.|.d.<.|.|.
-00000330: 641d 3c00 7c02 7c07 1800 7c03 641e 3c00  d.<.|.|...|.d.<.
-00000340: 7c09 7c03 641f 3c00 7c02 7c09 1800 7c03  |.|.d.<.|.|...|.
-00000350: 6420 3c00 7c07 7c0a 1800 7c03 6421 3c00  d <.|.|...|.d!<.
-00000360: 7c09 7c0a 1800 7c03 6422 3c00 7c0a 7c03  |.|...|.d"<.|.|.
-00000370: 6423 3c00 7c07 7c09 1400 7c02 1b00 7c03  d#<.|.|...|...|.
-00000380: 6424 3c00 7c07 7c09 1700 7c0a 1800 7c03  d$<.|.|...|...|.
-00000390: 6425 3c00 7c02 7c07 1800 7c09 1800 7c0a  d%<.|.|...|...|.
-000003a0: 1700 7c03 6426 3c00 7406 7c07 7c09 7c0a  ..|.d&<.t.|.|.|.
-000003b0: 7c02 8304 7c03 6427 3c00 7407 7c07 7c09  |...|.d'<.t.|.|.
-000003c0: 7c0a 7c02 8304 7c03 6428 3c00 7408 7c07  |.|...|.d(<.t.|.
-000003d0: 7c09 7c0a 7c02 8304 7c03 6429 3c00 7409  |.|.|...|.d)<.t.
-000003e0: 7c07 7c09 7c0a 7c02 8304 7c03 642a 3c00  |.|.|.|...|.d*<.
-000003f0: 740a 7c07 7c09 7c0a 7c02 8304 7c03 642b  t.|.|.|.|...|.d+
-00000400: 3c00 740b 7c07 7c09 7c0a 7c02 8304 7c03  <.t.|.|.|.|...|.
-00000410: 642c 3c00 740c 6a0d 7c03 642d 8d01 5300  d,<.t.j.|.d-..S.
-00000420: 292e 61f4 0600 000a 0a09 5061 7261 6d65  ).a.......Parame
-00000430: 7465 7273 0a09 2d2d 2d2d 2d2d 2d2d 2d2d  ters..----------
-00000440: 0a09 6669 6c65 3120 3a20 7374 720a 0909  ..file1 : str...
-00000450: 4765 6e6f 6d69 6320 7265 6769 6f6e 7320  Genomic regions 
-00000460: 696e 2042 4544 2028 4272 6f77 7365 7220  in BED (Browser 
-00000470: 4578 7465 6e73 6962 6c65 2044 6174 612c  Extensible Data,
-00000480: 2068 7474 7073 3a2f 2f67 656e 6f6d 652e   https://genome.
-00000490: 7563 7363 2e65 6475 2f46 4151 2f46 4151  ucsc.edu/FAQ/FAQ
-000004a0: 666f 726d 6174 2e68 746d 6c23 666f 726d  format.html#form
-000004b0: 6174 3129 2c20 4245 442d 6c69 6b65 206f  at1), BED-like o
-000004c0: 7220 4269 6742 6564 2066 6f72 6d61 742e  r BigBed format.
-000004d0: 0a09 0954 6865 2042 4544 2d6c 696b 6520  ...The BED-like 
-000004e0: 666f 726d 6174 2069 6e63 6c75 6465 7320  format includes 
-000004f0: 2762 6564 3327 2c27 6265 6434 272c 2762  'bed3','bed4','b
-00000500: 6564 3627 2c27 6265 6431 3227 2c27 6265  ed6','bed12','be
-00000510: 6467 7261 7068 272c 276e 6172 726f 7770  dgraph','narrowp
-00000520: 6561 6b27 2c20 2762 726f 6164 7065 616b  eak', 'broadpeak
-00000530: 272c 2767 6170 7065 6470 6561 6b27 2e20  ','gappedpeak'. 
-00000540: 4245 4420 616e 6420 4245 442d 6c69 6b65  BED and BED-like
-00000550: 0a09 0966 6f72 6d61 7420 6361 6e20 6265  ...format can be
-00000560: 2070 6c61 696e 2074 6578 742c 2063 6f6d   plain text, com
-00000570: 7072 6573 7365 6420 282e 677a 2c20 2e7a  pressed (.gz, .z
-00000580: 2c20 2e62 7a2c 202e 627a 322c 202e 627a  , .bz, .bz2, .bz
-00000590: 6970 3229 206f 7220 7265 6d6f 7465 2028  ip2) or remote (
-000005a0: 6874 7470 3a2f 2f2c 2068 7474 7073 3a2f  http://, https:/
-000005b0: 2f2c 2066 7470 3a2f 2f29 2066 696c 6573  /, ftp://) files
-000005c0: 2e20 446f 206e 6f74 2063 6f6d 7072 6573  . Do not compres
-000005d0: 730a 0909 4269 6742 6564 2066 6f72 616d  s...BigBed foram
-000005e0: 742e 2042 6967 4265 6420 6669 6c65 2063  t. BigBed file c
-000005f0: 616e 2061 6c73 6f20 6265 2061 2072 656d  an also be a rem
-00000600: 6f74 6520 6669 6c65 2e0a 0966 696c 6532  ote file...file2
-00000610: 203a 2073 7472 0a09 0947 656e 6f6d 6963   : str...Genomic
-00000620: 2072 6567 696f 6e73 2069 6e20 4245 4420   regions in BED 
-00000630: 2842 726f 7773 6572 2045 7874 656e 7369  (Browser Extensi
-00000640: 626c 6520 4461 7461 2c20 6874 7470 733a  ble Data, https:
-00000650: 2f2f 6765 6e6f 6d65 2e75 6373 632e 6564  //genome.ucsc.ed
-00000660: 752f 4641 512f 4641 5166 6f72 6d61 742e  u/FAQ/FAQformat.
-00000670: 6874 6d6c 2366 6f72 6d61 7431 292c 2042  html#format1), B
-00000680: 4544 2d6c 696b 6520 6f72 2042 6967 4265  ED-like or BigBe
-00000690: 6420 666f 726d 6174 2e0a 0909 5468 6520  d format....The 
-000006a0: 4245 442d 6c69 6b65 2066 6f72 6d61 7420  BED-like format 
-000006b0: 696e 636c 7564 6573 2027 6265 6433 272c  includes 'bed3',
-000006c0: 2762 6564 3427 2c27 6265 6436 272c 2762  'bed4','bed6','b
-000006d0: 6564 3132 272c 2762 6564 6772 6170 6827  ed12','bedgraph'
-000006e0: 2c27 6e61 7272 6f77 7065 616b 272c 2027  ,'narrowpeak', '
-000006f0: 6272 6f61 6470 6561 6b27 2c27 6761 7070  broadpeak','gapp
-00000700: 6564 7065 616b 272e 2042 4544 2061 6e64  edpeak'. BED and
-00000710: 2042 4544 2d6c 696b 650a 0909 666f 726d   BED-like...form
-00000720: 6174 2063 616e 2062 6520 706c 6169 6e20  at can be plain 
-00000730: 7465 7874 2c20 636f 6d70 7265 7373 6564  text, compressed
-00000740: 2028 2e67 7a2c 202e 7a2c 202e 627a 2c20   (.gz, .z, .bz, 
-00000750: 2e62 7a32 2c20 2e62 7a69 7032 2920 6f72  .bz2, .bzip2) or
-00000760: 2072 656d 6f74 6520 2868 7474 703a 2f2f   remote (http://
-00000770: 2c20 6874 7470 733a 2f2f 2c20 6674 703a  , https://, ftp:
-00000780: 2f2f 2920 6669 6c65 732e 2044 6f20 6e6f  //) files. Do no
-00000790: 7420 636f 6d70 7265 7373 0a09 0942 6967  t compress...Big
-000007a0: 4265 6420 666f 7261 6d74 2e20 4269 6742  Bed foramt. BigB
-000007b0: 6564 2066 696c 6520 6361 6e20 616c 736f  ed file can also
-000007c0: 2062 6520 6120 7265 6d6f 7465 2066 696c   be a remote fil
-000007d0: 652e 0a09 6472 6177 735f 6e20 3a20 696e  e...draws_n : in
-000007e0: 740a 0909 5469 6d65 7320 6f66 2064 7261  t...Times of dra
-000007f0: 7769 6e67 2073 616d 706c 6573 2077 6974  wing samples wit
-00000800: 6820 7265 706c 6163 656d 656e 742e 2053  h replacement. S
-00000810: 6574 2074 6f20 2730 2720 746f 2074 7572  et to '0' to tur
-00000820: 6e20 6f66 6620 626f 6f74 7374 7261 7069  n off bootstrapi
-00000830: 6e67 2e0a 0964 7261 775f 6672 6163 203a  ng...draw_frac :
-00000840: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
-00000850: 0a09 0954 6865 2073 697a 6520 6f66 2073  ...The size of s
-00000860: 7562 7361 6d70 6c65 2e20 5468 6520 6465  ubsample. The de
-00000870: 6661 756c 7420 6973 2030 2e38 3520 2838  fault is 0.85 (8
-00000880: 3525 206f 6620 7468 6520 6f72 6967 6e61  5% of the origna
-00000890: 6c20 6765 6e6f 6d69 6320 7265 6769 6e6f  l genomic regino
-000008a0: 7320 7769 6c6c 2062 6520 7365 6c65 6374  s will be select
-000008b0: 6564 292e 0a09 6267 5f73 697a 6520 3a20  ed)...bg_size : 
-000008c0: 696e 742c 206f 7074 696f 6e61 6c0a 0909  int, optional...
-000008d0: 5468 6520 6566 6665 6374 6976 6520 6261  The effective ba
-000008e0: 636b 6772 6f75 6e64 2067 656e 6f6d 6520  ckground genome 
-000008f0: 7369 7a65 2e20 4162 6f75 7420 312e 3447  size. About 1.4G
-00000900: 6220 6f66 2074 6865 2068 756d 616e 2067  b of the human g
-00000910: 656e 6f6d 6520 6172 652e 2054 6865 2064  enome are. The d
-00000920: 6566 6175 6c74 2069 7320 3134 3234 3635  efault is 142465
-00000930: 3539 3330 2e0a 0a09 5265 7475 726e 730a  5930....Returns.
-00000940: 092d 2d2d 2d2d 2d2d 0a09 7061 6e64 6173  .-------..pandas
-00000950: 2e53 6572 6965 730a 0909 5061 6e64 6173  .Series...Pandas
-00000960: 2053 6572 6965 7320 6f66 2027 636f 6566   Series of 'coef
-00000970: 5f6f 6273 272c 2027 636f 6566 5f65 7870  _obs', 'coef_exp
-00000980: 272c 2763 6f65 665f 7261 7469 6f27 2c20  ','coef_ratio', 
-00000990: 2763 6f65 665f 7261 7469 6f5f 6c6f 7727  'coef_ratio_low'
-000009a0: 2c20 2763 6f65 665f 7261 7469 6f5f 6869  , 'coef_ratio_hi
-000009b0: 6768 272e 0a09 0927 636f 6566 5f6f 6273  gh'....'coef_obs
-000009c0: 2720 3a20 4f62 7365 7276 6564 206f 7665  ' : Observed ove
-000009d0: 726c 6170 2063 6f65 6666 6963 6965 6e74  rlap coefficient
-000009e0: 2062 6574 7765 656e 2074 776f 2042 4544   between two BED
-000009f0: 2066 696c 6573 2e0a 0909 2763 6f65 665f   files....'coef_
-00000a00: 6578 7027 203a 2045 7870 6563 7465 6420  exp' : Expected 
-00000a10: 6f76 6572 6c61 7020 636f 6566 6669 6369  overlap coeffici
-00000a20: 656e 7420 6265 7477 6565 6e20 7477 6f20  ent between two 
-00000a30: 4245 4420 6669 6c65 732e 0a09 0927 636f  BED files....'co
-00000a40: 6566 5f72 6174 696f 2720 3a20 5261 7469  ef_ratio' : Rati
-00000a50: 6f20 6265 7477 6565 6e20 2763 6f65 665f  o between 'coef_
-00000a60: 6f62 7327 2061 6e64 2027 636f 6566 5f65  obs' and 'coef_e
-00000a70: 7870 272e 0a09 0927 636f 6566 5f72 6174  xp'....'coef_rat
-00000a80: 696f 5f6c 6f77 2720 3a20 5468 6520 6c6f  io_low' : The lo
-00000a90: 7765 7220 626f 756e 6420 6f66 2039 3525  wer bound of 95%
-00000aa0: 2063 6f6e 6669 6465 6e63 6520 696e 7465   confidence inte
-00000ab0: 7276 616c 206f 6620 2763 6f65 665f 7261  rval of 'coef_ra
-00000ac0: 7469 6f27 2e0a 0909 2763 6f65 665f 7261  tio'....'coef_ra
-00000ad0: 7469 6f5f 6869 6768 2720 3a20 5468 6520  tio_high' : The 
-00000ae0: 7570 7065 7220 626f 756e 6420 6f66 2039  upper bound of 9
-00000af0: 3525 2063 6f6e 6669 6465 6e63 6520 696e  5% confidence in
-00000b00: 7465 7276 616c 206f 6620 2763 6f65 665f  terval of 'coef_
-00000b10: 7261 7469 6f27 2e0a 0a0a 097a 2247 6174  ratio'.....z"Gat
-00000b20: 6865 7269 6e67 2069 6e66 6f72 6d61 7469  hering informati
-00000b30: 6f6e 2066 6f72 2022 2573 2220 2e2e 2eda  on for "%s" ....
-00000b40: 044e 616d 657a 0641 2e6e 616d 65da 0543  .Namez.A.name..C
-00000b50: 6f75 6e74 7a10 412e 696e 7465 7276 616c  ountz.A.interval
-00000b60: 5f63 6f75 6e74 da0a 546f 7461 6c5f 7369  _count..Total_si
-00000b70: 7a65 7a15 412e 696e 7465 7276 616c 5f74  zez.A.interval_t
-00000b80: 6f74 616c 5f73 697a 65da 094d 6561 6e5f  otal_size..Mean_
-00000b90: 7369 7a65 7a14 412e 696e 7465 7276 616c  sizez.A.interval
-00000ba0: 5f6d 6561 6e5f 7369 7a65 da0b 4d65 6469  _mean_size..Medi
-00000bb0: 616e 5f73 697a 657a 1641 2e69 6e74 6572  an_sizez.A.inter
-00000bc0: 7661 6c5f 6d65 6469 616e 5f73 697a 65da  val_median_size.
-00000bd0: 084d 696e 5f73 697a 657a 1341 2e69 6e74  .Min_sizez.A.int
-00000be0: 6572 7661 6c5f 6d69 6e5f 7369 7a65 da08  erval_min_size..
-00000bf0: 4d61 785f 7369 7a65 7a13 412e 696e 7465  Max_sizez.A.inte
-00000c00: 7276 616c 5f6d 6178 5f73 697a 65da 0353  rval_max_size..S
-00000c10: 5444 7a12 412e 696e 7465 7276 616c 5f73  TDz.A.interval_s
-00000c20: 697a 655f 5344 da0c 4765 6e6f 6d69 635f  ize_SD..Genomic_
-00000c30: 7369 7a65 7a06 422e 6e61 6d65 7a10 422e  sizez.B.namez.B.
-00000c40: 696e 7465 7276 616c 5f63 6f75 6e74 7a15  interval_countz.
-00000c50: 422e 696e 7465 7276 616c 5f74 6f74 616c  B.interval_total
-00000c60: 5f73 697a 657a 1442 2e69 6e74 6572 7661  _sizez.B.interva
-00000c70: 6c5f 6d65 616e 5f73 697a 657a 1642 2e69  l_mean_sizez.B.i
-00000c80: 6e74 6572 7661 6c5f 6d65 6469 616e 5f73  nterval_median_s
-00000c90: 697a 657a 1342 2e69 6e74 6572 7661 6c5f  izez.B.interval_
-00000ca0: 6d69 6e5f 7369 7a65 7a13 422e 696e 7465  min_sizez.B.inte
-00000cb0: 7276 616c 5f6d 6178 5f73 697a 657a 1242  rval_max_sizez.B
-00000cc0: 2e69 6e74 6572 7661 6c5f 7369 7a65 5f53  .interval_size_S
-00000cd0: 447a 2043 616c 6375 6c61 7469 6e67 206f  Dz Calculating o
-00000ce0: 7665 726c 6170 7065 6420 6261 7365 7320  verlapped bases 
-00000cf0: 2e2e 2e7a 0647 2e73 697a 657a 0641 2e73  ...z.G.sizez.A.s
-00000d00: 697a 657a 0a4e 6f74 5f41 2e73 697a 657a  izez.Not_A.sizez
-00000d10: 0642 2e73 697a 657a 0a4e 6f74 5f42 2e73  .B.sizez.Not_B.s
-00000d20: 697a 657a 0c41 5f6e 6f74 5f42 2e73 697a  izez.A_not_B.siz
-00000d30: 657a 0c42 5f6e 6f74 5f41 2e73 697a 657a  ez.B_not_A.sizez
-00000d40: 0c41 5f61 6e64 5f42 2e73 697a 657a 1041  .A_and_B.sizez.A
-00000d50: 5f61 6e64 5f42 2e65 7870 5f73 697a 657a  _and_B.exp_sizez
-00000d60: 0b41 5f6f 725f 422e 7369 7a65 7a14 4e65  .A_or_B.sizez.Ne
-00000d70: 6974 6865 725f 415f 6e6f 725f 422e 7369  ither_A_nor_B.si
-00000d80: 7a65 7a0c 636f 6566 2e4f 7665 726c 6170  zez.coef.Overlap
-00000d90: 7a0c 636f 6566 2e4a 6163 6361 7264 7a09  z.coef.Jaccardz.
-00000da0: 636f 6566 2e44 6963 657a 0763 6f65 662e  coef.Dicez.coef.
-00000db0: 5353 7a0b 415f 616e 645f 422e 504d 497a  SSz.A_and_B.PMIz
-00000dc0: 0c41 5f61 6e64 5f42 2e4e 504d 4929 01da  .A_and_B.NPMI)..
-00000dd0: 0464 6174 6129 0e72 0300 0000 da07 6c6f  .data).r......lo
-00000de0: 6767 696e 67da 0469 6e66 6f72 0400 0000  gging..infor....
-00000df0: da05 6465 6275 6772 0200 0000 7205 0000  ..debugr....r...
-00000e00: 0072 0600 0000 7208 0000 0072 0700 0000  .r....r....r....
-00000e10: 7209 0000 0072 0a00 0000 da02 7064 da06  r....r......pd..
-00000e20: 5365 7269 6573 290b da05 6669 6c65 31da  Series)...file1.
-00000e30: 0566 696c 6532 da07 6267 5f73 697a 65da  .file2..bg_size.
-00000e40: 0772 6573 756c 7473 da09 6669 6c65 315f  .results..file1_
-00000e50: 6c73 74da 0966 696c 6532 5f6c 7374 5a05  lst..file2_lstZ.
-00000e60: 696e 666f 31da 0975 6e69 7142 6173 6531  info1..uniqBase1
-00000e70: 5a05 696e 666f 32da 0975 6e69 7142 6173  Z.info2..uniqBas
-00000e80: 6532 da0c 6f76 6572 6c61 7042 6173 6573  e2..overlapBases
-00000e90: a900 7228 0000 00fa 422f 5573 6572 732f  ..r(....B/Users/
-00000ea0: 6d31 3032 3332 342f 446f 6375 6d65 6e74  m102324/Document
-00000eb0: 732f 4769 7448 7562 2f63 6f62 696e 642f  s/GitHub/cobind/
-00000ec0: 6c69 622f 636f 6269 6e64 6162 696c 6974  lib/cobindabilit
-00000ed0: 792f 6f76 7374 6174 2e70 79da 086f 765f  y/ovstat.py..ov_
-00000ee0: 7374 6174 731b 0000 0073 5a00 0000 0022  stats....sZ...."
-00000ef0: 0401 0801 0803 0e01 0801 0c01 0c01 0c02  ................
-00000f00: 0c01 0c01 0c01 0c01 0c01 0802 0e01 0801  ................
-00000f10: 0c01 0c01 0c02 0c01 0c01 0c01 0c01 0c01  ................
-00000f20: 0803 0a01 0a02 0801 0801 0c01 0801 0c01  ................
-00000f30: 0c01 0c01 0801 1001 1001 1403 1201 1201  ................
-00000f40: 1201 1201 1201 1203 722a 0000 00da 085f  ........r*....._
-00000f50: 5f6d 6169 6e5f 5f7a 1464 6973 706c 6179  _main__z.display
-00000f60: 2e66 6c6f 6174 5f66 6f72 6d61 7463 0100  .float_formatc..
-00000f70: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00000f80: 0000 4300 0000 7308 0000 0064 017c 0016  ..C...s....d.|..
-00000f90: 0053 0029 024e 7a04 252e 3466 7228 0000  .S.).Nz.%.4fr(..
-00000fa0: 0029 01da 0178 7228 0000 0072 2800 0000  .)...xr(...r(...
-00000fb0: 7229 0000 00da 083c 6c61 6d62 6461 3e7c  r).....<lambda>|
-00000fc0: 0000 00f3 0000 0000 722d 0000 00e9 0100  ........r-......
-00000fd0: 0000 e902 0000 0029 0172 0f00 0000 2920  .......).r....) 
-00000fe0: da07 5f5f 646f 635f 5fda 0373 7973 721a  ..__doc__..sysr.
-00000ff0: 0000 00da 0670 616e 6461 7372 1d00 0000  .....pandasr....
-00001000: da11 636f 6269 6e64 6162 696c 6974 792e  ..cobindability.
-00001010: 4245 4472 0200 0000 7203 0000 0072 0400  BEDr....r....r..
-00001020: 0000 da15 636f 6269 6e64 6162 696c 6974  ....cobindabilit
-00001030: 792e 636f 6566 6361 6c72 0500 0000 7206  y.coefcalr....r.
-00001040: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00001050: 0000 720a 0000 00da 0d63 6f62 696e 6461  ..r......cobinda
-00001060: 6269 6c69 7479 720b 0000 00da 0a5f 5f61  bilityr......__a
-00001070: 7574 686f 725f 5fda 0d5f 5f63 6f70 7972  uthor__..__copyr
-00001080: 6967 6874 5f5f da0b 5f5f 6372 6564 6974  ight__..__credit
-00001090: 735f 5fda 0b5f 5f6c 6963 656e 7365 5f5f  s__..__license__
-000010a0: da0b 5f5f 7665 7273 696f 6e5f 5fda 0e5f  ..__version__.._
-000010b0: 5f6d 6169 6e74 6169 6e65 725f 5fda 095f  _maintainer__.._
-000010c0: 5f65 6d61 696c 5f5f da0a 5f5f 7374 6174  _email__..__stat
-000010d0: 7573 5f5f 722a 0000 00da 085f 5f6e 616d  us__r*.....__nam
-000010e0: 655f 5fda 0a73 6574 5f6f 7074 696f 6eda  e__..set_option.
-000010f0: 0461 7267 76da 0161 da05 7072 696e 7472  .argv..a..printr
-00001100: 2800 0000 7228 0000 0072 2800 0000 7229  (...r(...r(...r)
-00001110: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
-00001120: 0073 2600 0000 0406 0801 0801 0801 1401  .s&.............
-00001130: 2001 0c03 0401 0401 0401 0401 0601 0401   ...............
-00001140: 0401 0403 0a60 0801 1001 1601            .....`......
+00000140: 5f73 697a 65da 0b62 6564 5f74 6f5f 6c69  _size..bed_to_li
+00000150: 7374 da08 6265 645f 696e 666f 2906 da07  st..bed_info)...
+00000160: 6f76 5f63 6f65 66da 0a6f 765f 6a61 6363  ov_coef..ov_jacc
+00000170: 6172 64da 056f 765f 7373 da05 6f76 5f73  ard..ov_ss..ov_s
+00000180: 64da 0970 6d69 5f76 616c 7565 da0a 6e70  d..pmi_value..np
+00000190: 6d69 5f76 616c 7565 2901 da07 7665 7273  mi_value)...vers
+000001a0: 696f 6e7a 0a4c 6967 756f 2057 616e 67da  ionz.Liguo Wang.
+000001b0: 0843 6f70 796c 6566 74da 034d 4954 7a13  .Copyleft..MITz.
+000001c0: 7761 6e67 2e6c 6967 756f 406d 6179 6f2e  wang.liguo@mayo.
+000001d0: 6564 75da 0b44 6576 656c 6f70 6d65 6e74  edu..Development
+000001e0: e900 4e72 5363 0300 0000 0000 0000 0000  ..NrSc..........
+000001f0: 0000 0b00 0000 0500 0000 4300 0000 7320  ..........C...s 
+00000200: 0200 0069 007d 0374 007c 0083 017d 0474  ...i.}.t.|...}.t
+00000210: 007c 0183 017d 0574 01a0 0264 017c 0016  .|...}.t...d.|..
+00000220: 00a1 0101 0074 037c 0083 017d 067c 0664  .....t.|...}.|.d
+00000230: 0219 007c 0364 033c 007c 0664 0419 007c  ...|.d.<.|.d...|
+00000240: 0364 053c 007c 0664 0619 007c 0364 073c  .d.<.|.d...|.d.<
+00000250: 007c 0664 0819 007c 0364 093c 007c 0664  .|.d...|.d.<.|.d
+00000260: 0a19 007c 0364 0b3c 007c 0664 0c19 007c  ...|.d.<.|.d...|
+00000270: 0364 0d3c 007c 0664 0e19 007c 0364 0f3c  .d.<.|.d...|.d.<
+00000280: 007c 0664 1019 007c 0364 113c 007c 0664  .|.d...|.d.<.|.d
+00000290: 1219 007d 0774 01a0 0264 017c 0116 00a1  ...}.t...d.|....
+000002a0: 0101 0074 037c 0183 017d 087c 0864 0219  ...t.|...}.|.d..
+000002b0: 007c 0364 133c 007c 0864 0419 007c 0364  .|.d.<.|.d...|.d
+000002c0: 143c 007c 0864 0619 007c 0364 153c 007c  .<.|.d...|.d.<.|
+000002d0: 0864 0819 007c 0364 163c 007c 0864 0a19  .d...|.d.<.|.d..
+000002e0: 007c 0364 173c 007c 0864 0c19 007c 0364  .|.d.<.|.d...|.d
+000002f0: 183c 007c 0864 0e19 007c 0364 193c 007c  .<.|.d...|.d.<.|
+00000300: 0864 1019 007c 0364 1a3c 007c 0864 1219  .d...|.d.<.|.d..
+00000310: 007d 0974 01a0 0464 1ba1 0101 0074 057c  .}.t...d.....t.|
+00000320: 047c 0583 027d 0a7c 027c 0364 1c3c 007c  .|...}.|.|.d.<.|
+00000330: 077c 0364 1d3c 007c 027c 0718 007c 0364  .|.d.<.|.|...|.d
+00000340: 1e3c 007c 097c 0364 1f3c 007c 027c 0918  .<.|.|.d.<.|.|..
+00000350: 007c 0364 203c 007c 077c 0a18 007c 0364  .|.d <.|.|...|.d
+00000360: 213c 007c 097c 0a18 007c 0364 223c 007c  !<.|.|...|.d"<.|
+00000370: 0a7c 0364 233c 007c 077c 0914 007c 021b  .|.d#<.|.|...|..
+00000380: 007c 0364 243c 007c 077c 0917 007c 0a18  .|.d$<.|.|...|..
+00000390: 007c 0364 253c 007c 027c 0718 007c 0918  .|.d%<.|.|...|..
+000003a0: 007c 0a17 007c 0364 263c 0074 067c 077c  .|...|.d&<.t.|.|
+000003b0: 097c 0a7c 0283 047c 0364 273c 0074 077c  .|.|...|.d'<.t.|
+000003c0: 077c 097c 0a7c 0283 047c 0364 283c 0074  .|.|.|...|.d(<.t
+000003d0: 087c 077c 097c 0a7c 0283 047c 0364 293c  .|.|.|.|...|.d)<
+000003e0: 0074 097c 077c 097c 0a7c 0283 047c 0364  .t.|.|.|.|...|.d
+000003f0: 2a3c 0074 0a7c 077c 097c 0a7c 0283 047c  *<.t.|.|.|.|...|
+00000400: 0364 2b3c 0074 0b7c 077c 097c 0a7c 0283  .d+<.t.|.|.|.|..
+00000410: 047c 0364 2c3c 0074 0c6a 0d7c 0364 2d8d  .|.d,<.t.j.|.d-.
+00000420: 0153 0029 2e61 fc06 0000 0a0a 0950 6172  .S.).a.......Par
+00000430: 616d 6574 6572 730a 092d 2d2d 2d2d 2d2d  ameters..-------
+00000440: 2d2d 2d0a 0966 696c 6531 203a 2073 7472  ---..file1 : str
+00000450: 0a09 0947 656e 6f6d 6963 2072 6567 696f  ...Genomic regio
+00000460: 6e73 2069 6e20 4245 4420 2842 726f 7773  ns in BED (Brows
+00000470: 6572 2045 7874 656e 7369 626c 6520 4461  er Extensible Da
+00000480: 7461 2c20 6874 7470 733a 2f2f 6765 6e6f  ta, https://geno
+00000490: 6d65 2e75 6373 632e 6564 752f 4641 512f  me.ucsc.edu/FAQ/
+000004a0: 4641 5166 6f72 6d61 742e 6874 6d6c 2366  FAQformat.html#f
+000004b0: 6f72 6d61 7431 292c 2042 4544 2d6c 696b  ormat1), BED-lik
+000004c0: 6520 6f72 2042 6967 4265 6420 666f 726d  e or BigBed form
+000004d0: 6174 2e0a 0909 5468 6520 4245 442d 6c69  at....The BED-li
+000004e0: 6b65 2066 6f72 6d61 7420 696e 636c 7564  ke format includ
+000004f0: 6573 2027 6265 6433 272c 2762 6564 3427  es 'bed3','bed4'
+00000500: 2c27 6265 6436 272c 2762 6564 3132 272c  ,'bed6','bed12',
+00000510: 2762 6564 6772 6170 6827 2c27 6e61 7272  'bedgraph','narr
+00000520: 6f77 7065 616b 272c 2027 6272 6f61 6470  owpeak', 'broadp
+00000530: 6561 6b27 2c27 6761 7070 6564 7065 616b  eak','gappedpeak
+00000540: 272e 2042 4544 2061 6e64 2042 4544 2d6c  '. BED and BED-l
+00000550: 696b 650a 0909 666f 726d 6174 2063 616e  ike...format can
+00000560: 2062 6520 706c 6169 6e20 7465 7874 2c20   be plain text, 
+00000570: 636f 6d70 7265 7373 6564 2028 2e67 7a2c  compressed (.gz,
+00000580: 202e 7a2c 202e 627a 2c20 2e62 7a32 2c20   .z, .bz, .bz2, 
+00000590: 2e62 7a69 7032 2920 6f72 2072 656d 6f74  .bzip2) or remot
+000005a0: 6520 2868 7474 703a 2f2f 2c20 6874 7470  e (http://, http
+000005b0: 733a 2f2f 2c20 6674 703a 2f2f 2920 6669  s://, ftp://) fi
+000005c0: 6c65 732e 2044 6f20 6e6f 7420 636f 6d70  les. Do not comp
+000005d0: 7265 7373 0a09 0942 6967 4265 6420 666f  ress...BigBed fo
+000005e0: 7261 6d74 2e20 4269 6742 6564 2066 696c  ramt. BigBed fil
+000005f0: 6520 6361 6e20 616c 736f 2062 6520 6120  e can also be a 
+00000600: 7265 6d6f 7465 2066 696c 652e 0a09 6669  remote file...fi
+00000610: 6c65 3220 3a20 7374 720a 0909 4765 6e6f  le2 : str...Geno
+00000620: 6d69 6320 7265 6769 6f6e 7320 696e 2042  mic regions in B
+00000630: 4544 2028 4272 6f77 7365 7220 4578 7465  ED (Browser Exte
+00000640: 6e73 6962 6c65 2044 6174 612c 2068 7474  nsible Data, htt
+00000650: 7073 3a2f 2f67 656e 6f6d 652e 7563 7363  ps://genome.ucsc
+00000660: 2e65 6475 2f46 4151 2f46 4151 666f 726d  .edu/FAQ/FAQform
+00000670: 6174 2e68 746d 6c23 666f 726d 6174 3129  at.html#format1)
+00000680: 2c20 4245 442d 6c69 6b65 206f 7220 4269  , BED-like or Bi
+00000690: 6742 6564 2066 6f72 6d61 742e 0a09 0954  gBed format....T
+000006a0: 6865 2042 4544 2d6c 696b 6520 666f 726d  he BED-like form
+000006b0: 6174 2069 6e63 6c75 6465 7320 2762 6564  at includes 'bed
+000006c0: 3327 2c27 6265 6434 272c 2762 6564 3627  3','bed4','bed6'
+000006d0: 2c27 6265 6431 3227 2c27 6265 6467 7261  ,'bed12','bedgra
+000006e0: 7068 272c 276e 6172 726f 7770 6561 6b27  ph','narrowpeak'
+000006f0: 2c20 2762 726f 6164 7065 616b 272c 2767  , 'broadpeak','g
+00000700: 6170 7065 6470 6561 6b27 2e20 4245 4420  appedpeak'. BED 
+00000710: 616e 6420 4245 442d 6c69 6b65 0a09 0966  and BED-like...f
+00000720: 6f72 6d61 7420 6361 6e20 6265 2070 6c61  ormat can be pla
+00000730: 696e 2074 6578 742c 2063 6f6d 7072 6573  in text, compres
+00000740: 7365 6420 282e 677a 2c20 2e7a 2c20 2e62  sed (.gz, .z, .b
+00000750: 7a2c 202e 627a 322c 202e 627a 6970 3229  z, .bz2, .bzip2)
+00000760: 206f 7220 7265 6d6f 7465 2028 6874 7470   or remote (http
+00000770: 3a2f 2f2c 2068 7474 7073 3a2f 2f2c 2066  ://, https://, f
+00000780: 7470 3a2f 2f29 2066 696c 6573 2e20 446f  tp://) files. Do
+00000790: 206e 6f74 2063 6f6d 7072 6573 730a 0909   not compress...
+000007a0: 4269 6742 6564 2066 6f72 616d 742e 2042  BigBed foramt. B
+000007b0: 6967 4265 6420 6669 6c65 2063 616e 2061  igBed file can a
+000007c0: 6c73 6f20 6265 2061 2072 656d 6f74 6520  lso be a remote 
+000007d0: 6669 6c65 2e0a 0964 7261 7773 5f6e 203a  file...draws_n :
+000007e0: 2069 6e74 0a09 0954 696d 6573 206f 6620   int...Times of 
+000007f0: 6472 6177 696e 6720 7361 6d70 6c65 7320  drawing samples 
+00000800: 7769 7468 2072 6570 6c61 6365 6d65 6e74  with replacement
+00000810: 2e20 5365 7420 746f 2027 3027 2074 6f20  . Set to '0' to 
+00000820: 7475 726e 206f 6666 2062 6f6f 7473 7472  turn off bootstr
+00000830: 6170 696e 672e 0a09 6472 6177 5f66 7261  aping...draw_fra
+00000840: 6320 3a20 666c 6f61 742c 206f 7074 696f  c : float, optio
+00000850: 6e61 6c0a 0909 5468 6520 7369 7a65 206f  nal...The size o
+00000860: 6620 7375 6273 616d 706c 652e 2054 6865  f subsample. The
+00000870: 2064 6566 6175 6c74 2069 7320 302e 3835   default is 0.85
+00000880: 2028 3835 2520 6f66 2074 6865 206f 7269   (85% of the ori
+00000890: 676e 616c 2067 656e 6f6d 6963 2072 6567  gnal genomic reg
+000008a0: 696e 6f73 2077 696c 6c20 6265 2073 656c  inos will be sel
+000008b0: 6563 7465 6429 2e0a 0962 675f 7369 7a65  ected)...bg_size
+000008c0: 203a 2069 6e74 2c20 6f70 7469 6f6e 616c   : int, optional
+000008d0: 0a09 0954 6865 2065 6666 6563 7469 7665  ...The effective
+000008e0: 2062 6163 6b67 726f 756e 6420 6765 6e6f   background geno
+000008f0: 6d65 2073 697a 652e 2041 626f 7574 2031  me size. About 1
+00000900: 2e34 4762 206f 6620 7468 6520 6875 6d61  .4Gb of the huma
+00000910: 6e20 6765 6e6f 6d65 2061 7265 2e20 5468  n genome are. Th
+00000920: 6520 6465 6661 756c 7420 6973 2031 3432  e default is 142
+00000930: 3436 3535 3933 302e 0a0a 0952 6574 7572  4655930....Retur
+00000940: 6e73 0a09 2d2d 2d2d 2d2d 2d0a 0970 616e  ns..-------..pan
+00000950: 6461 732e 5365 7269 6573 0a09 0950 616e  das.Series...Pan
+00000960: 6461 7320 5365 7269 6573 206f 6620 2763  das Series of 'c
+00000970: 6f65 665f 6f62 7327 2c20 2763 6f65 665f  oef_obs', 'coef_
+00000980: 6578 7027 2c27 636f 6566 5f72 6174 696f  exp','coef_ratio
+00000990: 272c 2027 636f 6566 5f72 6174 696f 5f6c  ', 'coef_ratio_l
+000009a0: 6f77 272c 2027 636f 6566 5f72 6174 696f  ow', 'coef_ratio
+000009b0: 5f68 6967 6827 2e0a 0909 2763 6f65 665f  _high'....'coef_
+000009c0: 6f62 7327 203a 204f 6273 6572 7665 6420  obs' : Observed 
+000009d0: 636f 6c6c 6f63 6174 696f 6e20 636f 6566  collocation coef
+000009e0: 6669 6369 656e 7420 6265 7477 6565 6e20  ficient between 
+000009f0: 7477 6f20 4245 4420 6669 6c65 732e 0a09  two BED files...
+00000a00: 0927 636f 6566 5f65 7870 2720 3a20 4578  .'coef_exp' : Ex
+00000a10: 7065 6374 6564 2063 6f6c 6c6f 6361 7469  pected collocati
+00000a20: 6f6e 2063 6f65 6666 6963 6965 6e74 2062  on coefficient b
+00000a30: 6574 7765 656e 2074 776f 2042 4544 2066  etween two BED f
+00000a40: 696c 6573 2e0a 0909 2763 6f65 665f 7261  iles....'coef_ra
+00000a50: 7469 6f27 203a 2052 6174 696f 2062 6574  tio' : Ratio bet
+00000a60: 7765 656e 2027 636f 6566 5f6f 6273 2720  ween 'coef_obs' 
+00000a70: 616e 6420 2763 6f65 665f 6578 7027 2e0a  and 'coef_exp'..
+00000a80: 0909 2763 6f65 665f 7261 7469 6f5f 6c6f  ..'coef_ratio_lo
+00000a90: 7727 203a 2054 6865 206c 6f77 6572 2062  w' : The lower b
+00000aa0: 6f75 6e64 206f 6620 3935 2520 636f 6e66  ound of 95% conf
+00000ab0: 6964 656e 6365 2069 6e74 6572 7661 6c20  idence interval 
+00000ac0: 6f66 2027 636f 6566 5f72 6174 696f 272e  of 'coef_ratio'.
+00000ad0: 0a09 0927 636f 6566 5f72 6174 696f 5f68  ...'coef_ratio_h
+00000ae0: 6967 6827 203a 2054 6865 2075 7070 6572  igh' : The upper
+00000af0: 2062 6f75 6e64 206f 6620 3935 2520 636f   bound of 95% co
+00000b00: 6e66 6964 656e 6365 2069 6e74 6572 7661  nfidence interva
+00000b10: 6c20 6f66 2027 636f 6566 5f72 6174 696f  l of 'coef_ratio
+00000b20: 272e 0a0a 0a09 7a22 4761 7468 6572 696e  '.....z"Gatherin
+00000b30: 6720 696e 666f 726d 6174 696f 6e20 666f  g information fo
+00000b40: 7220 2225 7322 202e 2e2e da04 4e61 6d65  r "%s" .....Name
+00000b50: 7a06 412e 6e61 6d65 da05 436f 756e 747a  z.A.name..Countz
+00000b60: 1041 2e69 6e74 6572 7661 6c5f 636f 756e  .A.interval_coun
+00000b70: 74da 0a54 6f74 616c 5f73 697a 657a 1541  t..Total_sizez.A
+00000b80: 2e69 6e74 6572 7661 6c5f 746f 7461 6c5f  .interval_total_
+00000b90: 7369 7a65 da09 4d65 616e 5f73 697a 657a  size..Mean_sizez
+00000ba0: 1441 2e69 6e74 6572 7661 6c5f 6d65 616e  .A.interval_mean
+00000bb0: 5f73 697a 65da 0b4d 6564 6961 6e5f 7369  _size..Median_si
+00000bc0: 7a65 7a16 412e 696e 7465 7276 616c 5f6d  zez.A.interval_m
+00000bd0: 6564 6961 6e5f 7369 7a65 da08 4d69 6e5f  edian_size..Min_
+00000be0: 7369 7a65 7a13 412e 696e 7465 7276 616c  sizez.A.interval
+00000bf0: 5f6d 696e 5f73 697a 65da 084d 6178 5f73  _min_size..Max_s
+00000c00: 697a 657a 1341 2e69 6e74 6572 7661 6c5f  izez.A.interval_
+00000c10: 6d61 785f 7369 7a65 da03 5354 447a 1241  max_size..STDz.A
+00000c20: 2e69 6e74 6572 7661 6c5f 7369 7a65 5f53  .interval_size_S
+00000c30: 44da 0c47 656e 6f6d 6963 5f73 697a 657a  D..Genomic_sizez
+00000c40: 0642 2e6e 616d 657a 1042 2e69 6e74 6572  .B.namez.B.inter
+00000c50: 7661 6c5f 636f 756e 747a 1542 2e69 6e74  val_countz.B.int
+00000c60: 6572 7661 6c5f 746f 7461 6c5f 7369 7a65  erval_total_size
+00000c70: 7a14 422e 696e 7465 7276 616c 5f6d 6561  z.B.interval_mea
+00000c80: 6e5f 7369 7a65 7a16 422e 696e 7465 7276  n_sizez.B.interv
+00000c90: 616c 5f6d 6564 6961 6e5f 7369 7a65 7a13  al_median_sizez.
+00000ca0: 422e 696e 7465 7276 616c 5f6d 696e 5f73  B.interval_min_s
+00000cb0: 697a 657a 1342 2e69 6e74 6572 7661 6c5f  izez.B.interval_
+00000cc0: 6d61 785f 7369 7a65 7a12 422e 696e 7465  max_sizez.B.inte
+00000cd0: 7276 616c 5f73 697a 655f 5344 7a20 4361  rval_size_SDz Ca
+00000ce0: 6c63 756c 6174 696e 6720 6f76 6572 6c61  lculating overla
+00000cf0: 7070 6564 2062 6173 6573 202e 2e2e 7a06  pped bases ...z.
+00000d00: 472e 7369 7a65 7a06 412e 7369 7a65 7a0a  G.sizez.A.sizez.
+00000d10: 4e6f 745f 412e 7369 7a65 7a06 422e 7369  Not_A.sizez.B.si
+00000d20: 7a65 7a0a 4e6f 745f 422e 7369 7a65 7a0c  zez.Not_B.sizez.
+00000d30: 415f 6e6f 745f 422e 7369 7a65 7a0c 425f  A_not_B.sizez.B_
+00000d40: 6e6f 745f 412e 7369 7a65 7a0c 415f 616e  not_A.sizez.A_an
+00000d50: 645f 422e 7369 7a65 7a10 415f 616e 645f  d_B.sizez.A_and_
+00000d60: 422e 6578 705f 7369 7a65 7a0b 415f 6f72  B.exp_sizez.A_or
+00000d70: 5f42 2e73 697a 657a 144e 6569 7468 6572  _B.sizez.Neither
+00000d80: 5f41 5f6e 6f72 5f42 2e73 697a 657a 1063  _A_nor_B.sizez.c
+00000d90: 6f65 662e 436f 6c6c 6f63 6174 696f 6e7a  oef.Collocationz
+00000da0: 0c63 6f65 662e 4a61 6363 6172 647a 0963  .coef.Jaccardz.c
+00000db0: 6f65 662e 4469 6365 7a07 636f 6566 2e53  oef.Dicez.coef.S
+00000dc0: 537a 0b41 5f61 6e64 5f42 2e50 4d49 7a0c  Sz.A_and_B.PMIz.
+00000dd0: 415f 616e 645f 422e 4e50 4d49 2901 da04  A_and_B.NPMI)...
+00000de0: 6461 7461 290e 7203 0000 00da 076c 6f67  data).r......log
+00000df0: 6769 6e67 da04 696e 666f 7204 0000 00da  ging..infor.....
+00000e00: 0564 6562 7567 7202 0000 0072 0500 0000  .debugr....r....
+00000e10: 7206 0000 0072 0800 0000 7207 0000 0072  r....r....r....r
+00000e20: 0900 0000 720a 0000 00da 0270 64da 0653  ....r......pd..S
+00000e30: 6572 6965 7329 0b5a 0566 696c 6531 5a05  eries).Z.file1Z.
+00000e40: 6669 6c65 32da 0762 675f 7369 7a65 da07  file2..bg_size..
+00000e50: 7265 7375 6c74 735a 0966 696c 6531 5f6c  resultsZ.file1_l
+00000e60: 7374 5a09 6669 6c65 325f 6c73 745a 0569  stZ.file2_lstZ.i
+00000e70: 6e66 6f31 5a09 756e 6971 4261 7365 315a  nfo1Z.uniqBase1Z
+00000e80: 0569 6e66 6f32 5a09 756e 6971 4261 7365  .info2Z.uniqBase
+00000e90: 325a 0c6f 7665 726c 6170 4261 7365 73a9  2Z.overlapBases.
+00000ea0: 0072 2100 0000 fa42 2f55 7365 7273 2f6d  .r!....B/Users/m
+00000eb0: 3130 3233 3234 2f44 6f63 756d 656e 7473  102324/Documents
+00000ec0: 2f47 6974 4875 622f 636f 6269 6e64 2f6c  /GitHub/cobind/l
+00000ed0: 6962 2f63 6f62 696e 6461 6269 6c69 7479  ib/cobindability
+00000ee0: 2f6f 7673 7461 742e 7079 da08 6f76 5f73  /ovstat.py..ov_s
+00000ef0: 7461 7473 1b00 0000 735a 0000 0000 2204  tats....sZ....".
+00000f00: 0108 0108 030e 0108 010c 010c 010c 020c  ................
+00000f10: 010c 010c 010c 010c 0108 020e 0108 010c  ................
+00000f20: 010c 010c 020c 010c 010c 010c 010c 0108  ................
+00000f30: 030a 010a 0208 0108 010c 0108 010c 010c  ................
+00000f40: 010c 0108 0110 0110 0114 0312 0112 0112  ................
+00000f50: 0112 0112 0112 0372 2300 0000 da08 5f5f  .......r#.....__
+00000f60: 6d61 696e 5f5f 7a14 6469 7370 6c61 792e  main__z.display.
+00000f70: 666c 6f61 745f 666f 726d 6174 6301 0000  float_formatc...
+00000f80: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00000f90: 0043 0000 0073 0800 0000 6401 7c00 1600  .C...s....d.|...
+00000fa0: 5300 2902 4e7a 0425 2e34 6672 2100 0000  S.).Nz.%.4fr!...
+00000fb0: 2901 da01 7872 2100 0000 7221 0000 0072  )...xr!...r!...r
+00000fc0: 2200 0000 da08 3c6c 616d 6264 613e 7c00  ".....<lambda>|.
+00000fd0: 0000 f300 0000 0072 2600 0000 e901 0000  .......r&.......
+00000fe0: 00e9 0200 0000 2901 720f 0000 0029 20da  ......).r....) .
+00000ff0: 075f 5f64 6f63 5f5f da03 7379 7372 1a00  .__doc__..sysr..
+00001000: 0000 da06 7061 6e64 6173 721d 0000 00da  ....pandasr.....
+00001010: 1163 6f62 696e 6461 6269 6c69 7479 2e42  .cobindability.B
+00001020: 4544 7202 0000 0072 0300 0000 7204 0000  EDr....r....r...
+00001030: 00da 1563 6f62 696e 6461 6269 6c69 7479  ...cobindability
+00001040: 2e63 6f65 6663 616c 7205 0000 0072 0600  .coefcalr....r..
+00001050: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
+00001060: 0072 0a00 0000 da0d 636f 6269 6e64 6162  .r......cobindab
+00001070: 696c 6974 7972 0b00 0000 da0a 5f5f 6175  ilityr......__au
+00001080: 7468 6f72 5f5f da0d 5f5f 636f 7079 7269  thor__..__copyri
+00001090: 6768 745f 5fda 0b5f 5f63 7265 6469 7473  ght__..__credits
+000010a0: 5f5f da0b 5f5f 6c69 6365 6e73 655f 5fda  __..__license__.
+000010b0: 0b5f 5f76 6572 7369 6f6e 5f5f da0e 5f5f  .__version__..__
+000010c0: 6d61 696e 7461 696e 6572 5f5f da09 5f5f  maintainer__..__
+000010d0: 656d 6169 6c5f 5fda 0a5f 5f73 7461 7475  email__..__statu
+000010e0: 735f 5f72 2300 0000 da08 5f5f 6e61 6d65  s__r#.....__name
+000010f0: 5f5f da0a 7365 745f 6f70 7469 6f6e da04  __..set_option..
+00001100: 6172 6776 da01 61da 0570 7269 6e74 7221  argv..a..printr!
+00001110: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
+00001120: 0000 da08 3c6d 6f64 756c 653e 0300 0000  ....<module>....
+00001130: 7326 0000 0004 0608 0108 0108 0114 0120  s&............. 
+00001140: 010c 0304 0104 0104 0104 0106 0104 0104  ................
+00001150: 0104 030a 6008 0110 0116 01              ....`......
```

### Comparing `cobind-1.0.0/lib/cobindability/bbreader.py` & `cobind-1.0.1/lib/cobindability/bbreader.py`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/bw.py` & `cobind-1.0.1/lib/cobindability/bw.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,117 +19,137 @@
 __license__ = "MIT"
 __version__ = version.version
 __maintainer__ = "Liguo Wang"
 __email__ = "wang.liguo@mayo.edu"
 __status__ = "Development"
 
 
-def bigwig_corr(bed, bw1, bw2, outfile, na_label = 'nan', score_type='mean', exact_scores = True, keep_NA = False, top_x = 1.0, min_sig = 0):
-	"""
-	Calculate Pearson's and Spearman's correlations between two bigWig files
-
-	Parameters
-	----------
-	bed : list
-		List of genomic regions.
-	bw1 : str
-		Name of one bigWig file.
-	bw2 : str
-		Name of another bigWig file.
-	outfile : str
-		Name of the output TSV file.
-	na_label : str, optional
-		String representation of missing values. Default: 'nan'
-	score_type : str, optional
-		Summary statistic score type ('min','mean' or 'max') of a genomic region.
-		Default: 'mean'
-	exact_scores : bool, optional
-		If set, calculate the "exact" summary statistic score rather than
-		"zoom-level" score for each genomic region. Default: True
-	keep_NA : bool, optional
-		If set, all genomic regions will be kept even they do not have summary
-		statistic scores in either of the two bigWig files. Default: False
-	top_x : float, optional
-		Percentage ( if top_x in (0,1]) or number (if top_x > 1) of genomic
-		regions used to calculate Pearson, Spearman, Kendall's correlations.
-		default: 1.0 (i.e., use all genomic regions to calculate correlation coefficients)
-	min_sig : float, optional
-		Genomic regions with summary statistic equal or less than this value will be
-		filtered out.
-		default: 0 (i.e., use all genomic regions to calculate correlation coefficients)
-
-
-	Returns
-	-------
-	None.
-
-	"""
-	bw_1 = pyBigWig.open(bw1)
-	logging.debug(str(bw_1.header()))
-	bw_2 = pyBigWig.open(bw2)
-	logging.debug(str(bw_2.header()))
-
-	#check bigwig files
-	if bw_1.isBigWig():
-		pass
-	else:
-		logging.error("Not a bigWig file: %s" % bw1)
-	if bw_2.isBigWig():
-		pass
-	else:
-		logging.error("Not a bigWig file: %s" % bw2)
-
-	#check chrom IDs in bigwig files
-	#all_chroms1 = bw_1.chroms().keys()
-	#all_chroms2 = bw_2.chroms().keys()
-
-	names=[]
-	scores_1 = []
-	scores_2 = []
-	for (chrom ,start, end) in bed:
-		region_id = chrom + ':' + str(start) + '-' + str(end)
-		score_1 = bw_1.stats(chrom, start, end, type=score_type, exact=exact_scores).pop()
-		score_2 = bw_2.stats(chrom, start, end, type=score_type, exact=exact_scores).pop()
-		if (isinstance(score_1, (int, float)) is False):
-			if keep_NA:
-				score_1 = np.nan
-			else:
-				continue
-		if (isinstance(score_2, (int, float)) is False):
-			if keep_NA:
-				score_2 = np.nan
-			else:
-				continue
-		names.append(region_id)
-		scores_1.append(score_1)
-		scores_2.append(score_2)
-
-	bw1_name = os.path.basename(bw1) + '.' + score_type
-	bw2_name = os.path.basename(bw2) + '.' + score_type
-	df = pd.DataFrame(data={bw1_name : scores_1, bw2_name : scores_2 }, index=names, dtype=float)
-
-	logging.info("Sort dataframe by summary statistical scores ...")
-	df.sort_values(by=[bw1_name, bw1_name], ascending=False, ignore_index=False, inplace=True)
-
-	logging.info("Save dataframe to: \"%s\"" % outfile)
-	df.to_csv(outfile, na_rep=na_label, sep="\t", index=True, header=True, index_label="region_id")
-
-	#Still remove NAs, in order to calculate correlations
-	#if keep_NA:
-	df = df[df > min_sig]
-	df.dropna(axis=0, inplace=True)
-
-	if top_x > 0 and top_x <= 1:
-		top_n = int(len(df)* top_x)
-		logging.info("Select %d regions ..." % top_n)
-		df = df.head(top_n)
-	elif top_x > 1:
-		top_n = top_x
-		logging.info("Select %d regions ..." % top_n)
-		df = df.head(top_n)
-
-
-	(pearson_cor, pearson_p) = pearsonr(np.log2(df[bw1_name]), np.log2(df[bw2_name]))
-	(spearman_rho, spearman_p) = spearmanr(np.log2(df[bw1_name]), np.log2(df[bw2_name]))
-	(kendall_tau, kendall_p) = kendalltau(np.log2(df[bw1_name]), np.log2(df[bw2_name]))
-
-	return (pd.DataFrame(data={'Pearson_cor:' : [pearson_cor, pearson_p], 'Spearman_rho:' : [spearman_rho, spearman_p], 'Kendall_tau:' : [kendall_tau, kendall_p]}, index=['Correlation', 'P-value']))
+def bigwig_corr(bed, bw1, bw2, outfile, na_label='nan', score_type='mean',
+                exact_scores=True, keep_NA=False, top_x=1.0, min_sig=0):
+    """
+    Calculate Pearson's and Spearman's correlations between two bigWig files
+
+    Parameters
+    ----------
+    bed : list
+        List of genomic regions.
+    bw1 : str
+        Name of one bigWig file.
+    bw2 : str
+        Name of another bigWig file.
+    outfile : str
+        Name of the output TSV file.
+    na_label : str, optional
+        String representation of missing values. Default: 'nan'
+    score_type : str, optional
+        Summary statistic score type ('min','mean' or 'max') of a genomic
+        region. Default: 'mean'
+    exact_scores : bool, optional
+        If set, calculate the "exact" summary statistic score rather than
+        "zoom-level" score for each genomic region. Default: True
+    keep_NA : bool, optional
+        If set, all genomic regions will be kept even they do not have summary
+        statistic scores in either of the two bigWig files. Default: False
+    top_x : float, optional
+        Percentage ( if top_x in (0,1]) or number (if top_x > 1) of genomic
+        regions used to calculate Pearson, Spearman, Kendall's correlations.
+        default: 1.0 (i.e., use all genomic regions to calculate correlation
+        coefficients).
+    min_sig : float, optional
+        Genomic regions with summary statistic equal or less than this
+        value will be filtered out. default: 0 (i.e., use all genomic regions
+        to calculate correlation coefficients).
+
+
+    Returns
+    -------
+    None.
+
+    """
+    bw_1 = pyBigWig.open(bw1)
+    logging.debug(str(bw_1.header()))
+    bw_2 = pyBigWig.open(bw2)
+    logging.debug(str(bw_2.header()))
+
+    # check bigwig files
+    if bw_1.isBigWig():
+        pass
+    else:
+        logging.error("Not a bigWig file: %s" % bw1)
+    if bw_2.isBigWig():
+        pass
+    else:
+        logging.error("Not a bigWig file: %s" % bw2)
+
+    # check chrom IDs in bigwig files
+    # all_chroms1 = bw_1.chroms().keys()
+    # all_chroms2 = bw_2.chroms().keys()
+
+    names = []
+    scores_1 = []
+    scores_2 = []
+    for (chrom, start, end) in bed:
+        region_id = chrom + ':' + str(start) + '-' + str(end)
+        score_1 = bw_1.stats(
+            chrom, start, end, type=score_type, exact=exact_scores).pop()
+        score_2 = bw_2.stats(
+            chrom, start, end, type=score_type, exact=exact_scores).pop()
+        if (isinstance(score_1, (int, float)) is False):
+            if keep_NA:
+                score_1 = np.nan
+            else:
+                continue
+        if (isinstance(score_2, (int, float)) is False):
+            if keep_NA:
+                score_2 = np.nan
+            else:
+                continue
+        names.append(region_id)
+        scores_1.append(score_1)
+        scores_2.append(score_2)
+
+    bw1_name = os.path.basename(bw1) + '.' + score_type
+    bw2_name = os.path.basename(bw2) + '.' + score_type
+    df = pd.DataFrame(data={bw1_name: scores_1,
+                            bw2_name: scores_2},
+                      index=names,
+                      dtype=float)
+
+    logging.info("Sort dataframe by summary statistical scores ...")
+    df.sort_values(by=[bw1_name, bw1_name],
+                   ascending=False,
+                   ignore_index=False,
+                   inplace=True)
+
+    logging.info("Save dataframe to: \"%s\"" % outfile)
+    df.to_csv(outfile,
+              na_rep=na_label,
+              sep="\t",
+              index=True,
+              header=True,
+              index_label="region_id")
+
+    # Still remove NAs, in order to calculate correlations
+    # if keep_NA:
+    df = df[df > min_sig]
+    df.dropna(axis=0, inplace=True)
+
+    if top_x > 0 and top_x <= 1:
+        top_n = int(len(df) * top_x)
+        logging.info("Select %d regions ..." % top_n)
+        df = df.head(top_n)
+    elif top_x > 1:
+        top_n = top_x
+        logging.info("Select %d regions ..." % top_n)
+        df = df.head(top_n)
+
+    (pearson_cor, pearson_p) = pearsonr(
+        np.log2(df[bw1_name]), np.log2(df[bw2_name]))
+    (spearman_rho, spearman_p) = spearmanr(
+        np.log2(df[bw1_name]), np.log2(df[bw2_name]))
+    (kendall_tau, kendall_p) = kendalltau(
+        np.log2(df[bw1_name]), np.log2(df[bw2_name]))
+
+    return (pd.DataFrame(data={'Pearson_cor:': [pearson_cor, pearson_p],
+                               'Spearman_rho:': [spearman_rho, spearman_p],
+                               'Kendall_tau:': [kendall_tau, kendall_p]},
+                         index=['Correlation', 'P-value']))
```

### Comparing `cobind-1.0.0/lib/cobindability/coefcal.py` & `cobind-1.0.1/lib/cobindability/coefcal.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 __version__ = version.version
 __maintainer__ = "Liguo Wang"
 __email__ = "wang.liguo@mayo.edu"
 __status__ = "Development"
 
 def ov_coef(x, y, xy, g):
 	"""
-	Calculate the overlap coefficient.
+	Calculate the collocation coefficient.
 
 	Parameters
 	----------
 	x : int
 		The cardinality of A.
 	y : int
 		The cardinality of B.
@@ -34,15 +34,15 @@
 		The cardinality of A AND B.
 	g : int
 		The cardinality of background.
 
 	Returns
 	-------
 	float
-		Overlap coefficient.
+		Collocation coefficient.
 	"""
 	if xy > x or xy > y:
 		logging.error("Invalid parameters.")
 	if min(x,y,xy) < 0:
 		logging.error("Invalid parameters.")
 	if x == 0 or y == 0 or xy == 0:
 		return 0
@@ -204,8 +204,8 @@
 		logging.error("Invalid parameters.")
 	px = x/g
 	py = y/g
 	pxy = xy/g
 	if pxy == 0:
 		return -1
 	else:
-		return np.log(px*py)/np.log(pxy) - 1
+		return np.log(px*py)/np.log(pxy) - 1
```

### Comparing `cobind-1.0.0/lib/cobindability/findbed.py` & `cobind-1.0.1/lib/cobindability/findbed.py`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/ireader.py` & `cobind-1.0.1/lib/cobindability/ireader.py`

 * *Files identical despite different names*

### Comparing `cobind-1.0.0/lib/cobindability/ovstat.py` & `cobind-1.0.1/lib/cobindability/ovstat.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,123 +5,122 @@
 
 @author: m102324
 """
 
 import sys
 import logging
 import pandas as pd
-from cobindability.BED import bed_overlap_size, bedtolist, bedinfo
+from scipy import stats
+from cobindability.BED import bed_overlap_size, bed_to_list, bed_info
 from cobindability.coefcal import ov_coef, ov_jaccard, ov_ss, ov_sd, pmi_value, npmi_value
 from cobindability import version
 
 
 __author__ = "Liguo Wang"
 __copyright__ = "Copyleft"
 __credits__ = []
 __license__ = "MIT"
 __version__ = version.version
 __maintainer__ = "Liguo Wang"
 __email__ = "wang.liguo@mayo.edu"
 __status__ = "Development"
 
 
-def ov_stats(file1, file2, bg_size = 1400000000):
-	"""
-
-	Parameters
-	----------
-	file1 : str
-		Genomic regions in BED (Browser Extensible Data, https://genome.ucsc.edu/FAQ/FAQformat.html#format1), BED-like or BigBed format.
-		The BED-like format includes 'bed3','bed4','bed6','bed12','bedgraph','narrowpeak', 'broadpeak','gappedpeak'. BED and BED-like
-		format can be plain text, compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress
-		BigBed foramt. BigBed file can also be a remote file.
-	file2 : str
-		Genomic regions in BED (Browser Extensible Data, https://genome.ucsc.edu/FAQ/FAQformat.html#format1), BED-like or BigBed format.
-		The BED-like format includes 'bed3','bed4','bed6','bed12','bedgraph','narrowpeak', 'broadpeak','gappedpeak'. BED and BED-like
-		format can be plain text, compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress
-		BigBed foramt. BigBed file can also be a remote file.
-	draws_n : int
-		Times of drawing samples with replacement. Set to '0' to turn off bootstraping.
-	draw_frac : float, optional
-		The size of subsample. The default is 0.85 (85% of the orignal genomic reginos will be selected).
-	bg_size : int, optional
-		The effective background genome size. About 1.4Gb of the human genome are. The default is 1424655930.
-
-	Returns
-	-------
-	pandas.Series
-		Pandas Series of 'coef_obs', 'coef_exp','coef_ratio', 'coef_ratio_low', 'coef_ratio_high'.
-		'coef_obs' : Observed overlap coefficient between two BED files.
-		'coef_exp' : Expected overlap coefficient between two BED files.
-		'coef_ratio' : Ratio between 'coef_obs' and 'coef_exp'.
-		'coef_ratio_low' : The lower bound of 95% confidence interval of 'coef_ratio'.
-		'coef_ratio_high' : The upper bound of 95% confidence interval of 'coef_ratio'.
-
-
-	"""
-	results = {}
-	file1_lst = bedtolist (file1)
-	file2_lst = bedtolist (file2)
-
-
-	logging.info("Gathering information for \"%s\" ..." % file1)
-	info1 = bedinfo(file1)
-	results['A.name'] = info1['Name']
-	results['A.interval_count'] = info1['Count']
-	results['A.interval_total_size'] = info1['Total_size']
-	#results['A.interval_uniq_size'] = info1['Genomic_size']
-	results['A.interval_mean_size'] = info1['Mean_size']
-	results['A.interval_median_size'] = info1['Median_size']
-	results['A.interval_min_size'] = info1['Min_size']
-	results['A.interval_max_size'] = info1['Max_size']
-	results['A.interval_size_SD'] = info1['STD']
-	uniqBase1 = info1['Genomic_size']
-
-	logging.info("Gathering information for \"%s\" ..." % file2)
-	info2 = bedinfo(file2)
-	results['B.name'] = info2['Name']
-	results['B.interval_count'] = info2['Count']
-	results['B.interval_total_size'] = info2['Total_size']
-	#results['B.interval_uniq_size'] = info2['Genomic_size']
-	results['B.interval_mean_size'] = info2['Mean_size']
-	results['B.interval_median_size'] = info2['Median_size']
-	results['B.interval_min_size'] = info2['Min_size']
-	results['B.interval_max_size'] = info2['Max_size']
-	results['B.interval_size_SD'] = info2['STD']
-	uniqBase2 = info2['Genomic_size']
-
-	#calculate overall overlap coef
-	logging.debug("Calculating overlapped bases ...")
-	overlapBases = bed_overlap_size(file1_lst, file2_lst)
-
-	results['G.size'] = bg_size
-	results['A.size'] = uniqBase1
-	results['Not_A.size'] = bg_size - uniqBase1
-	results['B.size'] = uniqBase2
-	results['Not_B.size'] = bg_size - uniqBase2
-	results['A_not_B.size'] = uniqBase1 - overlapBases
-	results['B_not_A.size'] = uniqBase2 - overlapBases
-	results['A_and_B.size'] = overlapBases
-	results['A_and_B.exp_size'] = uniqBase1 * uniqBase2/bg_size
-	results['A_or_B.size'] = uniqBase1 + uniqBase2 -overlapBases
-	results['Neither_A_nor_B.size'] = bg_size - uniqBase1 - uniqBase2 + overlapBases
-
-
-	results['coef.Overlap'] = ov_coef(uniqBase1, uniqBase2, overlapBases, bg_size)
-	results['coef.Jaccard'] = ov_jaccard(uniqBase1, uniqBase2, overlapBases, bg_size)
-	results['coef.Dice'] = ov_sd(uniqBase1, uniqBase2, overlapBases, bg_size)
-	results['coef.SS'] = ov_ss(uniqBase1, uniqBase2, overlapBases, bg_size)
-	results['A_and_B.PMI'] = pmi_value(uniqBase1, uniqBase2, overlapBases, bg_size)
-	results['A_and_B.NPMI'] = npmi_value(uniqBase1, uniqBase2, overlapBases, bg_size)
-
-
-	return pd.Series(data=results)
-
-
+def ov_stats(file1, file2, name1 = None, name2 = None, bg_size = 1400000000):
+    """
+    Parameters
+    ----------
+    file1 : str
+        Genomic regions in BED (Browser Extensible Data, https://genome.ucsc.edu/FAQ/FAQformat.html#format1), BED-like or BigBed format.
+        The BED-like format includes 'bed3','bed4','bed6','bed12','bedgraph','narrowpeak', 'broadpeak','gappedpeak'. BED and BED-like
+        format can be plain text, compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress
+        BigBed foramt. BigBed file can also be a remote file.
+    file2 : str
+        Genomic regions in BED (Browser Extensible Data, https://genome.ucsc.edu/FAQ/FAQformat.html#format1), BED-like or BigBed format.
+        The BED-like format includes 'bed3','bed4','bed6','bed12','bedgraph','narrowpeak', 'broadpeak','gappedpeak'. BED and BED-like
+        format can be plain text, compressed (.gz, .z, .bz, .bz2, .bzip2) or remote (http://, https://, ftp://) files. Do not compress
+        BigBed foramt. BigBed file can also be a remote file.
+    name1: str, optional
+        Name of the 1st set of genomic interval. The default is None.
+    name2 : str, optional
+        Name of the 2nd set of genomic interval. The default is None.
+    bg_size : int, optional
+        The effective background genome size. About 1.4Gb of the human genome are. The default is 1424655930.
+
+    Returns
+    -------
+    pandas.Series
+        Pandas Series of 'coef_obs', 'coef_exp','coef_ratio', 'coef_ratio_low', 'coef_ratio_high'.
+        'coef_obs' : Observed collocation coefficient between two BED files.
+        'coef_exp' : Expected collocation coefficient between two BED files.
+        'coef_ratio' : Ratio between 'coef_obs' and 'coef_exp'.
+        'coef_ratio_low' : The lower bound of 95% confidence interval of 'coef_ratio'.
+        'coef_ratio_high' : The upper bound of 95% confidence interval of 'coef_ratio'.
+
+    """
+    print(name1, name2)
+    results = {}
+    file1_lst = bed_to_list(file1)
+    file2_lst = bed_to_list(file2)
+
+    logging.info("Gathering information for \"%s\" ..." % file1)
+    info1 = bed_info(file1)
+    if name1 is None:
+        results['A.name'] = info1['Name']
+    else:
+        results['A.name'] = name1
+    results['A.interval_count'] = info1['Count']
+    results['A.interval_total_size'] = info1['Total_size']
+    # results['A.interval_uniq_size'] = info1['Genomic_size']
+    results['A.interval_mean_size'] = info1['Mean_size']
+    results['A.interval_median_size'] = info1['Median_size']
+    results['A.interval_min_size'] = info1['Min_size']
+    results['A.interval_max_size'] = info1['Max_size']
+    results['A.interval_size_SD'] = info1['STD']
+    uniqBase1 = info1['Genomic_size']
+
+    logging.info("Gathering information for \"%s\" ..." % file2)
+    info2 = bed_info(file2)
+    if name2 is None:
+        results['B.name'] = info2['Name']
+    else:
+        results['B.name'] = name2
+    results['B.interval_count'] = info2['Count']
+    results['B.interval_total_size'] = info2['Total_size']
+    # results['B.interval_uniq_size'] = info2['Genomic_size']
+    results['B.interval_mean_size'] = info2['Mean_size']
+    results['B.interval_median_size'] = info2['Median_size']
+    results['B.interval_min_size'] = info2['Min_size']
+    results['B.interval_max_size'] = info2['Max_size']
+    results['B.interval_size_SD'] = info2['STD']
+    uniqBase2 = info2['Genomic_size']
+
+    # calculate overall collocation coef
+    logging.debug("Calculating overlapped bases ...")
+    overlapBases = bed_overlap_size(file1_lst, file2_lst)
+
+    results['G.size'] = bg_size
+    results['A.size'] = uniqBase1
+    results['Not_A.size'] = bg_size - uniqBase1
+    results['B.size'] = uniqBase2
+    results['Not_B.size'] = bg_size - uniqBase2
+    results['A_not_B.size'] = uniqBase1 - overlapBases
+    results['B_not_A.size'] = uniqBase2 - overlapBases
+    results['A_and_B.size'] = overlapBases
+    results['A_and_B.exp_size'] = uniqBase1 * uniqBase2/bg_size
+    results['A_or_B.size'] = uniqBase1 + uniqBase2 - overlapBases
+    results['Neither_A_nor_B.size'] = bg_size - uniqBase1 - uniqBase2 + overlapBases
+
+    results['coef.Collocation'] = ov_coef(uniqBase1, uniqBase2, overlapBases, bg_size)
+    results['coef.Jaccard'] = ov_jaccard(uniqBase1, uniqBase2, overlapBases, bg_size)
+    results['coef.Dice'] = ov_sd(uniqBase1, uniqBase2, overlapBases, bg_size)
+    results['coef.SS'] = ov_ss(uniqBase1, uniqBase2, overlapBases, bg_size)
+    results['A_and_B.PMI'] = pmi_value(uniqBase1, uniqBase2, overlapBases, bg_size)
+    results['A_and_B.NPMI'] = npmi_value(uniqBase1, uniqBase2, overlapBases, bg_size)
 
+    return pd.Series(data=results)
 
 
 if __name__ == '__main__':
-	pd.set_option('display.float_format', lambda x: '%.4f' % x)
-	a = ov_stats(sys.argv[1], sys.argv[2])
-	print (a)
-
+    pd.set_option('display.float_format', lambda x: '%.4f' % x)
+    a = ov_stats(sys.argv[1], sys.argv[2])
+    print(a)
```

### Comparing `cobind-1.0.0/setup.py` & `cobind-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import sys, os, platform, glob
 from distutils.core import setup
 from setuptools import *
 
 """
-Setup script for cobind  -- collocation analysis of genomics regions.
+Setup script for cobind  -- collocation analysis of genomics intervals.
 """
 
 
 def main():
     setup(  name = "cobind",
-            version = "1.0.0",
+            version = "1.0.1",
             python_requires='>=3.5',
             py_modules = [ 'psyco_full' ],
             packages = find_packages( 'lib' ),
             package_dir = { '': 'lib' },
             package_data = { '': ['*.ps'] },
             scripts = glob.glob( "bin/*.py"),
             ext_modules = [],
             test_suite = 'nose.collector',
             setup_requires = ['nose>=0.10.4','cython>=0.12'],
             author = "Liguo Wang",
             author_email ="wangliguo78@gmail.com",
             platforms = ['Linux','MacOS'],
             requires = [],
             install_requires = ['scipy', 'numpy', 'pandas', 'bx-python','pyBigWig'],
-            description = "collocation analysis of genomics regions",
+            description = "collocation analysis of genomics intervals",
             url = "https://cobind.readthedocs.io/en/latest/",
             zip_safe = False,
             dependency_links = [],
             classifiers=[
-                'Development Status :: 4 - Beta',
+                'Development Status :: 5 - Production/Stable',
                 'Environment :: Console',
                 'Intended Audience :: Science/Research',
-                'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
+                'License :: OSI Approved :: MIT License',
                 'Operating System :: MacOS :: MacOS X',
                 'Operating System :: POSIX',
                 'Programming Language :: Python',
                 'Topic :: Scientific/Engineering :: Bio-Informatics',
             ],
 
-            keywords='genome regions, overlap coefficient, cooccur, pointwise mutual information',
+            keywords='genome regions, collocation, overlap, cooccur',
              )
 
 
 if __name__ == "__main__":
     main()
```

