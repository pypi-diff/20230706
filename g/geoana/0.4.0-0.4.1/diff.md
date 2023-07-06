# Comparing `tmp/geoana-0.4.0.tar.gz` & `tmp/geoana-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoana-0.4.0.tar", last modified: Wed Oct 26 17:18:32 2022, max compression
+gzip compressed data, was "geoana-0.4.1.tar", last modified: Thu Jul  6 18:53:41 2023, max compression
```

## Comparing `geoana-0.4.0.tar` & `geoana-0.4.1.tar`

### file list

```diff
@@ -1,60 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.383398 geoana-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-26 17:15:30.000000 geoana-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-10-26 17:15:30.000000 geoana-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-10-26 17:18:32.383398 geoana-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-10-26 17:15:30.000000 geoana-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.375397 geoana-0.4.0/geoana/
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.375397 geoana-0.4.0/geoana/earthquake/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/earthquake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43873 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/earthquake/oksar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.379397 geoana-0.4.0/geoana/em/
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14001 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.379397 geoana-0.4.0/geoana/em/fdem/
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10864 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (121)    18893 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/layered.py
--rw-r--r--   0 runner    (1001) docker     (121)     5064 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/simple_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    50821 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/fdem/wholespace.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.379397 geoana-0.4.0/geoana/em/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12890 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/static/freespace.py
--rw-r--r--   0 runner    (1001) docker     (121)    24482 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/static/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (121)    31922 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/static/sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)    38382 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/static/wholespace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.379397 geoana-0.4.0/geoana/em/tdem/
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/tdem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8543 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/tdem/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2929 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/tdem/halfspace.py
--rw-r--r--   0 runner    (1001) docker     (121)    15326 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/tdem/simple_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    36451 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/em/tdem/wholespace.py
--rw-r--r--   0 runner    (1001) docker     (121)    20996 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/gravity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.379397 geoana-0.4.0/geoana/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.383398 geoana-0.4.0/geoana/kernels/_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5192 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/_rTE.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/_rTE.h
--rw-r--r--   0 runner    (1001) docker     (121)    17198 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/potential_field_prism.c
--rw-r--r--   0 runner    (1001) docker     (121)   970153 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana/kernels/_extensions/rTE.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     7325 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/rTE.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/_extensions/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     7012 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/potential_field_prism.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4886 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/kernels/tranverse_electric_reflections.py
--rw-r--r--   0 runner    (1001) docker     (121)     8704 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)    21783 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/spatial.py
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2022-10-26 17:15:30.000000 geoana-0.4.0/geoana/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:18:32.375397 geoana-0.4.0/geoana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-26 17:18:32.000000 geoana-0.4.0/geoana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 17:18:32.383398 geoana-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-10-26 17:15:30.000000 geoana-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.747113 geoana-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 18:51:22.000000 geoana-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 18:51:22.000000 geoana-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-06 18:53:41.747113 geoana-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-06 18:51:22.000000 geoana-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/earthquake/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/earthquake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43873 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/earthquake/oksar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana/em/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/fdem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/layered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/simple_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48584 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/fdem/wholespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/freespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31922 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38382 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/static/wholespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/em/tdem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15326 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/simple_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/em/tdem/wholespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/gravity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.743113 geoana-0.4.1/geoana/kernels/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/_rTE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/_rTE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17198 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/potential_field_prism.c
+-rw-r--r--   0 runner    (1001) docker     (123)   973806 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana/kernels/_extensions/rTE.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/rTE.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/_extensions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/potential_field_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/kernels/tranverse_electric_reflections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21783 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-06 18:51:22.000000 geoana-0.4.1/geoana/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.739113 geoana-0.4.1/geoana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 18:53:41.000000 geoana-0.4.1/geoana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:53:41.747113 geoana-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-06 18:51:22.000000 geoana-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:53:41.747113 geoana-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_earthquake_oksar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_electric_dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_layered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_magnetic_dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_fdem_planewave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54251 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_halfspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_em_tdem_planewave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_potential_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 18:51:22.000000 geoana-0.4.1/tests/test_utils.py
```

### Comparing `geoana-0.4.0/LICENSE` & `geoana-0.4.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2018 SimPEG Team
+Copyright (c) 2017 SimPEG Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `geoana-0.4.0/PKG-INFO` & `geoana-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoana
-Version: 0.4.0
+Version: 0.4.1
 Summary: Analytic expressions for geophysical responses
 Home-page: https://www.simpeg.xyz
 Download-URL: https://github.com/simpeg/geoana
 Author: SimPEG developers
 Author-email: lindseyheagy@gmail.com
 License: MIT License
 Keywords: geophysics,electromagnetics
```

