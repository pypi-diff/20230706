# Comparing `tmp/strax-1.5.1.tar.gz` & `tmp/strax-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.5.1.tar", last modified: Thu Jun 22 19:15:15 2023, max compression
+gzip compressed data, was "strax-1.5.2.tar", last modified: Thu Jul  6 20:31:24 2023, max compression
```

## Comparing `strax-1.5.1.tar` & `strax-1.5.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.967150 strax-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-22 19:15:12.000000 strax-1.5.1/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 19:15:12.000000 strax-1.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-22 19:15:12.000000 strax-1.5.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-22 19:15:12.000000 strax-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 19:15:12.000000 strax-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28313 2023-06-22 19:15:15.967150 strax-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-22 19:15:12.000000 strax-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-22 19:15:12.000000 strax-1.5.1/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 19:15:12.000000 strax-1.5.1/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 19:15:12.000000 strax-1.5.1/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:15:12.000000 strax-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 19:15:15.967150 strax-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-22 19:15:12.000000 strax-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/strax/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-22 19:15:12.000000 strax-1.5.1/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 19:15:12.000000 strax-1.5.1/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-06-22 19:15:12.000000 strax-1.5.1/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-22 19:15:12.000000 strax-1.5.1/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    96667 2023-06-22 19:15:12.000000 strax-1.5.1/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-22 19:15:12.000000 strax-1.5.1/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-22 19:15:12.000000 strax-1.5.1/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-22 19:15:12.000000 strax-1.5.1/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-06-22 19:15:12.000000 strax-1.5.1/strax/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27242 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-06-22 19:15:12.000000 strax-1.5.1/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-06-22 19:15:12.000000 strax-1.5.1/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-06-22 19:15:12.000000 strax-1.5.1/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28313 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.967150 strax-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.236858 strax-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-06 20:31:20.000000 strax-1.5.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-06 20:31:20.000000 strax-1.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-07-06 20:31:20.000000 strax-1.5.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 20:31:20.000000 strax-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:31:20.000000 strax-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28622 2023-07-06 20:31:24.236858 strax-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-06 20:31:20.000000 strax-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.228858 strax-1.5.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-06 20:31:20.000000 strax-1.5.2/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.228858 strax-1.5.2/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 20:31:20.000000 strax-1.5.2/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 20:31:20.000000 strax-1.5.2/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 20:31:20.000000 strax-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 20:31:24.240858 strax-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-06 20:31:20.000000 strax-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.232858 strax-1.5.2/strax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 20:31:20.000000 strax-1.5.2/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-06 20:31:20.000000 strax-1.5.2/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-07-06 20:31:20.000000 strax-1.5.2/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-06 20:31:20.000000 strax-1.5.2/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96667 2023-07-06 20:31:20.000000 strax-1.5.2/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-06 20:31:20.000000 strax-1.5.2/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-06 20:31:20.000000 strax-1.5.2/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-06 20:31:20.000000 strax-1.5.2/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-07-06 20:31:20.000000 strax-1.5.2/strax/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.232858 strax-1.5.2/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27242 2023-07-06 20:31:20.000000 strax-1.5.2/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.232858 strax-1.5.2/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18867 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-07-06 20:31:20.000000 strax-1.5.2/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-07-06 20:31:20.000000 strax-1.5.2/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.236858 strax-1.5.2/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-06 20:31:20.000000 strax-1.5.2/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-07-06 20:31:20.000000 strax-1.5.2/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-07-06 20:31:20.000000 strax-1.5.2/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.232858 strax-1.5.2/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28622 2023-07-06 20:31:23.000000 strax-1.5.2/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-06 20:31:24.000000 strax-1.5.2/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:31:23.000000 strax-1.5.2/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:31:23.000000 strax-1.5.2/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-06 20:31:23.000000 strax-1.5.2/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 20:31:23.000000 strax-1.5.2/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:24.236858 strax-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:31:20.000000 strax-1.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16088 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-07-06 20:31:20.000000 strax-1.5.2/tests/test_utils.py
```

### Comparing `strax-1.5.1/CODE-OF-CONDUCT.md` & `strax-1.5.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/CONTRIBUTING.md` & `strax-1.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/HISTORY.md` & `strax-1.5.2/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+1.5.2 / 2023-07-06
+---------------------
+* Use warning also in `abs_time_to_prev_next_interval` by @dachengx in https://github.com/AxFoundation/strax/pull/738
+
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.1...v1.5.2
+
+
 1.5.1 / 2023-06-22
 ---------------------
 * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
 * Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
 * Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
 * add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
 * Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
