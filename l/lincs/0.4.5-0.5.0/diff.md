# Comparing `tmp/lincs-0.4.5.tar.gz` & `tmp/lincs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.4.5.tar", last modified: Fri Jun  9 14:38:00 2023, max compression
+gzip compressed data, was "lincs-0.5.0.tar", last modified: Thu Jul  6 13:28:58 2023, max compression
```

## Comparing `lincs-0.4.5.tar` & `lincs-0.5.0.tar`

### file list

```diff
@@ -1,72 +1,248 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.5/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.5/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.5/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:38:00.511468 lincs-0.4.5/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)     4300 2023-06-09 14:37:55.000000 lincs-0.4.5/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      995 2023-06-09 13:32:09.000000 lincs-0.4.5/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    22755 2023-06-09 10:24:25.000000 lincs-0.4.5/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4684 2023-06-09 13:59:35.000000 lincs-0.4.5/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1687 2023-06-09 13:28:54.000000 lincs-0.4.5/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4260 2023-06-09 13:59:28.000000 lincs-0.4.5/lincs/liblincs/io/problem.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1931 2023-06-09 13:26:35.000000 lincs-0.4.5/lincs/liblincs/io/problem.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      983 2023-06-09 12:35:58.000000 lincs-0.4.5/lincs/liblincs/io/validation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      580 2023-06-09 12:31:29.000000 lincs-0.4.5/lincs/liblincs/io/validation.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
--rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
--rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     4872 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    17094 2023-06-09 13:31:54.000000 lincs-0.4.5/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.511468 lincs-0.4.5/lincs/liblincs/linear-programming/
--rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/alglib.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/alglib.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/linear-programming/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/linear-programming/glop.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/liblincs/linear-programming/test.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.5/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.5/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    14126 2023-06-09 08:40:23.000000 lincs-0.4.5/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-09 08:38:44.000000 lincs-0.4.5/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-09 14:38:00.507468 lincs-0.4.5/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)     5184 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     2504 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-09 14:38:00.000000 lincs-0.4.5/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.5/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-09 14:38:00.511468 lincs-0.4.5/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-09 14:37:30.000000 lincs-0.4.5/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-07-04 15:15:34.000000 lincs-0.5.0/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-07-04 15:15:34.000000 lincs-0.5.0/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      122 2023-07-04 15:15:34.000000 lincs-0.5.0/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)     5191 2023-07-06 13:28:58.275458 lincs-0.5.0/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)     4307 2023-07-06 13:28:53.000000 lincs-0.5.0/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1160 2023-07-05 16:05:46.000000 lincs-0.5.0/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    26193 2023-07-06 12:30:08.000000 lincs-0.5.0/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     5634 2023-07-05 07:34:25.000000 lincs-0.5.0/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      369 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    18418 2023-07-05 11:00:30.000000 lincs-0.5.0/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1189 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2735 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1058 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     8254 2023-07-06 06:53:40.000000 lincs-0.5.0/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3158 2023-07-05 07:33:27.000000 lincs-0.5.0/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4923 2023-07-06 06:53:14.000000 lincs-0.5.0/lincs/liblincs/io/problem.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2038 2023-07-06 07:12:12.000000 lincs-0.5.0/lincs/liblincs/io/problem.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1141 2023-07-06 05:20:37.000000 lincs-0.5.0/lincs/liblincs/io/validation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      583 2023-07-06 05:20:22.000000 lincs-0.5.0/lincs/liblincs/io/validation.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      187 2023-07-04 15:15:34.000000 lincs-0.5.0/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/
+-rw-rw-r--   0 user      (1002) user      (1002)       60 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/exception.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      477 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/exception.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/
+-rw-rw-r--   0 user      (1002) user      (1002)      232 2023-07-04 15:51:24.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1072 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/breed/reinitialize-least-accurate.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/
+-rw-rw-r--   0 user      (1002) user      (1002)     1525 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9322 2023-07-06 07:12:50.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1628 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14371 2023-07-06 07:11:39.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-rw-r--   0 user      (1002) user      (1002)     1885 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4508 2023-07-04 15:49:29.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1226 2023-07-04 15:47:09.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     4107 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      838 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      901 2023-07-05 15:47:35.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-iterations.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      913 2023-07-06 08:36:25.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/after-seconds.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      211 2023-07-06 08:30:11.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      779 2023-07-05 15:44:27.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      295 2023-07-05 15:22:15.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      824 2023-07-05 15:44:18.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/terminate/composite.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     7049 2023-07-06 12:20:11.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4324 2023-07-06 12:17:33.000000 lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9825 2023-07-05 07:35:23.000000 lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      591 2023-07-04 15:15:53.000000 lincs-0.5.0/lincs/liblincs/learning/ucncs-by-sat-by-coalitions.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    11212 2023-07-05 16:10:39.000000 lincs-0.5.0/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-07-05 16:00:50.000000 lincs-0.5.0/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    23013 2023-07-06 09:43:55.000000 lincs-0.5.0/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/linear-programming/
+-rw-rw-r--   0 user      (1002) user      (1002)       57 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/alglib.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2731 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/alglib.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       55 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/glop.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1591 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/linear-programming/test.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      785 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/randomness-utils.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/sat/
+-rw-rw-r--   0 user      (1002) user      (1002)       63 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/eval-max-sat.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1665 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/eval-max-sat.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       58 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/minisat.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1341 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/minisat.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2555 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/liblincs/sat/test.cpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.251458 lincs-0.5.0/lincs/liblincs/vendored/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.263458 lincs-0.5.0/lincs/liblincs/vendored/alglib/
+-rwxrwxr-x   0 user      (1002) user      (1002)   615853 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    65139 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibinternal.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   322558 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    88614 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/alglibmisc.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   493278 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   179632 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/ap.h
+-rwxrwxr-x   0 user      (1002) user      (1002)  1927587 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   438786 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/dataanalysis.h
+-rwxrwxr-x   0 user      (1002) user      (1002)    46242 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    10465 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/diffequations.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   126902 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    27863 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/fasttransforms.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   149125 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    33746 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/integration.h
+-rwxrwxr-x   0 user      (1002) user      (1002)  2674150 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   500164 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/interpolation.h
+-rwxrwxr-x   0 user      (1002) user      (1002)    76185 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)     7372 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_avx2.h
+-rwxrwxr-x   0 user      (1002) user      (1002)    39356 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)     4704 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_fma.h
+-rwxrwxr-x   0 user      (1002) user      (1002)    23798 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)     4058 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/kernels_sse2.h
+-rwxrwxr-x   0 user      (1002) user      (1002)  2288262 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   403192 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/linalg.h
+-rwxrwxr-x   0 user      (1002) user      (1002)  3545102 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   608685 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/optimization.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   752491 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)   198547 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/solvers.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   339371 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    77195 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/specialfunctions.h
+-rwxrwxr-x   0 user      (1002) user      (1002)   612951 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.cpp
+-rwxrwxr-x   0 user      (1002) user      (1002)    56614 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/statistics.h
+-rwxrwxr-x   0 user      (1002) user      (1002)        4 2023-07-05 07:10:51.000000 lincs-0.5.0/lincs/liblincs/vendored/alglib/stdafx.h
+-rw-rw-r--   0 user      (1002) user      (1002)   321644 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/doctest.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/
+-rw-rw-r--   0 user      (1002) user      (1002)    30623 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/EvalMaxSAT.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/
+-rw-rw-r--   0 user      (1002) user      (1002)     3857 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/Chrono.h
+-rw-rw-r--   0 user      (1002) user      (1002)     2559 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/View.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3617 2023-07-03 05:21:10.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/communicationlist.h
+-rw-rw-r--   0 user      (1002) user      (1002)     6040 2023-07-03 05:18:59.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/coutUtil.h
+-rw-rw-r--   0 user      (1002) user      (1002)      437 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/MaLib/math.h
+-rw-rw-r--   0 user      (1002) user      (1002)     8586 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4176 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/card_oe.h
+-rw-rw-r--   0 user      (1002) user      (1002)     7315 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     5242 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/cardincremental.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/
+-rw-rw-r--   0 user      (1002) user      (1002)     5770 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/BoundedQueue.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3208 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Constants.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3293 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Dimacs.h
+-rw-rw-r--   0 user      (1002) user      (1002)    68578 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    35867 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/Solver.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4067 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverStats.h
+-rw-rw-r--   0 user      (1002) user      (1002)    20417 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/SolverTypes.h
+-rw-rw-r--   0 user      (1002) user      (1002)    17254 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/core/lcm.cc
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.267458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/
+-rw-rw-r--   0 user      (1002) user      (1002)     2814 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alg.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4768 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Alloc.h
+-rw-rw-r--   0 user      (1002) user      (1002)      166 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Clone.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4772 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Heap.h
+-rw-rw-r--   0 user      (1002) user      (1002)     1825 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/IntTypes.h
+-rw-rw-r--   0 user      (1002) user      (1002)     6949 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Map.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3162 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Queue.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3276 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Sort.h
+-rw-rw-r--   0 user      (1002) user      (1002)     5992 2023-07-03 05:19:40.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/Vec.h
+-rw-rw-r--   0 user      (1002) user      (1002)     7663 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/VecThreads.h
+-rw-rw-r--   0 user      (1002) user      (1002)     1948 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/mtl/XAlloc.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/
+-rw-rw-r--   0 user      (1002) user      (1002)     9383 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     5078 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ClausesBuffer.h
+-rw-rw-r--   0 user      (1002) user      (1002)    24142 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     8631 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/MultiSolvers.h
+-rw-rw-r--   0 user      (1002) user      (1002)    20252 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     6800 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/ParallelSolver.h
+-rw-rw-r--   0 user      (1002) user      (1002)     6558 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     6099 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SharedCompanion.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3923 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     3805 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverCompanion.h
+-rw-rw-r--   0 user      (1002) user      (1002)     7213 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     3471 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/parallel/SolverConfiguration.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/
+-rw-rw-r--   0 user      (1002) user      (1002)    25949 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    11769 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/simp/SimpSolver.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/
+-rw-rw-r--   0 user      (1002) user      (1002)     3801 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    12150 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/Options.h
+-rw-rw-r--   0 user      (1002) user      (1002)     5376 2023-07-03 05:03:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/ParseUtils.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3135 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     2707 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/glucose/utils/System.h
+-rw-rw-r--   0 user      (1002) user      (1002)     1645 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1201 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/lazyvariable.h
+-rw-rw-r--   0 user      (1002) user      (1002)     8639 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/mcqd.h
+-rw-rw-r--   0 user      (1002) user      (1002)     6332 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/monglucose41.h
+-rw-rw-r--   0 user      (1002) user      (1002)      545 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1032 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualcard.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3281 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualmaxsat.h
+-rw-rw-r--   0 user      (1002) user      (1002)       58 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     5039 2023-06-30 07:45:05.000000 lincs-0.5.0/lincs/liblincs/vendored/eval-max-sat/virtualsat.h
+-rw-rw-r--   0 user      (1002) user      (1002)    39408 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/lov-e.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    62179 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/magic_enum.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.243457 lincs-0.5.0/lincs/liblincs/vendored/minisat/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/
+-rw-rw-r--   0 user      (1002) user      (1002)    34998 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    24022 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/Solver.h
+-rw-rw-r--   0 user      (1002) user      (1002)    17280 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/core/SolverTypes.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/
+-rw-rw-r--   0 user      (1002) user      (1002)     2839 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alg.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4379 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Alloc.h
+-rw-rw-r--   0 user      (1002) user      (1002)     5344 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Heap.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4204 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntMap.h
+-rw-rw-r--   0 user      (1002) user      (1002)     1763 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/IntTypes.h
+-rw-rw-r--   0 user      (1002) user      (1002)     6682 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Map.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3001 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Queue.h
+-rw-rw-r--   0 user      (1002) user      (1002)     2427 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Rnd.h
+-rw-rw-r--   0 user      (1002) user      (1002)     3276 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Sort.h
+-rw-rw-r--   0 user      (1002) user      (1002)     5588 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/Vec.h
+-rw-rw-r--   0 user      (1002) user      (1002)     1924 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/mtl/XAlloc.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/
+-rw-rw-r--   0 user      (1002) user      (1002)    22244 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    10816 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/simp/SimpSolver.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/
+-rw-rw-r--   0 user      (1002) user      (1002)     3816 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.cc
+-rw-rw-r--   0 user      (1002) user      (1002)    12153 2023-07-03 04:58:28.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/Options.h
+-rw-rw-r--   0 user      (1002) user      (1002)     4164 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/ParseUtils.h
+-rw-rw-r--   0 user      (1002) user      (1002)     5254 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.cc
+-rw-rw-r--   0 user      (1002) user      (1002)     3088 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/minisat/utils/System.h
+-rw-rw-r--   0 user      (1002) user      (1002)    57901 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/rapidcsv.h
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/valijson/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.271458 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/
+-rw-rw-r--   0 user      (1002) user      (1002)     9433 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/std_string_adapter.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    19320 2023-07-06 06:52:35.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/adapters/yaml_cpp_adapter.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      318 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraint_builder.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/
+-rw-rw-r--   0 user      (1002) user      (1002)     1929 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/basic_constraint.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    34401 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/concrete_constraints.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2030 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4649 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/constraints/constraint_visitor.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      856 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/exceptions.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/
+-rw-rw-r--   0 user      (1002) user      (1002)    16614 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/adapter.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    25566 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/basic_adapter.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2355 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/custom_allocator.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      649 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/debug.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1525 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/frozen_value.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10088 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_pointer.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1694 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/json_reference.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      339 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/optional.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       49 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/optional_bundled.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1206 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/internal/uri.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6144 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/schema.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)   102841 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/schema_parser.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     8346 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/subschema.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.275458 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/
+-rw-rw-r--   0 user      (1002) user      (1002)     1028 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/file_utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1378 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/utils/utf8_utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2488 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_results.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    68300 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validation_visitor.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2250 2023-06-29 16:25:29.000000 lincs-0.5.0/lincs/liblincs/vendored/valijson/validator.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    25311 2023-07-06 12:21:51.000000 lincs-0.5.0/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)     1184 2023-07-04 15:15:35.000000 lincs-0.5.0/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-07-06 13:28:58.247458 lincs-0.5.0/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)     5191 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)    10855 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-07-06 13:28:58.000000 lincs-0.5.0/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-07-04 15:15:35.000000 lincs-0.5.0/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-07-06 13:28:58.275458 lincs-0.5.0/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     4185 2023-07-06 13:26:27.000000 lincs-0.5.0/setup.py
```

### Comparing `lincs-0.4.5/COPYING` & `lincs-0.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.4.5/COPYING.LESSER` & `lincs-0.5.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.4.5/PKG-INFO` & `lincs-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.5
+Version: 0.5.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -23,17 +23,17 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.4.5/README.rst` & `lincs-0.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
 *lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <COPYING>`_ and `COPYING.LESSER <COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
```

### Comparing `lincs-0.4.5/lincs/command_line_interface.py` & `lincs-0.5.0/lincs/command_line_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -105,48 +105,59 @@
 
         if isinstance(command, click.Group):
             for name, command in command.commands.items():
                 walk(prefix + [name], command)
 
     walk([], main)
 
-    for obj_name in sorted(dir(lincs)):
-        if obj_name.startswith("_"):
-            continue
-
-        obj = getattr(lincs, obj_name)
-        print(f"lincs.{obj_name}")
-        print("=" * len(f"lincs.{obj_name}"))
-        print()
-        if obj.__doc__:
-            print(obj.__doc__)
+    def walk(path, node, type_name=None):
+        if '.'.join(path) in [
+            "lincs.command_line_interface",
+            "lincs.visualization.plt",
+        ]:
+            return
+
+        title = f"{'.'.join(path)}: {type_name or type(node).__name__}"
+        print(title)
+        print("-" * len(title))
+
+        if type_name is not None:
+            return
+
+        if type(node) in [str, dict, property]:
             print()
-        if isinstance(obj, type):
-            for attr_name in sorted(dir(obj)):
-                if attr_name.startswith("_") and attr_name not in ["__init__"]:  # @todo Include some other dunders
-                    continue
-                if (
-                    obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind", "ValueType"}
-                    and
-                    attr_name in {"as_integer_ratio", "bit_count", "bit_length", "conjugate", "denominator", "from_bytes", "imag", "numerator", "to_bytes", "attr_name", "name", "names", "values"}
-                ):
-                    continue
-                if (
-                    obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind"}
-                    and
-                    attr_name in {"real"}
-                ):
-                    continue
-                print(f"{attr_name}")
-                print("-" * len(attr_name))
-                print()
-                doc = getattr(obj, attr_name).__doc__
-                if doc:
-                    print(doc)
-                    print()
+            return
+
+        if node.__doc__:
+            print(node.__doc__)
+        print()
+
+        if type(node) in [type(walk), type(lincs.Model.dump)]:
+            return
+
+        if '.'.join(path) in [
+            "lincs.Criterion.CategoryCorrelation",
+            "lincs.Criterion.ValueType",
+            "lincs.SufficientCoalitions.Kind",
+        ]:
+            for name in node.names:
+                walk(path + [name], name, type_name="value")
+            return
+
+        for name in sorted(dir(node)):
+            if name not in ["__init__"] and name.startswith("__") and name.endswith("__"):
+                continue
+
+            # Avoid weird recursion
+            if name in path:
+                continue
+
+            walk(path + [name], getattr(node, name))
+
+    walk(["lincs"], lincs)
 
 
 @main.group(
     help="Generate synthetic data.",
 )
 def generate():
     pass