### Comparing `geoana-0.4.0/README.rst` & `geoana-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/earthquake/oksar.py` & `geoana-0.4.1/geoana/earthquake/oksar.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/__init__.py` & `geoana-0.4.1/geoana/em/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/base.py` & `geoana-0.4.1/geoana/em/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def epsilon(self, value):
 
         try:
             value = float(value)
         except:
             raise TypeError(f"epsilon must be a number, got {type(value)}")
 
-        if value <= 0.0:
+        if value < 0.0:
             raise ValueError("epsilon must be greater than 0")
 
         self._epsilon = value
 
 
 class BaseDipole:
     """Base class for dipoles; namely the location and orientation.
```

### Comparing `geoana-0.4.0/geoana/em/fdem/__init__.py` & `geoana-0.4.1/geoana/em/fdem/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/fdem/base.py` & `geoana-0.4.1/geoana/em/fdem/base.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/fdem/halfspace.py` & `geoana-0.4.1/geoana/em/fdem/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/fdem/layered.py` & `geoana-0.4.1/geoana/em/fdem/layered.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Magnetic permeability for all layers (and at all frequencies). For non-dispersive
         permeability (no viscous remanent magnetization) or for an instance of
         **MagneticDipoleLayeredHalfSpace** at a single frequency, *mu* is assigned with a
         (n_layer) np.ndarray. For dispersive permeability and multiple frequencies, *mu*
         is assigned with a (n_layer, n_frequency) np.ndarray.
     epsilon : (n_layer) np.ndarray or (n_layer, n_frequency) np.ndarray
         Dielectric permittivity for all layers (and at all frequencies). Only applicable when
-        *quasistatic* == ``True``. For non-dispersive permittivity or for an instance of
+        *quasistatic* == ``False``. For non-dispersive permittivity or for an instance of
         **MagneticDipoleLayeredHalfSpace** at a single frequency, *epsilon* is assigned with
         a (n_layer) np.ndarray. For dispersive permittivity and multiple frequencies,
         *epsilon* is assigned with a (n_layer, n_frequency) np.ndarray.
 
     """
 
     def __init__(self, frequency, thickness, **kwargs):
```

### Comparing `geoana-0.4.0/geoana/em/fdem/simple_functions.py` & `geoana-0.4.1/geoana/em/fdem/simple_functions.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/fdem/wholespace.py` & `geoana-0.4.1/geoana/em/fdem/wholespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -539,39 +539,23 @@
         >>> plot2Ddata(xyz[:, 0:2], np.imag(a[f_ind, :, 2]), ax=ax2, scale='log', ncontour=25)
         >>> ax2.set_xlabel('X')
         >>> ax2.set_yticks([])
         >>> ax2.autoscale(tight=True)
         >>> ax2.set_title('Imag component {} Hz'.format(frequency[f_ind]))
 
         """
-        # r = self.distance(xyz)
-        # f = (
-        #     (1j * self.omega * self.mu * self.moment) / (4 * np.pi * r) *
-        #     np.exp(-1j * self.wavenumber * r)
-        # )
-        # f = np.kron(np.ones(1, 3), np.atleast_2d(f).T)
-        # return self.dot_orientation(f)
-
-        n_freq = len(self.frequency)
-        n_loc = np.shape(xyz)[0]
-
-        r = self.distance(xyz)
+        xyz = check_xyz_dim(xyz)
+        r = np.linalg.norm(xyz, axis=-1)
         k = self.wavenumber
-
-        tile_r = np.tile(r.reshape((1, n_loc)), (n_freq, 1))
-        tile_w = np.tile(self.omega.reshape((n_freq, 1)), (1, n_loc))
-
-        a = (1j * tile_w * self.mu * self.moment) * (
-            1 / (4*np.pi*tile_r) * np.exp(-1j*np.outer(k, r))
-        )
-
-        v = self.orientation.reshape(1, 1, 3)
-        a = a.reshape((n_freq, n_loc, 1))
-
-        return np.kron(v, a).squeeze()
+        omega = self.omega
+        for i in range(r.ndim):
+            k = k[..., None]
+            omega = omega[..., None]
+        f = 1j * omega * self.mu * self.moment / (4 * np.pi * r) * np.exp(-1j * k * r)
+        return (f[..., None] * self.orientation).squeeze()
 
     def electric_field(self, xyz):
         r"""Electric field for the harmonic magnetic dipole at a set of gridded locations.
 
         For a harmonic magnetic dipole oriented in the :math:`\hat{u}` direction with
         moment amplitude :math:`m` and harmonic frequency :math:`f`, this method computes the
         electric field at the set of gridded xyz locations provided.