```

### Comparing `strax-1.5.1/LICENSE` & `strax-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/PKG-INFO` & `strax-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.5.1
+Version: 1.5.2
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,14 +22,22 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.2 / 2023-07-06
+        ---------------------
+        * Use warning also in `abs_time_to_prev_next_interval` by @dachengx in https://github.com/AxFoundation/strax/pull/738
+        
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.1...v1.5.2
+        
+        
         1.5.1 / 2023-06-22
         ---------------------
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
         * Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
         * Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
         * add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
         * Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
```

### Comparing `strax-1.5.1/README.md` & `strax-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/bin/rechunker` & `strax-1.5.2/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/setup.py` & `strax-1.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='strax',
-                 version='1.5.1',
+                 version='1.5.2',
                  description='Streaming analysis for xenon TPCs',
                  author='Jelle Aalbers',
                  url='https://github.com/AxFoundation/strax',
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
                  tests_require=requires + tests_requires,
                  long_description=readme + '\n\n' + history,
```

### Comparing `strax-1.5.1/strax/__init__.py` & `strax-1.5.2/strax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.5.1/strax/chunk.py` & `strax-1.5.2/strax/chunk.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/config.py` & `strax-1.5.2/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/context.py` & `strax-1.5.2/strax/context.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/corrections.py` & `strax-1.5.2/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/dtypes.py` & `strax-1.5.2/strax/dtypes.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/io.py` & `strax-1.5.2/strax/io.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/mailbox.py` & `strax-1.5.2/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/cut_plugin.py` & `strax-1.5.2/strax/plugins/cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/loop_plugin.py` & `strax-1.5.2/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/merge_only_plugin.py` & `strax-1.5.2/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/overlap_window_plugin.py` & `strax-1.5.2/strax/plugins/overlap_window_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/parrallel_source_plugin.py` & `strax-1.5.2/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/plugins/plugin.py` & `strax-1.5.2/strax/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/data_reduction.py` & `strax-1.5.2/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/general.py` & `strax-1.5.2/strax/processing/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,15 +380,15 @@
         raise ValueError('time of things should be sorted!')
     try:
         _check_time_is_sorted(strax.endtime(things))
     except Exception:
         warnings.warn(
             'endtime of things is not sorted! '
             'touching_windows will return the indices of the '
-            'first and last things which are touching the container')
+            'first and last things which are touching the container.')
     try:
         _check_time_is_sorted(containers['time'])
     except Exception:
         raise ValueError('time of containers should be sorted!')
     for objects, names in zip([things, containers], ['things', 'containers']):
         try:
             _check_objects_non_negative_length(objects)
