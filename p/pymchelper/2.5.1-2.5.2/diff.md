# Comparing `tmp/pymchelper-2.5.1.tar.gz` & `tmp/pymchelper-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymchelper-2.5.1.tar", last modified: Fri Jun 23 13:19:40 2023, max compression
+gzip compressed data, was "pymchelper-2.5.2.tar", last modified: Thu Jul  6 17:07:32 2023, max compression
```

## Comparing `pymchelper-2.5.1.tar` & `pymchelper-2.5.2.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-23 13:19:08.000000 pymchelper-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-23 13:19:40.740245 pymchelper-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-23 13:19:08.000000 pymchelper-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/executor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/
--rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/bmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/csg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/common/rexx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/flair/db/
--rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/card.db
--rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/card.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/flair/db/db2ini.r
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/fluka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/readers/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/binary_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2016.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bin2010.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/shieldhit/detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/fortran_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/detector/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/shieldhit/particle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/mcscripter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/utils/radiotherapy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/radiotherapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/radiotherapy/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/utils/runmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.740245 pymchelper-2.5.1/pymchelper/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/fortranformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/mcpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/shieldhit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/trip98cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/trip98ddd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-23 13:19:09.000000 pymchelper-2.5.1/pymchelper/writers/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:19:40.736245 pymchelper-2.5.1/pymchelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 13:19:40.000000 pymchelper-2.5.1/pymchelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-23 13:19:40.740245 pymchelper-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-23 13:19:09.000000 pymchelper-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.506768 pymchelper-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 17:07:00.000000 pymchelper-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-06 17:07:32.506768 pymchelper-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-06 17:07:00.000000 pymchelper-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.498767 pymchelper-2.5.2/pymchelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.498767 pymchelper-2.5.2/pymchelper/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/executor/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/executor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.498767 pymchelper-2.5.2/pymchelper/flair/
+-rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.498767 pymchelper-2.5.2/pymchelper/flair/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/bmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/csg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/common/rexx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/flair/db/
+-rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/db/card.db
+-rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/db/card.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/flair/db/db2ini.r
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6631 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/fluka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/readers/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14649 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/binary_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bdo2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bdo2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bin2010.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/readers/topas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/shieldhit/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/estimator_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/fortran_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/detector/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/shieldhit/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/simulator_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/utils/mcscripter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.502767 pymchelper-2.5.2/pymchelper/utils/radiotherapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/utils/radiotherapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/utils/radiotherapy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/utils/runmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.506768 pymchelper-2.5.2/pymchelper/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/fortranformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/mcpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/shieldhit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/trip98cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/trip98ddd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-06 17:07:00.000000 pymchelper-2.5.2/pymchelper/writers/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:07:32.498767 pymchelper-2.5.2/pymchelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 17:07:32.000000 pymchelper-2.5.2/pymchelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 17:07:32.506768 pymchelper-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-06 17:07:00.000000 pymchelper-2.5.2/setup.py
```

### Comparing `pymchelper-2.5.1/PKG-INFO` & `pymchelper-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.5.1/README.md` & `pymchelper-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/__init__.py` & `pymchelper-2.5.2/pymchelper/__init__.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/axis.py` & `pymchelper-2.5.2/pymchelper/axis.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/estimator.py` & `pymchelper-2.5.2/pymchelper/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/executor/options.py` & `pymchelper-2.5.2/pymchelper/executor/options.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import logging
 import os
+from pathlib import Path
 import sys
+from typing import Optional
+
+from pymchelper.simulator_type import SimulatorType
 
 
 class MCEnvironment:
     """
     `MCEnvironment` subclasses are helpful to discover which MC engine (i.e. FLUKA or SHIELD-HIT12A) is being used
     they provide information about expected executable filename, by inspecting the path to executable filename
     (i.e. checking if it ends with `rfluka`) we can find corresponding code type
@@ -13,47 +17,75 @@
 
 
 class FlukaEnvironment(MCEnvironment):
     """
     FLUKA Environment
     """
     executable_filename = 'rfluka'
+    simulator_type = SimulatorType.fluka
 
 
 class SH12AEnvironmentLinux(MCEnvironment):
     """
     SHIELD-HIT12A Environment for Linux
     """
     executable_filename = 'shieldhit'
+    simulator_type = SimulatorType.shieldhit
 
 
 class SH12AEnvironmentWindows(MCEnvironment):
     """
     SHIELD-HIT12A Environment for Windows
     """
     executable_filename = 'shieldhit.exe'
+    simulator_type = SimulatorType.shieldhit
+
+
+class TopasEnvironment(MCEnvironment):
+    """TOPAS Environment"""
+
+    executable_filename = 'topas'
+    simulator_type = SimulatorType.topas
 
 
 class SimulationSettings:
     """
     This class is responsible for keeping track of options for MC simulation:
       - location of the MC simulator executable
       - additional options provided by the user
       - location of the input files or directories
     Moreover this class performs automatic discovery of the MC input
