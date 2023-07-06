# Comparing `tmp/funfluid-202307061936.tar.gz` & `tmp/funfluid-202307061944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funfluid-202307061936.tar", last modified: Thu Jul  6 11:36:50 2023, max compression
+gzip compressed data, was "funfluid-202307061944.tar", last modified: Thu Jul  6 11:44:02 2023, max compression
```

## Comparing `funfluid-202307061936.tar` & `funfluid-202307061944.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.103154 funfluid-202307061936/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307061936/LICENSE
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-06 11:36:50.103154 funfluid-202307061936/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       84 2023-07-03 09:06:44.000000 funfluid-202307061936/README.md
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/common/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/common/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/common/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/common/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307061936/funfluid/common/base/cache.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/common/flow/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/common/flow/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/common/particle/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/common/particle/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/experiment/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/experiment/chlamydomonas/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/experiment/chlamydomonas/analyse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/analyse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/analyse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid/experiment/chlamydomonas/base/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/base/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/base/base.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/base/globalconfig.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/background.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/contain.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/particle.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/experiment/chlamydomonas/plot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/plot/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/plot/core.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/plot/property.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/experiment/chlamydomonas/progress/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/progress/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/progress/video_progress.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307061936/funfluid/experiment/chlamydomonas/run.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/lbm/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/lbm/core/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/core/__init__.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1871 2023-07-03 11:14:20.000000 funfluid-202307061936/funfluid/lbm/core/buff.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-07-03 11:15:06.000000 funfluid-202307061936/funfluid/lbm/core/lattice.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/core/shape.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/core/speed_nb.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/lbm/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/example_cavity1.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/example_cavity3.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/example_obstacle.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/example_poiseuille.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/example/example_turek.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/obs_array.py
--rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/lbm/params.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307061936/funfluid/simulate/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/simulate/ellipse/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307061936/funfluid/simulate/ellipse/analyse.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/example/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/simulate/ellipse/example/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307061936/funfluid/simulate/ellipse/example/largs_plot_example.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/simulate/ellipse/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/project/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1441 2023-07-03 09:06:44.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/example.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/project/models/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/models/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/models/flow.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1232 2023-07-06 09:11:33.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/project.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/project/track/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       47 2023-07-03 09:47:30.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/track/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7672 2023-07-06 11:36:47.000000 funfluid-202307061936/funfluid/simulate/ellipse/project/track/plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/simulate/ellipse/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/simulate/ellipse/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/simulate/ellipse/utils/largs_plot.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/tecplot/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/tecplot/__init__.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/tecplot/templates/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/tecplot/templates/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307061936/funfluid/tecplot/templates/templates1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.099154 funfluid-202307061936/funfluid/tecplot/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/tecplot/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/tecplot/utils/connect.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.103154 funfluid-202307061936/funfluid/temp/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/temp/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-07-03 10:43:22.000000 funfluid-202307061936/funfluid/temp/data_fit.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      108 2023-07-03 10:43:39.000000 funfluid-202307061936/funfluid/temp/temp1.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.103154 funfluid-202307061936/funfluid/utils/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061936/funfluid/utils/__init__.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307061936/funfluid/utils/log.py
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307061936/funfluid/utils/timer.py
-drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:36:50.095153 funfluid-202307061936/funfluid.egg-info/
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-06 11:36:50.000000 funfluid-202307061936/funfluid.egg-info/PKG-INFO
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2670 2023-07-06 11:36:50.000000 funfluid-202307061936/funfluid.egg-info/SOURCES.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-06 11:36:50.000000 funfluid-202307061936/funfluid.egg-info/dependency_links.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-06 11:36:50.000000 funfluid-202307061936/funfluid.egg-info/requires.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-06 11:36:50.000000 funfluid-202307061936/funfluid.egg-info/top_level.txt
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-06 11:36:50.103154 funfluid-202307061936/setup.cfg
--rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307061936/setup.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.975550 funfluid-202307061944/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    11357 2023-06-30 08:49:06.000000 funfluid-202307061944/LICENSE
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-06 11:44:02.975550 funfluid-202307061944/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       84 2023-07-03 09:06:44.000000 funfluid-202307061944/README.md
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.959550 funfluid-202307061944/funfluid/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        2 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.963549 funfluid-202307061944/funfluid/common/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/common/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.963549 funfluid-202307061944/funfluid/common/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/common/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2837 2023-06-30 08:49:51.000000 funfluid-202307061944/funfluid/common/base/cache.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.963549 funfluid-202307061944/funfluid/common/flow/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/common/flow/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/common/particle/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/common/particle/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/analyse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/analyse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4563 2023-06-30 08:50:16.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/analyse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/base/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/base/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3815 2023-06-30 08:50:20.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/base/base.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1869 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/base/globalconfig.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2977 2023-06-30 08:50:23.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/background.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     4707 2023-06-30 08:50:30.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/contain.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     9205 2023-06-30 08:50:37.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/particle.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/plot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/plot/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/plot/core.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      239 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/plot/property.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/experiment/chlamydomonas/progress/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/progress/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2909 2023-06-30 08:50:45.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/progress/video_progress.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1573 2023-06-30 08:50:10.000000 funfluid-202307061944/funfluid/experiment/chlamydomonas/run.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/lbm/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       64 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/lbm/core/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       70 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/core/__init__.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     1871 2023-07-03 11:14:20.000000 funfluid-202307061944/funfluid/lbm/core/buff.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    21837 2023-07-03 11:15:06.000000 funfluid-202307061944/funfluid/lbm/core/lattice.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)    13442 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/core/shape.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    10645 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/core/speed_nb.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/lbm/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1921 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/example_cavity1.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1994 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/example_cavity3.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3324 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/example_obstacle.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2581 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/example_poiseuille.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3349 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/example/example_turek.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     3662 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/obs_array.py
+-rwxrwxr-x   0 bingtao   (1000) bingtao   (1000)     2364 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/lbm/params.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/simulate/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:53:23.000000 funfluid-202307061944/funfluid/simulate/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/simulate/ellipse/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/simulate/ellipse/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 12:54:13.000000 funfluid-202307061944/funfluid/simulate/ellipse/analyse.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.967550 funfluid-202307061944/funfluid/simulate/ellipse/example/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/simulate/ellipse/example/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     3179 2023-06-30 08:49:55.000000 funfluid-202307061944/funfluid/simulate/ellipse/example/largs_plot_example.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1379 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/simulate/ellipse/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/simulate/ellipse/project/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:31:46.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1441 2023-07-03 09:06:44.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/example.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/simulate/ellipse/project/models/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:36.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/models/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 13:34:30.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/models/flow.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1232 2023-07-06 09:11:33.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/project.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/simulate/ellipse/project/track/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       47 2023-07-03 09:47:30.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/track/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     7744 2023-07-06 11:44:01.000000 funfluid-202307061944/funfluid/simulate/ellipse/project/track/plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/simulate/ellipse/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/simulate/ellipse/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      563 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/simulate/ellipse/utils/largs_plot.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/tecplot/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/tecplot/__init__.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/tecplot/templates/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/tecplot/templates/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)    15193 2023-06-30 08:50:52.000000 funfluid-202307061944/funfluid/tecplot/templates/templates1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/tecplot/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/tecplot/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      143 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/tecplot/utils/connect.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.971550 funfluid-202307061944/funfluid/temp/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/temp/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     1405 2023-07-03 10:43:22.000000 funfluid-202307061944/funfluid/temp/data_fit.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      108 2023-07-03 10:43:39.000000 funfluid-202307061944/funfluid/temp/temp1.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.975550 funfluid-202307061944/funfluid/utils/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        0 2023-06-30 08:49:06.000000 funfluid-202307061944/funfluid/utils/__init__.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      262 2023-06-30 08:50:57.000000 funfluid-202307061944/funfluid/utils/log.py
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      729 2023-06-30 08:50:55.000000 funfluid-202307061944/funfluid/utils/timer.py
+drwxrwxr-x   0 bingtao   (1000) bingtao   (1000)        0 2023-07-06 11:44:02.963549 funfluid-202307061944/funfluid.egg-info/
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      188 2023-07-06 11:44:02.000000 funfluid-202307061944/funfluid.egg-info/PKG-INFO
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)     2670 2023-07-06 11:44:02.000000 funfluid-202307061944/funfluid.egg-info/SOURCES.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        1 2023-07-06 11:44:02.000000 funfluid-202307061944/funfluid.egg-info/dependency_links.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       30 2023-07-06 11:44:02.000000 funfluid-202307061944/funfluid.egg-info/requires.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)        9 2023-07-06 11:44:02.000000 funfluid-202307061944/funfluid.egg-info/top_level.txt
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)       38 2023-07-06 11:44:02.975550 funfluid-202307061944/setup.cfg
+-rw-rw-r--   0 bingtao   (1000) bingtao   (1000)      421 2023-07-02 11:44:45.000000 funfluid-202307061944/setup.py
```

### Comparing `funfluid-202307061936/LICENSE` & `funfluid-202307061944/LICENSE`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/common/base/cache.py` & `funfluid-202307061944/funfluid/common/base/cache.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/analyse/analyse.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/analyse/analyse.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/base/base.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/base/base.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/base/globalconfig.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/base/globalconfig.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/background.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/background.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/contain.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/contain.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/detect/particle.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/detect/particle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/progress/video_progress.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/progress/video_progress.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/experiment/chlamydomonas/run.py` & `funfluid-202307061944/funfluid/experiment/chlamydomonas/run.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/core/buff.py` & `funfluid-202307061944/funfluid/lbm/core/buff.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/core/lattice.py` & `funfluid-202307061944/funfluid/lbm/core/lattice.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/core/shape.py` & `funfluid-202307061944/funfluid/lbm/core/shape.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/core/speed_nb.py` & `funfluid-202307061944/funfluid/lbm/core/speed_nb.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/example/example_cavity1.py` & `funfluid-202307061944/funfluid/lbm/example/example_cavity1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/example/example_cavity3.py` & `funfluid-202307061944/funfluid/lbm/example/example_cavity3.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/example/example_obstacle.py` & `funfluid-202307061944/funfluid/lbm/example/example_obstacle.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/example/example_poiseuille.py` & `funfluid-202307061944/funfluid/lbm/example/example_poiseuille.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/example/example_turek.py` & `funfluid-202307061944/funfluid/lbm/example/example_turek.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/obs_array.py` & `funfluid-202307061944/funfluid/lbm/obs_array.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/lbm/params.py` & `funfluid-202307061944/funfluid/lbm/params.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/example/largs_plot_example.py` & `funfluid-202307061944/funfluid/simulate/ellipse/example/largs_plot_example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/plot.py` & `funfluid-202307061944/funfluid/simulate/ellipse/plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/project/example.py` & `funfluid-202307061944/funfluid/simulate/ellipse/project/example.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/project/project.py` & `funfluid-202307061944/funfluid/simulate/ellipse/project/project.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/project/track/plot.py` & `funfluid-202307061944/funfluid/simulate/ellipse/project/track/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,26 +101,28 @@
         for i, record in enumerate(self.snapshot_steps):
             self.lns.append(
                 plt.plot([], [], color=record['color'], marker=record['marker'], linewidth=record['line_width'])[0])
         return self.lns
 
     def _get_ellipse_data(self, step, canvas: Canvas, *args, **kwargs):
         a, b = self.a, self.b
-        x0, y0 = self.df['x'][step], self.df['y'][step]
-        theta = self.df['theta'][step]
+        tmp_df = self.df[self.df['step'] == step]
+        x0, y0 = tmp_df['x'][0], tmp_df['y'][0]
+        theta = tmp_df['theta'][0]
         phi = np.array([i / 100. * np.pi for i in range(-1, 201)])
         x = x0 + np.cos(theta) * a * np.cos(phi) - np.sin(theta) * b * np.sin(phi)
         y = y0 + (np.sin(theta) * a * np.cos(phi) + np.cos(theta) * b * np.sin(phi)) / canvas.aspect
 
         x[0] = x0
         y[0] = y0
         return x, y
 
     def plot_update(self, step, canvas: Canvas):
-        self.lns[0].set_data(self.df['x'][:step], self.df['y'][:step])
+        tmp_df = self.df[self.df['step'] <= step]
+        self.lns[0].set_data(tmp_df['x'], tmp_df['y'])
         self.lns[1].set_data(*self._get_ellipse_data(step=step, canvas=canvas))
 
         for i, record in enumerate(self.snapshot_steps):
             if record['step'] <= step:
                 self.lns[i + 2].set_data(*self._get_ellipse_data(record['step'], canvas=canvas))
             else:
                 self.lns[i + 2].set_data([], [])
```

### Comparing `funfluid-202307061936/funfluid/simulate/ellipse/utils/largs_plot.py` & `funfluid-202307061944/funfluid/simulate/ellipse/utils/largs_plot.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/tecplot/templates/templates1.py` & `funfluid-202307061944/funfluid/tecplot/templates/templates1.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/temp/data_fit.py` & `funfluid-202307061944/funfluid/temp/data_fit.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid/utils/timer.py` & `funfluid-202307061944/funfluid/utils/timer.py`

 * *Files identical despite different names*

### Comparing `funfluid-202307061936/funfluid.egg-info/SOURCES.txt` & `funfluid-202307061944/funfluid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

