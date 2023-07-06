# Comparing `tmp/fio-plot-1.1.6.tar.gz` & `tmp/fio-plot-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio-plot-1.1.6.tar", last modified: Fri Apr 14 22:50:05 2023, max compression
+gzip compressed data, was "fio-plot-1.1.7.tar", last modified: Thu Jul  6 12:01:12 2023, max compression
```

## Comparing `fio-plot-1.1.6.tar` & `fio-plot-1.1.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.178011 fio-plot-1.1.6/
--rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.6/CHANGELOG.md
--rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.6/LICENSE
--rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.6/MANIFEST.in
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-14 22:50:05.177539 fio-plot-1.1.6/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.6/README.md
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.121284 fio-plot-1.1.6/bench_fio/
--rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.128845 fio-plot-1.1.6/bench_fio/benchlib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/benchlib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/checks.py
--rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/display.py
--rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/generatefio.py
--rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/benchlib/network.py
--rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/parseini.py
--rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.6/bench_fio/benchlib/runfio.py
--rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.6/bench_fio/benchlib/supporting.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.130188 fio-plot-1.1.6/bench_fio/scripts/
--rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/scripts/bench-fio.sh
--rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bench_fio/scripts/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.130941 fio-plot-1.1.6/bench_fio/templates/
--rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.6/bench_fio/templates/precondition.fio
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.132554 fio-plot-1.1.6/bin/
--rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bin/bench-fio
--rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.6/bin/fio-plot
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.148867 fio-plot-1.1.6/docs/
--rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.6/docs/bench_fio_call_graph.png
--rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.6/docs/fio_plot_call_graph.png
--rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.6/docs/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.153430 fio-plot-1.1.6/fio_plot/
--rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.6/fio_plot/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.173887 fio-plot-1.1.6/fio_plot/fiolib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.6/fio_plot/fiolib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    11216 2023-04-13 16:36:30.000000 fio-plot-1.1.6/fio_plot/fiolib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     7815 2023-04-13 14:07:16.000000 fio-plot-1.1.6/fio_plot/fiolib/bar2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-04-12 15:00:11.000000 fio-plot-1.1.6/fio_plot/fiolib/bar3d.py
--rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.6/fio_plot/fiolib/barhistogram.py
--rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/dataimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/dataimport_support.py
--rw-r--r--   0 nan03      (501) staff       (20)      781 2023-04-12 15:29:38.000000 fio-plot-1.1.6/fio_plot/fiolib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.6/fio_plot/fiolib/flightchecks.py
--rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/getdata.py
--rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-13 16:47:00.000000 fio-plot-1.1.6/fio_plot/fiolib/graph2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6947 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/graph2dsupporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     2349 2023-04-13 16:36:48.000000 fio-plot-1.1.6/fio_plot/fiolib/iniparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     3275 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     6298 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/jsonparsing_support.py
--rw-r--r--   0 nan03      (501) staff       (20)    14737 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/shared_chart.py
--rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-13 15:02:14.000000 fio-plot-1.1.6/fio_plot/fiolib/supporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     4018 2023-04-14 22:48:06.000000 fio-plot-1.1.6/fio_plot/fiolib/table_support.py
--rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.6/fio_plot/fiolib/tables.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.157043 fio-plot-1.1.6/fio_plot.egg-info/
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/SOURCES.txt
--rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/dependency_links.txt
--rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/entry_points.txt
--rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/requires.txt
--rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-14 22:50:05.000000 fio-plot-1.1.6/fio_plot.egg-info/top_level.txt
--rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-14 22:50:05.178103 fio-plot-1.1.6/setup.cfg
--rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-14 22:48:06.000000 fio-plot-1.1.6/setup.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-14 22:50:05.175636 fio-plot-1.1.6/tests/
--rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.6/tests/bench_fio_test.py
--rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.6/tests/test_3d.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.859130 fio-plot-1.1.7/
+-rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.7/CHANGELOG.md
+-rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.7/LICENSE
+-rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.7/MANIFEST.in
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-07-06 12:01:12.857143 fio-plot-1.1.7/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-07-06 11:34:54.000000 fio-plot-1.1.7/README.md
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.776755 fio-plot-1.1.7/bench_fio/
+-rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.7/bench_fio/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bench_fio/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.781867 fio-plot-1.1.7/bench_fio/benchlib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bench_fio/benchlib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10826 2023-07-06 11:35:07.000000 fio-plot-1.1.7/bench_fio/benchlib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.7/bench_fio/benchlib/checks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2918 2023-07-06 11:35:07.000000 fio-plot-1.1.7/bench_fio/benchlib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3390 2023-07-06 11:35:07.000000 fio-plot-1.1.7/bench_fio/benchlib/display.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2323 2023-07-06 11:35:07.000000 fio-plot-1.1.7/bench_fio/benchlib/generatefio.py
+-rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.7/bench_fio/benchlib/network.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1804 2023-07-06 11:51:55.000000 fio-plot-1.1.7/bench_fio/benchlib/parseini.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6819 2023-07-06 11:35:07.000000 fio-plot-1.1.7/bench_fio/benchlib/runfio.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.7/bench_fio/benchlib/supporting.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.782940 fio-plot-1.1.7/bench_fio/scripts/
+-rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bench_fio/scripts/bench-fio.sh
+-rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bench_fio/scripts/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.783633 fio-plot-1.1.7/bench_fio/templates/
+-rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.7/bench_fio/templates/precondition.fio
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.785033 fio-plot-1.1.7/bin/
+-rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bin/bench-fio
+-rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.7/bin/fio-plot
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.812782 fio-plot-1.1.7/docs/
+-rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.7/docs/bench_fio_call_graph.png
+-rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.7/docs/fio_plot_call_graph.png
+-rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.7/docs/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.819345 fio-plot-1.1.7/fio_plot/
+-rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.7/fio_plot/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.7/fio_plot/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.851814 fio-plot-1.1.7/fio_plot/fiolib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.7/fio_plot/fiolib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    11216 2023-04-13 16:36:30.000000 fio-plot-1.1.7/fio_plot/fiolib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     7815 2023-04-13 14:07:16.000000 fio-plot-1.1.7/fio_plot/fiolib/bar2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-04-12 15:00:11.000000 fio-plot-1.1.7/fio_plot/fiolib/bar3d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.7/fio_plot/fiolib/barhistogram.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.7/fio_plot/fiolib/dataimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.7/fio_plot/fiolib/dataimport_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)      781 2023-04-12 15:29:38.000000 fio-plot-1.1.7/fio_plot/fiolib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.7/fio_plot/fiolib/flightchecks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.7/fio_plot/fiolib/getdata.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-13 16:47:00.000000 fio-plot-1.1.7/fio_plot/fiolib/graph2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6947 2023-04-14 22:48:06.000000 fio-plot-1.1.7/fio_plot/fiolib/graph2dsupporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2349 2023-04-13 16:36:48.000000 fio-plot-1.1.7/fio_plot/fiolib/iniparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.7/fio_plot/fiolib/jsonimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3275 2023-04-14 22:48:06.000000 fio-plot-1.1.7/fio_plot/fiolib/jsonparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6298 2023-04-14 22:48:06.000000 fio-plot-1.1.7/fio_plot/fiolib/jsonparsing_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)    14737 2023-04-14 22:48:06.000000 fio-plot-1.1.7/fio_plot/fiolib/shared_chart.py
+-rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-13 15:02:14.000000 fio-plot-1.1.7/fio_plot/fiolib/supporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4018 2023-04-14 22:48:06.000000 fio-plot-1.1.7/fio_plot/fiolib/table_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.7/fio_plot/fiolib/tables.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.823191 fio-plot-1.1.7/fio_plot.egg-info/
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 nan03      (501) staff       (20)        1 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       70 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/entry_points.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       40 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/requires.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       19 2023-07-06 12:01:12.000000 fio-plot-1.1.7/fio_plot.egg-info/top_level.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       38 2023-07-06 12:01:12.859370 fio-plot-1.1.7/setup.cfg
+-rw-r--r--   0 nan03      (501) staff       (20)      909 2023-07-06 11:37:25.000000 fio-plot-1.1.7/setup.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-07-06 12:01:12.853722 fio-plot-1.1.7/tests/
+-rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.7/tests/bench_fio_test.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.7/tests/test_3d.py
```

### Comparing `fio-plot-1.1.6/CHANGELOG.md` & `fio-plot-1.1.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/LICENSE` & `fio-plot-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/PKG-INFO` & `fio-plot-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.6
+Version: 1.1.7
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.6/README.md` & `fio-plot-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/bench_fio/__init__.py` & `fio-plot-1.1.7/bench_fio/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/argparsing.py` & `fio-plot-1.1.7/bench_fio/benchlib/argparsing.py`

 * *Files 7% similar despite different names*

```diff
@@ -273,14 +273,20 @@
     )
     ag.add_argument(
         "--create",
         help="Create target files if they don't exist. This is the default for fio but not for bench_fio",
         action="store_true",
         default=False,
     )