@@ -646,50 +630,30 @@
         >>> )
         >>> ax2.set_xlabel('X')
         >>> ax2.set_yticks([])
         >>> ax2.autoscale(tight=True)
         >>> ax2.set_title('Imag component {} Hz'.format(frequency[f_ind]))
 
         """
-        # dxyz = self.vector_distance(xyz)
-        # r = repeat_scalar(self.distance(xyz))
-        # kr = self.wavenumber*r
-        # ikr = 1j * kr
-
-        # front_term = (
-        #     (1j * self.omega * self.mu * self.moment) / (4. * np.pi * r**2) *
-        #     (ikr + 1) * np.exp(-ikr)
-        # )
-        # return front_term * self.cross_orientation(dxyz) / r
-
-        n_freq = len(self.frequency)
-        n_loc = np.shape(xyz)[0]
-
+        xyz = check_xyz_dim(xyz)
+        dxyz = xyz - self.location
+        r = np.linalg.norm(dxyz, axis=-1)
         k = self.wavenumber
-        r = self.distance(xyz)
-
-        # (n_freq, n_loc)
-        tile_r = np.tile(r.reshape((1, n_loc)), (n_freq, 1))
-        tile_w = np.tile(self.omega.reshape((n_freq, 1)), (1, n_loc))
-        kr = np.outer(k, r)
+        omega = self.omega
+        for i in range(r.ndim):
+            k = k[..., None]
+            omega = omega[..., None]
+        kr = k * r
         ikr = 1j * kr
 
-        first_term = (
-            (1j * tile_w * self.mu * self.moment) *
-            (1 / (4 * np.pi * tile_r**2) * (ikr + 1) * np.exp(-ikr))
-        ).reshape((n_freq, n_loc, 1))
-        first_term = np.tile(first_term, (1, 1, 3))
-
-        r = repeat_scalar(r)
-        dxyz = self.vector_distance(xyz)
-
-        second_term = (self.cross_orientation(dxyz) / r).reshape((1, n_loc, 3))
-        second_term = np.tile(second_term, (n_freq, 1, 1))
-
-        return (first_term * second_term).squeeze()
+        front_term = (
+             (1j * omega * self.mu * self.moment) / (4. * np.pi * r**2) *
+             (ikr + 1) * np.exp(-ikr)
+        ) / r
+        return (front_term[..., None] * np.cross(dxyz, self.orientation)).squeeze()
 
     def current_density(self, xyz):
         r"""Current density for the harmonic magnetic dipole at a set of gridded locations.
 
         For a harmonic magnetic dipole oriented in the :math:`\hat{u}` direction with
         moment amplitude :math:`m` and harmonic frequency :math:`f`, this method computes the
         current density at the set of gridded xyz locations provided.