-    (i.e. whether this is SHIELD-HIT12A input or FLUKA input)
+    (i.e. whether this is SHIELD-HIT12A, Fluka or TOPAS input)
     """
 
-    def __init__(self, input_path, simulator_exec_path=None, cmdline_opts=None):
-        # input file or directory
+    def __init__(self, input_path: str, simulator_type: Optional[SimulatorType]=None,
+                 simulator_exec_path: str=None, cmdline_opts: str=None):
+        # Input file or directory
         self.input_path = input_path
 
-        # discover the type of MC engine based on the type of input files/directories
-        # `self._mc_environment` is set to one of the `MCEnvironment` subclasses
-        self._mc_environment = self._discover_mc_engine(input_path)
+        # Set `self._mc_environment` to the proper `MCEnvironment` subclass
+        # If `simulator_type` is provided by user, then we use it to set proper `MCEnvironment` subclass
+        # Otherwise, we try to guess based on provided input path
+        if simulator_type:
+            if simulator_type == SimulatorType.shieldhit:
+                if sys.platform == 'win32':
+                    self._mc_environment = SH12AEnvironmentWindows
+                else:
+                    self._mc_environment = SH12AEnvironmentLinux
+            elif simulator_type == SimulatorType.fluka:
+                self._mc_environment = FlukaEnvironment
+            elif simulator_type == SimulatorType.topas:
+                self._mc_environment = TopasEnvironment
+        else:
+            self._mc_environment = self._discover_mc_engine(input_path)
+
+        if not self._mc_environment:
+            raise Exception(f"Unable to determine MC engine type for {input_path}")
+
+        self.simulator_type = self._mc_environment.simulator_type
 
         # set `self.executable_path` to the value provided by user, or if it is missing
         # perform automatic discovery of the *location* of MC engine executable file by scanning PATH env. variable
         self.executable_path = simulator_exec_path
         if not self.executable_path:
             self.executable_path = self._discover_mc_exec_location(self._mc_environment.executable_filename)
 
@@ -118,36 +150,40 @@
         unsupported = {'-b', '--beamfile', '-g', '--geofile', '-m', '--matfile', '-d', '--detectfile'}
         # raise an error if some of the unsupported option was provided by user (i.e. via -m option to `runmc` command)
         if options_set & unsupported:
             # TODO replace exception with warning and ignore such options  # skipcq: PYL-W0511
             raise SyntaxError("Unsupported option encountered: {:s}".format(",".join(options_set & unsupported)))
 
     @staticmethod
-    def _discover_mc_engine(input_path):
+    def _discover_mc_engine(input_path_str: str):
         """
         Analyse the input path and based on its type set proper MC engine
         In case of failure return None
         """
-
+        input_path = Path(input_path_str)
         # raise exception if invalid path is provided
-        if not os.path.exists(input_path):
+        if not input_path.exists():
             raise Exception("Input path {:s} doesn't exists".format(input_path))
 
-        # Fluka input files are provided as the single file
-        # TODO cross-check if the `*.inp` extension is needed  # skipcq: PYL-W0511
-        if os.path.isfile(input_path):
-            return FlukaEnvironment
+        # Fluka and TOPAS input files are provided as the single file
+        # We return proper MC engine based on the file extension
+        if input_path.is_file():
+            if input_path_str.endswith('.inp'):
+                return FlukaEnvironment
+            if input_path_str.endswith('.txt'):
+                return TopasEnvironment
         # SHIELD-HIT12A input is in the form of directory with multiple files
-        # TODO add a check if the directory contains (beam.dat, mat.dat, geo.dat and detect.dat)  # skipcq: PYL-W0511
-        if os.path.isdir(input_path):
-            # in case pymchelper runs on Windows choose a SHIELD-HIT12A environment which is Windows specific
-            # (executable file being `shieldhit.exe` instead of `shieldhit`)
-            if sys.platform == 'win32':
-                return SH12AEnvironmentWindows
-            return SH12AEnvironmentLinux
+        elif input_path.is_dir():
+            # We check if directory contains the required SHIELDHIT-12A input files
+            if all(input_path.joinpath(file).exists() for file in ['beam.dat', 'mat.dat', 'geo.dat', 'detect.dat']):
+                # in case pymchelper runs on Windows choose a SHIELDHIT-12A environment which is Windows specific
+                # (executable file being `shieldhit.exe` instead of `shieldhit`)
+                if sys.platform == 'win32':
+                    return SH12AEnvironmentWindows
+                return SH12AEnvironmentLinux
         return None
 
     @staticmethod
     def _discover_mc_exec_location(exec_filename):
         """
         Scans PATH variable for the possible location of the MC engine exec_filename.
         Works on POSIX (Linux and MacOSX) and Windows systems
