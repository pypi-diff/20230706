# Comparing `tmp/bluepymm-0.8.7.tar.gz` & `tmp/bluepymm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepymm-0.8.7.tar", last modified: Mon Feb 27 15:16:16 2023, max compression
+gzip compressed data, was "bluepymm-0.9.0.tar", last modified: Thu Jul  6 09:13:43 2023, max compression
```

## Comparing `bluepymm-0.8.7.tar` & `bluepymm-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-27 15:16:14.000000 bluepymm-0.8.7/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-02-27 15:16:14.000000 bluepymm-0.8.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-27 15:16:14.000000 bluepymm-0.8.7/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-27 15:16:14.000000 bluepymm-0.8.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-27 15:16:14.000000 bluepymm-0.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-27 15:16:16.835696 bluepymm-0.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-02-27 15:16:14.000000 bluepymm-0.8.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/legacy/create_hoc_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/prepare_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/prepare_combos/prepare_emodel_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/run_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/run_combos/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/select_combos/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/select_combos/table_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/templates/cell_template_neurodamus.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/templates/cell_template_neuron.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/bluepymm/validate_output/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/validate_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-02-27 15:16:14.000000 bluepymm-0.8.7/bluepymm/validate_output/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.831696 bluepymm-0.8.7/bluepymm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-27 15:16:16.000000 bluepymm-0.8.7/bluepymm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-27 15:16:16.835696 bluepymm-0.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-27 15:16:14.000000 bluepymm-0.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:16.835696 bluepymm-0.8.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_bluepymm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_calculate_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_create_mm_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_megate_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_parse_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_prepare_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_prepare_emodel_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_process_megate_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_run_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_select_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_sqlite_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_table_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-02-27 15:16:14.000000 bluepymm-0.8.7/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-02-27 15:16:14.000000 bluepymm-0.8.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 09:13:33.000000 bluepymm-0.9.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-07-06 09:13:33.000000 bluepymm-0.9.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-06 09:13:33.000000 bluepymm-0.9.0/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 09:13:33.000000 bluepymm-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 09:13:33.000000 bluepymm-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 09:13:43.292847 bluepymm-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-06 09:13:33.000000 bluepymm-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.288847 bluepymm-0.9.0/bluepymm/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/legacy/create_hoc_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.288847 bluepymm-0.9.0/bluepymm/prepare_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/prepare_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16419 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/prepare_combos/create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/prepare_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/prepare_combos/parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/prepare_combos/prepare_emodel_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/run_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/run_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/run_combos/calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/run_combos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/select_combos/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16467 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/select_combos/table_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6660 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/templates/cell_template_neurodamus.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4762 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/templates/cell_template_neuron.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/bluepymm/validate_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/validate_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-06 09:13:33.000000 bluepymm-0.9.0/bluepymm/validate_output/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.288847 bluepymm-0.9.0/bluepymm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 09:13:43.000000 bluepymm-0.9.0/bluepymm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 09:13:43.292847 bluepymm-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-06 09:13:33.000000 bluepymm-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:43.292847 bluepymm-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_bluepymm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_calculate_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_create_mm_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10714 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_megate_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_parse_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_prepare_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_prepare_emodel_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_process_megate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_run_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_select_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_sqlite_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15008 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_table_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-06 09:13:33.000000 bluepymm-0.9.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69513 2023-07-06 09:13:33.000000 bluepymm-0.9.0/versioneer.py
```

### Comparing `bluepymm-0.8.7/COPYING` & `bluepymm-0.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/COPYING.lesser` & `bluepymm-0.9.0/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/LICENSE.txt` & `bluepymm-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/PKG-INFO` & `bluepymm-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.8.7
+Version: 0.9.0
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.8.7/README.rst` & `bluepymm-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/__init__.py` & `bluepymm-0.9.0/bluepymm/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/legacy/__init__.py` & `bluepymm-0.9.0/bluepymm/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/legacy/create_hoc_files.py` & `bluepymm-0.9.0/bluepymm/legacy/create_hoc_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/main.py` & `bluepymm-0.9.0/bluepymm/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/prepare_combos/__init__.py` & `bluepymm-0.9.0/bluepymm/prepare_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/prepare_combos/create_mm_sqlite.py` & `bluepymm-0.9.0/bluepymm/prepare_combos/create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/prepare_combos/main.py` & `bluepymm-0.9.0/bluepymm/prepare_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/prepare_combos/parse_files.py` & `bluepymm-0.9.0/bluepymm/prepare_combos/parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/prepare_combos/prepare_emodel_dirs.py` & `bluepymm-0.9.0/bluepymm/prepare_combos/prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/run_combos/__init__.py` & `bluepymm-0.9.0/bluepymm/run_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/run_combos/calculate_scores.py` & `bluepymm-0.9.0/bluepymm/run_combos/calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/run_combos/main.py` & `bluepymm-0.9.0/bluepymm/run_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/__init__.py` & `bluepymm-0.9.0/bluepymm/select_combos/__init__.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/main.py` & `bluepymm-0.9.0/bluepymm/select_combos/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/megate_output.py` & `bluepymm-0.9.0/bluepymm/select_combos/megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/process_megate_config.py` & `bluepymm-0.9.0/bluepymm/select_combos/process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/reporting.py` & `bluepymm-0.9.0/bluepymm/select_combos/reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,20 +370,29 @@
         for emodel, emodel_info in emodel_infos.items():
             if emodel_info is not None:
                 emodel_ext_neurondb_rows, \
                     megate_scores, emodel_score_values, fullmtypes, \
                     emodel_megate_passed_all, emodel_median_scores, \
                     emodel_passed_combos = \
                     emodel_info