@@ -466,61 +466,74 @@
     that things do not overlap.
     
     :param things: Numpy structured array containing strax time fields
     :param intervals: Numpy structured array containing time fields
     :returns: Two integer arrays with the time difference to the 
         previous and next intervals. 
     """
-    _things_do_not_overlap = (strax.endtime(things)[:-1] - things['time'][1:]) <= 0
-    assert np.all(_things_do_not_overlap), 'Things overlap!'
+    try:
+        _check_time_is_sorted(things['time'])
+    except Exception:
+        raise ValueError('time of things should be sorted!')
+    try:
+        _check_time_is_sorted(strax.endtime(things))
+    except Exception:
+        warnings.warn(
+            'endtime of things is not sorted! '
+            'times_to_next returned by abs_time_to_prev_next_interval '
+            'might be larger than expected.')
+    try:
+        _check_time_is_sorted(intervals['time'])
+    except Exception:
+        raise ValueError('time of intervals should be sorted!')
 
     times_to_prev = np.ones(len(things), dtype=np.int64) * -1
     times_to_next = np.ones(len(things), dtype=np.int64) * -1
-    
+
     _empty_events_or_intervals = ((len(things) == 0) 
-                                  or (len(intervals)== 0))
+                                  or (len(intervals) == 0))
     if _empty_events_or_intervals:
         return times_to_prev, times_to_next
-        
+
     _abs_time_to_prev_next(things, intervals, times_to_prev, times_to_next)
-    
+
     return times_to_prev, times_to_next
 
+
 @numba.njit
 def _abs_time_to_prev_next(things, intervals, times_to_prev, times_to_next):
     veto_intervals_seen = 0
-    last_thing_end = 0
     for thing_ind, thing_i in enumerate(things):
         current_event_time = thing_i['time']
         current_event_endtime = strax.endtime(thing_i)
-        
+
         # Exploit the fact that events cannot overlap...
         # Loop over veto intervals until:
         #   - current veto interval endtime starts overlapping with 
         #    current event. This is the interval from which we need to 
         #    start looping for the next event.
         #   - current veto_interval time starts to be larger than current 
         #    event time. Only then we can be sure we have computed the 
         #    shortest time delay as endtime is not sorted...
         for veto_interval in intervals[veto_intervals_seen:]:
             _interval_start_after_thing = veto_interval['time'] >= current_event_time
             if _interval_start_after_thing:             
                 break
-            
+
             # Always update endtime until it becomes negative:
             dt = current_event_time - strax.endtime(veto_interval)
             _ends_befor_event = dt >= 0
             if _ends_befor_event:
                 times_to_prev[thing_ind] = dt
                 veto_intervals_seen += 1
-        
+
         # Now check if current veto is still within event or already after it:
         for veto_interval in intervals[veto_intervals_seen:]:
             _current_interval_before_thing_ends = veto_interval['time'] < current_event_endtime
             if _current_interval_before_thing_ends:
                 continue
 
             # Now current veto is after event so store time:
-            times_to_next[thing_ind] = veto_interval['time']  - current_event_endtime
+            times_to_next[thing_ind] = veto_interval['time'] - current_event_endtime
             break
-            
+
         veto_intervals_seen = max(0, veto_intervals_seen-1)
```

### Comparing `strax-1.5.1/strax/processing/hitlets.py` & `strax-1.5.2/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/peak_building.py` & `strax-1.5.2/strax/processing/peak_building.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/peak_merging.py` & `strax-1.5.2/strax/processing/peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/peak_properties.py` & `strax-1.5.2/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/peak_splitting.py` & `strax-1.5.2/strax/processing/peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/pulse_processing.py` & `strax-1.5.2/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processing/statistics.py` & `strax-1.5.2/strax/processing/statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/processor.py` & `strax-1.5.2/strax/processor.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/run_selection.py` & `strax-1.5.2/strax/run_selection.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/storage/common.py` & `strax-1.5.2/strax/storage/common.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/storage/file_rechunker.py` & `strax-1.5.2/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/storage/files.py` & `strax-1.5.2/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/storage/mongo.py` & `strax-1.5.2/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/storage/zipfiles.py` & `strax-1.5.2/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/testutils.py` & `strax-1.5.2/strax/testutils.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax/utils.py` & `strax-1.5.2/strax/utils.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/strax.egg-info/PKG-INFO` & `strax-1.5.2/strax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.5.1
+Version: 1.5.2
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,14 +22,22 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.2 / 2023-07-06
+        ---------------------
+        * Use warning also in `abs_time_to_prev_next_interval` by @dachengx in https://github.com/AxFoundation/strax/pull/738
+        
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.1...v1.5.2
+        
+        
         1.5.1 / 2023-06-22
         ---------------------
         * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
         * Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
         * Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
         * add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
         * Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
```

### Comparing `strax-1.5.1/strax.egg-info/SOURCES.txt` & `strax-1.5.2/strax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_child_plugins.py` & `strax-1.5.2/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_config.py` & `strax-1.5.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_context.py` & `strax-1.5.2/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_core.py` & `strax-1.5.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_corrections.py` & `strax-1.5.2/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_cut_plugin.py` & `strax-1.5.2/tests/test_cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_data_reduction.py` & `strax-1.5.2/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_fixed_plugin_cache.py` & `strax-1.5.2/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_general_processing.py` & `strax-1.5.2/tests/test_general_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,41 +318,32 @@
     dummy_array3['time'][0] = np.iinfo(np.int64).min // 2 + 1
     dummy_array3['time'][-1] = np.iinfo(np.int64).max // 2 - 1
     res1 = strax.sort_by_time(dummy_array3)
     res2 = np.sort(dummy_array3, order=('time', 'channel'))
     assert np.all(res1 == res2)
 
     _test_sort_by_time_peaks(time)
-    
-    
+
+
 def _test_sort_by_time_peaks(time):
-    """Explicit test to check if peaks a re sorted correctly.
+    """
+    Explicit test to check if peaks a re sorted correctly.
     """
     dummy_array = np.zeros(len(time), strax.time_fields 
                             + [(('dummy_channel_number', 'channel'), np.int16)]
                            )
     dummy_array['time'] = time
     dummy_array['channel'] = -1
-    
+
     res1 = strax.sort_by_time(dummy_array)
     res2 = np.sort(dummy_array, order='time')
     assert np.all(res1 == res2)
 
-    
-class Test_abs_time_to_prev_next_interval(unittest.TestCase):
-
-    def test_overlapping_raises_error(self):
-        events = np.zeros(2, strax.time_fields)
-        vetos = np.zeros(1, strax.time_fields)
-
-        events['time'] = [5, 10]
-        events['endtime'] = [15, 20]
-        self.assertRaises(AssertionError, strax.abs_time_to_prev_next_interval, events, vetos)
 