```

### Comparing `pymchelper-2.5.1/pymchelper/executor/runner.py` & `pymchelper-2.5.2/pymchelper/executor/runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from copy import deepcopy
 import logging
 import os
+from pathlib import Path
+import re
 import shutil
 import subprocess
 import timeit
 from multiprocessing import Pool
 
 from enum import IntEnum
+from pymchelper.executor.options import SimulationSettings
 
-from pymchelper.input_output import frompattern
+from pymchelper.simulator_type import SimulatorType
+from pymchelper.input_output import frompattern, get_topas_estimators
 
 
 class OutputDataType(IntEnum):
     """
     Output type requested by user plots (i.e .png) or text data
     """
     plot = 1
@@ -20,15 +24,17 @@
 
 
 class Runner:
     """
     Main class responsible for configuring and starting multiple parallel MC simulation processes
     It can be used to access combined averaged results of the simulation.
     """
-    def __init__(self, jobs=None, keep_workspace_after_run=False, output_directory='.'):
+    def __init__(self, settings: SimulationSettings, jobs: int=None,
+                 keep_workspace_after_run: bool=False, output_directory: str='.'):
+        self.settings = settings
 
         # create pool of processes, waiting to be started by run method
         # if jobs is not specified, os.cpu_count() would be used
         self._pool = Pool(processes=jobs)
 
         # User of the runner has two options: either to specify number of parallel jobs by
         # setting the self.jobs to given number, or to leave it as None. If self.jobs is None
@@ -41,34 +47,59 @@
         self.jobs = self._pool._processes
 
         # workspace is a collection of working directories
         # this manager is responsible for creating and cleaning working directories
         self.workspace_manager = WorkspaceManager(output_directory=output_directory,
                                                   keep_workspace_after_run=keep_workspace_after_run)
 
-    def run(self, settings):
+    def run(self):
         """
         Execute parallel simulation processes, creating workspace (and working directories) in the `output_directory`
         In case of successful execution return True, otherwise return False
         """
         start_time = timeit.default_timer()
 
-        # SHIELD-HIT12A and Fluka require RNG seeds to be integers greater or equal to 1
-        # each of the workers needs to have its own different RNG seed
-        rng_seeds = range(1, self.jobs + 1)
+        if self.settings.simulator_type in [SimulatorType.shieldhit, SimulatorType.fluka]:
+            # SHIELD-HIT12A and Fluka require RNG seeds to be integers greater or equal to 1
+            # each of the workers needs to have its own different RNG seed
+            rng_seeds = range(1, self.jobs + 1)
+
+        elif self.settings.simulator_type == SimulatorType.topas:
+            # For TOPAS we don't need to create multiple working directories and a pool of workers,
+            # as we can use embedded parallelization in TOPAS.
+            # For that we need to modify the input file and set the number of threads to the number of jobs.
+            # We set one rng seed, so one working directory and one worker will be created.
+
+            modified_input_filename = Path(self.settings.input_path).name.replace(".txt", "_modified.txt")
+            modified_input_path = Path(self.settings.input_path).parent / modified_input_filename
+
+            with open(self.settings.input_path, 'r') as f:
+                config = f.read()
+                if "i:Ts/NumberOfThreads" in config:
+                    pattern = r"i:Ts/NumberOfThreads\s*=\s*\d+"
+                    replacement = f"i:Ts/NumberOfThreads = {self.jobs}"
+                    config = re.sub(pattern, replacement, config)
+                else:
+                    config = f"i:Ts/NumberOfThreads = {self.jobs}\n" + config
+
+            modified_input_path.write_text(config)
+
+            self.settings.input_path = str(modified_input_path)
+
+            rng_seeds = [1]
 
         # create working directories