@@ -848,61 +812,30 @@
         >>> )
         >>> ax2.set_xlabel('X')
         >>> ax2.set_yticks([])
         >>> ax2.autoscale(tight=True)
         >>> ax2.set_title('Imag component {} Hz'.format(frequency[f_ind]))
 
         """
-        # dxyz = self.vector_distance(xyz)
-        # r = repeat_scalar(self.distance(xyz))
-        # kr = self.wavenumber*r
-        # ikr = 1j*kr
-
-        # front_term = self.moment / (4. * np.pi * r**3) * np.exp(-ikr)
-        # symmetric_term = (
-        #     repeat_scalar(self.dot_orientation(dxyz)) * dxyz *
-        #     (-kr**2 + 3*ikr + 3) / r**2
-        # )
-        # oriented_term = (
-        #     (kr**2 - ikr - 1) *
-        #     np.kron(self.orientation, np.ones((dxyz.shape[0], 1)))
-        # )
-
-        # return front_term * (symmetric_term + oriented_term)
-
-        n_freq = len(self.frequency)
-        n_loc = np.shape(xyz)[0]
-
+        xyz = check_xyz_dim(xyz)
+        dxyz = xyz - self.location
+        r = np.linalg.norm(dxyz, axis=-1)
         k = self.wavenumber
-        r = self.distance(xyz)
-        dxyz = self.vector_distance(xyz)
-
-        # (n_freq, n_loc)
-        kr = np.outer(k, r)
+        for i in range(r.ndim):
+            k = k[..., None]
+        kr = k * r
         ikr = 1j * kr
-        tile_r = np.outer(np.ones(n_freq), r)
 
-        front_term = self.moment * (
-            1 / (4 * np.pi * tile_r**3) * np.exp(-ikr)
-        ).reshape((n_freq, n_loc, 1))
-        front_term = np.tile(front_term, (1, 1, 3))
-
-        temp_1 = repeat_scalar(self.dot_orientation(dxyz)) * dxyz
-        temp_1 = np.tile(temp_1.reshape((1, n_loc, 3)), (n_freq, 1, 1))
-        temp_2 = (-kr**2 + 3*ikr + 3) / tile_r**2
-        temp_2 = np.tile(temp_2.reshape((n_freq, n_loc, 1)), (1, 1, 3))
-        symmetric_term = temp_1 * temp_2
-
-        temp_1 = (kr**2 - ikr - 1)
-        temp_1 = np.tile(temp_1.reshape((n_freq, n_loc, 1)), (1, 1, 3))
-        temp_2 = np.kron(self.orientation, np.ones((dxyz.shape[0], 1)))
-        temp_2 = np.tile(temp_2.reshape((1, n_loc, 3)), (n_freq, 1, 1))
-        oriented_term = temp_1 * temp_2
+        front_term = self.moment / (4. * np.pi * r**3) * np.exp(-ikr)
+
+        symmetric_term = (dxyz @ self.orientation)[None, ...]*((-kr**2 + 3*ikr + 3) / r**2)
+
+        oriented_term = (kr**2 - ikr - 1)[..., None] * self.orientation
 
-        return (front_term * (symmetric_term + oriented_term)).squeeze()
+        return (front_term[..., None] * (symmetric_term[..., None] * dxyz + oriented_term)).squeeze()
 
     def magnetic_flux_density(self, xyz):
         r"""Magnetic flux density for the harmonic magnetic dipole at a set of gridded locations.
 
         For a harmonic magnetic dipole oriented in the :math:`\hat{u}` direction with
         moment amplitude :math:`m` and harmonic frequency :math:`f`, this method computes the
         magnetic flux density at the set of gridded xyz locations provided.
```

### Comparing `geoana-0.4.0/geoana/em/static/__init__.py` & `geoana-0.4.1/geoana/em/static/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/static/freespace.py` & `geoana-0.4.1/geoana/em/static/freespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,23 @@
             Point mass location in units m.
 
         Returns
         -------
         (..., 3) numpy.ndarray
             Magnetic flux density or prism at location xyz in units :math:`T`.
         """
-        return mu_0 * self.magnetic_field(xyz)
+        xyz = check_xyz_dim(xyz)
+        H = self.magnetic_field(xyz)
+        is_inside = (
+            np.all(xyz >= self.min_location, axis=-1)
+            & np.all(xyz <= self.max_location, axis=-1)
+        )
+        H[is_inside] = H[is_inside] + self.magnetization
+
+        return mu_0 * H
 
     def magnetic_field_gradient(self, xyz):
         """
         Magnetic field gradient due to a prism.
 
         Parameters
         ----------