+    ag.add_argument(
+        "--parallel",
+        help="Testing devices in parallel. The default for testing devices in sequential",
+        action="store_true",
+        default=False,
+    )
     return parser
 
 def get_argument_description():
     descriptions = {
         "target": "Test target(s)",
         "template": "Job template",
         "engine": "I/O Engine",
@@ -308,10 +314,11 @@
         "ss_ramp": "Steady state rampup",
         "entire_device": "Benchmark entire device",
         "ceph_pool": "Ceph RBD pool",
         "destructive": "Allow destructive writes",
         "remote":"Use remote server",
         "remote_checks": "Check remote for open TCP port",
         "remote_timeout": "Check remote timeout (s)",
-        "create": "Create if target doesn't exist"
+        "create": "Create if target doesn't exist",
+        "parallel": "Testing devices in parallel"
     }
     return descriptions
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/checks.py` & `fio-plot-1.1.7/bench_fio/benchlib/checks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/defaultsettings.py` & `fio-plot-1.1.7/bench_fio/benchlib/defaultsettings.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     settings["mixed"] = ["readwrite", "rw", "randrw"]
     settings["invalidate"] = 1
     settings["ceph_pool"] = None
     settings["destructive"] = False
     settings["remote"] = False
     settings["remote_checks"] = False
     settings["remote_timeout"] = 2