-                ext_neurondb = ext_neurondb.append(emodel_ext_neurondb_rows)
+                ext_neurondb = pandas.concat(
+                    [ext_neurondb, emodel_ext_neurondb_rows], axis=0
+                ).reset_index(drop=True)
 
-                megate_passed_all = megate_passed_all.append(
-                    emodel_megate_passed_all)
-                median_scores = median_scores.append(emodel_median_scores)
-                passed_combos = passed_combos.append(emodel_passed_combos)
+                megate_passed_all = pandas.concat(
+                    [megate_passed_all, emodel_megate_passed_all], axis=0
+                ).reset_index(drop=True)
+
+                median_scores = pandas.concat(
+                    [median_scores, emodel_median_scores], axis=0
+                ).reset_index(drop=True)
+
+                passed_combos = pandas.concat(
+                    [passed_combos, emodel_passed_combos], axis=0
+                ).reset_index(drop=True)
 
                 # Reporting per e-model
                 add_plot_to_report(
                     pp,
                     plot_morphs_per_feature_for_emodel,
                     emodel,
                     megate_scores,
```

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/sqlite_io.py` & `bluepymm-0.9.0/bluepymm/select_combos/sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/select_combos/table_processing.py` & `bluepymm-0.9.0/bluepymm/select_combos/table_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,15 @@
         return (emodel, None)
 
     emodel_mtype_etype_thresholds = emodel_mtype_etypes.loc[
         :, ['emodel', 'fullmtype', 'etype']]
     emodel_mtype_etype_thresholds['megate_feature_threshold'] = None
 
     print('Getting megating thresholds for emodel %s' % emodel)
-    emodel_mtype_etype_thresholds.apply(
+    emodel_mtype_etype_thresholds = emodel_mtype_etype_thresholds.apply(
         lambda row: row_threshold_transform(row, megate_patterns),
         axis=1)
 
     # select score values relevant to this e-model
     emodel_score_values = score_values[(combos.emodel == emodel) &
                                        (combos.is_exemplar == 0)].copy()
     emodel_score_values.dropna(axis=1, how='all', inplace=True)
```

### Comparing `bluepymm-0.8.7/bluepymm/templates/cell_template_neurodamus.jinja2` & `bluepymm-0.9.0/bluepymm/templates/cell_template_neurodamus.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/templates/cell_template_neuron.jinja2` & `bluepymm-0.9.0/bluepymm/templates/cell_template_neuron.jinja2`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/tools.py` & `bluepymm-0.9.0/bluepymm/tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm/validate_output/main.py` & `bluepymm-0.9.0/bluepymm/validate_output/main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/bluepymm.egg-info/PKG-INFO` & `bluepymm-0.9.0/bluepymm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepymm
-Version: 0.8.7
+Version: 0.9.0
 Summary: Model Management Python Library (bluepymm)
 Home-page: https://github.com/BlueBrain/BluePyMM
 Author: BlueBrain Project, EPFL
 Author-email: werner.vangeit@epfl.ch
 Keywords: optimisation,neuroscience,BlueBrainProject
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `bluepymm-0.8.7/bluepymm.egg-info/SOURCES.txt` & `bluepymm-0.9.0/bluepymm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/setup.py` & `bluepymm-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,25 @@
 
 import versioneer
 
 setuptools.setup(
     name="bluepymm",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
-    install_requires=['sh', 'bluepyopt', 'matplotlib', 'pandas', 'numpy',
-                      'ipyparallel', 'lxml', 'h5py', 'pyyaml'],
+    install_requires=[
+        "sh",
+        "bluepyopt",
+        "matplotlib",
+        "pandas>=2.0.0",
+        "numpy",
+        "ipyparallel",
+        "lxml",
+        "h5py",
+        "pyyaml",
+    ],
     packages=setuptools.find_packages(exclude=('notebook',)),
     author="BlueBrain Project, EPFL",
     author_email="werner.vangeit@epfl.ch",
     description="Model Management Python Library (bluepymm)",
     long_description="Model Management Python Library (bluepymm)",
     url='https://github.com/BlueBrain/BluePyMM',
     keywords=[
```

### Comparing `bluepymm-0.8.7/tests/test_bluepymm.py` & `bluepymm-0.9.0/tests/test_bluepymm.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_calculate_scores.py` & `bluepymm-0.9.0/tests/test_calculate_scores.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_create_mm_sqlite.py` & `bluepymm-0.9.0/tests/test_create_mm_sqlite.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_legacy.py` & `bluepymm-0.9.0/tests/test_legacy.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_main.py` & `bluepymm-0.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_megate_output.py` & `bluepymm-0.9.0/tests/test_megate_output.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_parse_files.py` & `bluepymm-0.9.0/tests/test_parse_files.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_prepare_combos.py` & `bluepymm-0.9.0/tests/test_prepare_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_prepare_emodel_dirs.py` & `bluepymm-0.9.0/tests/test_prepare_emodel_dirs.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_process_megate_config.py` & `bluepymm-0.9.0/tests/test_process_megate_config.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_reporting.py` & `bluepymm-0.9.0/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_run_combos.py` & `bluepymm-0.9.0/tests/test_run_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_select_combos.py` & `bluepymm-0.9.0/tests/test_select_combos.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_sqlite_io.py` & `bluepymm-0.9.0/tests/test_sqlite_io.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_table_processing.py` & `bluepymm-0.9.0/tests/test_table_processing.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/tests/test_tools.py` & `bluepymm-0.9.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `bluepymm-0.8.7/versioneer.py` & `bluepymm-0.9.0/versioneer.py`

 * *Files identical despite different names*