@@ -181,15 +192,15 @@
 )
 def classification_problem(
     criteria_count,
     categories_count,
     output_problem,
     random_seed
 ):
-    problem = lincs.generate_problem(
+    problem = lincs.generate_classification_problem(
         criteria_count,
         categories_count,
         random_seed=random_seed,
     )
     problem.dump(output_problem)
 
 
@@ -242,22 +253,22 @@
 def classification_model(
     problem,
     output_model,
     random_seed,
     model_type,
     mrsort__fixed_weights_sum,
 ):
-    problem = lincs.load_problem(problem)
+    problem = lincs.Problem.load(problem)
     assert model_type == "mrsort"
-    model = lincs.generate_mrsort_model(
+    model = lincs.generate_mrsort_classification_model(
         problem,
         random_seed=random_seed,
         fixed_weights_sum=mrsort__fixed_weights_sum,
     )
-    model.dump(output_model)
+    model.dump(problem, output_model)
 
 
 @generate.command(
     help="""
         Generate synthetic classified alternatives.
 
         PROBLEM is a *classification problem* file describing the problem to generate alternatives for.
@@ -285,37 +296,51 @@
 @click.option(
     "--max-imbalance",
     type=click.FloatRange(min=0.0, max=1.0, max_open=True),
     default=None,
     help="Ensure that categories are balanced, by forcing their size to differ from the perfectly balanced size by at most this fraction.",
 )
 @click.option(
+    "--misclassified-count",
+    type=click.IntRange(min=0),
+    default=0,
+    help="Misclassify that many alternatives.",
+)
+@click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
     default=random.randrange(2**30),
 )
 def classified_alternatives(
     problem,
     model,
     alternatives_count,
     output_classified_alternatives,
     max_imbalance,
+    misclassified_count,
     random_seed,
 ):
-    problem = lincs.load_problem(problem)
-    model = lincs.load_model(problem, model)
-    alternatives = lincs.generate_alternatives(
+    problem = lincs.Problem.load(problem)
+    model = lincs.Model.load(problem, model)
+    alternatives = lincs.generate_classified_alternatives(
         problem,
         model,
         alternatives_count,
         random_seed=random_seed,
         max_imbalance=max_imbalance,
     )
-    alternatives.dump(output_classified_alternatives)
+    if misclassified_count:
+        lincs.misclassify_alternatives(
+            problem,
+            alternatives,
+            misclassified_count,
+            random_seed=random_seed + 27,  # Arbitrary, does not hurt
+        )
+    alternatives.dump(problem, output_classified_alternatives)
 
 
 @main.group(
     help="Make graphs from data.",
 )
 def visualize():
     pass
@@ -355,18 +380,18 @@
 def classification_model(
     problem,
     model,
     alternatives,
     alternatives_count,
     output,
 ):
-    problem = lincs.load_problem(problem)
-    model = lincs.load_model(problem, model)
+    problem = lincs.Problem.load(problem)
+    model = lincs.Model.load(problem, model)
     if alternatives is not None:
-        alternatives = lincs.load_alternatives(problem, alternatives)
+        alternatives = lincs.Alternatives.load(problem, alternatives)
     lincs.visualization.visualize_model(problem, model, alternatives, alternatives_count, output)
 
 
 @main.group(
     help="Learn a model.",
 )
 def learn():
@@ -396,20 +421,19 @@
     default="-",
     help="Write the learned classification model to this file instead of standard output.",
 )
 @options_tree(
     "model-type",
     dict(
         help="The type of classification model to learn.",
-        type=click.Choice(["mrsort"]),
+        type=click.Choice(["mrsort", "ucncs"]),
         default="mrsort",
         show_default=True,
     ),
     {
-        "ucncs": [],
         "mrsort": [
             (
                 "strategy",
                 dict(
                     help="The top-level strategy to use to learn the MRSort model. See https://mics-lab.github.io/lincs/user-guide.html#learning-strategies about strategies.",
                     type=click.Choice(["weights-profiles-breed"]),
                     default="weights-profiles-breed",
@@ -434,14 +458,24 @@
                                 type=click.IntRange(min=1),
                                 default=None,
                                 show_default=True,
                             ),
                             {},
                         ),
                         (
+                            "max-duration-seconds",
+                            dict(
+                                help="The maximum duration to learn the MRSort model, in seconds.",
+                                type=click.FloatRange(min=0),
+                                default=None,
+                                show_default=True,
+                            ),
+                            {},
+                        ),
+                        (
                             "models-count",
                             dict(
                                 help="The number of temporary MRSort models to train. The result of the learning will be the most accurate of those models.",
                                 type=click.IntRange(min=1),
                                 default=9,
                                 show_default=True,
                             ),
@@ -531,77 +565,129 @@
                                             show_default=True,
                                         ),
                                         {},
                                     ),
                                 ],
                             },
                         ),
+                        (
+                            "verbose",
+                            dict(
+                                help="Print information about the learning process on stderr while learning.",
+                                is_flag=True,
+                            ),
+                            {},
+                        )
                     ],
                 },
             ),
         ],
+        "ucncs": [
+            (
+                "approach",
+                dict(
+                    help="The general approach to transform the learning problem into a satisfiability problem.",
+                    type=click.Choice(["sat-by-coalitions", "max-sat-by-coalitions"]),
+                    default="sat-by-coalitions",
+                    show_default=True,
+                ),
+                {},
+            ),
+        ],
     },
 )
 def classification_model(
     problem,
     learning_set,
     output_model,
     model_type,
     mrsort__strategy,
     mrsort__weights_profiles_breed__target_accuracy,
     mrsort__weights_profiles_breed__max_iterations,
+    mrsort__weights_profiles_breed__max_duration_seconds,
     mrsort__weights_profiles_breed__models_count,
     mrsort__weights_profiles_breed__initialization_strategy,
     mrsort__weights_profiles_breed__weights_strategy,
     mrsort__weights_profiles_breed__linear_program__solver,
     mrsort__weights_profiles_breed__profiles_strategy,
     mrsort__weights_profiles_breed__accuracy_heuristic__random_seed,
     mrsort__weights_profiles_breed__accuracy_heuristic__processor,
     mrsort__weights_profiles_breed__breed_strategy,
     mrsort__weights_profiles_breed__reinitialize_least_accurate__portion,
+    mrsort__weights_profiles_breed__verbose,
+    ucncs__approach,
 ):
-    problem = lincs.load_problem(problem)
-    learning_set = lincs.load_alternatives(problem, learning_set)
+    problem = lincs.Problem.load(problem)
+    learning_set = lincs.Alternatives.load(problem, learning_set)
 
     if model_type == "mrsort":
         if mrsort__strategy == "weights-profiles-breed":
-            models = lincs.make_models(problem, learning_set, mrsort__weights_profiles_breed__models_count, mrsort__weights_profiles_breed__accuracy_heuristic__random_seed)
-
-            assert mrsort__weights_profiles_breed__max_iterations is None
-            termination_strategy = lincs.TerminateAtAccuracy(math.ceil(mrsort__weights_profiles_breed__target_accuracy * len(learning_set.alternatives)))
+            learning_data = lincs.LearnMrsortByWeightsProfilesBreed.LearningData.make(problem, learning_set, mrsort__weights_profiles_breed__models_count, mrsort__weights_profiles_breed__accuracy_heuristic__random_seed)
 
             if mrsort__weights_profiles_breed__initialization_strategy == "maximize-discrimination-per-criterion":
-                profiles_initialization_strategy = lincs.InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(models)
+                profiles_initialization_strategy = lincs.InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(learning_data)
 
             if mrsort__weights_profiles_breed__weights_strategy == "linear-program":
                 if mrsort__weights_profiles_breed__linear_program__solver == "glop":
-                    weights_optimization_strategy = lincs.OptimizeWeightsUsingGlop(models)
+                    weights_optimization_strategy = lincs.OptimizeWeightsUsingGlop(learning_data)
                 elif mrsort__weights_profiles_breed__linear_program__solver == "alglib":
-                    weights_optimization_strategy = lincs.OptimizeWeightsUsingAlglib(models)
+                    weights_optimization_strategy = lincs.OptimizeWeightsUsingAlglib(learning_data)
 
             if mrsort__weights_profiles_breed__profiles_strategy == "accuracy-heuristic":
                 if mrsort__weights_profiles_breed__accuracy_heuristic__processor == "cpu":
-                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnCpu(models)
+                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnCpu(learning_data)
                 elif mrsort__weights_profiles_breed__accuracy_heuristic__processor == "gpu":
-                    gpu_models = lincs.make_gpu_models(models)
-                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnGpu(models, gpu_models)
+                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnGpu(learning_data)
+
+            if mrsort__weights_profiles_breed__breed_strategy == "reinitialize-least-accurate":
+                count = int(mrsort__weights_profiles_breed__reinitialize_least_accurate__portion * mrsort__weights_profiles_breed__models_count)
+                breeding_strategy = lincs.ReinitializeLeastAccurate(learning_data, profiles_initialization_strategy, count)
+
+            termination_strategies = [lincs.TerminateAtAccuracy(
+                learning_data,
+                math.ceil(mrsort__weights_profiles_breed__target_accuracy * len(learning_set.alternatives)),
+            )]
+            if mrsort__weights_profiles_breed__max_iterations is not None:
+                termination_strategies.append(lincs.TerminateAfterIterations(learning_data, mrsort__weights_profiles_breed__max_iterations))
+            if mrsort__weights_profiles_breed__max_duration_seconds is not None:
+                termination_strategies.append(lincs.TerminateAfterSeconds(mrsort__weights_profiles_breed__max_duration_seconds))
+            if len(termination_strategies) == 1:
+                termination_strategy = termination_strategies[0]
+            else:
+                termination_strategy = lincs.TerminateWhenAny(termination_strategies)
+
+            observers = []
+            if mrsort__weights_profiles_breed__verbose:
+                class VerboseObserver(lincs.LearnMrsortByWeightsProfilesBreed.Observer):
+                    def __init__(self, learning_data):
+                        super().__init__()
+                        self.learning_data = learning_data
+
+                    def after_iteration(self):
+                        print("Best accuracy:", self.learning_data.get_best_accuracy(), file=sys.stderr)
 
-            assert mrsort__weights_profiles_breed__breed_strategy == "reinitialize-least-accurate"
-            assert mrsort__weights_profiles_breed__reinitialize_least_accurate__portion == 0.5
+                observers.append(VerboseObserver(learning_data))
 
-            learning = lincs.WeightsProfilesBreedMrSortLearning(
-                models,
+            learning = lincs.LearnMrsortByWeightsProfilesBreed(
+                learning_data,
                 profiles_initialization_strategy,
                 weights_optimization_strategy,
                 profiles_improvement_strategy,
+                breeding_strategy,
                 termination_strategy,
+                observers,
             )
+    elif model_type == "ucncs":
+        if ucncs__approach == "sat-by-coalitions":
+            learning = lincs.LearnUcncsBySatByCoalitionsUsingMinisat(problem, learning_set)
+        elif ucncs__approach == "max-sat-by-coalitions":
+            learning = lincs.LearnUcncsBySatByCoalitionsUsingEvalmaxsat(problem, learning_set)
 
     model = learning.perform()
-    model.dump(output_model)
+    model.dump(problem, output_model)
 
 
 @main.command(
     help="""
         Classify alternatives.
 
         PROBLEM is a *classification problem* file.
@@ -629,19 +715,19 @@
 )
 def classify(
     problem,
     model,
     alternatives,
     output_classified_alternatives,
 ):
-    problem = lincs.load_problem(problem)
-    model = lincs.load_model(problem, model)
-    alternatives = lincs.load_alternatives(problem, alternatives)
+    problem = lincs.Problem.load(problem)
+    model = lincs.Model.load(problem, model)
+    alternatives = lincs.Alternatives.load(problem, alternatives)
     lincs.classify_alternatives(problem, model, alternatives)
-    alternatives.dump(output_classified_alternatives)
+    alternatives.dump(problem, output_classified_alternatives)
 
 
 @main.command(
     help="""
         Compute a classification accuracy.
 
         PROBLEM is a *classification problem* file.
@@ -664,12 +750,12 @@
     type=click.File(mode="r"),
 )
 def classification_accuracy(
     problem,
     model,
     testing_set,
 ):
-    problem = lincs.load_problem(problem)
-    model = lincs.load_model(problem, model)
-    testing_set = lincs.load_alternatives(problem, testing_set)
+    problem = lincs.Problem.load(problem)
+    model = lincs.Model.load(problem, model)
+    testing_set = lincs.Alternatives.load(problem, testing_set)
     result = lincs.classify_alternatives(problem, model, testing_set)
     print(f"{result.unchanged}/{result.changed + result.unchanged}")
```

### Comparing `lincs-0.4.5/lincs/liblincs/generation.cpp` & `lincs-0.5.0/lincs/liblincs/generation.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -4,42 +4,55 @@
 
 #include <algorithm>
 #include <cassert>
 #include <random>
 
 #include "classification.hpp"
 
+#include "vendored/doctest.h"  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
+
+
+namespace {
+
+bool env_is_true(const char* name) {
+  const char* value = std::getenv(name);
+  return value && std::string(value) == "true";
+}
+
+const bool skip_long = env_is_true("LINCS_DEV_SKIP_LONG");
+
+}  // namespace
 
 namespace lincs {
 
-Problem generate_problem(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
+Problem generate_classification_problem(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
   // There is nothing random yet. There will be when other value types and category correlations are added.
 
-  std::vector<Problem::Criterion> criteria;
+  std::vector<Criterion> criteria;
   criteria.reserve(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     criteria.emplace_back(
       "Criterion " + std::to_string(criterion_index + 1),
-      Problem::Criterion::ValueType::real,
-      Problem::Criterion::CategoryCorrelation::growing
+      Criterion::ValueType::real,
+      Criterion::CategoryCorrelation::growing
     );
   }
 
-  std::vector<Problem::Category> categories;
+  std::vector<Category> categories;
   categories.reserve(categories_count);
   for (unsigned category_index = 0; category_index != categories_count; ++category_index) {
     categories.emplace_back(
       "Category " + std::to_string(category_index + 1)
     );
   }
 
   return Problem{criteria, categories};
 }
 
-Model generate_mrsort_model(const Problem& problem, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
+Model generate_mrsort_classification_model(const Problem& problem, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
   const unsigned categories_count = problem.categories.size();
   const unsigned criteria_count = problem.criteria.size();
 
   std::mt19937 gen(random_seed);
 
   // Profile can take any values. We arbitrarily generate them uniformly
   std::uniform_real_distribution<float> values_distribution(0.01f, 0.99f);
@@ -82,29 +95,58 @@
   const float weights_sum = fixed_weights_sum ? *fixed_weights_sum : 1.f / std::uniform_real_distribution<float>(0.f, 1.f)(gen);
   std::vector<float> denormalized_weights(criteria_count);
   std::transform(
     normalized_weights.begin(), normalized_weights.end(),
     denormalized_weights.begin(),
     [weights_sum](float w) { return w * weights_sum; });
 
-  Model::SufficientCoalitions coalitions{
-    Model::SufficientCoalitions::Kind::weights,
-    denormalized_weights,
-  };
+  SufficientCoalitions coalitions{SufficientCoalitions::weights, denormalized_weights};
 
   std::vector<Model::Boundary> boundaries;
   boundaries.reserve(categories_count - 1);
   for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
     boundaries.emplace_back(profiles[category_index], coalitions);
   }
 
   return Model(problem, boundaries);
 }
 
-Alternatives generate_uniform_alternatives(
+TEST_CASE("Generate MR-Sort model - random weights sum") {
+  Problem problem = generate_classification_problem(3, 2, 42);
+  Model model = generate_mrsort_classification_model(problem, 42);
+
+  std::ostringstream oss;
+  model.dump(problem, oss);
+  CHECK(oss.str() == R"(kind: ncs-classification-model
+format_version: 1
+boundaries:
+  - profile: [0.3770493, 0.7906122, 0.9417]
+    sufficient_coalitions:
+      kind: weights
+      criterion_weights: [0.235266, 0.7035596, 0.3437337]
+)");
+}
+
+TEST_CASE("Generate MR-Sort model - fixed weights sum") {
+  Problem problem = generate_classification_problem(3, 2, 42);
+  Model model = generate_mrsort_classification_model(problem, 42, 2);
+
+  std::ostringstream oss;
+  model.dump(problem, oss);
+  CHECK(oss.str() == R"(kind: ncs-classification-model
+format_version: 1
+boundaries:
+  - profile: [0.3770493, 0.7906122, 0.9417]
+    sufficient_coalitions:
+      kind: weights
+      criterion_weights: [0.3668696, 1.097118, 0.5360122]
+)");
+}
+
+Alternatives generate_uniform_classified_alternatives(
   const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   std::mt19937& gen
 ) {
   const unsigned criteria_count = problem.criteria.size();
 
@@ -144,15 +186,37 @@
 unsigned max_category_size(const unsigned alternatives_count, const unsigned categories_count, const float max_imbalance) {
   assert(max_imbalance >= 0);
   assert(max_imbalance <= 1);
 
   return std::ceil(alternatives_count * (1 + max_imbalance) / categories_count);
 }
 
-Alternatives generate_balanced_alternatives(
+TEST_CASE("Balanced category sizes") {
+  CHECK(min_category_size(100, 2, 0) == 50);
+  CHECK(max_category_size(100, 2, 0) == 50);
+  CHECK(min_category_size(100, 2, 1) == 0);
+  CHECK(max_category_size(100, 2, 1) == 100);
+
+  CHECK(min_category_size(100, 2, 0.2) == 40);
+  CHECK(max_category_size(100, 2, 0.2) == 61);  // Should be 60, but floating point arithmetics...
+
+  CHECK(min_category_size(100'000, 2, 0.2) == 40000);
+  CHECK(max_category_size(100'000, 2, 0.2) == 60001);  // Should be 60000
+
+  CHECK(min_category_size(150, 3, 0.2) == 40);
+  CHECK(max_category_size(150, 3, 0.2) == 60);
+
+  CHECK(min_category_size(100, 2, 0.3) == 35);
+  CHECK(max_category_size(100, 2, 0.3) == 65);
+
+  CHECK(min_category_size(99, 2, 0.2) == 39);
+  CHECK(max_category_size(99, 2, 0.2) == 60);
+}
+
+Alternatives generate_balanced_classified_alternatives(
   const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   const float max_imbalance,
   std::mt19937& gen
 ) {
   assert(max_imbalance >= 0);
@@ -175,93 +239,217 @@
   const int multiplier = 10;
 
   const unsigned min_size = min_category_size(alternatives_count, categories_count, max_imbalance);
   const unsigned max_size = max_category_size(alternatives_count, categories_count, max_imbalance);
 
   std::vector<Alternative> alternatives;
   alternatives.reserve(alternatives_count);
-  std::map<std::string, unsigned> histogram;
-  for (const auto& category : problem.categories) {
-    histogram[category.name] = 0;
-  }
+  std::vector<unsigned> histogram(categories_count, 0);
 
   int max_iterations_with_no_effect = max_iterations_with_no_effect_with_empty_category;
 
   // Step 1: fill all categories to exactly the min size
   // (skip if min size is zero)
   int iterations_with_no_effect = 0;
   while (min_size > 0) {
     ++iterations_with_no_effect;
 
-    Alternatives candidates = generate_uniform_alternatives(problem, model, multiplier * alternatives_count, gen);
+    Alternatives candidates = generate_uniform_classified_alternatives(problem, model, multiplier * alternatives_count, gen);
 
     for (const auto& candidate : candidates.alternatives) {
-      assert(candidate.category);
-      const std::string& category = *candidate.category;
-      if (histogram[category] < min_size) {
+      assert(candidate.category_index);
+      const unsigned category_index = *candidate.category_index;
+      if (histogram[category_index] < min_size) {
         alternatives.push_back(candidate);
-        ++histogram[category];
+        ++histogram[category_index];
         iterations_with_no_effect = 0;
       }
     }
 
-    if (std::all_of(histogram.begin(), histogram.end(), [min_size](const auto it) { return it.second >= min_size; })) {
+    if (std::all_of(histogram.begin(), histogram.end(), [min_size](const auto size) { return size >= min_size; })) {
       // Success
       break;
     }
 
-    if (std::all_of(histogram.begin(), histogram.end(), [](const auto it) { return it.second > 0; })) {
+    if (std::all_of(histogram.begin(), histogram.end(), [](const auto size) { return size > 0; })) {
       max_iterations_with_no_effect = max_iterations_with_no_effect_with_all_categories_populated;
     }
 
     if (iterations_with_no_effect > max_iterations_with_no_effect) {
       throw BalancedAlternativesGenerationException(histogram);
     }
   }
 
   // Step 2: reach target size, keeping all categories below or at the max size
   iterations_with_no_effect = 0;
   while (true) {
     ++iterations_with_no_effect;
 
-    Alternatives candidates = generate_uniform_alternatives(problem, model, multiplier * alternatives_count, gen);
+    Alternatives candidates = generate_uniform_classified_alternatives(problem, model, multiplier * alternatives_count, gen);
 
     for (const auto& candidate : candidates.alternatives) {
-      assert(candidate.category);
-      const std::string& category = *candidate.category;
-      if (histogram[category] < max_size) {
+      assert(candidate.category_index);
+      const unsigned category_index = *candidate.category_index;
+      if (histogram[category_index] < max_size) {
         alternatives.push_back(candidate);
-        ++histogram[category];
+        ++histogram[category_index];
         iterations_with_no_effect = 0;
       }
 
       if (alternatives.size() == alternatives_count) {
         assert(std::all_of(
           histogram.begin(), histogram.end(),
-          [min_size, max_size](const auto it) { return it.second >= min_size && it.second <= max_size; }));
+          [min_size, max_size](const auto size) { return size >= min_size && size <= max_size; }));
         return Alternatives(problem, alternatives);
       }
     }
 
     if (iterations_with_no_effect > max_iterations_with_no_effect) {
       throw BalancedAlternativesGenerationException(histogram);
     }
   }
 }
 
-Alternatives generate_alternatives(
+Alternatives generate_classified_alternatives(
   const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   const unsigned random_seed,
   const std::optional<float> max_imbalance
 ) {
   std::mt19937 gen(random_seed);
 
   if (max_imbalance) {
-    return generate_balanced_alternatives(problem, model, alternatives_count, *max_imbalance, gen);
+    return generate_balanced_classified_alternatives(problem, model, alternatives_count, *max_imbalance, gen);
   } else {
-    return generate_uniform_alternatives(problem, model, alternatives_count, gen);
+    return generate_uniform_classified_alternatives(problem, model, alternatives_count, gen);
   }
 }
 
+void check_histogram(const Problem& problem, const Model& model, const std::optional<float> max_imbalance, const unsigned a, const unsigned b) {
+  REQUIRE(problem.categories.size() == 2);
+
+  Alternatives alternatives = generate_classified_alternatives(problem, model, 100, 42, max_imbalance);
+
+  std::vector<unsigned> histogram(2, 0);
+  for (const auto& alternative : alternatives.alternatives) {
+    ++histogram[*alternative.category_index];
+  }
+  CHECK(histogram[0] == a);
+  CHECK(histogram[1] == b);
+}
+
+TEST_CASE("Generate balanced classified alternatives") {
+  Problem problem = generate_classification_problem(3, 2, 42);
+  Model model = generate_mrsort_classification_model(problem, 42, 2);
+
+  check_histogram(problem, model, std::nullopt, 80, 20);
+  check_histogram(problem, model, 0.5, 63, 37);
+  check_histogram(problem, model, 0.2, 56, 44);
+  check_histogram(problem, model, 0.1, 54, 46);
+  check_histogram(problem, model, 0.0, 50, 50);
+}
+
+TEST_CASE("Generate balanced classified alternatives - many seeds") {
+  // Assert that we can generate a balanced learning set for all generated models
+
+  const unsigned alternatives_seed = 42;  // If we succeed with this arbitrary seed, we're confident we'll succeed with any seed
+
+  // (dynamic OpenMP scheduling because iteration durations vary a lot)
+  #pragma omp parallel for collapse(3) schedule(dynamic, 1)
+  for (unsigned criteria_count = 1; criteria_count != 7; ++criteria_count) {
+    for (unsigned categories_count = 2; categories_count != 7; ++categories_count) {
+      for (unsigned model_seed = 0; model_seed != (skip_long ? 10 : 100); ++model_seed) {
+        Problem problem = generate_classification_problem(criteria_count, categories_count, 42);
+
+        CAPTURE(criteria_count);
+        CAPTURE(categories_count);
+        CAPTURE(model_seed);
+
+        Model model = generate_mrsort_classification_model(problem, model_seed);
+
+        // There *are* failures for larger numbers of criteria or categories,
+        // but there is not much I can imagine doing to avoid that.
+        bool expect_success = true;
+        // Known failures: when the first (resp. last) profile and threshold are low (resp. high),
+        // it's too difficult to find random alternatives in the first (resp. last) category.
+        if (criteria_count == 3 && categories_count == 4 && model_seed == 24) expect_success = false;
+        if (criteria_count == 5 && categories_count == 5 && model_seed == 45) expect_success = false;
+        if (criteria_count == 5 && categories_count == 6 && model_seed == 8) expect_success = false;
+        if (criteria_count == 6 && categories_count == 2 && model_seed == 87) expect_success = false;
+        if (criteria_count == 6 && categories_count == 4 && model_seed == 21) expect_success = false;
+        if (criteria_count == 6 && categories_count == 4 && model_seed == 43) expect_success = false;
+        if (criteria_count == 6 && categories_count == 4 && model_seed == 52) expect_success = false;
+        if (criteria_count == 6 && categories_count == 5 && model_seed == 8) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 11) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 14) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 26) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 29) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 42) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 54) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 76) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 78) expect_success = false;
+        if (criteria_count == 6 && categories_count == 6 && model_seed == 96) expect_success = false;
+
+        try {
+          Alternatives alternatives = generate_classified_alternatives(problem, model, 100, alternatives_seed, 0);
+          CHECK(expect_success);
+        } catch (BalancedAlternativesGenerationException& e) {
+          CHECK(!expect_success);
+        }
+      }
+    }
+  }
+}
+
+TEST_CASE("Exploratory test: 'std::shuffle' *can* keep something in place") {
+  std::vector<unsigned> v(100);
+  std::iota(v.begin(), v.end(), 0);
+
+  CHECK(v[76] == 76);
+  CHECK(v[77] == 77);
+  CHECK(v[78] == 78);
+
+  std::mt19937 gen(0);
+  std::shuffle(v.begin(), v.end(), gen);
+
+  CHECK(v[76] == 31);
+  CHECK(v[77] == 77);  // Kept
+  CHECK(v[78] == 71);
+}
+
+void misclassify_alternatives(const Problem& problem, Alternatives* alternatives, const unsigned count, const unsigned random_seed) {
+  const unsigned categories_count = problem.categories.size();
+  const unsigned alternatives_count = alternatives->alternatives.size();
+
+  std::mt19937 gen(random_seed);
+
+  std::vector<unsigned> alternative_indexes(alternatives_count);
+  std::iota(alternative_indexes.begin(), alternative_indexes.end(), 0);
+  std::shuffle(alternative_indexes.begin(), alternative_indexes.end(), gen);
+  alternative_indexes.resize(count);
+
+  for (const unsigned alternative_index : alternative_indexes) {
+    auto& alternative = alternatives->alternatives[alternative_index];
+
+    // Choose new index in [0, alternative.category_index - 1] U [alternative.category_index + 1, categories_count - 1]
+    // => choose in [0, categories_count - 2] and increment if >= alternative.category_index
+    unsigned new_category_index = std::uniform_int_distribution<unsigned>(0, categories_count - 2)(gen);
+    if (new_category_index >= *alternative.category_index) {
+      ++new_category_index;
+    }
+
+    alternative.category_index = new_category_index;
+  }
+}
+
+TEST_CASE("Misclassify alternatives") {
+  Problem problem = generate_classification_problem(3, 2, 42);
+  Model model = generate_mrsort_classification_model(problem, 42, 2);
+  Alternatives alternatives = generate_classified_alternatives(problem, model, 100, 42, 0.2);
+
+  misclassify_alternatives(problem, &alternatives, 10, 42);
+
+  CHECK(classify_alternatives(problem, model, &alternatives).changed == 10);
+}
+
 } // namespace lincs
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/alternatives.cpp` & `lincs-0.5.0/lincs/liblincs/io/alternatives.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 // Copyright 2023 Vincent Jacques
 
 #include "alternatives.hpp"
 
-#include <rapidcsv.h>
+#include "../vendored/rapidcsv.h"
 
 
 namespace lincs {
 
-void Alternatives::dump(std::ostream& os) const {
+void Alternatives::dump(const Problem& problem, std::ostream& os) const {
   const unsigned criteria_count = problem.criteria.size();
   const unsigned alternatives_count = alternatives.size();
 
   rapidcsv::Document doc;
 
   doc.SetColumnName(0, "name");
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
@@ -21,24 +21,28 @@
 
   for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
     const Alternative& alternative = alternatives[alternative_index];
     doc.SetCell<std::string>(0, alternative_index, alternative.name);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
       doc.SetCell<float>(criterion_index + 1, alternative_index, alternative.profile[criterion_index]);
     }
-    if (alternative.category) {
-      doc.SetCell<std::string>(criteria_count + 1, alternative_index, *alternative.category);
+    if (alternative.category_index) {
+      doc.SetCell<std::string>(criteria_count + 1, alternative_index, problem.categories[*alternative.category_index].name);
     }
   }
 
   doc.Save(os);
 }
 
 Alternatives Alternatives::load(const Problem& problem, std::istream& is) {
   const unsigned criteria_count = problem.criteria.size();
+  std::map<std::string, unsigned> category_indexes;
+  for (const auto& category: problem.categories) {
+    category_indexes[category.name] = category_indexes.size();
+  }
 
   // I don't know why constructing the rapidcsv::Document directly from 'is' sometimes results in an empty document.
   // So, read the whole stream into a string and construct the document from that.
   std::string s(std::istreambuf_iterator<char>(is), {});
   std::istringstream iss(s);
   rapidcsv::Document doc(iss);
 
@@ -50,15 +54,15 @@
     alternative.name = doc.GetCell<std::string>("name", row_index);
     alternative.profile.reserve(criteria_count);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
       alternative.profile.push_back(doc.GetCell<float>(problem.criteria[criterion_index].name, row_index));
     }
     std::string category = doc.GetCell<std::string>("category", row_index);
     if (category != "") {
-      alternative.category = category;
+      alternative.category_index = category_indexes[category];
     }
     alternatives.push_back(alternative);
   }
 
   return Alternatives{problem, alternatives};
 }
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/alternatives.hpp` & `lincs-0.5.0/lincs/liblincs/io/alternatives.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 
 namespace lincs {
 
 struct Alternative {
   std::string name;
   std::vector<float> profile;
-  std::optional<std::string> category;
+  std::optional<unsigned> category_index;
 
   Alternative() {}
-  Alternative(const std::string& name_, const std::vector<float>& profile_, const std::optional<std::string>& category_): name(name_), profile(profile_), category(category_) {}
+  Alternative(const std::string& name_, const std::vector<float>& profile_, const std::optional<unsigned>& category_index_): name(name_), profile(profile_), category_index(category_index_) {}
 
-  bool operator==(const Alternative& other) const { return name == other.name && profile == other.profile && category == other.category; }
+  bool operator==(const Alternative& other) const { return name == other.name && profile == other.profile && category_index == other.category_index; }
 };
 
 struct Alternatives {
   const Problem& problem;
   std::vector<Alternative> alternatives;
 
   Alternatives(const Problem& problem_, const std::vector<Alternative>& alternatives_): problem(problem_), alternatives(alternatives_) {}
 
-  void dump(std::ostream&) const;
+  void dump(const Problem&, std::ostream&) const;
   static Alternatives load(const Problem&, std::istream&);
 };
 
 }  // namespace lincs
 
 #endif  // LINCS__IO__ALTERNATIVES_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/model.hpp` & `lincs-0.5.0/lincs/liblincs/io/model.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,84 @@
 // Copyright 2023 Vincent Jacques
 
 #ifndef LINCS__IO__MODEL_HPP
 #define LINCS__IO__MODEL_HPP
 
+#include <boost/dynamic_bitset.hpp>
+
 #include "problem.hpp"
 
 
 namespace lincs {
 
+struct SufficientCoalitions {
+  // Sufficient coalitions form an https://en.wikipedia.org/wiki/Upper_set in the set of parts of the set of criteria.
+  // This upset can be defined:
+  //   - by the weights of the criteria
+  //   - explicitly by its roots
+
+  // Enum for runtime type discrimination
+  enum class Kind { weights, roots } kind;
+
+  // Tags for compile time type discrimination
+  struct Weights {};
+  static constexpr Weights weights = {};
+  struct Roots {};
+  static constexpr Roots roots = {};
+
+  // Only one of the following two fields is used, depending on the kind.
+  // Rationale for not using dynamic polymorphism: enable classification of many alternatives without the cost of virtual functions.
+  // (Could/should be challenged at some point.)
+  std::vector<float> criterion_weights;  // Indexed by criterion_index
+  std::vector<boost::dynamic_bitset<>> upset_roots;  // Each bitset is indexed by criterion_index and is true if the criterion is in the coalition
+
+  SufficientCoalitions(Weights, const std::vector<float>& criterion_weights_) : kind(Kind::weights), criterion_weights(criterion_weights_) {}
+
+  SufficientCoalitions(Roots, const unsigned criteria_count, const std::vector<std::vector<unsigned>>& upset_roots_) : kind(Kind::roots), upset_roots() {
+    upset_roots.reserve(upset_roots_.size());
+    for (const auto& root: upset_roots_) {
+      upset_roots.emplace_back(criteria_count);
+      for (unsigned criterion_index: root) {
+        upset_roots.back()[criterion_index] = true;
+      }
+    }
+  }
+
+  std::vector<std::vector<unsigned>> get_upset_roots() const {
+    std::vector<std::vector<unsigned>> result;
+    result.reserve(upset_roots.size());
+    for (const auto& root: upset_roots) {
+      result.emplace_back();
+      for (unsigned criterion_index = 0; criterion_index != root.size(); ++criterion_index) {
+        if (root[criterion_index]) {
+          result.back().push_back(criterion_index);
+        }
+      }
+    }
+    return result;
+  }
+};
+
 struct Model {
   const Problem& problem;
 
-  struct SufficientCoalitions {
-    // Sufficient coalitions form an https://en.wikipedia.org/wiki/Upper_set in the set of parts of the set of criteria.
-    // This upset can be defined:
-    enum class Kind {
-      weights,  // by the weights of the criteria
-      // @todo Add upset_roots,  // explicitly by its roots
-    } kind;
-
-    std::vector<float> criterion_weights;
-
-    SufficientCoalitions() {};
-    SufficientCoalitions(Kind kind_, const std::vector<float>& criterion_weights_): kind(kind_), criterion_weights(criterion_weights_) {}
-  };
-
   struct Boundary {
     std::vector<float> profile;
     SufficientCoalitions sufficient_coalitions;
 
-    Boundary() {};
     Boundary(const std::vector<float>& profile_, const SufficientCoalitions& sufficient_coalitions_): profile(profile_), sufficient_coalitions(sufficient_coalitions_) {}
 
     bool operator==(const Boundary& other) const { return profile == other.profile && sufficient_coalitions.kind == other.sufficient_coalitions.kind && sufficient_coalitions.criterion_weights == other.sufficient_coalitions.criterion_weights; }
   };
 
   std::vector<Boundary> boundaries;  // boundary_index 0 is between category_index 0 and category_index 1
 
   Model(const Problem& problem_, const std::vector<Boundary>& boundaries_) : problem(problem_), boundaries(boundaries_) {}
 
   static const std::string json_schema;
-  void dump(std::ostream&) const;
+  void dump(const Problem&, std::ostream&) const;
   static Model load(const Problem&, std::istream&);
 };
 
 }  // namespace lincs
 
 #endif  // LINCS__IO__MODEL_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/problem.cpp` & `lincs-0.5.0/lincs/liblincs/io/problem.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 // Copyright 2023 Vincent Jacques
 
 #include "problem.hpp"
 
 #include <cassert>
 
-#include <magic_enum.hpp>
 #include <yaml-cpp/yaml.h>
 
+#include "../vendored/magic_enum.hpp"
 #include "validation.hpp"
 
-#include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
+#include "../vendored/doctest.h"  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 namespace YAML {
 
 template<>
-struct convert<lincs::Problem::Category> {
-  static Node encode(const lincs::Problem::Category& category) {
+struct convert<lincs::Category> {
+  static Node encode(const lincs::Category& category) {
     Node node;
     node["name"] = category.name;
 
     return node;
   }
 
-  static bool decode(const Node& node, lincs::Problem::Category& category) {
+  static bool decode(const Node& node, lincs::Category& category) {
     category.name = node["name"].as<std::string>();
 
     return true;
   }
 };
 
 template<>
-struct convert<lincs::Problem::Criterion> {
-  static Node encode(const lincs::Problem::Criterion& criterion) {
+struct convert<lincs::Criterion> {
+  static Node encode(const lincs::Criterion& criterion) {
     Node node;
     node["name"] = criterion.name;
     node["value_type"] = std::string(magic_enum::enum_name(criterion.value_type));
     node["category_correlation"] = std::string(magic_enum::enum_name(criterion.category_correlation));
 
     return node;
   }
 
-  static bool decode(const Node& node, lincs::Problem::Criterion& criterion) {
+  static bool decode(const Node& node, lincs::Criterion& criterion) {
     criterion.name = node["name"].as<std::string>();
-    // @todo Handle error where value_type category_correlation does not properly convert back to enum
-    criterion.value_type = magic_enum::enum_cast<lincs::Problem::Criterion::ValueType>(node["value_type"].as<std::string>()).value();
-    criterion.category_correlation = magic_enum::enum_cast<lincs::Problem::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>()).value();
+    criterion.value_type = magic_enum::enum_cast<lincs::Criterion::ValueType>(node["value_type"].as<std::string>()).value();
+    criterion.category_correlation = magic_enum::enum_cast<lincs::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>()).value();
 
     return true;
   }
 };
 
 }  // namespace YAML
 
@@ -57,18 +56,18 @@
 
 const std::string Problem::json_schema(R"($schema: https://json-schema.org/draft/2020-12/schema
 title: Classification problem
 type: object
 properties:
   kind:
     type: string
-    enum: [classification-problem]
+    const: classification-problem
   format_version:
-    # type: integer  # @todo Why does this fail? (Error: <root> [format_version]: Value type not permitted by 'type' constraint.)
-    enum: [1]
+    type: integer
+    const: 1
   criteria:
     type: array
     items:
       type: object
       properties:
         name:
           type: string
@@ -134,38 +133,71 @@
     node["criteria"].as<std::vector<Criterion>>(),
     node["categories"].as<std::vector<Category>>()
   );
 }
 
 TEST_CASE("dumping then loading problem preserves data") {
   Problem problem{
-    {{"Criterion 1", Problem::Criterion::ValueType::real, Problem::Criterion::CategoryCorrelation::growing}},
+    {{"Criterion 1", Criterion::ValueType::real, Criterion::CategoryCorrelation::growing}},
     {{"Category 1"}, {"Category 2"}},
   };
 
   std::stringstream ss;
   problem.dump(ss);
 
+  CHECK(ss.str() == R"(kind: classification-problem
+format_version: 1
+criteria:
+  - name: Criterion 1
+    value_type: real
+    category_correlation: growing
+categories:
+  - name: Category 1
+  - name: Category 2
+)");
+
   Problem problem2 = Problem::load(ss);
   CHECK(problem2.criteria == problem.criteria);
   CHECK(problem2.categories == problem.categories);
 }
 
 TEST_CASE("Parsing error") {
   std::istringstream iss("*");
 
   CHECK_THROWS_WITH_AS(
     Problem::load(iss),
     "yaml-cpp: error at line 1, column 2: alias not found after *",
     YAML::Exception);
 }
 
-TEST_CASE("Validation error") {
+TEST_CASE("Validation error - not an object") {
   std::istringstream iss("42");
 
   CHECK_THROWS_WITH_AS(
     Problem::load(iss),
     "JSON validation failed:\n - <root>: Value type not permitted by 'type' constraint.",
     JsonValidationException);
 }
 
+TEST_CASE("Validation error - bad enum") {
+  std::istringstream iss(R"(kind: classification-problem
+format_version: 1
+criteria:
+  - name: Criterion 1
+    value_type: invalid
+    category_correlation: growing
+categories:
+  - name: Category 1
+  - name: Category 2
+)");
+
+  CHECK_THROWS_WITH_AS(
+    Problem::load(iss),
+    R"(JSON validation failed:
+ - <root> [criteria] [0] [value_type]: Failed to match against any enum values.
+ - <root> [criteria] [0]: Failed to validate against schema associated with property name 'value_type'.
+ - <root> [criteria]: Failed to validate item #0 in array.
+ - <root>: Failed to validate against schema associated with property name 'criteria'.)",
+    JsonValidationException);
+}
+
 }  // namespace lincs
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/problem.hpp` & `lincs-0.5.0/lincs/liblincs/io/problem.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -5,57 +5,59 @@
 
 #include <string>
 #include <vector>
 
 
 namespace lincs {
 
-struct Problem {
-  struct Criterion {
-    std::string name;
-
-    enum class ValueType {
-      real,
-      // @todo Add integer
-      // @todo Add enumerated
-    } value_type;
-
-    enum class CategoryCorrelation {
-      growing,
-      // @todo Add decreasing
-      // @todo Add single-peaked
-      // @todo Add single-valleyed
-      // @todo Add unknown
-    } category_correlation;
-
-    // @todo Remove these constructors
-    // The struct is usable without them in C++, and they were added only to allow using bp::init in the Python module
-    // (Do it for other structs as well)
-    Criterion() {}
-    Criterion(const std::string& name_, ValueType value_type_, CategoryCorrelation category_correlation_): name(name_), value_type(value_type_), category_correlation(category_correlation_) {}
-
-    // @todo Remove this operator
-    // The struct is usable without it in C++, and it was added only to allow using bp::vector_indexing_suite in the Python module
-    // (Do it for other structs as well)
-    bool operator==(const Criterion& other) const {
-      return name == other.name && value_type == other.value_type && category_correlation == other.category_correlation;
-    }
-  };
+struct Criterion {
+  std::string name;
 
-  std::vector<Criterion> criteria;
+  enum class ValueType {
+    real,
+    // @todo Add integer
+    // @todo Add enumerated
+  } value_type;
+
+  enum class CategoryCorrelation {
+    growing,
+    // @todo Add decreasing
+    // @todo Add single-peaked
+    // @todo Add single-valleyed
+    // @todo Add unknown
+  } category_correlation;
+
+  // @todo Add min and max values (with the possibility of infinite values?)
+  // (Currently they are assumed to be 0 and 1 everywhere in the code; this is no small task)
+
+  // @todo Remove these constructors
+  // The struct is usable without them in C++, and they were added only to allow using bp::init in the Python module
+  // (Do it for other structs as well)
+  Criterion() {}
+  Criterion(const std::string& name_, ValueType value_type_, CategoryCorrelation category_correlation_): name(name_), value_type(value_type_), category_correlation(category_correlation_) {}
+
+  // @todo Remove this operator
+  // The struct is usable without it in C++, and it was added only to allow using bp::vector_indexing_suite in the Python module
+  // (Do it for other structs as well)
+  bool operator==(const Criterion& other) const {
+    return name == other.name && value_type == other.value_type && category_correlation == other.category_correlation;
+  }
+};
 
-  struct Category {
-    std::string name;
+struct Category {
+  std::string name;
 
-    Category() {}
-    Category(const std::string& name_): name(name_) {}
+  Category() {}
+  Category(const std::string& name_): name(name_) {}
 
-    bool operator==(const Category& other) const { return name == other.name; }
-  };
+  bool operator==(const Category& other) const { return name == other.name; }
+};
 
+struct Problem {
+  std::vector<Criterion> criteria;
   std::vector<Category> categories;
 
   Problem(const std::vector<Criterion>& criteria_, const std::vector<Category>& categories_): criteria(criteria_), categories(categories_) {}
 
   static const std::string json_schema;
   void dump(std::ostream&) const;
   static Problem load(std::istream&);
```

### Comparing `lincs-0.4.5/lincs/liblincs/io/validation.hpp` & `lincs-0.5.0/lincs/liblincs/io/validation.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2023 Vincent Jacques
 
 #ifndef LINCS__IO__VALIDATION_HPP
 #define LINCS__IO__VALIDATION_HPP
 
 #include <yaml-cpp/yaml.h>
-#include <valijson_yamlcpp_bundled.hpp>
 
+#include "../vendored/valijson/schema.hpp"
 
 namespace lincs {
 
 class JsonValidationException : public std::runtime_error {
  public:
   JsonValidationException(const std::string& message) : std::runtime_error(message) {}
 };
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic/desirability.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
+#ifndef LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
+#define LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
 
-#include <lov-e.hpp>
+#include "../../../../vendored/lov-e.hpp"
 
 
 namespace lincs {
 
 struct Desirability {
   static constexpr float zero_value = 0;
 
@@ -51,8 +51,8 @@
 
 template<>
 __inline__
 void Device::memset<lincs::Desirability>(const std::size_t n, const char v, lincs::Desirability* const p) {
   Device::force_memset<lincs::Desirability>(n, v, p);
 }
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
+#endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC__DESIRABILITY_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -4,62 +4,60 @@
 #include "../../../randomness-utils.hpp"
 
 
 namespace lincs {
 
 void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles() {
   #pragma omp parallel for
-  for (unsigned model_index = 0; model_index != models.models_count; ++model_index) {
+  for (unsigned model_index = 0; model_index != learning_data.models_count; ++model_index) {
     improve_model_profiles(model_index);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profiles(const unsigned model_index) {
-  Array1D<Host, unsigned> criterion_indexes(models.criteria_count, uninitialized);
-  // Not worth parallelizing because models.criteria_count is typically small
-  for (unsigned crit_idx_idx = 0; crit_idx_idx != models.criteria_count; ++crit_idx_idx) {
+  Array1D<Host, unsigned> criterion_indexes(learning_data.criteria_count, uninitialized);
+  // Not worth parallelizing because criteria_count is typically small
+  for (unsigned crit_idx_idx = 0; crit_idx_idx != learning_data.criteria_count; ++crit_idx_idx) {
     criterion_indexes[crit_idx_idx] = crit_idx_idx;
   }
 
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
-  for (unsigned profile_index = 0; profile_index != models.categories_count - 1; ++profile_index) {
-    shuffle(models.urbgs[model_index], ref(criterion_indexes));
+  for (unsigned profile_index = 0; profile_index != learning_data.categories_count - 1; ++profile_index) {
+    shuffle(learning_data.urbgs[model_index], ref(criterion_indexes));
     improve_model_profile(model_index, profile_index, criterion_indexes);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   ArrayView1D<Host, const unsigned> criterion_indexes
 ) {
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
-  for (unsigned crit_idx_idx = 0; crit_idx_idx != models.criteria_count; ++crit_idx_idx) {
+  for (unsigned crit_idx_idx = 0; crit_idx_idx != learning_data.criteria_count; ++crit_idx_idx) {
     improve_model_profile(model_index, profile_index, criterion_indexes[crit_idx_idx]);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index
 ) {
   // WARNING: We're assuming all criteria have values in [0, 1]
-  // @todo Can we relax this assumption?
-  // This is consistent with our comment in the header file, but slightly less generic than Sobrie's thesis
   const float lowest_destination =
     profile_index == 0 ? 0. :
-    models.profiles[criterion_index][profile_index - 1][model_index];
+    learning_data.profiles[criterion_index][profile_index - 1][model_index];
   const float highest_destination =
-    profile_index == models.categories_count - 2 ? 1. :
-    models.profiles[criterion_index][profile_index + 1][model_index];
+    profile_index == learning_data.categories_count - 2 ? 1. :
+    learning_data.profiles[criterion_index][profile_index + 1][model_index];
 
-  float best_destination = models.profiles[criterion_index][profile_index][model_index];
+  float best_destination = learning_data.profiles[criterion_index][profile_index][model_index];
   float best_desirability = Desirability().value();
 
   if (lowest_destination == highest_destination) {
     assert(best_destination == lowest_destination);
     return;
   }
 
@@ -78,40 +76,40 @@
     // Map (embarrassingly parallel)
     float destination = highest_destination;
     // By specification, std::uniform_real_distribution should never return its highest value,
     // but "most existing implementations have a bug where they may occasionally" return it,
     // so we work around that bug by calling it again until it doesn't.
     // Ref: https://en.cppreference.com/w/cpp/numeric/random/uniform_real_distribution
     while (destination == highest_destination) {
-      destination = std::uniform_real_distribution<float>(lowest_destination, highest_destination)(models.urbgs[model_index]);
+      destination = std::uniform_real_distribution<float>(lowest_destination, highest_destination)(learning_data.urbgs[model_index]);
     }
     const float desirability = compute_move_desirability(
       model_index, profile_index, criterion_index, destination).value();
     // Single-key reduce (divide and conquer?) (atomic compare-and-swap?)
     if (desirability > best_desirability) {
       best_desirability = desirability;
       best_destination = destination;
     }
   }
 
   // @todo Desirability can be as high as 2. The [0, 1] interval is a weird choice.
-  if (std::uniform_real_distribution<float>(0, 1)(models.urbgs[model_index]) <= best_desirability) {
-    models.profiles[criterion_index][profile_index][model_index] = best_destination;
+  if (std::uniform_real_distribution<float>(0, 1)(learning_data.urbgs[model_index]) <= best_desirability) {
+    learning_data.profiles[criterion_index][profile_index][model_index] = best_destination;
   }
 }
 
 Desirability ImproveProfilesWithAccuracyHeuristicOnCpu::compute_move_desirability(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index,
   const float destination
 ) {
   Desirability d;
 
-  for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
+  for (unsigned alternative_index = 0; alternative_index != learning_data.learning_alternatives_count; ++alternative_index) {
     update_move_desirability(
       model_index, profile_index, criterion_index, destination, alternative_index, &d);
   }
 
   return d;
 }
 
@@ -119,28 +117,29 @@
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index,
   const float destination,
   const unsigned alternative_index,
   Desirability* desirability
 ) {
-  const float current_position = models.profiles[criterion_index][profile_index][model_index];
-  const float weight = models.weights[criterion_index][model_index];
+  const float current_position = learning_data.profiles[criterion_index][profile_index][model_index];
+  const float weight = learning_data.weights[criterion_index][model_index];
 
-  const float value = models.learning_alternatives[criterion_index][alternative_index];
-  const unsigned learning_assignment = models.learning_assignments[alternative_index];
-  const unsigned model_assignment = WeightsProfilesBreedMrSortLearning::get_assignment(models, model_index, alternative_index);
+  const float value = learning_data.learning_alternatives[criterion_index][alternative_index];
+  const unsigned learning_assignment = learning_data.learning_assignments[alternative_index];
+  const unsigned model_assignment = LearnMrsortByWeightsProfilesBreed::get_assignment(learning_data, model_index, alternative_index);
 
   // @todo Factorize with get_assignment
+  // (Same remark in accuracy-heuristic-on-gpu.cu)
   float weight_at_or_above_profile = 0;
-  for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
-    const float alternative_value = models.learning_alternatives[criterion_index][alternative_index];
-    const float profile_value = models.profiles[criterion_index][profile_index][model_index];
+  for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
+    const float alternative_value = learning_data.learning_alternatives[criterion_index][alternative_index];
+    const float profile_value = learning_data.profiles[criterion_index][profile_index][model_index];
     if (alternative_value >= profile_value) {
-      weight_at_or_above_profile += models.weights[criterion_index][model_index];
+      weight_at_or_above_profile += learning_data.weights[criterion_index][model_index];
     }
   }
 
   // These imbricated conditionals could be factorized, but this form has the benefit
   // of being a direct translation of the top of page 78 of Sobrie's thesis.
   // Correspondance:
   // - learning_assignment: bottom index of A*
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
+#ifndef LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
+#define LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
 
-#include "../../weights-profiles-breed-mrsort.hpp"
+#include "../../mrsort-by-weights-profiles-breed.hpp"
 #include "accuracy-heuristic/desirability.hpp"
 
 
 namespace lincs {
 
-class ImproveProfilesWithAccuracyHeuristicOnCpu : public WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy {
+class ImproveProfilesWithAccuracyHeuristicOnCpu : public LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy {
  public:
-  explicit ImproveProfilesWithAccuracyHeuristicOnCpu(Models& models_) : models(models_) {}
+  explicit ImproveProfilesWithAccuracyHeuristicOnCpu(LearningData& learning_data_) : learning_data(learning_data_) {}
 
  public:
   void improve_profiles() override;
 
  private:
   void improve_model_profiles(const unsigned model_index);
 
@@ -44,13 +44,13 @@
     const unsigned criterion_index,
     const float destination,
     const unsigned alternative_index,
     Desirability* desirability
   );
 
  private:
-  Models& models;
+  LearningData& learning_data;
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
+#endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.cu`

 * *Files 13% similar despite different names*

```diff
@@ -15,17 +15,14 @@
   const ArrayView3D<Device, const float> profiles,
   const unsigned model_index,
   const unsigned alternative_index
 ) {
   const unsigned criteria_count = learning_alternatives.s1();
   const unsigned categories_count = profiles.s1() + 1;
 
-  // @todo Evaluate if it's worth storing and updating the gpu_models' assignments
-  // (instead of recomputing them here)
-
   // Not parallelizable in this form because the loop gets interrupted by a return. But we could rewrite it
   // to always perform all its iterations, and then it would be yet another map-reduce, with the reduce
   // phase keeping the maximum 'category_index' that passes the weight threshold.
   for (unsigned category_index = categories_count - 1; category_index != 0; --category_index) {
     const unsigned profile_index = category_index - 1;
     float weight_at_or_above_profile = 0;
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
@@ -66,15 +63,14 @@
   const unsigned model_assignment = get_assignment(
     learning_alternatives,
     weights,
     profiles,
     model_index,
     alternative_index);
 
-  // @todo Factorize with get_assignment
   float weight_at_or_above_profile = 0;
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     const float alternative_value = learning_alternatives[criterion_index][alternative_index];
     const float profile_value = profiles[criterion_index][profile_index][model_index];
     if (alternative_value >= profile_value) {
       weight_at_or_above_profile += weights[criterion_index][model_index];
     }
@@ -236,127 +232,125 @@
   }
 }
 
 }  // namespace
 
 namespace lincs {
 
-ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels::make(const Models& models) {
+ImproveProfilesWithAccuracyHeuristicOnGpu::GpuLearningData ImproveProfilesWithAccuracyHeuristicOnGpu::GpuLearningData::make(const LearningData& learning_data) {
   return {
-    models.categories_count,
-    models.criteria_count,
-    models.learning_alternatives_count,
-    models.learning_alternatives.template clone_to<Device>(),
-    models.learning_assignments.template clone_to<Device>(),
-    models.models_count,
-    Array2D<Device, float>(models.criteria_count, models.models_count, uninitialized),
-    Array3D<Device, float>(models.criteria_count, (models.categories_count - 1), models.models_count, uninitialized),
-    Array2D<Device, Desirability>(models.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::destinations_count, uninitialized),
-    Array2D<Device, float>(models.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::destinations_count, uninitialized),
+    learning_data.categories_count,
+    learning_data.criteria_count,
+    learning_data.learning_alternatives_count,
+    learning_data.learning_alternatives.template clone_to<Device>(),
+    learning_data.learning_assignments.template clone_to<Device>(),
+    learning_data.models_count,
+    Array2D<Device, float>(learning_data.criteria_count, learning_data.models_count, uninitialized),
+    Array3D<Device, float>(learning_data.criteria_count, (learning_data.categories_count - 1), learning_data.models_count, uninitialized),
+    Array2D<Device, Desirability>(learning_data.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::destinations_count, uninitialized),
+    Array2D<Device, float>(learning_data.models_count, ImproveProfilesWithAccuracyHeuristicOnGpu::destinations_count, uninitialized),
   };
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles() {
   // Get optimized weights
-  copy(host_models.weights, ref(gpu_models.weights));
+  copy(host_learning_data.weights, ref(gpu_learning_data.weights));
   // Get (re-)initialized profiles
-  copy(host_models.profiles, ref(gpu_models.profiles));
+  copy(host_learning_data.profiles, ref(gpu_learning_data.profiles));
 
   #pragma omp parallel for
-  for (unsigned model_index = 0; model_index != gpu_models.models_count; ++model_index) {
+  for (unsigned model_index = 0; model_index != gpu_learning_data.models_count; ++model_index) {
     improve_model_profiles(model_index);
   }
 
   // Set improved profiles
-  copy(gpu_models.profiles, ref(host_models.profiles));
+  copy(gpu_learning_data.profiles, ref(host_learning_data.profiles));
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_model_profiles(const unsigned model_index) {
-  Array1D<Host, unsigned> criterion_indexes(gpu_models.criteria_count, uninitialized);
-  // Not worth parallelizing because models.criteria_count is typically small
-  for (unsigned crit_idx_idx = 0; crit_idx_idx != gpu_models.criteria_count; ++crit_idx_idx) {
+  Array1D<Host, unsigned> criterion_indexes(gpu_learning_data.criteria_count, uninitialized);
+  // Not worth parallelizing because learning_data.criteria_count is typically small
+  for (unsigned crit_idx_idx = 0; crit_idx_idx != gpu_learning_data.criteria_count; ++crit_idx_idx) {
     criterion_indexes[crit_idx_idx] = crit_idx_idx;
   }
 
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
-  for (unsigned profile_index = 0; profile_index != gpu_models.categories_count - 1; ++profile_index) {
-    shuffle(host_models.urbgs[model_index], ref(criterion_indexes));
+  for (unsigned profile_index = 0; profile_index != gpu_learning_data.categories_count - 1; ++profile_index) {
+    shuffle(host_learning_data.urbgs[model_index], ref(criterion_indexes));
     improve_model_profile(model_index, profile_index, criterion_indexes);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   const ArrayView1D<Host, const unsigned> criterion_indexes
 ) {
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
-  for (unsigned crit_idx_idx = 0; crit_idx_idx != gpu_models.criteria_count; ++crit_idx_idx) {
+  for (unsigned crit_idx_idx = 0; crit_idx_idx != gpu_learning_data.criteria_count; ++crit_idx_idx) {
     improve_model_profile(model_index, profile_index, criterion_indexes[crit_idx_idx]);
   }
 }
 
 void ImproveProfilesWithAccuracyHeuristicOnGpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index
 ) {
   // WARNING: We're assuming all criteria have values in [0, 1]
-  // @todo Can we relax this assumption?
-  // This is consistent with our comment in the header file, but slightly less generic than Sobrie's thesis
   const float lowest_destination =
     profile_index == 0 ? 0. :
-    host_models.profiles[criterion_index][profile_index - 1][model_index];
+    host_learning_data.profiles[criterion_index][profile_index - 1][model_index];
   const float highest_destination =
-    profile_index == host_models.categories_count - 2 ? 1. :
-    host_models.profiles[criterion_index][profile_index + 1][model_index];
+    profile_index == host_learning_data.categories_count - 2 ? 1. :
+    host_learning_data.profiles[criterion_index][profile_index + 1][model_index];
 
   if (lowest_destination == highest_destination) {
-    assert(host_models.profiles[criterion_index][profile_index][model_index] == lowest_destination);
+    assert(host_learning_data.profiles[criterion_index][profile_index][model_index] == lowest_destination);
     return;
   }
 
   Array1D<Host, float> host_destinations(destinations_count, uninitialized);
   for (unsigned destination_index = 0; destination_index != destinations_count; ++destination_index) {
     float destination = highest_destination;
     // By specification, std::uniform_real_distribution should never return its highest value,
     // but "most existing implementations have a bug where they may occasionally" return it,
     // so we work around that bug by calling it again until it doesn't.
     // Ref: https://en.cppreference.com/w/cpp/numeric/random/uniform_real_distribution
     while (destination == highest_destination) {
-      destination = std::uniform_real_distribution<float>(lowest_destination, highest_destination)(host_models.urbgs[model_index]);
+      destination = std::uniform_real_distribution<float>(lowest_destination, highest_destination)(host_learning_data.urbgs[model_index]);
     }
     host_destinations[destination_index] = destination;
   }
 
-  copy(host_destinations, ref(gpu_models.destinations[model_index]));
-  gpu_models.desirabilities[model_index].fill_with_zeros();
-  Grid grid = grid::make(gpu_models.learning_alternatives_count, destinations_count);
+  copy(host_destinations, ref(gpu_learning_data.destinations[model_index]));
+  gpu_learning_data.desirabilities[model_index].fill_with_zeros();
+  Grid grid = grid::make(gpu_learning_data.learning_alternatives_count, destinations_count);
   compute_move_desirabilities__kernel<<<LOVE_CONFIG(grid)>>>(
-    gpu_models.learning_alternatives,
-    gpu_models.learning_assignments,
-    gpu_models.weights,
-    gpu_models.profiles,
+    gpu_learning_data.learning_alternatives,
+    gpu_learning_data.learning_assignments,
+    gpu_learning_data.weights,
+    gpu_learning_data.profiles,
     model_index,
     profile_index,
     criterion_index,
-    gpu_models.destinations[model_index],
-    ref(gpu_models.desirabilities[model_index]));
+    gpu_learning_data.destinations[model_index],
+    ref(gpu_learning_data.desirabilities[model_index]));
   check_last_cuda_error_sync_stream(cudaStreamDefault);
 
   apply_best_move__kernel<<<1, 1>>>(
-    ref(gpu_models.profiles),
+    ref(gpu_learning_data.profiles),
     model_index,
     profile_index,
     criterion_index,
-    gpu_models.destinations[model_index],
-    gpu_models.desirabilities[model_index],
-    std::uniform_real_distribution<float>(0, 1)(host_models.urbgs[model_index]));
+    gpu_learning_data.destinations[model_index],
+    gpu_learning_data.desirabilities[model_index],
+    std::uniform_real_distribution<float>(0, 1)(host_learning_data.urbgs[model_index]));
   check_last_cuda_error_sync_stream(cudaStreamDefault);
 
   // @todo Double-check and document why we don't need [model_index] here
-  copy(gpu_models.profiles[criterion_index][profile_index], host_models.profiles[criterion_index][profile_index]);
+  copy(gpu_learning_data.profiles[criterion_index][profile_index], host_learning_data.profiles[criterion_index][profile_index]);
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/improve-profiles/accuracy-heuristic-on-gpu.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
+#ifndef LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
+#define LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
 
-#include "../../weights-profiles-breed-mrsort.hpp"
+#include "../../mrsort-by-weights-profiles-breed.hpp"
 #include "accuracy-heuristic/desirability.hpp"
 
 
 namespace lincs {
 
-class ImproveProfilesWithAccuracyHeuristicOnGpu : public WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy {
- public:
-  struct GpuModels;
+class ImproveProfilesWithAccuracyHeuristicOnGpu : public LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy {
+ private:
+  struct GpuLearningData {
+    unsigned categories_count;
+    unsigned criteria_count;
+    unsigned learning_alternatives_count;
+    Array2D<Device, float> learning_alternatives;
+    Array1D<Device, unsigned> learning_assignments;
+    unsigned models_count;
+    Array2D<Device, float> weights;
+    Array3D<Device, float> profiles;
+
+    Array2D<Device, Desirability> desirabilities;
+    Array2D<Device, float> destinations;
+
+    static GpuLearningData make(const LearningData&);
+  };
 
  public:
-  explicit ImproveProfilesWithAccuracyHeuristicOnGpu(Models& host_models_, GpuModels& gpu_models_) : host_models(host_models_), gpu_models(gpu_models_) {}
+  explicit ImproveProfilesWithAccuracyHeuristicOnGpu(LearningData& host_learning_data_) : host_learning_data(host_learning_data_), gpu_learning_data(std::move(GpuLearningData::make(host_learning_data))) {}
 
  public:
   void improve_profiles() override;
 
  private:
   void improve_model_profiles(const unsigned model_index);
 
@@ -31,32 +45,16 @@
   void improve_model_profile(
     const unsigned model_index,
     const unsigned profile_index,
     const unsigned criterion_index
   );
 
  private:
-  Models& host_models;
-  GpuModels& gpu_models;
+  LearningData& host_learning_data;
+  GpuLearningData gpu_learning_data;
 
   static const unsigned destinations_count = 64;
 };
 
-struct ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels {
-  unsigned categories_count;
-  unsigned criteria_count;
-  unsigned learning_alternatives_count;
-  Array2D<Device, float> learning_alternatives;
-  Array1D<Device, unsigned> learning_assignments;
-  unsigned models_count;
-  Array2D<Device, float> weights;
-  Array3D<Device, float> profiles;
-
-  Array2D<Device, Desirability> desirabilities;
-  Array2D<Device, float> destinations;
-
-  static GpuModels make(const Models&);
-};
-
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
+#endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_GPU_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 // Copyright 2023 Vincent Jacques
 
 #include "probabilistic-maximal-discrimination-power-per-criterion.hpp"
 
 
 namespace lincs {
 
-InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(Models& models_) : models(models_) {
-  for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
+InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(LearningData& learning_data_) : learning_data(learning_data_) {
+  for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
     generators.emplace_back();
-    for (unsigned profile_index = 0; profile_index != models.categories_count - 1; ++profile_index) {
+    for (unsigned profile_index = 0; profile_index != learning_data.categories_count - 1; ++profile_index) {
       generators.back().emplace_back(get_candidate_probabilities(criterion_index, profile_index));
     }
   }
 }
 
 std::map<float, double> InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::get_candidate_probabilities(
   unsigned criterion_index,
   unsigned profile_index
 ) {
   std::vector<float> values_below;
   // The size used for 'reserve' is a few times larger than the actual final size,
   // so we're allocating too much memory. As it's temporary, I don't think it's too bad.
   // If 'initialize' ever becomes the centre of focus for our optimization effort, we should measure.
-  values_below.reserve(models.learning_alternatives_count);
+  values_below.reserve(learning_data.learning_alternatives_count);
   std::vector<float> values_above;
-  values_above.reserve(models.learning_alternatives_count);
+  values_above.reserve(learning_data.learning_alternatives_count);
   // This loop could/should be done once outside this function
-  for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
-    const float value = models.learning_alternatives[criterion_index][alternative_index];
-    const unsigned assignment = models.learning_assignments[alternative_index];
+  for (unsigned alternative_index = 0; alternative_index != learning_data.learning_alternatives_count; ++alternative_index) {
+    const float value = learning_data.learning_alternatives[criterion_index][alternative_index];
+    const unsigned assignment = learning_data.learning_assignments[alternative_index];
     if (assignment == profile_index) {
       values_below.push_back(value);
     } else if (assignment == profile_index + 1) {
       values_above.push_back(value);
     }
   }
 
@@ -54,40 +54,40 @@
     }
   }
 
   return candidate_probabilities;
 }
 
 void InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::initialize_profiles(
-  std::vector<unsigned>::const_iterator model_indexes_begin,
-  const std::vector<unsigned>::const_iterator model_indexes_end
+  unsigned model_indexes_begin,
+  const unsigned model_indexes_end
 ) {
   // Embarrassingly parallel
   for (; model_indexes_begin != model_indexes_end; ++model_indexes_begin) {
-    const unsigned model_index = *model_indexes_begin;
+    const unsigned model_index = learning_data.model_indexes[model_indexes_begin];
 
     // Embarrassingly parallel
-    for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
+    for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
       // Not parallel because of the profiles ordering constraint
-      for (unsigned category_index = models.categories_count - 1; category_index != 0; --category_index) {
+      for (unsigned category_index = learning_data.categories_count - 1; category_index != 0; --category_index) {
         const unsigned profile_index = category_index - 1;
-        float value = generators[criterion_index][profile_index](models.urbgs[model_index]);
+        float value = generators[criterion_index][profile_index](learning_data.urbgs[model_index]);
 
-        if (profile_index != models.categories_count - 2) {
-          value = std::min(value, models.profiles[criterion_index][profile_index + 1][model_index]);
+        if (profile_index != learning_data.categories_count - 2) {
+          value = std::min(value, learning_data.profiles[criterion_index][profile_index + 1][model_index]);
         }
         // @todo Add a unit test that triggers the following assertion
         // (This will require removing the code to enforce the order of profiles above)
         // Then restore the code to enforce the order of profiles
         // Note, this assertion does not protect us from initializing a model with two identical profiles.
         // Is it really that bad?
         assert(
-          profile_index == models.categories_count - 2
-          || models.profiles[criterion_index][profile_index + 1][model_index] >= value);
+          profile_index == learning_data.categories_count - 2
+          || learning_data.profiles[criterion_index][profile_index + 1][model_index] >= value);
 
-        models.profiles[criterion_index][profile_index][model_index] = value;
+        learning_data.profiles[criterion_index][profile_index][model_index] = value;
       }
     }
   }
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
+#ifndef LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
+#define LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
 
-#include "../../weights-profiles-breed-mrsort.hpp"
+#include "../../mrsort-by-weights-profiles-breed.hpp"
 #include "../../../randomness-utils.hpp"
 
 namespace lincs {
 
-class InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion : public WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy {
+class InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion : public LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy {
  public:
-  InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(Models& models_);
+  InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(LearningData& learning_data_);
 
  public:
-  void initialize_profiles(
-    std::vector<unsigned>::const_iterator model_indexes_begin,
-    const std::vector<unsigned>::const_iterator model_indexes_end
-  ) override;
+  void initialize_profiles(unsigned model_indexes_begin, unsigned model_indexes_end) override;
 
  private:
   std::map<float, double> get_candidate_probabilities(
     unsigned criterion_index,
     unsigned profile_index
   );
 
  private:
-  Models& models;
+  LearningData& learning_data;
   std::vector<std::vector<ProbabilityWeightedGenerator<float>>> generators;
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
+#endif  // LINCS__LEARNING__MRSORT_BY_WEIGHTS_PROFILES_BREED__INITIALIZE_PROFILES__PROBABILISTIC_MAXIMAL_DISCRIMINATION_POWER_PER_CRITERION_HPP
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed/optimize-weights/linear-program.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #include "../../../linear-programming/alglib.hpp"
 
 namespace lincs {
 
 template<typename LinearProgram>
 void OptimizeWeightsUsingLinearProgram<LinearProgram>::optimize_weights() {
   #pragma omp parallel for
-  for (unsigned model_index = 0; model_index != models.models_count; ++model_index) {
+  for (unsigned model_index = 0; model_index != learning_data.models_count; ++model_index) {
     optimize_model_weights(model_index);
   }
 }
 
 template<typename LinearProgram>
 void OptimizeWeightsUsingLinearProgram<LinearProgram>::optimize_model_weights(unsigned model_index) {
   const float epsilon = 1e-6;
@@ -22,71 +22,71 @@
 
   std::vector<typename LinearProgram::variable_type> weight_variables;
   std::vector<typename LinearProgram::variable_type> x_variables;
   std::vector<typename LinearProgram::variable_type> xp_variables;
   std::vector<typename LinearProgram::variable_type> y_variables;
   std::vector<typename LinearProgram::variable_type> yp_variables;
 
-  weight_variables.reserve(models.criteria_count);
-  for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
+  weight_variables.reserve(learning_data.criteria_count);
+  for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
     weight_variables.push_back(program.create_variable());
   }
 
-  x_variables.reserve(models.learning_alternatives_count);
-  xp_variables.reserve(models.learning_alternatives_count);
-  y_variables.reserve(models.learning_alternatives_count);
-  yp_variables.reserve(models.learning_alternatives_count);
-  for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
+  x_variables.reserve(learning_data.learning_alternatives_count);
+  xp_variables.reserve(learning_data.learning_alternatives_count);
+  y_variables.reserve(learning_data.learning_alternatives_count);
+  yp_variables.reserve(learning_data.learning_alternatives_count);
+  for (unsigned alternative_index = 0; alternative_index != learning_data.learning_alternatives_count; ++alternative_index) {
     x_variables.push_back(program.create_variable());
     xp_variables.push_back(program.create_variable());
     y_variables.push_back(program.create_variable());
     yp_variables.push_back(program.create_variable());
   }
 
   program.mark_all_variables_created();
 
-  for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
+  for (unsigned alternative_index = 0; alternative_index != learning_data.learning_alternatives_count; ++alternative_index) {
     program.set_objective_coefficient(xp_variables[alternative_index], 1);
     program.set_objective_coefficient(yp_variables[alternative_index], 1);
 
-    const unsigned category_index = models.learning_assignments[alternative_index];
+    const unsigned category_index = learning_data.learning_assignments[alternative_index];
 
     if (category_index != 0) {
       auto c = program.create_constraint();
       c.set_bounds(1, 1);
       c.set_coefficient(x_variables[alternative_index], -1);
       c.set_coefficient(xp_variables[alternative_index], 1);
-      for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
-        const float alternative_value = models.learning_alternatives[criterion_index][alternative_index];
-        const float profile_value = models.profiles[criterion_index][category_index - 1][model_index];
+      for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
+        const float alternative_value = learning_data.learning_alternatives[criterion_index][alternative_index];
+        const float profile_value = learning_data.profiles[criterion_index][category_index - 1][model_index];
         if (alternative_value >= profile_value) {
           c.set_coefficient(weight_variables[criterion_index], 1);
         }
       }
     }
 
-    if (category_index != models.categories_count - 1) {
+    if (category_index != learning_data.categories_count - 1) {
       auto c = program.create_constraint();
       c.set_bounds(1 - epsilon, 1 - epsilon);
       c.set_coefficient(y_variables[alternative_index], 1);
       c.set_coefficient(yp_variables[alternative_index], -1);
-      for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
-        const float alternative_value = models.learning_alternatives[criterion_index][alternative_index];
-        const float profile_value = models.profiles[criterion_index][category_index][model_index];
+      for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
+        const float alternative_value = learning_data.learning_alternatives[criterion_index][alternative_index];
+        const float profile_value = learning_data.profiles[criterion_index][category_index][model_index];
         if (alternative_value >= profile_value) {
           c.set_coefficient(weight_variables[criterion_index], 1);
         }
       }
     }
   }
 
   auto values = program.solve();
 
-  for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
-    models.weights[criterion_index][model_index] = values[weight_variables[criterion_index]];
+  for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
+    learning_data.weights[criterion_index][model_index] = values[weight_variables[criterion_index]];
   }
 }
 
 template class OptimizeWeightsUsingLinearProgram<GlopLinearProgram>;
 template class OptimizeWeightsUsingLinearProgram<AlglibLinearProgram>;
 
 }  // namespace lincs
```

### Comparing `lincs-0.4.5/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.5.0/lincs/liblincs/learning/mrsort-by-weights-profiles-breed.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 // Copyright 2023 Vincent Jacques
 
-#include "weights-profiles-breed-mrsort.hpp"
+#include "mrsort-by-weights-profiles-breed.hpp"
 
 #include <map>
 
-#include "../median-and-max.hpp"
+#include "exception.hpp"
 
 
 namespace lincs {
 
-WeightsProfilesBreedMrSortLearning::Models WeightsProfilesBreedMrSortLearning::Models::make(const Problem& problem, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed) {
-  std::map<std::string, unsigned> category_indexes;
-  for (const auto& category: problem.categories) {
-    category_indexes[category.name] = category_indexes.size();
-  }
-
+LearnMrsortByWeightsProfilesBreed::LearningData LearnMrsortByWeightsProfilesBreed::LearningData::make(const Problem& problem, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed) {
   const unsigned criteria_count = problem.criteria.size();
   const unsigned categories_count = problem.categories.size();
   const unsigned alternatives_count = learning_set.alternatives.size();
 
   Array2D<Host, float> alternatives(criteria_count, alternatives_count, uninitialized);
   Array1D<Host, unsigned> assignments(alternatives_count, uninitialized);
 
   for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
     const Alternative& alt = learning_set.alternatives[alternative_index];
 
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
       alternatives[criterion_index][alternative_index] = alt.profile[criterion_index];
     }
 
-    assignments[alternative_index] = category_indexes[*alt.category];
+    assignments[alternative_index] = *alt.category_index;
   }
 
+  std::vector<unsigned> model_indexes(models_count);
+  std::iota(model_indexes.begin(), model_indexes.end(), 0);
+
   Array2D<Host, float> weights(criteria_count, models_count, uninitialized);
   Array3D<Host, float> profiles(criteria_count, (categories_count - 1), models_count, uninitialized);
+  Array1D<Host, unsigned> accuracies(models_count, zeroed);
 
   std::vector<std::mt19937> urbgs(models_count);
   for (unsigned model_index = 0; model_index != models_count; ++model_index) {
     urbgs[model_index].seed(random_seed * (model_index + 1));
   }
 
   return {
     problem,
     categories_count,
     criteria_count,
     alternatives_count,
     std::move(alternatives),
     std::move(assignments),
+    0,
     models_count,
+    std::move(model_indexes),
     std::move(weights),
     std::move(profiles),
+    std::move(accuracies),
     std::move(urbgs),
   };
 }
 
-Model WeightsProfilesBreedMrSortLearning::Models::get_model(const unsigned model_index) const {
+Model LearnMrsortByWeightsProfilesBreed::LearningData::get_model(const unsigned model_index) const {
   assert(model_index < models_count);
 
   std::vector<float> model_weights;
   model_weights.reserve(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     model_weights.push_back(weights[criterion_index][model_index]);
   }
-  Model::SufficientCoalitions coalitions{Model::SufficientCoalitions::Kind::weights, model_weights};
+  SufficientCoalitions coalitions{SufficientCoalitions::weights, model_weights};
 
   std::vector<Model::Boundary> boundaries;
   boundaries.reserve(categories_count - 1);
   for (unsigned cat_index = 0; cat_index != categories_count - 1; ++cat_index) {
     std::vector<float> boundary_profile;
     boundary_profile.reserve(criteria_count);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
@@ -74,92 +76,104 @@
     }
     boundaries.emplace_back(boundary_profile, coalitions);
   }
 
   return Model{problem, boundaries};
 }
 
-Model WeightsProfilesBreedMrSortLearning::perform() {
-  std::vector<unsigned> model_indexes(models.models_count, 0);
-  std::iota(model_indexes.begin(), model_indexes.end(), 0);
-  profiles_initialization_strategy.initialize_profiles(model_indexes.begin(), model_indexes.end());
+Model LearnMrsortByWeightsProfilesBreed::perform() {
+  profiles_initialization_strategy.initialize_profiles(0, learning_data.models_count);
 
-  unsigned best_accuracy = 0;
-
-  for (int iteration_index = 0; !termination_strategy.terminate(iteration_index, best_accuracy); ++iteration_index) {
-    if (iteration_index != 0) {
-      profiles_initialization_strategy.initialize_profiles(model_indexes.begin(), model_indexes.begin() + models.models_count / 2);
-    }
+  unsigned iterations_without_progress = 0;
+  // Limit is arbitrary; unit tests show 40 is required, so 100 seems OK with some margin
+  while (iterations_without_progress < 100) {
+    const unsigned previous_best_accuracy = learning_data.get_best_accuracy();
 
+    // Improve
     weights_optimization_strategy.optimize_weights();
     profiles_improvement_strategy.improve_profiles();
 
-    auto p = partition_models_by_accuracy();
-    model_indexes = std::move(p.first);
-    best_accuracy = p.second;
-  }
+    // Sort model_indexes by increasing model accuracy
+    for (unsigned model_index = 0; model_index != learning_data.models_count; ++model_index) {
+      learning_data.accuracies[model_index] = compute_accuracy(model_index);
+    }
+    std::sort(
+      learning_data.model_indexes.begin(), learning_data.model_indexes.end(),
+      [this](unsigned left_model_index, unsigned right_model_index) {
+        return learning_data.accuracies[left_model_index] < learning_data.accuracies[right_model_index];
+      }
+    );
 
-  return models.get_model(model_indexes.back());
-}
+    // Interrupt if no progress
+    const unsigned new_best_accuracy = learning_data.get_best_accuracy();
+    if (new_best_accuracy > previous_best_accuracy) {
+      iterations_without_progress = 0;
+    } else {
+      ++iterations_without_progress;
+    }
 
-std::pair<std::vector<unsigned>, unsigned> WeightsProfilesBreedMrSortLearning::partition_models_by_accuracy() {
-  std::vector<unsigned> accuracies(models.models_count, 0);
-  for (unsigned model_index = 0; model_index != models.models_count; ++model_index) {
-    accuracies[model_index] = get_accuracy(model_index);
-  }
+    // Succeed?
+    if (new_best_accuracy == learning_data.learning_alternatives_count || termination_strategy.terminate()) {
+      return learning_data.get_model(learning_data.model_indexes.back());
+    }
 
-  std::vector<unsigned> model_indexes(models.models_count, 0);
-  std::iota(model_indexes.begin(), model_indexes.end(), 0);
-  ensure_median_and_max(
-    model_indexes.begin(), model_indexes.end(),
-    [&accuracies](unsigned left_model_index, unsigned right_model_index) {
-      return accuracies[left_model_index] < accuracies[right_model_index];
-    });
+    // Breed
+    breeding_strategy.breed();
+
+    // Observe
+    for (auto observer : observers) {
+      observer->after_iteration();
+    }
+
+    ++learning_data.iteration_index;
+  }
 
-  return std::make_pair(model_indexes, accuracies[model_indexes.back()]);
+  // Fail
+  throw LearningFailureException();
 }
 
-unsigned WeightsProfilesBreedMrSortLearning::get_accuracy(const unsigned model_index) {
+unsigned LearnMrsortByWeightsProfilesBreed::compute_accuracy(const unsigned model_index) {
   unsigned accuracy = 0;
 
-  for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
+  for (unsigned alternative_index = 0; alternative_index != learning_data.learning_alternatives_count; ++alternative_index) {
     if (is_correctly_assigned(model_index, alternative_index)) {
       ++accuracy;
     }
   }
 
   return accuracy;
 }
 
-bool WeightsProfilesBreedMrSortLearning::is_correctly_assigned(
+bool LearnMrsortByWeightsProfilesBreed::is_correctly_assigned(
     const unsigned model_index,
     const unsigned alternative_index) {
-  const unsigned expected_assignment = models.learning_assignments[alternative_index];
-  const unsigned actual_assignment = get_assignment(models, model_index, alternative_index);
+  const unsigned expected_assignment = learning_data.learning_assignments[alternative_index];
+  const unsigned actual_assignment = get_assignment(learning_data, model_index, alternative_index);
 
   return actual_assignment == expected_assignment;
 }
 
-unsigned WeightsProfilesBreedMrSortLearning::get_assignment(const Models& models, const unsigned model_index, const unsigned alternative_index) {
+unsigned LearnMrsortByWeightsProfilesBreed::get_assignment(const LearningData& learning_data, const unsigned model_index, const unsigned alternative_index) {
   // @todo Evaluate if it's worth storing and updating the models' assignments
   // (instead of recomputing them here)
-  assert(model_index < models.models_count);
-  assert(alternative_index < models.learning_alternatives_count);
+  // Same question in accuracy-heuristic-on-gpu.cu
+  assert(model_index < learning_data.models_count);
+  assert(alternative_index < learning_data.learning_alternatives_count);
 
   // Not parallelizable in this form because the loop gets interrupted by a return. But we could rewrite it
   // to always perform all its iterations, and then it would be yet another map-reduce, with the reduce
   // phase keeping the maximum 'category_index' that passes the weight threshold.
-  for (unsigned category_index = models.categories_count - 1; category_index != 0; --category_index) {
+  for (unsigned category_index = learning_data.categories_count - 1; category_index != 0; --category_index) {
     const unsigned profile_index = category_index - 1;
     float weight_at_or_above_profile = 0;
-    for (unsigned criterion_index = 0; criterion_index != models.criteria_count; ++criterion_index) {
-      const float alternative_value = models.learning_alternatives[criterion_index][alternative_index];
-      const float profile_value = models.profiles[criterion_index][profile_index][model_index];
+    for (unsigned criterion_index = 0; criterion_index != learning_data.criteria_count; ++criterion_index) {
+      const float alternative_value = learning_data.learning_alternatives[criterion_index][alternative_index];
+      const float profile_value = learning_data.profiles[criterion_index][profile_index][model_index];
       if (alternative_value >= profile_value) {
-        weight_at_or_above_profile += models.weights[criterion_index][model_index];
+        weight_at_or_above_profile += learning_data.weights[criterion_index][model_index];
       }
     }
     if (weight_at_or_above_profile >= 1) {
       return category_index;
     }
   }
   return 0;
```

### Comparing `lincs-0.4.5/lincs/liblincs/liblincs_module.cpp` & `lincs-0.5.0/lincs/liblincs/liblincs_module.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 
 #include <iostream>
 
 #include <boost/python.hpp>
 #include <boost/python/suite/indexing/vector_indexing_suite.hpp>
 #include <boost/iostreams/concepts.hpp>
 #include <boost/iostreams/stream.hpp>
-#include <magic_enum.hpp>
+
+#include "vendored/magic_enum.hpp"
 
 #ifndef DOCTEST_CONFIG_DISABLE
 #define DOCTEST_CONFIG_IMPLEMENT_WITH_MAIN
 #endif
-#include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
+#include "vendored/doctest.h"  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 // @todo Consider using pybind11, which advertises itself as an evolved and simplified version of Boost.Python
 namespace bp = boost::python;
 
 namespace {
 
@@ -36,22 +37,22 @@
 };
 
 void dump_problem(const lincs::Problem& problem, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
   problem.dump(out_stream);
 }
 
-void dump_model(const lincs::Model& model, bp::object& out_file) {
+void dump_model(const lincs::Model& model, const lincs::Problem& problem, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
-  model.dump(out_stream);
+  model.dump(problem, out_stream);
 }
 
-void dump_alternatives(const lincs::Alternatives& alternatives, bp::object& out_file) {
+void dump_alternatives(const lincs::Alternatives& alternatives, const lincs::Problem& problem, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
-  alternatives.dump(out_stream);
+  alternatives.dump(problem, out_stream);
 }
 
 class PythonInputDevice : public boost::iostreams::source {
   public:
 
   explicit PythonInputDevice(bp::object in_file_) : in_file(in_file_) {}
 
@@ -150,271 +151,388 @@
       &std_optional_converter<T>::convertible,
       &std_optional_converter<T>::construct,
       bp::type_id<std::optional<T>>()
     );
   }
 };
 
-lincs::WeightsProfilesBreedMrSortLearning::Models* make_models(
+lincs::LearnMrsortByWeightsProfilesBreed::LearningData* make_learning_data(
   const lincs::Problem& problem,
   const lincs::Alternatives& learning_set,
   const unsigned models_count,
   const unsigned random_seed
 ) {
-  return new lincs::WeightsProfilesBreedMrSortLearning::Models(std::move(
-    lincs::WeightsProfilesBreedMrSortLearning::Models::make(problem, learning_set, models_count, random_seed)));
+  return new lincs::LearnMrsortByWeightsProfilesBreed::LearningData(std::move(
+    lincs::LearnMrsortByWeightsProfilesBreed::LearningData::make(problem, learning_set, models_count, random_seed)));
 }
 
-lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels* make_gpu_models(
-  const lincs::WeightsProfilesBreedMrSortLearning::Models& models
-) {
-  return new lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels(std::move(
-    lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels::make(models)));
+std::optional<unsigned> get_alternative_category_index(const lincs::Alternative& alt) {
+  return alt.category_index;
 }
 
-std::optional<std::string> get_alternative_category(const lincs::Alternative& alt) {
-  return alt.category;
-}
-
-void set_alternative_category(lincs::Alternative& alt, std::optional<std::string> category) {
-  alt.category = category;
+void set_alternative_category_index(lincs::Alternative& alt, std::optional<unsigned> category_index) {
+  alt.category_index = category_index;
 }
 
 }  // namespace
 
 template <typename T>
-void auto_enum(const std::string& name) {
+auto auto_enum(const std::string& name) {
   auto e = bp::enum_<T>(name.c_str());
   for(T value : magic_enum::enum_values<T>()) {
     e.value(std::string(magic_enum::enum_name(value)).c_str(), value);
   }
+  return e;
 }
 
 BOOST_PYTHON_MODULE(liblincs) {
   iterable_converter()
     .from_python<std::vector<float>>()
-    .from_python<std::vector<lincs::Problem::Category>>()
-    .from_python<std::vector<lincs::Problem::Criterion>>()
+    .from_python<std::vector<unsigned>>()
+    .from_python<std::vector<std::vector<unsigned>>>()
+    .from_python<std::vector<lincs::Category>>()
+    .from_python<std::vector<lincs::Criterion>>()
     .from_python<std::vector<lincs::Model::Boundary>>()
-    .from_python<std::vector<lincs::Model::SufficientCoalitions>>()
+    .from_python<std::vector<lincs::SufficientCoalitions>>()
     .from_python<std::vector<lincs::Alternative>>()
+    .from_python<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy*>>()
+    .from_python<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::Observer*>>()
   ;
 
   std_optional_converter<float>::enroll();
-  std_optional_converter<std::string>::enroll();
-
-  // @todo Decide wether we nest types or not, use the same nesting in Python and C++
-  auto_enum<lincs::Problem::Criterion::ValueType>("ValueType");
-  auto_enum<lincs::Problem::Criterion::CategoryCorrelation>("CategoryCorrelation");
-  auto_enum<lincs::Model::SufficientCoalitions::Kind>("SufficientCoalitionsKind");
+  std_optional_converter<unsigned>::enroll();
 
-  bp::class_<lincs::Problem::Criterion>("Criterion", bp::init<std::string, lincs::Problem::Criterion::ValueType, lincs::Problem::Criterion::CategoryCorrelation>())
-    .def_readwrite("name", &lincs::Problem::Criterion::name)
-    .def_readwrite("value_type", &lincs::Problem::Criterion::value_type)
-    .def_readwrite("category_correlation", &lincs::Problem::Criterion::category_correlation)
+  auto criterion_class = bp::class_<lincs::Criterion>("Criterion", bp::init<std::string, lincs::Criterion::ValueType, lincs::Criterion::CategoryCorrelation>())
+    .def_readwrite("name", &lincs::Criterion::name)
+    .def_readwrite("value_type", &lincs::Criterion::value_type)
+    .def_readwrite("category_correlation", &lincs::Criterion::category_correlation)
   ;
+  // Note that nested things are at global scope as well. This is not wanted, not used, but doesn't hurt
+  // because 'liblincs' is only partially imported into module 'lincs' (see '__init__.py').
+  criterion_class.attr("ValueType") = auto_enum<lincs::Criterion::ValueType>("ValueType");
+  criterion_class.attr("CategoryCorrelation") = auto_enum<lincs::Criterion::CategoryCorrelation>("CategoryCorrelation");
 
-  bp::class_<lincs::Problem::Category>("Category", bp::init<std::string>())
-    .def_readwrite("name", &lincs::Problem::Category::name)
+  bp::class_<lincs::Category>("Category", bp::init<std::string>())
+    .def_readwrite("name", &lincs::Category::name)
   ;
 
-  bp::class_<std::vector<lincs::Problem::Category>>("categories_vector")
-    .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Category>>())
+  bp::class_<std::vector<lincs::Category>>("categories_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Category>>())
   ;
-  bp::class_<std::vector<lincs::Problem::Criterion>>("criteria_vector")
-    .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Criterion>>())
+  bp::class_<std::vector<lincs::Criterion>>("criteria_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Criterion>>())
   ;
 
-  bp::scope().attr("PROBLEM_JSON_SCHEMA") = lincs::Problem::json_schema;
-  bp::class_<lincs::Problem>("Problem", bp::init<std::vector<lincs::Problem::Criterion>, std::vector<lincs::Problem::Category>>())
+  auto problem_class = bp::class_<lincs::Problem>("Problem", bp::init<std::vector<lincs::Criterion>, std::vector<lincs::Category>>())
     .def_readwrite("criteria", &lincs::Problem::criteria)
     .def_readwrite("categories", &lincs::Problem::categories)
     .def(
       "dump",
       &dump_problem,
       (bp::arg("self"), "out"),
       "Dump the problem to the provided `.write()`-supporting file-like object, in YAML format."
     )
+    .def(
+      "load",
+      &load_problem,
+      (bp::arg("in")),
+      "Load a problem from the provided `.read()`-supporting file-like object, in YAML format."
+    )
+    .staticmethod("load")
   ;
-  // @todo Make these 'staticmethod's of Alternatives. Same for other load and generate functions.
+  problem_class.attr("JSON_SCHEMA") = lincs::Problem::json_schema;
   bp::def(
-    "load_problem",
-    &load_problem,
-    (bp::arg("in")),
-    "Load a problem from the provided `.read()`-supporting file-like object, in YAML format."
-  );
-  bp::def(
-    "generate_problem",
-    &lincs::generate_problem,
+    "generate_classification_problem",
+    &lincs::generate_classification_problem,
     (bp::arg("criteria_count"), "categories_count", "random_seed"),
     "Generate a problem with `criteria_count` criteria and `categories_count` categories."
   );
 
-  bp::class_<lincs::Model::SufficientCoalitions>("SufficientCoalitions", bp::init<lincs::Model::SufficientCoalitions::Kind, std::vector<float>>())
-    .def_readwrite("kind", &lincs::Model::SufficientCoalitions::kind)
-    .def_readwrite("criterion_weights", &lincs::Model::SufficientCoalitions::criterion_weights)
-  ;
+  // @todo Double-check why we need both an enum 'Kind' and two tag classes 'Weights' and 'Roots'; simplify or document
+  bp::class_<lincs::SufficientCoalitions::Weights>("Weights", bp::no_init);
+  bp::class_<lincs::SufficientCoalitions::Roots>("Roots", bp::no_init);
+  auto sufficient_coalitions_class = bp::class_<lincs::SufficientCoalitions>("SufficientCoalitions", bp::no_init)
+    .def(bp::init<lincs::SufficientCoalitions::Weights, std::vector<float>>())
+    .def(bp::init<lincs::SufficientCoalitions::Roots, unsigned, std::vector<std::vector<unsigned>>>())
+    .def_readwrite("kind", &lincs::SufficientCoalitions::kind)
+    .def_readwrite("criterion_weights", &lincs::SufficientCoalitions::criterion_weights)
+  ;
+  sufficient_coalitions_class.attr("Kind") = auto_enum<lincs::SufficientCoalitions::Kind>("Kind");
+  sufficient_coalitions_class.attr("weights") = lincs::SufficientCoalitions::weights;
+  sufficient_coalitions_class.attr("roots") = lincs::SufficientCoalitions::roots;
 
   bp::class_<std::vector<float>>("floats_vector")
     .def(bp::vector_indexing_suite<std::vector<float>>())
   ;
-  bp::class_<lincs::Model::Boundary>("Boundary", bp::init<std::vector<float>, lincs::Model::SufficientCoalitions>())
-    .def_readwrite("profile", &lincs::Model::Boundary::profile)
-    .def_readwrite("sufficient_coalitions", &lincs::Model::Boundary::sufficient_coalitions)
-  ;
-  bp::class_<std::vector<lincs::Model::Boundary>>("boundaries_vector")
-    .def(bp::vector_indexing_suite<std::vector<lincs::Model::Boundary>>())
-  ;
-  bp::scope().attr("MODEL_JSON_SCHEMA") = lincs::Model::json_schema;
-  bp::class_<lincs::Model>("Model", bp::init<const lincs::Problem&, const std::vector<lincs::Model::Boundary>&>())
+  auto model_class = bp::class_<lincs::Model>("Model", bp::init<const lincs::Problem&, const std::vector<lincs::Model::Boundary>&>())
     .def_readwrite("boundaries", &lincs::Model::boundaries)
     .def(
       "dump",
       &dump_model,
-      (bp::arg("self"), "out"),
+      (bp::arg("self"), "problem", "out"),
       "Dump the model to the provided `.write()`-supporting file-like object, in YAML format."
     )
+    .def(
+      "load",
+      &load_model,
+      (bp::arg("problem"), "in"),
+      "Load a model for the provided `problem`, from the provided `.read()`-supporting file-like object, in YAML format."
+    )
+    .staticmethod("load")
+  ;
+  model_class.attr("JSON_SCHEMA") = lincs::Model::json_schema;
+  model_class.attr("Boundary") = bp::class_<lincs::Model::Boundary>("Boundary", bp::init<std::vector<float>, lincs::SufficientCoalitions>())
+    .def_readwrite("profile", &lincs::Model::Boundary::profile)
+    .def_readwrite("sufficient_coalitions", &lincs::Model::Boundary::sufficient_coalitions)
+  ;
+  bp::class_<std::vector<lincs::Model::Boundary>>("boundaries_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Model::Boundary>>())
   ;
   bp::def(
-    "load_model",
-    &load_model,
-    (bp::arg("problem"), "in"),
-    "Load a model for the provided `problem`, from the provided `.read()`-supporting file-like object, in YAML format."
-  );
-  bp::def(
-    "generate_mrsort_model",
-    &lincs::generate_mrsort_model,
+    "generate_mrsort_classification_model",
+    &lincs::generate_mrsort_classification_model,
     (bp::arg("problem"), "random_seed", bp::arg("fixed_weights_sum")=std::optional<float>()),
     "Generate an MR-Sort model for the provided `problem`."
   );
 
   bp::class_<lincs::Alternative>(
     "Alternative",
-    bp::init<std::string, std::vector<float>, std::optional<std::string>>(
-      (bp::arg("name"), "profile", (bp::arg("category")=std::optional<std::string>()))
+    bp::init<std::string, std::vector<float>, std::optional<unsigned>>(
+      (bp::arg("name"), "profile", (bp::arg("category")=std::optional<unsigned>()))
     )
   )
     .def_readwrite("name", &lincs::Alternative::name)
     .def_readwrite("profile", &lincs::Alternative::profile)
-    .add_property("category", &get_alternative_category, &set_alternative_category)
+    .add_property("category_index", &get_alternative_category_index, &set_alternative_category_index)
   ;
   bp::class_<std::vector<lincs::Alternative>>("alternatives_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Alternative>>())
   ;
   bp::class_<lincs::Alternatives>("Alternatives", bp::init<const lincs::Problem&, const std::vector<lincs::Alternative>&>())
     .def_readwrite("alternatives", &lincs::Alternatives::alternatives)
     .def(
       "dump",
       &dump_alternatives,
-      (bp::arg("self"), "out"),
+      (bp::arg("self"), "problem", "out"),
       "Dump the set of alternatives to the provided `.write()`-supporting file-like object, in CSV format."
     )
+    .def(
+      "load",
+      &load_alternatives,
+      (bp::arg("problem"), "in"),
+      "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
+    )
+    .staticmethod("load")
   ;
   bp::def(
-    "load_alternatives",
-    &load_alternatives,
-    (bp::arg("problem"), "in"),
-    "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
-  );
-  bp::def(
-    "generate_alternatives",
-    &lincs::generate_alternatives,
+    "generate_classified_alternatives",
+    &lincs::generate_classified_alternatives,
     (bp::arg("problem"), "model", "alternatives_count", "random_seed", bp::arg("max_imbalance")=std::optional<float>()),
     "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `problem`, classified according to the provided `model`."
   );
+  bp::def(
+    "misclassify_alternatives",
+    &lincs::misclassify_alternatives,
+    (bp::arg("problem"), "alternatives", "count", "random_seed"),
+    "Misclassify `count` alternatives from the provided `alternatives`."
+  );
 
   bp::class_<lincs::ClassificationResult>("ClassificationResult", bp::no_init)
     .def_readonly("changed", &lincs::ClassificationResult::changed)
     .def_readonly("unchanged", &lincs::ClassificationResult::unchanged)
   ;
   bp::def(
     "classify_alternatives",
     &lincs::classify_alternatives,
     (bp::arg("problem"), "model", "alternatives"),
     "Classify the provided `alternatives` according to the provided `model`."
   );
 
-  bp::class_<lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy, boost::noncopyable>("ProfilesInitializationStrategy", bp::no_init)
-    .def("initialize_profiles", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy::initialize_profiles));
+  auto learn_wbp_class = bp::class_<lincs::LearnMrsortByWeightsProfilesBreed>("LearnMrsortByWeightsProfilesBreed", bp::no_init)
+    .def(bp::init<
+      lincs::LearnMrsortByWeightsProfilesBreed::LearningData&,
+      lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy&
+    >(
+      (
+        bp::arg("learning_data"),
+        "profiles_initialization_strategy",
+        "weights_optimization_strategy",
+        "profiles_improvement_strategy",
+        "breeding_strategy",
+        "termination_strategy"
+      )
+    ))
+    .def(bp::init<
+      lincs::LearnMrsortByWeightsProfilesBreed::LearningData&,
+      lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy&,
+      lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy&,
+      std::vector<lincs::LearnMrsortByWeightsProfilesBreed::Observer*>
+    >(
+      (
+        bp::arg("learning_data"),
+        "profiles_initialization_strategy",
+        "weights_optimization_strategy",
+        "profiles_improvement_strategy",
+        "breeding_strategy",
+        "termination_strategy",
+        "observers"
+      )
+    ))
+    .def("perform", &lincs::LearnMrsortByWeightsProfilesBreed::perform)
+  ;
+
+  learn_wbp_class.attr("LearningData") = bp::class_<lincs::LearnMrsortByWeightsProfilesBreed::LearningData, boost::noncopyable>("LearningData", bp::no_init)
+    .def("make", &make_learning_data, bp::return_value_policy<bp::manage_new_object>()).staticmethod("make")
+    // @todo Expose all attributes to allow non-trivial Python strategies and observers
+    .def("get_best_accuracy", &lincs::LearnMrsortByWeightsProfilesBreed::LearningData::get_best_accuracy)
+  ;
+
+  struct ProfilesInitializationStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy> {
+    void initialize_profiles(const unsigned begin, const unsigned end) override { this->get_override("initialize_profiles")(begin, end); }
+  };
+
+  learn_wbp_class.attr("ProfilesInitializationStrategy") = bp::class_<ProfilesInitializationStrategyWrap, boost::noncopyable>("ProfilesInitializationStrategy")
+    .def("initialize_profiles", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy::initialize_profiles))
+  ;
 
   bp::class_<
     lincs::InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion,
-    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy>
+    bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy>
   >(
     "InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion",
-    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
-    .def("initialize_profiles", &lincs::InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::initialize_profiles);
+    .def("initialize_profiles", &lincs::InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion::initialize_profiles)
+  ;
 
-  bp::class_<lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy, boost::noncopyable>("WeightsOptimizationStrategy", bp::no_init)
-    .def("optimize_weights", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy::optimize_weights));
+  struct WeightsOptimizationStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy> {
+    void optimize_weights() override { this->get_override("optimize_weights")(); }
+  };
+
+  learn_wbp_class.attr("WeightsOptimizationStrategy") = bp::class_<WeightsOptimizationStrategyWrap, boost::noncopyable>("WeightsOptimizationStrategy")
+    .def("optimize_weights", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy::optimize_weights))
+  ;
 
   bp::class_<
     lincs::OptimizeWeightsUsingGlop,
-    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy>
+    bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy>
   >(
     "OptimizeWeightsUsingGlop",
-    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
-    .def("optimize_weights", &lincs::OptimizeWeightsUsingGlop::optimize_weights);
+    .def("optimize_weights", &lincs::OptimizeWeightsUsingGlop::optimize_weights)
+  ;
 
   bp::class_<
     lincs::OptimizeWeightsUsingAlglib,
-    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy>
+    bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::WeightsOptimizationStrategy>
   >(
     "OptimizeWeightsUsingAlglib",
-    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
-    .def("optimize_weights", &lincs::OptimizeWeightsUsingAlglib::optimize_weights);
+    .def("optimize_weights", &lincs::OptimizeWeightsUsingAlglib::optimize_weights)
+  ;
 
-  bp::class_<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy, boost::noncopyable>("ProfilesImprovementStrategy", bp::no_init)
-    .def("improve_profiles", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy::improve_profiles));
+  struct ProfilesImprovementStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy> {
+    void improve_profiles() override { this->get_override("improve_profiles")(); }
+  };
+
+  learn_wbp_class.attr("ProfilesImprovementStrategy") = bp::class_<ProfilesImprovementStrategyWrap, boost::noncopyable>("ProfilesImprovementStrategy")
+    .def("improve_profiles", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy::improve_profiles))
+  ;
 
   bp::class_<
     lincs::ImproveProfilesWithAccuracyHeuristicOnCpu,
-    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy>
+    bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy>
   >(
     "ImproveProfilesWithAccuracyHeuristicOnCpu",
-    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
-    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles);
+    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles)
+  ;
 
   bp::class_<
     lincs::ImproveProfilesWithAccuracyHeuristicOnGpu,
-    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy>
+    bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::ProfilesImprovementStrategy>,
+    boost::noncopyable
   >(
     "ImproveProfilesWithAccuracyHeuristicOnGpu",
-    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&, lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels&>()
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&>()
   )
-    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles);
+    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles)
+  ;
 
-  struct TerminationStrategyWrap : lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy, bp::wrapper<lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy> {
-    bool terminate(unsigned iteration_index, unsigned best_accuracy) override {
-      return this->get_override("terminate")(iteration_index, best_accuracy);
-    }
+  struct BreedingStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy> {
+    void breed() override { this->get_override("breed")(); }
   };
 
-  bp::class_<TerminationStrategyWrap, boost::noncopyable>("TerminationStrategy")
-    .def("terminate", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy::terminate));
+  learn_wbp_class.attr("BreedingStrategy") = bp::class_<BreedingStrategyWrap, boost::noncopyable>("BreedingStrategy")
+    .def("breed", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy::breed))
+  ;
 
-  bp::class_<lincs::TerminateAtAccuracy, bp::bases<lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy>>("TerminateAtAccuracy", bp::init<unsigned>())
-    .def("terminate", &lincs::TerminateAtAccuracy::terminate);
+  bp::class_<lincs::ReinitializeLeastAccurate, bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::BreedingStrategy>>(
+    "ReinitializeLeastAccurate",
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&, lincs::LearnMrsortByWeightsProfilesBreed::ProfilesInitializationStrategy&, unsigned>()
+  )
+    .def("breed", &lincs::ReinitializeLeastAccurate::breed)
+  ;
+
+  struct TerminationStrategyWrap : lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy> {
+    bool terminate() override { return this->get_override("terminate")(); }
+  };
 
-  bp::class_<lincs::WeightsProfilesBreedMrSortLearning::Models, boost::noncopyable>("Models", bp::no_init);
-  bp::def("make_models", &make_models, bp::return_value_policy<bp::manage_new_object>());
+  learn_wbp_class.attr("TerminationStrategy") = bp::class_<TerminationStrategyWrap, boost::noncopyable>("TerminationStrategy")
+    .def("terminate", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy::terminate))
+  ;
 
-  bp::class_<lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels, boost::noncopyable>("GpuModels", bp::no_init);
-  bp::def("make_gpu_models", &make_gpu_models, bp::return_value_policy<bp::manage_new_object>());
-
-  bp::class_<lincs::WeightsProfilesBreedMrSortLearning>(
-    "WeightsProfilesBreedMrSortLearning",
-    bp::init<
-      lincs::WeightsProfilesBreedMrSortLearning::Models&,
-      lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy&,
-      lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy&,
-      lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy&,
-      lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy&
-    >()
+  bp::class_<lincs::TerminateAtAccuracy, bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy>>(
+    "TerminateAtAccuracy",
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&, unsigned>()
   )
-    .def("perform", &lincs::WeightsProfilesBreedMrSortLearning::perform)
+    .def("terminate", &lincs::TerminateAtAccuracy::terminate)
+  ;
+
+  bp::class_<lincs::TerminateAfterIterations, bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy>>(
+    "TerminateAfterIterations",
+    bp::init<lincs::LearnMrsortByWeightsProfilesBreed::LearningData&, unsigned>()
+  )
+    .def("terminate", &lincs::TerminateAfterIterations::terminate)
+  ;
+
+  bp::class_<lincs::TerminateAfterSeconds, bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy>>(
+    "TerminateAfterSeconds",
+    bp::init<float>()
+  )
+    .def("terminate", &lincs::TerminateAfterSeconds::terminate)
+  ;
+
+  bp::class_<lincs::TerminateWhenAny, bp::bases<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy>>(
+    "TerminateWhenAny",
+    bp::init<std::vector<lincs::LearnMrsortByWeightsProfilesBreed::TerminationStrategy*>>()
+  )
+    .def("terminate", &lincs::TerminateWhenAny::terminate)
+  ;
+
+  struct ObserverWrap : lincs::LearnMrsortByWeightsProfilesBreed::Observer, bp::wrapper<lincs::LearnMrsortByWeightsProfilesBreed::Observer> {
+    void after_iteration() override { this->get_override("after_iteration")(); }
+  };
+
+  learn_wbp_class.attr("Observer") = bp::class_<ObserverWrap, boost::noncopyable>("Observer")
+    .def("after_iteration", bp::pure_virtual(&lincs::LearnMrsortByWeightsProfilesBreed::Observer::after_iteration))
+  ;
+
+
+  bp::class_<lincs::LearnUcncsBySatByCoalitionsUsingMinisat>("LearnUcncsBySatByCoalitionsUsingMinisat", bp::init<const lincs::Problem&, const lincs::Alternatives&>())
+    .def("perform", &lincs::LearnUcncsBySatByCoalitionsUsingMinisat::perform)
+  ;
+
+  bp::class_<lincs::LearnUcncsBySatByCoalitionsUsingEvalmaxsat>("LearnUcncsBySatByCoalitionsUsingEvalmaxsat", bp::init<const lincs::Problem&, const lincs::Alternatives&>())
+    .def("perform", &lincs::LearnUcncsBySatByCoalitionsUsingEvalmaxsat::perform)
   ;
 }
```

### Comparing `lincs-0.4.5/lincs/liblincs/linear-programming/alglib.hpp` & `lincs-0.5.0/lincs/liblincs/linear-programming/alglib.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #ifndef LINCS__LINEAR_PROGRAMMING__ALGLIB_HPP
 #define LINCS__LINEAR_PROGRAMMING__ALGLIB_HPP
 
 #include <cassert>
 #include <map>
 
-#include <alglib/optimization.h>
+#include "../vendored/alglib/optimization.h"
 
 
 namespace lincs {
 
 class AlglibLinearProgram {
  public:
   AlglibLinearProgram() : next_variable_index(0), objective_coefficients(), state() {}
```

### Comparing `lincs-0.4.5/lincs/liblincs/linear-programming/glop.hpp` & `lincs-0.5.0/lincs/liblincs/linear-programming/glop.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 // Copyright 2023 Vincent Jacques
 
 #ifndef LINCS__LINEAR_PROGRAMMING__GLOP_HPP
 #define LINCS__LINEAR_PROGRAMMING__GLOP_HPP
 
 #include <ortools/glop/lp_solver.h>
+#undef CHECK
+#undef CHECK_EQ
+#undef CHECK_NE
+#undef CHECK_LT
+#undef CHECK_GT
+#undef CHECK_LE
+#undef CHECK_GE
+#undef LOG
 
 
 namespace lincs {
 
 class GlopLinearProgram {
  public:
   typedef operations_research::glop::ColIndex variable_type;
```

### Comparing `lincs-0.4.5/lincs/liblincs/linear-programming/test.cpp` & `lincs-0.5.0/lincs/liblincs/linear-programming/test.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2023 Vincent Jacques
 
 #include <limits>
 
 #include "alglib.hpp"
 #include "glop.hpp"
 
-#include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
+#include "../vendored/doctest.h"  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 template<typename LinearProgram>
 void test_linear_program() {
   const float infinity = std::numeric_limits<float>::infinity();
 
   LinearProgram lp;
```

### Comparing `lincs-0.4.5/lincs/liblincs/randomness-utils.cpp` & `lincs-0.5.0/lincs/liblincs/randomness-utils.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // Copyright 2023 Vincent Jacques
 
 #include "randomness-utils.hpp"
 
-#include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
+#include "vendored/doctest.h"  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 TEST_CASE("ProbabilityWeightedGenerator") {
   std::map<std::string, double> value_probabilities = {
     {"a", 0.1},
     {"b", 0.2},
     {"c", 0.3},
```

### Comparing `lincs-0.4.5/lincs/liblincs/randomness-utils.hpp` & `lincs-0.5.0/lincs/liblincs/randomness-utils.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.4.5/lincs/visualization.py` & `lincs-0.5.0/lincs/visualization.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,20 +15,17 @@
     collections = ax.stackplot(
         xs, unstacked_ys,
         labels=[category.name for category in problem.categories],
         alpha=0.4,
     )
     colors = [collection.get_facecolor() for collection in collections]
 
-    # @todo Rethink class Alternative to also expose its assigned category *index*, not just category name
-    category_indexes = {category.name: index for index, category in enumerate(problem.categories)}
-
     if alternatives:
         for alternative in alternatives.alternatives[:alternatives_count]:
-            color = colors[category_indexes[alternative.category]]
+            color = colors[alternative.category_index]
             ax.plot(
                 xs, list(alternative.profile),
                 "o--",
                 label=alternative.name,
                 color=color,
                 alpha=1,
             )
```

### Comparing `lincs-0.4.5/lincs.egg-info/PKG-INFO` & `lincs-0.5.0/lincs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.4.5
+Version: 0.5.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -23,17 +23,17 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python (3.7+) package and a command-line utility.
 
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.5/COPYING.LESSER>`_.
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.5.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
 *lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
 Its `documentation <http://mics-lab.github.io/lincs/>`_
 and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
```

### Comparing `lincs-0.4.5/setup.py` & `lincs-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright 2023 Vincent Jacques
 
 import glob
+import itertools
 import os
+import sys
 import setuptools
 import setuptools.command.build_ext
 
 
-version = "0.4.5"
+version = "0.5.0"
 
 with open("README.rst") as f:
     long_description = f.read()
 for file in ["COPYING", "COPYING.LESSER"]:
     long_description = long_description.replace(f" <{file}>`_", f" <https://github.com/MICS-Lab/lincs/blob/v{version}/{file}>`_")
 for lang in ["yaml", "shell", "text", "diff"]:
     long_description = long_description.replace(f".. highlight:: {lang}", "")
@@ -32,14 +34,16 @@
 
     def _compile(obj, src, ext, cc_args, extra_postargs, pp_opts):
         if os.path.splitext(src)[1] == ".cu":
             self.set_executable("compiler_so", "nvcc")
             postargs = extra_postargs["nvcc"]
         else:
             postargs = extra_postargs["gcc"]
+        if "/vendored/" in src:
+            postargs = postargs + ["-w"]
 
         default_compile(obj, src, ext, cc_args, postargs, pp_opts)
         self.compiler_so = default_compiler_so
 
     self._compile = _compile
 
 
@@ -47,32 +51,35 @@
     def build_extensions(self):
         customize_compiler_for_nvcc(self.compiler)
         setuptools.command.build_ext.build_ext.build_extensions(self)
 
 
 liblincs = setuptools.Extension(
     "liblincs",
-    sources=glob.glob("lincs/liblincs/**/*.cpp", recursive=True) + glob.glob("lincs/liblincs/**/*.cu", recursive=True),
+    sources=list(itertools.chain.from_iterable(
+        glob.glob(f"lincs/liblincs/**/*.{ext}", recursive=True)
+        for ext in ["c", "cc", "cpp", "cu"]
+    )),
     libraries=[
-        "boost_python310",
+        f"boost_python{sys.version_info.major}{sys.version_info.minor}",
         "ortools",
-        "python3.10",  # Make the Python module usable as a C++ shared library without -lpython3.10 (still linked, but implicitly)
+        f"python{sys.version_info.major}.{sys.version_info.minor}{'m' if sys.hexversion < 0x03080000 else ''}",  # Weirdly required because of BoostPython
         "yaml-cpp",
         "cudart",
-        "alglib",
     ],
     define_macros=[("DOCTEST_CONFIG_DISABLE", None)],
+    # @todo Support building without CUDA (required on macOS)
+    # @todo Support several versions of CUDA?
     include_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/include"],
     library_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/lib"],
-    # runtime_library_dirs=["/usr/local/cuda-12.1/targets/x86_64-linux/lib"],
     # Non-standard: the dict is accessed in `customize_compiler_for_nvcc`
     # to get the standard form for `extra_compile_args`
     extra_compile_args={
-        "gcc": ["-fopenmp"],
-        "nvcc": ["-Xcompiler", "-fopenmp,-fPIC"],
+        "gcc": ["-std=c++17", "-fopenmp", "-Werror=switch"],
+        "nvcc": ["-std=c++17", "-Xcompiler", "-fopenmp,-fPIC,-Werror=switch"],
     },
     extra_link_args=["-fopenmp"],
 )
 
 setuptools.setup(
     name="lincs",
     version=version,
```