-    settings["tmpjobfile"] = "/tmp/tmpjobfile.fio"
     settings["create"] = False
+    settings["parallel"] = False
     settings["loop_items"] = [
         "target",
         "mode",
         "iodepth",
         "numjobs",
         "block_size",
     ]
@@ -72,15 +72,16 @@
         "type",
         "benchmarks",
         "entire_device",
         "basename_list",
         "destructive",
         "precondition",
         "template",
-        "create"
+        "create",
+        "parallel"
     ]
     settings["basename_list"] = [
         "precondition_template"
     ]
     return settings
 
 def map_settings_to_fio():
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/display.py` & `fio-plot-1.1.7/bench_fio/benchlib/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
                 if length > max_length:
                     max_length = length
     data["length"] = max_length
     return data
 
 def calculate_duration(settings, tests):
     number_of_tests = len(tests) * settings["loops"]
+    if settings["parallel"]:
+        number_of_tests = number_of_tests/len(settings["target"])
     time_per_test = settings["runtime"]
     if time_per_test:
         duration_in_seconds = number_of_tests * time_per_test
         duration = str(datetime.timedelta(seconds=duration_in_seconds))
     else:
         duration = None
     return duration
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/generatefio.py` & `fio-plot-1.1.7/bench_fio/benchlib/generatefio.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 import configparser
 from . import (defaultsettings, checks)
 
-def write_fio_job_file(settings, parser):
+def write_fio_job_file(tmpjobfile, parser):
     try:
-        with open(f"{settings['tmpjobfile']}", 'w') as configfile:
+        with open(tmpjobfile, 'w') as configfile:
             parser.write(configfile, space_around_delimiters=False)
     except IOError:
-        print(f"Failed to write temporary Fio job file at {settings['tmpjobfile']}")
+        print(f"Failed to write temporary Fio job file at tmpjobfile")
 
 def filter_options(settings, config, mapping, benchmark, output_directory):
     boolean = {"True": 1, "False": 0}
     config['FIOJOB'] = {}
     for k,v in settings.items():
         key = k
         value = v