-        
+class Test_abs_time_to_prev_next_interval(unittest.TestCase):
     def test_empty_inputs(self):
         events = np.zeros(1, strax.time_fields)
         vetos = np.zeros(0, strax.time_fields)
 
         events['time'] = 1
         events['endtime'] = 2
         res_prev, res_next = strax.abs_time_to_prev_next_interval(events, vetos)
@@ -369,73 +360,72 @@
         _results_are_empty = (len(res_prev) == 0) and (len(res_next) == 0) 
         assert _results_are_empty
 
         events = np.zeros(0, strax.time_fields)
         vetos = np.zeros(0, strax.time_fields)
         res_prev, res_next = strax.abs_time_to_prev_next_interval(events, vetos)
 
-    
     def test_with_dt_fields(self):
         pass
-    
+
     @hypothesis.given(things=
                       hyp_numpy.arrays(np.int64,
                     hypothesis.strategies.integers(1, 10),
                     elements=hypothesis.strategies.integers(0, 1000),
                     unique=False),
         intervals=
                       hyp_numpy.arrays(np.int64,
                        hypothesis.strategies.integers(1, 100),
                        elements=hypothesis.strategies.integers(0, 100),
                        unique=True),
         )
-    
+
     @hypothesis.settings(deadline=None)
     def test_correct_time_delays(self, things, intervals):
         _things, _intervals = self._make_correct_things_and_intervals(things, intervals)
         res_prev, res_next = strax.abs_time_to_prev_next_interval(_things, _intervals)
         
         # Compare for each event:
         for thing_i, e in enumerate(_things):
             dt_prev = e['time'] - _intervals['endtime'] 
             dt_prev[dt_prev < 0] = 99999
             dt_prev = np.min(dt_prev)
-            
+
             msg = (f'Found {res_prev[thing_i]}, but expected {dt_prev}'
             f' for thing number {thing_i} of things: {_things} and intervals: {_intervals}')
             if res_prev[thing_i] != -1:
                 assert dt_prev == res_prev[thing_i], msg
             else:
                 assert dt_prev == 99999, msg
-            
+
             dt_next = _intervals['time']  - e['endtime'] 
             dt_next[dt_next < 0] = 99999
             dt_next = np.min(dt_next)
-            
+
             msg = (f'Found {res_next[thing_i]}, but expected {dt_next}'
             f' for thing number {thing_i} of things: {_things} and intervals: {_intervals}')
             if res_next[thing_i] != -1:
                 assert dt_next == res_next[thing_i], msg
             else:
                 assert dt_next == 99999, msg
-                
+
     def _make_correct_things_and_intervals(self, things, intervals):
         _things = np.zeros(len(things), strax.time_fields)
         _things['time'] = things
         _things['endtime'] = things + 100
-        
+
         _intervals = np.zeros(len(intervals), strax.time_fields)
         _intervals['time'] = intervals
         _intervals['endtime'] = intervals + 10
-        
+
         _things = strax.sort_by_time(_things)
         _intervals = strax.sort_by_time(_intervals)
-        
+
         # Cut down overlapping _things and remove empty intervals to not 
         # trigger overlapping error:
         dt = _things['endtime'][:-1] - _things['time'][1:]
         dt[dt < 0] = 0
         _things['endtime'][:-1] = _things['endtime'][:-1] - dt
         _is_not_empty_interval =( _things['endtime'] - _things['time']) > 0
         _things = _things[_is_not_empty_interval]
-        
+
         return _things, _intervals
```

### Comparing `strax-1.5.1/tests/test_get_zarr.py` & `strax-1.5.2/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_helpers.py` & `strax-1.5.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_hitlet.py` & `strax-1.5.2/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_inline_plugin.py` & `strax-1.5.2/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_lone_hit_integration.py` & `strax-1.5.2/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_loop_plugins.py` & `strax-1.5.2/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_mailbox.py` & `strax-1.5.2/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_mongo_frontend.py` & `strax-1.5.2/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_multi_output.py` & `strax-1.5.2/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_overlap_plugin.py` & `strax-1.5.2/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_peak_merging.py` & `strax-1.5.2/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_peak_processing.py` & `strax-1.5.2/tests/test_peak_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_peak_properties.py` & `strax-1.5.2/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_peak_splitting.py` & `strax-1.5.2/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_pulse_processing.py` & `strax-1.5.2/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_saving.py` & `strax-1.5.2/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_statistics.py` & `strax-1.5.2/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_storage.py` & `strax-1.5.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_superruns.py` & `strax-1.5.2/tests/test_superruns.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.1/tests/test_utils.py` & `strax-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