-        self.workspace_manager.create_working_directories(simulation_input_path=settings.input_path,
+        self.workspace_manager.create_working_directories(simulation_input_path=self.settings.input_path,
                                                           rng_seeds=rng_seeds)
 
         # rng seeds injection to settings for each SingleSimulationExecutor call
         # TODO consider better way of doing it  # skipcq: PYL-W0511
         settings_list = []
         for rng_seed in rng_seeds:
-            current_settings = deepcopy(settings)  # do not modify original arguments
+            current_settings = deepcopy(self.settings)  # do not modify original arguments
             current_settings.set_rng_seed(rng_seed)
             settings_list.append(current_settings)
 
         # create executor callable object for current run
         executor = SingleSimulationExecutor()
 
         try:
@@ -80,34 +111,41 @@
             self._pool.terminate()
             logging.info('Pool is terminated')
             self.workspace_manager.clean()
             return False
 
         elapsed = timeit.default_timer() - start_time
         logging.info("run elapsed time {:.3f} seconds".format(elapsed))
+
         return True
 
     def get_data(self):
         """
         Scans the output directory for location of the working directories (like run_1, run_2).
         Takes all files from all working directories in `output_dir`,
         merges their content to form pymchelper Estimator objects.
         For each of the output file a single Estimator objects is created, which holds numpy arrays with results.
         Return dictionary with keys being output filenames, and values being Estimator objects
         """
         start_time = timeit.default_timer()
 
-        # TODO line below is specific to SHIELD-HIT12A, should be generalised  # skipcq: PYL-W0511
         # scans output directory for MC simulation output files
-        output_files_pattern = os.path.join(self.workspace_manager.output_dir_absolute_path, "run_*", "*.bdo")
-        logging.debug("Files to merge {:s}".format(output_files_pattern))
-
         estimators_dict = {}
-        # convert output files to list of estimator objects
-        estimators_list = frompattern(output_files_pattern)
+        estimators_list = []
+
+        if self.settings.simulator_type == SimulatorType.shieldhit:
+            output_files_pattern = str(Path(self.workspace_manager.output_dir_absolute_path) / "run_*" / "*.bdo")
+            logging.debug("Files to merge %s", output_files_pattern)
+            # convert output files to list of estimator objects
+            estimators_list = frompattern(output_files_pattern)
+
+        elif self.settings.simulator_type == SimulatorType.topas:
+            output_files_path = str(Path(self.workspace_manager.output_dir_absolute_path) / "run_1")
+            estimators_list = get_topas_estimators(output_files_path)
+
         for estimator in estimators_list:
             logging.debug("Appending estimator for {:s}".format(estimator.file_corename))
             estimators_dict[estimator.file_corename] = estimator
         elapsed = timeit.default_timer() - start_time
         logging.info("Workspace reading {:.3f} seconds".format(elapsed))
 
         return estimators_dict
```

### Comparing `pymchelper-2.5.1/pymchelper/flair/Data.py` & `pymchelper-2.5.2/pymchelper/flair/Data.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/Input.py` & `pymchelper-2.5.2/pymchelper/flair/Input.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/common/bmath.py` & `pymchelper-2.5.2/pymchelper/flair/common/bmath.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/common/csg.py` & `pymchelper-2.5.2/pymchelper/flair/common/csg.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/common/fortran.py` & `pymchelper-2.5.2/pymchelper/flair/common/fortran.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/common/log.py` & `pymchelper-2.5.2/pymchelper/flair/common/log.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/common/rexx.py` & `pymchelper-2.5.2/pymchelper/flair/common/rexx.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/db/card.db` & `pymchelper-2.5.2/pymchelper/flair/db/card.db`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/db/card.ini` & `pymchelper-2.5.2/pymchelper/flair/db/card.ini`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/flair/db/db2ini.r` & `pymchelper-2.5.2/pymchelper/flair/db/db2ini.r`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/input_output.py` & `pymchelper-2.5.2/pymchelper/input_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 import os
 from collections import defaultdict
 from glob import glob
-from typing import Optional
+from pathlib import Path
+from typing import List, Optional
 
 import numpy as np
 
 from pymchelper.estimator import ErrorEstimate, Estimator, average_with_nan
+from pymchelper.readers.topas import TopasReaderFactory
 from pymchelper.readers.fluka import FlukaReader, FlukaReaderFactory
 from pymchelper.readers.shieldhit.general import SHReaderFactory
 from pymchelper.readers.shieldhit.reader_base import SHReader
 from pymchelper.writers.common import Converters
 
 logger = logging.getLogger(__name__)
 
@@ -18,21 +20,26 @@
 def guess_reader(filename):
     """
     Guess a reader based on file contents or extensions.
     In some cases (i.e. binary SH12A files) access to file contents is needed.
     :param filename:
     :return: Instantiated reader object
     """
+    reader = None
     fluka_reader = FlukaReaderFactory(filename).get_reader()
     if fluka_reader:
         reader = fluka_reader(filename)
     else:
         sh_reader = SHReaderFactory(filename).get_reader()
         if sh_reader:
             reader = sh_reader(filename)
+        else:
+            topas_reader = TopasReaderFactory(filename).get_reader()
+            if topas_reader:
+                reader = topas_reader(filename)
     return reader
 
 
 def guess_corename(filename):
     """
     Guess a reader based on file contents or extensions.
     In some cases (i.e. binary SH12A files) access to file contents is needed.
@@ -90,26 +97,27 @@
         if error != ErrorEstimate.none:
             for page in result.pages:
                 page.error_raw = np.zeros_like(page.data_raw)
 
         # loop over all files with n running from 2
         for n, filename in enumerate(input_file_list[1:], start=2):
             current_estimator = fromfile(filename)  # x
+            logger.info("Reading file %s (%d/%d)", filename, n, len(input_file_list))
 
             if not current_estimator:
                 logger.warning("File %s could not be read", filename)
                 return None
 
             for current_page, result_page in zip(current_estimator.pages, result.pages):
                 # got a page with "concatenate normalisation"
                 if getattr(current_page, 'page_normalized', 2) == 4:
-                    logger.info("Concatenating page %s", current_page.name)
+                    logger.debug("Concatenating page %s", current_page.name)
                     result_page.data_raw = np.concatenate((result_page.data_raw, current_page.data_raw))
                 else:
-                    logger.info("Averaging page %s", current_page.name)
+                    logger.debug("Averaging page %s", current_page.name)
                     # Running variance algorithm based on algorithm by B. P. Welford,
                     # presented in Donald Knuth's Art of Computer Programming, Vol 2, page 232, 3rd edition.
                     # Can be found here: http://www.johndcook.com/blog/standard_deviation/
                     # and https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Online_algorithm
                     delta = current_page.data_raw - result_page.data_raw  # delta = x - mean
                     result_page.data_raw += delta / np.float64(n)
                     if error != ErrorEstimate.none:
@@ -140,35 +148,49 @@
 
 def frompattern(pattern: str, error: ErrorEstimate = ErrorEstimate.stderr, nan: bool = True):
     """
     Reads all files matching pattern, e.g.: 'foobar_*.bdo', and returns a list of averaged estimators.
 
     :param pattern: pattern to be matched for reading.
     :param error: error estimation, see class ErrorEstimate class in pymchelper.estimator
-    :param nan: if True, NaN (not a number) are excluded when averaing data.
+    :param nan: if True, NaN (not a number) are excluded when averaging data.
     :return: a list of estimators, or an empty list if no files were found.
     """
 
     try:
         list_of_matching_files = glob(pattern)
     except TypeError as e:  # noqa: F841
         list_of_matching_files = pattern
 
     core_names_dict = group_input_files(list_of_matching_files)
 
     result = [fromfilelist(filelist, error, nan) for _, filelist in core_names_dict.items()]
+
     return result
 
 
+def get_topas_estimators(output_files_path: str) -> List[Estimator]:
+    """Get Topas estimators from provided directory"""
+    estimators_list = []
+    for path in Path(output_files_path).iterdir():
+        topas_reader = TopasReaderFactory(str(path)).get_reader()
+        if topas_reader:
+            reader = topas_reader(path)
+            estimator = Estimator()
+            reader.read(estimator)
+            estimators_list.append(estimator)
+
+    return estimators_list
+
+
 def convertfromlist(filelist, error, nan, outputdir, converter_name, options, outputfile=None):
     """
-
     :param filelist:
     :param error: error estimation, see class ErrorEstimate class in pymchelper.estimator
-    :param nan: if True, NaN (not a number) are excluded when averaing data.
+    :param nan: if True, NaN (not a number) are excluded when averaging data.
     :param outputdir:
     :param converter_name:
     :param options:
     :param outputfile:
     :return:
     """
     estimator = fromfilelist(filelist, error, nan)
```

### Comparing `pymchelper-2.5.1/pymchelper/page.py` & `pymchelper-2.5.2/pymchelper/page.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/common.py` & `pymchelper-2.5.2/pymchelper/readers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/fluka.py` & `pymchelper-2.5.2/pymchelper/readers/fluka.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/binary_spec.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/binary_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
     page_diff_start = 0xDDD2  # /* array holding 1 or 2 lower bounds, for 1-D or 2-D respectively */
     page_diff_stop = 0xDDD3  # /* array holding 1 or 2 upper bounds, for 1-D or 2-D respectively */
     page_diff_size = 0xDDD4  # /* array holding 1 or 2 number of bins, for 1-D or 2-D respectively */
     page_diff_units = 0xDDD5  # /* ASCII string of ;-separated units along each dimension. %s;%s;%s where latter
     #          two %s are the differential units, and the first is the data in
     #          non-differential form. */
 
+    phase_space_population = 0xDDE0  # /* number of particles in phase space */
+
     # /* Filter data attached to page */
     page_filter_name = 0xDDF0  # /* name of filter containing one or more rules */
     page_filter_rules_no = 0xDDF1  # /* number of filter rules applied */
     page_filter_e_min = 0xDDF2  # /* lower energy threshold, emin */
     page_filter_emax = 0xDDF3  # /* upper energy threshold, emin */
 
     # Group 0xEE00 - 0xEEFF : Estimator specific tags
@@ -155,35 +157,30 @@
 
     # /* Group 0xFFCC - 0xFFFF : Diagnostics, may be ignored by readers. */
     comment = 0xFFCC  # /* 0xFFCC-omment */
     debug = 0xFFCD  # /* 0xFFCD-ebug */
     error = 0xFFCE  # /* 0xFFCE-rror */
 
 
-estimator_tags_to_save = (
-
-)
+estimator_tags_to_save = ()
 
 page_tags_to_save = (
     SHBDOTagID.detector_type,
     SHBDOTagID.page_number,
     SHBDOTagID.page_normalized,
     SHBDOTagID.page_scale_factor,
     SHBDOTagID.page_offset,
     SHBDOTagID.page_unit_ids,
-
     SHBDOTagID.detector_unit,
-
     SHBDOTagID.page_diff_flag,
     SHBDOTagID.page_diff_type,
     SHBDOTagID.page_diff_start,
     SHBDOTagID.page_diff_stop,
     SHBDOTagID.page_diff_size,
     SHBDOTagID.page_diff_units,
-
     SHBDOTagID.page_filter_name,
     SHBDOTagID.page_filter_rules_no,
     SHBDOTagID.page_filter_e_min,
     SHBDOTagID.page_filter_emax,
 )
 
 # replace this dictionary with tuple estimator_tags_to_save
@@ -277,54 +274,44 @@
 
 unit_name_from_unit_id = {
     SHBDOUnitID.SH_SCORING_UNIT_NONE: "",
     SHBDOUnitID.SH_SCORING_UNIT_AU: "a.u.",
     SHBDOUnitID.SH_SCORING_UNIT_PCT: "%",
     SHBDOUnitID.SH_SCORING_UNIT_PMIL: "%%",
     SHBDOUnitID.SH_SCORING_UNIT_RELATIVE: "rel.units",
-
     SHBDOUnitID.SH_SCORING_UNIT_CM: "cm",
     SHBDOUnitID.SH_SCORING_UNIT_CM2: "cm^2",
     SHBDOUnitID.SH_SCORING_UNIT_CM3: "cm^3",
     SHBDOUnitID.SH_SCORING_UNIT_PCM: "/cm",
     SHBDOUnitID.SH_SCORING_UNIT_PCM2: "/cm^2",
     SHBDOUnitID.SH_SCORING_UNIT_PCM3: "/cm^3",
-
     SHBDOUnitID.SH_SCORING_UNIT_M: "m",
     SHBDOUnitID.SH_SCORING_UNIT_M2: "m^2",
     SHBDOUnitID.SH_SCORING_UNIT_M3: "m^3",
     SHBDOUnitID.SH_SCORING_UNIT_PM: "/m",
     SHBDOUnitID.SH_SCORING_UNIT_PM2: "/m^2",
     SHBDOUnitID.SH_SCORING_UNIT_PM3: "/m^3",
-
     SHBDOUnitID.SH_SCORING_UNIT_GPCM3: "g/cm^3",
     SHBDOUnitID.SH_SCORING_UNIT_KGPM3: "kg/m^3",
-
     SHBDOUnitID.SH_SCORING_UNIT_KEVPUM: "keV/um",
     SHBDOUnitID.SH_SCORING_UNIT_MEVPCM: "MeV/cm",
     SHBDOUnitID.SH_SCORING_UNIT_MEVCM2PG: "MeV cm^2/g",
-
     SHBDOUnitID.SH_SCORING_UNIT_MEVPG: "MeV/g",
     SHBDOUnitID.SH_SCORING_UNIT_GY: "Gy",
     SHBDOUnitID.SH_SCORING_UNIT_GYRBE: "Gy(RBE)",  # /* Probably there are new ICRU rules here */
     SHBDOUnitID.SH_SCORING_UNIT_GYRE: "Gy(RE)",
     SHBDOUnitID.SH_SCORING_UNIT_SV: "Sv",
     SHBDOUnitID.SH_SCORING_UNIT_DOSERAD: "Rad",
     SHBDOUnitID.SH_SCORING_UNIT_DOSEREM: "Rem",
-
     SHBDOUnitID.SH_SCORING_UNIT_DEGREES: "deg",
     SHBDOUnitID.SH_SCORING_UNIT_RADIANS: "rad",
     SHBDOUnitID.SH_SCORING_UNIT_SR: "sr",
-
     SHBDOUnitID.SH_SCORING_UNIT_COUNT: "#",
-
     SHBDOUnitID.SH_SCORING_UNIT_MEV: "MeV",
     SHBDOUnitID.SH_SCORING_UNIT_MEVPNUC: "MeV/nucleon",
     SHBDOUnitID.SH_SCORING_UNIT_MEVPAMU: "MeV/amu",
-
     SHBDOUnitID.SH_SCORING_UNIT_NUCN: "",
     SHBDOUnitID.SH_SCORING_UNIT_MEVPC2: "MeV/c^2",
     SHBDOUnitID.SH_SCORING_UNIT_U: "u",
-
     SHBDOUnitID.SH_SCORING_UNIT_MATID: "",
     SHBDOUnitID.SH_SCORING_UNIT_NZONE: "",
 }
```

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/general.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/general.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_base.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_base.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2016.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bdo2016.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bdo2019.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bdo2019.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/readers/shieldhit/reader_bin2010.py` & `pymchelper-2.5.2/pymchelper/readers/shieldhit/reader_bin2010.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/run.py` & `pymchelper-2.5.2/pymchelper/run.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/shieldhit/detector/detector_type.py` & `pymchelper-2.5.2/pymchelper/shieldhit/detector/detector_type.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/shieldhit/detector/estimator.py` & `pymchelper-2.5.2/pymchelper/shieldhit/detector/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/shieldhit/detector/fortran_card.py` & `pymchelper-2.5.2/pymchelper/shieldhit/detector/fortran_card.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/shieldhit/detector/geometry.py` & `pymchelper-2.5.2/pymchelper/shieldhit/detector/geometry.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/shieldhit/particle.py` & `pymchelper-2.5.2/pymchelper/shieldhit/particle.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/utils/mcscripter.py` & `pymchelper-2.5.2/pymchelper/utils/mcscripter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/utils/radiotherapy/plan.py` & `pymchelper-2.5.2/pymchelper/utils/radiotherapy/plan.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/utils/runmc.py` & `pymchelper-2.5.2/pymchelper/utils/runmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import sys
 import argparse
 import timeit
 
 from pymchelper.executor.options import SimulationSettings
 from pymchelper.executor.runner import OutputDataType, Runner
+from pymchelper.simulator_type import SimulatorType
 from pymchelper.writers.plots import PlotDataWriter, ImageWriter
 
 
 def set_logger_level(args):
     """
     Set logger verbosity and quietness based on parsed arguments
     Checks for presence of quiet (-q) and verbose (-v) switches
@@ -46,14 +47,17 @@
     """
 
     if args is None:
         args = sys.argv[1:]
     import pymchelper
 
     parser = argparse.ArgumentParser()
+    parser.add_argument('-s', '--simulator', help='Simulator type: shieldhit, topas or fluka '
+                                                  '(automatically detected if not provided))',
+                        type=str, choices=[s.name for s in SimulatorType], default=None)
     parser.add_argument('-e', '--executable', help='path to MC executable '
                                                    '(automatically detected if not provided)',
                         type=str, default=None)
     parser.add_argument('-j', '--jobs',
                         help='Number of jobs to run simultaneously (default: {:d})'.format(os.cpu_count()),
                         type=int, default=None)
     parser.add_argument('-m', '--mc-options', help='MC simulation options (default: empty string)',
@@ -98,30 +102,32 @@
 
     # set MC simulation settings based on:
     #   - MC simulation input file (i.e. *.inp file for FLUKA) or
     #     directories (i.e. directory with beam.dat, geo.dat etc for SHIELD-HIT12A)
     #   - location of MC simulator executable file (i.e. `shieldhit` or `rfluka`)
     #   - simulation options for the MC engine provided via -m switch (i.e. --time or -v)
     settings = SimulationSettings(input_path=parsed_args.input,
+                                  simulator_type=parsed_args.simulator,
                                   simulator_exec_path=parsed_args.executable,
                                   cmdline_opts=parsed_simulation_opts)
 
     # create runner object based on MC options and dedicated parallel jobs number
     # note that runner object is only created here, no simulation is started at this point
     # and no directories are being created
-    runner_obj = Runner(jobs=parsed_args.jobs,
+    runner_obj = Runner(settings=settings,
+                        jobs=parsed_args.jobs,
                         keep_workspace_after_run=parsed_args.keep,
                         output_directory=parsed_args.outdir)
 
     # start parallel execution of MC simulation
     # temporary directories needed for parallel execution as well as the output are being saved in `outdir`
     # in case of successful execution this would return list of temporary workspaces directories
     # containing partial results from simultaneous parallel executions
     start_time = timeit.default_timer()
-    runner_obj.run(settings=settings)
+    runner_obj.run()
     elapsed = timeit.default_timer() - start_time
     print("MC simulation took {:.3f} seconds".format(elapsed))
 
     # if simulation was successful proceed to data extraction by combining partial results from simultaneous executions
     # each simulation can produce multiple files
     # results are stored in a dictionary (`data_dict`) with keys being filenames
     # and values being pymchelper `Estimator` objects (which keep i.e. numpy arrays with results)
```

### Comparing `pymchelper-2.5.1/pymchelper/version.py` & `pymchelper-2.5.2/pymchelper/version.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/common.py` & `pymchelper-2.5.2/pymchelper/writers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/excel.py` & `pymchelper-2.5.2/pymchelper/writers/excel.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/fortranformatter.py` & `pymchelper-2.5.2/pymchelper/writers/fortranformatter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/hdf.py` & `pymchelper-2.5.2/pymchelper/writers/hdf.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/inspector.py` & `pymchelper-2.5.2/pymchelper/writers/inspector.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/json.py` & `pymchelper-2.5.2/pymchelper/writers/json.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/plots.py` & `pymchelper-2.5.2/pymchelper/writers/plots.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/shieldhit.py` & `pymchelper-2.5.2/pymchelper/writers/shieldhit.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/sparse.py` & `pymchelper-2.5.2/pymchelper/writers/sparse.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/trip98cube.py` & `pymchelper-2.5.2/pymchelper/writers/trip98cube.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/trip98ddd.py` & `pymchelper-2.5.2/pymchelper/writers/trip98ddd.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper/writers/writer.py` & `pymchelper-2.5.2/pymchelper/writers/writer.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.5.1/pymchelper.egg-info/PKG-INFO` & `pymchelper-2.5.2/pymchelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.5.1
+Version: 2.5.2
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.5.1/pymchelper.egg-info/SOURCES.txt` & `pymchelper-2.5.2/pymchelper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 pymchelper/VERSION
 pymchelper/__init__.py
 pymchelper/axis.py
 pymchelper/estimator.py
 pymchelper/input_output.py
 pymchelper/page.py
 pymchelper/run.py
+pymchelper/simulator_type.py
 pymchelper/version.py
 pymchelper.egg-info/PKG-INFO
 pymchelper.egg-info/SOURCES.txt
 pymchelper.egg-info/dependency_links.txt
 pymchelper.egg-info/entry_points.txt
 pymchelper.egg-info/requires.txt
 pymchelper.egg-info/top_level.txt
@@ -30,14 +31,15 @@
 pymchelper/flair/common/rexx.py
 pymchelper/flair/db/card.db
 pymchelper/flair/db/card.ini
 pymchelper/flair/db/db2ini.r
 pymchelper/readers/__init__.py
 pymchelper/readers/common.py
 pymchelper/readers/fluka.py
+pymchelper/readers/topas.py
 pymchelper/readers/shieldhit/__init__.py
 pymchelper/readers/shieldhit/binary_spec.py
 pymchelper/readers/shieldhit/general.py
 pymchelper/readers/shieldhit/reader_base.py
 pymchelper/readers/shieldhit/reader_bdo2016.py
 pymchelper/readers/shieldhit/reader_bdo2019.py
 pymchelper/readers/shieldhit/reader_bin2010.py
```

### Comparing `pymchelper-2.5.1/pymchelper.egg-info/requires.txt` & `pymchelper-2.5.2/pymchelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 [dicom:python_version == "3.11"]
 pydicom>=2.3.1
 
 [excel]
 xlwt
 
 [full]
-h5py
 xlwt
 matplotlib
+h5py
 scipy
 hipsterplot
 bashplotlib
 
 [full:python_version < "3.11"]
 pydicom
```

### Comparing `pymchelper-2.5.1/setup.py` & `pymchelper-2.5.2/setup.py`

 * *Files identical despite different names*