@@ -33,14 +33,14 @@
         #print(f"key: {key} - Value: {value} - {type(value)}")
 
     config['FIOJOB']["write_bw_log"] = f"{output_directory}/{benchmark['mode']}-iodepth-{benchmark['iodepth']}-numjobs-{benchmark['numjobs']}"
     config['FIOJOB']["write_lat_log"] = f"{output_directory}/{benchmark['mode']}-iodepth-{benchmark['iodepth']}-numjobs-{benchmark['numjobs']}"
     config['FIOJOB']["write_iops_log"] = f"{output_directory}/{benchmark['mode']}-iodepth-{benchmark['iodepth']}-numjobs-{benchmark['numjobs']}"
     return config
 
-def generate_fio_job_file(settings, benchmark, output_directory):
+def generate_fio_job_file(settings, benchmark, output_directory, tmpjobfile):
     config = configparser.ConfigParser()
     mapping = defaultsettings.map_settings_to_fio()
     config = filter_options(settings, config, mapping, benchmark, output_directory)
-    write_fio_job_file(settings, config)
+    write_fio_job_file(tmpjobfile, config)
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/network.py` & `fio-plot-1.1.7/bench_fio/benchlib/network.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/parseini.py` & `fio-plot-1.1.7/bench_fio/benchlib/parseini.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,18 @@
         else:
             returndict[x] = config["benchfio"][x]
     return returndict
 
 def read_ini_data(args, config):
     if len(args) != 2:
         return False
-    
-    filename = args[1]
+    if args[1] == "-h" or args[1] == "--help":
+        return False
+    else:
+        filename = args[1]
     
     if not os.path.isfile(filename):
         print(f"Config file {filename} not found.")
         sys.exit(1)
     
     try:
         config.read(filename)
@@ -44,8 +46,10 @@
     return True
 
 
 def get_settings_from_ini(args):
     config = configparser.ConfigParser(converters={'list': lambda x: [i.strip() for i in x.split(',')]})
     if read_ini_data(args, config):
         returndict = process_options(config)
-        return returndict
+        return returndict
+    else:
+        return None
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/runfio.py` & `fio-plot-1.1.7/bench_fio/benchlib/runfio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python3
 import subprocess
 import sys
 import os
 import copy
 from numpy import linspace
 import time
+from operator import itemgetter
+from itertools import groupby
+from threading import Thread
 
 from . import ( 
     supporting,
     generatefio,
     defaultsettings
 )
 
@@ -38,30 +41,31 @@
     except KeyboardInterrupt:
         print(f"\n ctrl-c pressed - Aborted by user....\n")
         sys.exit(1)
     return result
 
 
 def run_fio(settings, benchmark):
+    tmpjobfile = f"/tmp/{os.path.basename(benchmark['target'])}-tmpjobfile.fio"
     output_directory = supporting.generate_output_directory(settings, benchmark)
     output_file = f"{output_directory}/{benchmark['mode']}-{benchmark['iodepth']}-{benchmark['numjobs']}.json"
-    generatefio.generate_fio_job_file(settings, benchmark, output_directory)
+    generatefio.generate_fio_job_file(settings, benchmark, output_directory, tmpjobfile)
     
     ### We build up the fio command line here
     command = [
         "fio"
     ]
     
     command.append("--output-format=json")
     command.append(f"--output={output_file}") # fio bug
 
     if settings["remote"]:
         command.append(f"--client={settings['remote']}")
 
-    command.append(settings["tmpjobfile"])
+    command.append(tmpjobfile)
     # End of command line creation
     
     if not settings["dry_run"]:
         supporting.make_directory(output_directory)
         run_raw_command(command, output_file)
         if settings["remote"]:
             fix_json_file(output_file) # to fix FIO json output bug
@@ -110,28 +114,48 @@
             run_fio(settings_copy, benchmark)
 
     elif settings["precondition"] and not settings["destructive"]:
         print(f"\n When running preconditionning, also enable the destructive flag to be 100% sure.\n")
         sys.exit(1)
 
 
-def run_benchmarks(settings, benchmarks):
-    # pprint.pprint(benchmarks)
+def worker(benchmarks, settings):
     run = 0
     progress_benchmarks = ProgressBar(benchmarks) if not settings["quiet"] else benchmarks
     for benchmark in progress_benchmarks:
         loops = 0
         while loops < settings["loops"]:
             run += 1
             loops += 1
             run_precondition_benchmark(settings, benchmark["target"], run)
             drop_caches()
             run_fio(settings, benchmark)
 
 