```

### Comparing `geoana-0.4.0/geoana/em/static/halfspace.py` & `geoana-0.4.1/geoana/em/static/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/static/sphere.py` & `geoana-0.4.1/geoana/em/static/sphere.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/static/wholespace.py` & `geoana-0.4.1/geoana/em/static/wholespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/tdem/__init__.py` & `geoana-0.4.1/geoana/em/tdem/__init__.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/tdem/base.py` & `geoana-0.4.1/geoana/em/tdem/base.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/tdem/halfspace.py` & `geoana-0.4.1/geoana/em/tdem/halfspace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/tdem/simple_functions.py` & `geoana-0.4.1/geoana/em/tdem/simple_functions.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/em/tdem/wholespace.py` & `geoana-0.4.1/geoana/em/tdem/wholespace.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/gravity.py` & `geoana-0.4.1/geoana/gravity.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/_rTE.cpp` & `geoana-0.4.1/geoana/kernels/_extensions/_rTE.cpp`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/_rTE.h` & `geoana-0.4.1/geoana/kernels/_extensions/_rTE.h`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/potential_field_prism.c` & `geoana-0.4.1/geoana/kernels/_extensions/potential_field_prism.c`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/rTE.cpp` & `geoana-0.4.1/geoana/kernels/_extensions/rTE.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "geoana/kernels/_extensions/_rTE.h"
         ],
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,24 +93,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -394,17 +398,14 @@
     operator T&() { return *ptr; }
     template<typename U> bool operator ==(U other) { return *ptr == other; }
     template<typename U> bool operator !=(U other) { return *ptr != other; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -474,14 +475,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -581,35 +587,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1651,26 +1657,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -2030,14 +2036,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -2072,22 +2095,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -6268,15 +6299,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -8246,15 +8277,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -10549,15 +10580,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -10622,15 +10653,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -13302,15 +13333,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -18825,15 +18856,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -19029,15 +19060,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -19192,15 +19223,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -19214,15 +19245,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -19314,15 +19345,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -19345,15 +19376,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19578,15 +19609,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -19598,15 +19629,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19727,15 +19758,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -20244,15 +20275,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -20368,55 +20404,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20601,15 +20621,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_geoana__kernels___extensions__rTE) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -21639,28 +21659,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -22301,15 +22321,15 @@
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -22846,61 +22866,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -22908,15 +22946,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -24210,15 +24248,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -24364,15 +24402,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -24614,15 +24652,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24810,15 +24848,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -25044,15 +25082,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/rTE.pyx` & `geoana-0.4.1/geoana/kernels/_extensions/rTE.pyx`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/_extensions/setup.py` & `geoana-0.4.1/geoana/kernels/_extensions/setup.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/potential_field_prism.py` & `geoana-0.4.1/geoana/kernels/potential_field_prism.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/kernels/tranverse_electric_reflections.py` & `geoana-0.4.1/geoana/kernels/tranverse_electric_reflections.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/plotting_utils.py` & `geoana-0.4.1/geoana/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/shapes.py` & `geoana-0.4.1/geoana/shapes.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/spatial.py` & `geoana-0.4.1/geoana/spatial.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana/utils.py` & `geoana-0.4.1/geoana/utils.py`

 * *Files identical despite different names*

### Comparing `geoana-0.4.0/geoana.egg-info/PKG-INFO` & `geoana-0.4.1/geoana.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoana
-Version: 0.4.0
+Version: 0.4.1
 Summary: Analytic expressions for geophysical responses
 Home-page: https://www.simpeg.xyz
 Download-URL: https://github.com/simpeg/geoana
 Author: SimPEG developers
 Author-email: lindseyheagy@gmail.com
 License: MIT License
 Keywords: geophysics,electromagnetics
```

### Comparing `geoana-0.4.0/geoana.egg-info/SOURCES.txt` & `geoana-0.4.1/geoana.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -41,8 +41,25 @@
 geoana/kernels/tranverse_electric_reflections.py
 geoana/kernels/_extensions/__init__.py
 geoana/kernels/_extensions/_rTE.cpp
 geoana/kernels/_extensions/_rTE.h
 geoana/kernels/_extensions/potential_field_prism.c
 geoana/kernels/_extensions/rTE.cpp
 geoana/kernels/_extensions/rTE.pyx
-geoana/kernels/_extensions/setup.py
+geoana/kernels/_extensions/setup.py
+tests/test_docs.py
+tests/test_earthquake_oksar.py
+tests/test_em_fdem_base.py
+tests/test_em_fdem_electric_dipole.py
+tests/test_em_fdem_layered.py
+tests/test_em_fdem_magnetic_dipole.py
+tests/test_em_fdem_planewave.py
+tests/test_em_simple.py
+tests/test_em_static.py
+tests/test_em_tdem_base.py
+tests/test_em_tdem_halfspace.py
+tests/test_em_tdem_planewave.py
+tests/test_gravity.py
+tests/test_plotting_utils.py
+tests/test_potential_prism.py
+tests/test_spatial.py
+tests/test_utils.py
```

### Comparing `geoana-0.4.0/setup.py` & `geoana-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return config
 
 with open('README.rst') as f:
     LONG_DESCRIPTION = ''.join(f.readlines())
 
 metadata = dict(
     name = 'geoana',
-    version = '0.4.0',
+    version = '0.4.1',
     python_requires=">=3.6",
     setup_requires=[
         "numpy>=1.8",
         "cython>=0.2",
     ],
     install_requires = [
         'numpy>=1.8',
```