+def run_benchmarks(settings, benchmarks):
+    # pprint.pprint(benchmarks)
+    if not settings["parallel"]:
+        worker(benchmarks, settings)
+    else:
+        group_benchmarks = []
+        for _, items in groupby(benchmarks, key=itemgetter("target")):
+            group_benchmarks.append(list(items))
+        thread_list = []
+        for target in range(len(group_benchmarks)):
+            t = Thread(target=worker, args=(group_benchmarks[target], settings))
+            thread_list.append(t)
+    
+        for t in thread_list:
+            t.setDaemon(True)
+            t.start()
+
+        for t in thread_list:
+            t.join()
+
+
 def ProgressBar(iterObj):
     """https://stackoverflow.com/questions/3160699/python-progress-bar/49234284#49234284"""
 
     def SecToStr(sec):
         m, s = divmod(sec, 60)
         h, m = divmod(m, 60)
         return "%d:%02d:%02d" % (h, m, s)
```

### Comparing `fio-plot-1.1.6/bench_fio/benchlib/supporting.py` & `fio-plot-1.1.7/bench_fio/benchlib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/bench_fio/scripts/bench-fio.sh` & `fio-plot-1.1.7/bench_fio/scripts/bench-fio.sh`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/docs/bench_fio_call_graph.png` & `fio-plot-1.1.7/docs/bench_fio_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/docs/fio_plot_call_graph.png` & `fio-plot-1.1.7/docs/fio_plot_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/__init__.py` & `fio-plot-1.1.7/fio_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/argparsing.py` & `fio-plot-1.1.7/fio_plot/fiolib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/bar2d.py` & `fio-plot-1.1.7/fio_plot/fiolib/bar2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/bar3d.py` & `fio-plot-1.1.7/fio_plot/fiolib/bar3d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/barhistogram.py` & `fio-plot-1.1.7/fio_plot/fiolib/barhistogram.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/dataimport.py` & `fio-plot-1.1.7/fio_plot/fiolib/dataimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/dataimport_support.py` & `fio-plot-1.1.7/fio_plot/fiolib/dataimport_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/defaultsettings.py` & `fio-plot-1.1.7/fio_plot/fiolib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/flightchecks.py` & `fio-plot-1.1.7/fio_plot/fiolib/flightchecks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/getdata.py` & `fio-plot-1.1.7/fio_plot/fiolib/getdata.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/graph2d.py` & `fio-plot-1.1.7/fio_plot/fiolib/graph2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/graph2dsupporting.py` & `fio-plot-1.1.7/fio_plot/fiolib/graph2dsupporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/iniparsing.py` & `fio-plot-1.1.7/fio_plot/fiolib/iniparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/jsonimport.py` & `fio-plot-1.1.7/fio_plot/fiolib/jsonimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/jsonparsing.py` & `fio-plot-1.1.7/fio_plot/fiolib/jsonparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/jsonparsing_support.py` & `fio-plot-1.1.7/fio_plot/fiolib/jsonparsing_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/shared_chart.py` & `fio-plot-1.1.7/fio_plot/fiolib/shared_chart.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/supporting.py` & `fio-plot-1.1.7/fio_plot/fiolib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/table_support.py` & `fio-plot-1.1.7/fio_plot/fiolib/table_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot/fiolib/tables.py` & `fio-plot-1.1.7/fio_plot/fiolib/tables.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/fio_plot.egg-info/PKG-INFO` & `fio-plot-1.1.7/fio_plot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.6
+Version: 1.1.7
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.6/fio_plot.egg-info/SOURCES.txt` & `fio-plot-1.1.7/fio_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/setup.py` & `fio-plot-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="fio-plot",
-        version="1.1.6",
+        version="1.1.7",
         author="louwrentius",
         description="Create charts from FIO storage benchmark tool output",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/louwrentius/fio-plot/", 
         packages=setuptools.find_packages(),
         install_requires=['numpy','matplotlib','Pillow', 'pyan3', 'pyparsing'],
```

### Comparing `fio-plot-1.1.6/tests/bench_fio_test.py` & `fio-plot-1.1.7/tests/bench_fio_test.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.6/tests/test_3d.py` & `fio-plot-1.1.7/tests/test_3d.py`

 * *Files identical despite different names*

