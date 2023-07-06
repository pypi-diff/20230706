# Comparing `tmp/popmon-1.4.4.tar.gz` & `tmp/popmon-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popmon-1.4.4.tar", last modified: Fri May 26 09:00:56 2023, max compression
+gzip compressed data, was "popmon-1.4.5.tar", last modified: Thu Jul  6 14:54:25 2023, max compression
```

## Comparing `popmon-1.4.4.tar` & `popmon-1.4.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.061332 popmon-1.4.4/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-26 09:00:44.000000 popmon-1.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-26 09:00:44.000000 popmon-1.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3792 2023-05-26 09:00:44.000000 popmon-1.4.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)    23345 2023-05-26 09:00:56.057332 popmon-1.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21523 2023-05-26 09:00:44.000000 popmon-1.4.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/
--rw-r--r--   0 root         (0) root         (0)     1893 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/alerting/
--rw-r--r--   0 root         (0) root         (0)     1627 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4197 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/alerts_summary.py
--rw-r--r--   0 root         (0) root         (0)    18616 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/alerting/compute_tl_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/
--rw-r--r--   0 root         (0) root         (0)     1280 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/apply_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/comparison/
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/comparisons.py
--rw-r--r--   0 root         (0) root         (0)    15490 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/comparison/hist_comparer.py
--rw-r--r--   0 root         (0) root         (0)    19311 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/functions.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/hist_numpy.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/merge_statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/analysis/profiling/
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8232 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/hist_profiler.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/profiles.py
--rw-r--r--   0 root         (0) root         (0)    11323 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/analysis/profiling/pull_calculator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/base/
--rw-r--r--   0 root         (0) root         (0)     1224 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6973 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/module.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     4730 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/base/registry.py
--rw-r--r--   0 root         (0) root         (0)    14500 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/decorators/
--rw-r--r--   0 root         (0) root         (0)     1215 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/pandas.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/decorators/spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/extensions/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/extension.py
--rw-r--r--   0 root         (0) root         (0)     2479 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/extensions/profile_diptest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/hist/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.041331 popmon-1.4.4/popmon/hist/filling/
--rw-r--r--   0 root         (0) root         (0)     1745 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/filling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6570 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/hist_splitter.py
--rw-r--r--   0 root         (0) root         (0)    10908 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/hist/hist_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/io/
--rw-r--r--   0 root         (0) root         (0)     1299 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/file_reader.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/file_writer.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/io/json_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/notebooks/
--rw-r--r--   0 root         (0) root         (0)    19461 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)     5777 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    11902 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
--rw-r--r--   0 root         (0) root         (0)    11762 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/notebooks/popmon_tutorial_reports.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1108 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/amazing_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     5208 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/dataset_splitter.py
--rw-r--r--   0 root         (0) root         (0)     7102 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/metrics.py
--rw-r--r--   0 root         (0) root         (0)    16465 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/metrics_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    11202 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/report.py
--rw-r--r--   0 root         (0) root         (0)     9117 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/report_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/pipeline/timing.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/stats/
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stats/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11198 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stats/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.045331 popmon-1.4.4/popmon/stitching/
--rw-r--r--   0 root         (0) root         (0)     1234 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stitching/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20217 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/stitching/hist_stitcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.049332 popmon-1.4.4/popmon/test_data/
--rw-r--r--   0 root         (0) root         (0)    73043 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/data_generator_hists.json.gz
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/example.json
--rw-r--r--   0 root         (0) root         (0)    15152 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/example_histogram.json
--rw-r--r--   0 root         (0) root         (0)   696816 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/flight_delays.csv.gz
--rw-r--r--   0 root         (0) root         (0)   692782 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/flight_delays_reference.csv.gz
--rw-r--r--   0 root         (0) root         (0)    79082 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/synthetic_histograms.json
--rw-r--r--   0 root         (0) root         (0)    64368 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/test_data/test.csv.gz
--rw-r--r--   0 root         (0) root         (0)     2705 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-26 09:00:45.000000 popmon-1.4.4/popmon/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/
--rw-r--r--   0 root         (0) root         (0)     1645 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/alert_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    15429 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/histogram_section.py
--rw-r--r--   0 root         (0) root         (0)     8517 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/overview_section.py
--rw-r--r--   0 root         (0) root         (0)     3079 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/report_generator.py
--rw-r--r--   0 root         (0) root         (0)    10829 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/section_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/templates/
--rw-r--r--   0 root         (0) root         (0)      835 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/aggregated-overview.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon/visualization/templates/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.053332 popmon-1.4.4/popmon/visualization/templates/assets/css/
--rw-r--r--   0 root         (0) root         (0)   155712 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)     2090 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/css/custom-style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.057332 popmon-1.4.4/popmon/visualization/templates/assets/js/
--rw-r--r--   0 root         (0) root         (0)    78586 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)     2943 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/custom-script.js
--rwxr-xr-x   0 root         (0) root         (0)     2532 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.easing.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)  3682474 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/plotly.js
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/assets/js/scrolling-nav.js
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/card.html
--rw-r--r--   0 root         (0) root         (0)     1003 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/core.html
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/footer.html
--rw-r--r--   0 root         (0) root         (0)      782 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/header.html
--rw-r--r--   0 root         (0) root         (0)      988 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/modal-popup.html
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/notebook_iframe.html
--rw-r--r--   0 root         (0) root         (0)     2739 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/section.html
--rw-r--r--   0 root         (0) root         (0)     1401 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/templates/table.html
--rw-r--r--   0 root         (0) root         (0)     7295 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/traffic_light_section_generator.py
--rw-r--r--   0 root         (0) root         (0)    26741 2023-05-26 09:00:44.000000 popmon-1.4.4/popmon/visualization/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 09:00:56.037331 popmon-1.4.4/popmon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23345 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3410 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-26 09:00:56.000000 popmon-1.4.4/popmon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     4571 2023-05-26 09:00:44.000000 popmon-1.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-26 09:00:44.000000 popmon-1.4.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 09:00:56.061332 popmon-1.4.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.011726 popmon-1.4.5/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-06 14:54:14.000000 popmon-1.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-06 14:54:14.000000 popmon-1.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-07-06 14:54:14.000000 popmon-1.4.5/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-07-06 14:54:25.011726 popmon-1.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21523 2023-07-06 14:54:14.000000 popmon-1.4.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon/
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon/alerting/
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/alerts_summary.py
+-rw-r--r--   0 root         (0) root         (0)    18853 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/alerting/compute_tl_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13919 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/apply_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/comparison/
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8823 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/comparisons.py
+-rw-r--r--   0 root         (0) root         (0)    15744 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/comparison/hist_comparer.py
+-rw-r--r--   0 root         (0) root         (0)    19472 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/functions.py
+-rw-r--r--   0 root         (0) root         (0)    18777 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/hist_numpy.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/merge_statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/analysis/profiling/
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8254 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/hist_profiler.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/analysis/profiling/pull_calculator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.991726 popmon-1.4.5/popmon/base/
+-rw-r--r--   0 root         (0) root         (0)     1224 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7096 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/module.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4833 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/base/registry.py
+-rw-r--r--   0 root         (0) root         (0)    14549 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/decorators/
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/decorators/spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/extensions/
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/extension.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/extensions/profile_diptest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/hist/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/hist/filling/
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/filling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6638 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/hist_splitter.py
+-rw-r--r--   0 root         (0) root         (0)    10961 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/hist/hist_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/io/
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/file_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/file_writer.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/io/json_reader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.995726 popmon-1.4.5/popmon/notebooks/
+-rw-r--r--   0 root         (0) root         (0)    19461 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5777 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11902 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_incremental_data.ipynb
+-rw-r--r--   0 root         (0) root         (0)    11762 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/notebooks/popmon_tutorial_reports.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/amazing_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     5208 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/dataset_splitter.py
+-rw-r--r--   0 root         (0) root         (0)     7116 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    16532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/metrics_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    11282 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/report.py
+-rw-r--r--   0 root         (0) root         (0)     9162 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/report_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/pipeline/timing.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/stats/
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stats/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.999726 popmon-1.4.5/popmon/stitching/
+-rw-r--r--   0 root         (0) root         (0)     1234 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stitching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20246 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/stitching/hist_stitcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.003726 popmon-1.4.5/popmon/test_data/
+-rw-r--r--   0 root         (0) root         (0)    73043 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/data_generator_hists.json.gz
+-rw-r--r--   0 root         (0) root         (0)      128 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/example.json
+-rw-r--r--   0 root         (0) root         (0)    15152 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/example_histogram.json
+-rw-r--r--   0 root         (0) root         (0)   696816 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/flight_delays.csv.gz
+-rw-r--r--   0 root         (0) root         (0)   692782 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/flight_delays_reference.csv.gz
+-rw-r--r--   0 root         (0) root         (0)    79082 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/synthetic_histograms.json
+-rw-r--r--   0 root         (0) root         (0)    64368 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/test_data/test.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-07-06 14:54:15.000000 popmon-1.4.5/popmon/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.003726 popmon-1.4.5/popmon/visualization/
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6321 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/alert_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15385 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/histogram_section.py
+-rw-r--r--   0 root         (0) root         (0)     8532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/overview_section.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/report_generator.py
+-rw-r--r--   0 root         (0) root         (0)    10860 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/section_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.007726 popmon-1.4.5/popmon/visualization/templates/
+-rw-r--r--   0 root         (0) root         (0)      835 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/aggregated-overview.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.983726 popmon-1.4.5/popmon/visualization/templates/assets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.007726 popmon-1.4.5/popmon/visualization/templates/assets/css/
+-rw-r--r--   0 root         (0) root         (0)   155712 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)     2090 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/css/custom-style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:25.011726 popmon-1.4.5/popmon/visualization/templates/assets/js/
+-rw-r--r--   0 root         (0) root         (0)    78586 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)     2943 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/custom-script.js
+-rwxr-xr-x   0 root         (0) root         (0)     2532 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.easing.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)  3682474 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/plotly.js
+-rw-r--r--   0 root         (0) root         (0)      927 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/assets/js/scrolling-nav.js
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/card.html
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/core.html
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/footer.html
+-rw-r--r--   0 root         (0) root         (0)      782 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/header.html
+-rw-r--r--   0 root         (0) root         (0)      988 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/modal-popup.html
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/notebook_iframe.html
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/section.html
+-rw-r--r--   0 root         (0) root         (0)     1401 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/templates/table.html
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/traffic_light_section_generator.py
+-rw-r--r--   0 root         (0) root         (0)    26880 2023-07-06 14:54:14.000000 popmon-1.4.5/popmon/visualization/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 14:54:24.987726 popmon-1.4.5/popmon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23345 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 14:54:24.000000 popmon-1.4.5/popmon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5119 2023-07-06 14:54:14.000000 popmon-1.4.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-06 14:54:14.000000 popmon-1.4.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 14:54:25.011726 popmon-1.4.5/setup.cfg
```

### Comparing `popmon-1.4.4/LICENSE` & `popmon-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/NOTICE` & `popmon-1.4.5/NOTICE`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/PKG-INFO` & `popmon-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.4
+Version: 1.4.5
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.4/README.rst` & `popmon-1.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/__init__.py` & `popmon-1.4.5/popmon/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/alerting/__init__.py` & `popmon-1.4.5/popmon/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/alerting/alerts_summary.py` & `popmon-1.4.5/popmon/alerting/alerts_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
     _input_keys = ("read_key",)
     _output_keys = ("store_key",)
 
     def __init__(
         self,
         read_key,
-        store_key="",
+        store_key: str = "",
         features=None,
         ignore_features=None,
-        combined_variable="_AGGREGATE_",
-    ):
+        combined_variable: str = "_AGGREGATE_",
+    ) -> None:
         """Initialize an instance of AlertsSummary module.
 
         :param str read_key: key of input data to read from datastore.
         :param str store_key: key of output data to store in datastore (optional).
         :param str combined_variable: name of artificial variable that combines all alerts. default is '_AGGREGATE_'.
         :param list features: features of data frames to pick up from input data (optional).
         :param list ignore_features: list of features to ignore (optional).
```

### Comparing `popmon-1.4.4/popmon/alerting/compute_tl_bounds.py` & `popmon-1.4.5/popmon/alerting/compute_tl_bounds.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import numpy as np
 import pandas as pd
 
 from popmon.analysis.apply_func import ApplyFunc
 from popmon.base import Module, Pipeline
 
 
-def traffic_light_summary(row, cols=None, prefix=""):
+def traffic_light_summary(row, cols=None, prefix: str = ""):
     """Make a summary of traffic light alerts present in the dataframe
 
     Count number of green, yellow and red traffic lights.
 
     Evaluate with df.apply(traffic_light_summary, axis=1)
 
     :param pd.Series row: row to calculate traffic light summary of.
@@ -56,15 +56,17 @@
     traffic_lights = np.array([row[c] for c in cols])
     x["n_red"] = (traffic_lights == 2).sum()
     x["n_yellow"] = (traffic_lights == 1).sum()
     x["n_green"] = (traffic_lights == 0).sum()
     return pd.Series(x)
 
 
-def traffic_light(value, red_high, yellow_high, yellow_low=0, red_low=0):
+def traffic_light(
+    value, red_high, yellow_high, yellow_low: int = 0, red_low: int = 0
+) -> int:
     """Get the corresponding traffic light given a value and traffic light bounds.
 
     :param float value: value to check
     :param float red_high: higher bound of red traffic light
     :param float yellow_high: higher bound of yellow traffic light
     :param float yellow_low: lower bound of yellow traffic light (optional)
     :param float red_low: lower bound of red traffic light (optional)
@@ -116,25 +118,25 @@
     _input_keys = ("read_key",)
     _output_keys = ("store_key", "apply_funcs_key")
 
     def __init__(
         self,
         read_key,
         monitoring_rules=None,
-        store_key="",
+        store_key: str = "",
         features=None,
         ignore_features=None,
-        apply_funcs_key="",
+        apply_funcs_key: str = "",
         func=None,
-        metrics_wide=False,
-        prefix="traffic_light_",
-        suffix="",
-        entire=False,
+        metrics_wide: bool = False,
+        prefix: str = "traffic_light_",
+        suffix: str = "",
+        entire: bool = False,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of TrafficLightBounds module.
 
         :param str read_key: key of input data to read from datastore
         :param str store_key: key of output data to store in datastore (optional)
         :param dict monitoring_rules: dict of traffic light bounds => key is feature:metric and value is bounds
         :param list features: features of data frames to pick up from input data (optional)
         :param list ignore_features: list of features to ignore (optional)
@@ -167,15 +169,15 @@
         if not callable(self.traffic_light_func):
             raise TypeError("supplied function must be callable object")
 
     def get_description(self):
         """Returns the traffic light function as description."""
         return self.traffic_light_func.__name__
 
-    def _set_traffic_lights(self, feature, cols, pattern, rule):
+    def _set_traffic_lights(self, feature, cols, pattern, rule) -> None:
         process_cols = fnmatch.filter(cols, pattern)
 
         for pcol in process_cols:
             name = f"{feature}:{pcol}"
             if name not in self.traffic_lights:
                 key = rule(name, feature, pattern)
                 bounds = self.monitoring_rules[key]
@@ -246,18 +248,18 @@
         return self.traffic_lights, self.traffic_light_funcs
 
 
 def pull_bounds(
     row,
     red_high,
     yellow_high,
-    yellow_low=0,
-    red_low=0,
-    suffix_mean="_mean",
-    suffix_std="_std",
+    yellow_low: int = 0,
+    red_low: int = 0,
+    suffix_mean: str = "_mean",
+    suffix_std: str = "_std",
     cols=None,
 ):
     """Calculate traffic light pull bounds for list of cols
 
     Function can be used with ApplyFunc module.
 
     :param pd.Series row: row to apply this function to.
@@ -303,18 +305,18 @@
     return pd.Series(x)
 
 
 def df_single_op_pull_bounds(
     df,
     red_high,
     yellow_high,
-    yellow_low=0,
-    red_low=0,
-    suffix_mean="_mean",
-    suffix_std="_std",
+    yellow_low: int = 0,
+    red_low: int = 0,
+    suffix_mean: str = "_mean",
+    suffix_std: str = "_std",
     cols=None,
 ):
     """Calculate traffic light pull bounds for list of cols on first row only
 
     Function can be used with ApplyFunc module.
 
     :param pd.DataFrame df: df to apply this function to
@@ -337,18 +339,18 @@
 class DynamicBounds(Pipeline):
     """Calculate dynamic traffic light bounds based on pull thresholds and dynamic mean and std.deviation."""
 
     def __init__(
         self,
         read_key,
         rules,
-        store_key="",
-        suffix_mean="_mean",
-        suffix_std="_std",
-    ):
+        store_key: str = "",
+        suffix_mean: str = "_mean",
+        suffix_std: str = "_std",
+    ) -> None:
         """Initialize an instance of DynamicTrafficLightBounds.
 
         :param str read_key: key of input data to read from data store, only used to extract feature list.
         :param dict rules: dict of traffic light bounds => key is feature:metric and value is bounds
         :param str store_key: key of dynamic traffic light boundaries to store in data store, e.g. used for plotting.
         :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
         :param str suffix_std: suffix of std. std column = metric + suffix_std
@@ -381,18 +383,18 @@
 class StaticBounds(Pipeline):
     """Calculate static traffic light bounds based on pull thresholds and static mean and std.deviation."""
 
     def __init__(
         self,
         read_key,
         rules,
-        store_key="",
-        suffix_mean="_mean",
-        suffix_std="_std",
-    ):
+        store_key: str = "",
+        suffix_mean: str = "_mean",
+        suffix_std: str = "_std",
+    ) -> None:
         """Initialize an instance of StaticBounds.
 
         :param str read_key: key of input data to read from data store, only used to extract feature list.
         :param dict rules: dict of traffic light bounds => key is feature:metric and value is bounds
         :param str store_key: key of dynamic traffic light boundaries to store in data store, e.g. used for plotting.
         :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
         :param str suffix_std: suffix of std. std column = metric + suffix_std
@@ -428,15 +430,17 @@
 
     Steps:
 
     - Generate static traffic light bounds by expanding the wildcarded monitoring rules
     - Apply them to profiled test statistics data
     """
 
-    def __init__(self, read_key, store_key, rules, expanded_rules_key=""):
+    def __init__(
+        self, read_key, store_key, rules, expanded_rules_key: str = ""
+    ) -> None:
         """Initialize an instance of TrafficLightBounds.
 
         :param str read_key: key of input data to read from data store, only used to extract feature list.
         :param str store_key: results of traffic light bounds after applied to input data, to store in data store.
         :param dict rules: input dict of wildcard traffic light bounds => key is feature:metric
                                       and value is bounds
         :param str expanded_rules_key: store key of expanded monitoring rules to store in data store,
```

### Comparing `popmon-1.4.4/popmon/analysis/__init__.py` & `popmon-1.4.5/popmon/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/analysis/apply_func.py` & `popmon-1.4.5/popmon/analysis/apply_func.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
+from __future__ import annotations
 
 import warnings
-from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from popmon.base import Module
 from popmon.utils import parallel
 
@@ -36,22 +35,22 @@
 
     _input_keys = ("apply_to_key", "assign_to_key", "apply_funcs_key")
     _output_keys = ("store_key",)
 
     def __init__(
         self,
         apply_to_key,
-        store_key="",
-        assign_to_key="",
-        apply_funcs_key="",
+        store_key: str = "",
+        assign_to_key: str = "",
+        apply_funcs_key: str = "",
         features=None,
         apply_funcs=None,
         metrics=None,
-        msg="",
-    ):
+        msg: str = "",
+    ) -> None:
         """Initialize an instance of ApplyFunc.
 
         :param str apply_to_key: key of the input data to apply funcs to.
         :param str assign_to_key: key of the input data to assign function applied-output to. (optional)
         :param str store_key: key of the output data to store in the datastore (optional)
         :param str apply_funcs_key: key of to-be-applied functions in data to store (optional)
         :param list features: list of features to pick up from input data and apply funcs to (optional)
@@ -143,16 +142,16 @@
                 "kwargs": kwargs,
             }
         )
 
     def transform(
         self,
         apply_to_data: dict,
-        assign_to_data: Optional[dict] = None,
-        apply_funcs: Optional[list] = None,
+        assign_to_data: dict | None = None,
+        apply_funcs: list | None = None,
     ):
         """
         Apply functions to specified feature and metrics
 
         Each feature/metric combination is treated as a pandas series
 
         :param datastore: input datastore
```

### Comparing `popmon-1.4.4/popmon/analysis/comparison/__init__.py` & `popmon-1.4.5/popmon/analysis/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/analysis/comparison/comparisons.py` & `popmon-1.4.5/popmon/analysis/comparison/comparisons.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
 @Comparisons.register(
     key="unknown_labels",
     description="Are categories observed in a given time slot that are not present in the reference?",
     dim=1,
     htype="cat",
 )
-def unknown_labels(hist1, hist2):
+def unknown_labels(hist1, hist2) -> bool:
     # check consistency of bin_labels
     labels1 = hist1.keySet
     labels2 = hist2.keySet
     subset = labels1 <= labels2
     return not subset
```

### Comparing `popmon-1.4.4/popmon/analysis/comparison/hist_comparer.py` & `popmon-1.4.5/popmon/analysis/comparison/hist_comparer.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     get_consistent_numpy_entries,
     get_consistent_numpy_ndgrids,
 )
 from popmon.base import Pipeline
 from popmon.hist.hist_utils import COMMON_HIST_TYPES, is_numeric
 
 
-def hist_compare(row, hist_name1="", hist_name2=""):
+def hist_compare(row, hist_name1: str = "", hist_name2: str = ""):
     """Function to compare two histograms
 
     Apply statistical tests to compare two input histograms, such as:
     Chi2, KS, Pearson, max probability difference.
     For categorical histograms, also check for unknown labels.
 
     :param pd.Series row: row to apply compare function to
@@ -103,19 +103,19 @@
 
     def __init__(
         self,
         func_hist_collector,
         read_key,
         store_key,
         assign_to_key=None,
-        hist_col="histogram",
-        suffix="comp",
+        hist_col: str = "histogram",
+        suffix: str = "comp",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of RollingHistComparer.
 
         :param func_hist_collector: histogram collection function
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param str assign_to_key: key of the input data to assign function applied-output to. (optional)
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
@@ -156,18 +156,18 @@
     """Compare histogram to previous rolling histograms"""
 
     def __init__(
         self,
         read_key,
         store_key,
         window,
-        shift=1,
-        hist_col="histogram",
-        suffix="roll",
-    ):
+        shift: int = 1,
+        hist_col: str = "histogram",
+        suffix: str = "roll",
+    ) -> None:
         """Initialize an instance of RollingHistComparer.
 
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param int window: size of rolling window
         :param int shift: shift of rolling window. default is 1.
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
@@ -197,17 +197,17 @@
 class PreviousHistComparer(RollingHistComparer):
     """Compare histogram to previous histograms"""
 
     def __init__(
         self,
         read_key,
         store_key,
-        hist_col="histogram",
-        suffix="prev1",
-    ):
+        hist_col: str = "histogram",
+        suffix: str = "prev1",
+    ) -> None:
         """Initialize an instance of PreviousHistComparer.
 
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
         :param str suffix: column/key of rolling histogram. default is 'prev' -> column = 'histogram_prev'
         """
@@ -224,18 +224,18 @@
 class ExpandingHistComparer(HistComparer):
     """Compare histogram to previous expanding histograms"""
 
     def __init__(
         self,
         read_key,
         store_key,
-        shift=1,
-        hist_col="histogram",
-        suffix="expanding",
-    ):
+        shift: int = 1,
+        hist_col: str = "histogram",
+        suffix: str = "expanding",
+    ) -> None:
         """Initialize an instance of ExpandingHistComparer.
 
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param int shift: shift of rolling window. default is 1.
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
         :param str suffix: column/key of rolling histogram. default is 'expanding' -> column = 'histogram_expanding'
@@ -263,17 +263,17 @@
     """Compare histogram to reference histograms"""
 
     def __init__(
         self,
         reference_key,
         assign_to_key,
         store_key,
-        hist_col="histogram",
-        suffix="ref",
-    ):
+        hist_col: str = "histogram",
+        suffix: str = "ref",
+    ) -> None:
         """Initialize an instance of ReferenceHistComparer.
 
         :param str reference_key: key of input data to read from data store
         :param str assign_to_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
         :param str suffix: column/key of rolling histogram. default is 'ref' -> column = 'histogram_ref'
@@ -302,18 +302,18 @@
 
     def __init__(
         self,
         func_hist_collector,
         read_key,
         store_key,
         assign_to_key=None,
-        hist_col="histogram",
+        hist_col: str = "histogram",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of NormHistComparer.
 
         :param func_hist_collector: histogram collection function
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param str assign_to_key: key of the input data to assign function applied-output to. (optional)
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
@@ -345,15 +345,17 @@
 
         super().__init__(modules=[hist_collector, hist_comparer])
 
 
 class RollingNormHistComparer(NormHistComparer):
     """Compare histogram to previous rolling normalized histograms"""
 
-    def __init__(self, read_key, store_key, window, shift=1, hist_col="histogram"):
+    def __init__(
+        self, read_key, store_key, window, shift: int = 1, hist_col: str = "histogram"
+    ) -> None:
         """Initialize an instance of RollingNormHistComparer.
 
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param int window: size of rolling window
         :param int shift: shift of rolling window. default is 1.
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
@@ -379,15 +381,17 @@
         )
         return super().transform(datastore)
 
 
 class ExpandingNormHistComparer(NormHistComparer):
     """Compare histogram to previous expanding normalized histograms"""
 
-    def __init__(self, read_key, store_key, shift=1, hist_col="histogram"):
+    def __init__(
+        self, read_key, store_key, shift: int = 1, hist_col: str = "histogram"
+    ) -> None:
         """Initialize an instance of ExpandingNormHistComparer.
 
         :param str read_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param int shift: shift of rolling window. default is 1.
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
         """
@@ -408,15 +412,17 @@
         )
         return super().transform(datastore)
 
 
 class ReferenceNormHistComparer(NormHistComparer):
     """Compare histogram to reference normalized histograms"""
 
-    def __init__(self, reference_key, assign_to_key, store_key, hist_col="histogram"):
+    def __init__(
+        self, reference_key, assign_to_key, store_key, hist_col: str = "histogram"
+    ) -> None:
         """Initialize an instance of ReferenceNormHistComparer.
 
         :param str reference_key: key of input data to read from data store
         :param str assign_to_key: key of input data to read from data store
         :param str store_key: key of output data to store in data store
         :param str hist_col: column/key in input df/dict that contains the histogram. default is 'histogram'
         """
```

### Comparing `popmon-1.4.4/popmon/analysis/functions.py` & `popmon-1.4.5/popmon/analysis/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     get_consistent_numpy_entries,
     set_2dgrid,
 )
 from popmon.hist.hist_utils import COMMON_HIST_TYPES, is_numeric
 from popmon.stats.numpy import probability_distribution_mean_covariance
 
 
-def pull(row, suffix_mean="_mean", suffix_std="_std", cols=None):
+def pull(row, suffix_mean: str = "_mean", suffix_std: str = "_std", cols=None):
     """Calculate normalized residual (pull) for list of cols
 
     Function can be used by ApplyFunc module.
 
     :param pd.Series row: row to apply pull function to
     :param list cols: list of cols to calculate pull of
     :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
@@ -70,80 +70,80 @@
         )
         for m in cols
     }
 
     return pd.Series(x)
 
 
-def expanding_mean(df, shift=1):
+def expanding_mean(df, shift: int = 1):
     """Calculate expanding mean of all numeric columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int shift: size of shift. default is 1.
     :return: df with expanding means of columns
     """
     return df.shift(shift).expanding().mean()
 
 
-def expanding_std(df, shift=1):
+def expanding_std(df, shift: int = 1):
     """Calculate expanding std of all numeric columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int shift: size of shift. default is 1.
     :return: df with expanding std of columns
     """
     return df.shift(shift).expanding().std()
 
 
-def expanding_apply(df, func, shift=1, *args, **kwargs):
+def expanding_apply(df, func, shift: int = 1, *args, **kwargs):
     """Calculate expanding apply() to all columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param func: function to be applied
     :param int shift: size of shift. default is 1.
     :param args: args passed on to function
     :param kwargs: kwargs passed on to function
     :return: df with expanding results of function applied to all columns
     """
     return df.shift(shift).expanding().apply(func, args=args, **kwargs)
 
 
-def rolling_std(df, window, shift=1):
+def rolling_std(df, window, shift: int = 1):
     """Calculate rolling std of all numeric columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int shift: size of shift. default is 1.
     :param int window: size of rolling window.
     :return: df with rolling std of columns
     """
     return df.shift(shift).rolling(window).std()
 
 
-def rolling_mean(df, window, shift=1):
+def rolling_mean(df, window, shift: int = 1):
     """Calculate rolling mean of all numeric columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int shift: size of shift. default is 1.
     :param int window: size of rolling window.
     :return: df with rolling mean of columns
     """
     return df.shift(shift).rolling(window).mean()
 
 
-def rolling_apply(df, window, func, shift=1, *args, **kwargs):
+def rolling_apply(df, window, func, shift: int = 1, *args, **kwargs):
     """Calculate rolling apply() to all columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int window: size of rolling window.
     :param func: function to be applied
@@ -152,15 +152,15 @@
     :param kwargs: kwargs passed on to function
     :return: df with rolling results of function applied to all columns
     """
     # raw=False already use Future setting
     return df.shift(shift).rolling(window).apply(func, raw=False, args=args, **kwargs)
 
 
-def rolling_lr(df, window, index=0, shift=0):
+def rolling_lr(df, window, index: int = 0, shift: int = 0):
     """Calculate rolling scipy lin_regress() to all columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int window: size of rolling window.
     :param int index: index of lin_regress results to return. default is 0.
@@ -171,15 +171,15 @@
     return (
         df.shift(shift)
         .rolling(window)
         .apply(lambda x: linregress(np.arange(len(x)), x)[index], raw=True)
     )
 
 
-def rolling_lr_zscore(df, window, shift=0):
+def rolling_lr_zscore(df, window, shift: int = 0):
     """Calculate rolling z-score of scipy lin_regress() to all columns of a pandas dataframe
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe
     :param int window: size of rolling window.
     :param int shift: size of shift. default is 0.
@@ -198,15 +198,15 @@
             except Exception:
                 y[name] = np.nan
         return y
 
     return roll(df, window=window, shift=shift).apply(func, axis=1)
 
 
-def roll(df, window, shift=1):
+def roll(df, window, shift: int = 1):
     """Implementation of rolling window that can handle non-numerical columns such as histograms
 
     :param pd.DataFrame df: input dataframe to apply rolling function to.
     :param int window: size of rolling window
     :param int shift: shift of dataframe, default is 1 (optional)
     """
     assert shift >= 0
@@ -246,15 +246,15 @@
 
     d = [{c: reshape(vals, i) for i, c in enumerate(cols)} for vals in arr]
     rolled_df = pd.DataFrame(data=d, index=df.index)
 
     return rolled_df
 
 
-def expand(df, shift=1):
+def expand(df, shift: int = 1):
     """Implementation of expanding window that can handle non-numerical values such as histograms
 
     Split up input array into expanding sub-arrays
 
     :param pd.DataFrame df: input dataframe to apply rolling function to.
     :param int shift: shift of dataframe, default is 1 (optional)
     :param fillvalue: default value to fill dataframe in case shift > 0 (optional)
@@ -279,29 +279,29 @@
 
     d = [{c: reshape(vals, i) for i, c in enumerate(cols)} for vals in arr]
     expanded_df = pd.DataFrame(data=d, index=df.index)
 
     return expanded_df
 
 
-def expanding_hist(df, shift=1, *args, **kwargs):
+def expanding_hist(df, shift: int = 1, *args, **kwargs):
     """Apply expanding histogram sum
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe with column of histograms
     :param int shift: shift of dataframe, default is 1 (optional)
     :param args: args passed on to hist_sum function
     :param kwargs: kwargs passed on to hist_sum function
     :return: dataframe with expanding hist_sum results
     """
     return expand(df, shift=shift).apply(hist_sum, axis=1, args=args, **kwargs)
 
 
-def rolling_hist(df, window, shift=1, *args, **kwargs):
+def rolling_hist(df, window, shift: int = 1, *args, **kwargs):
     """Apply rolling histogram sum
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe with column of histograms
     :param int window: size of rolling window
     :param int shift: shift of dataframe, default is 1 (optional)
@@ -310,15 +310,15 @@
     :return: dataframe with rolling hist_sum results
     """
     return roll(df, window=window, shift=shift).apply(
         hist_sum, axis=1, args=args, **kwargs
     )
 
 
-def hist_sum(x, hist_name=""):
+def hist_sum(x, hist_name: str = ""):
     """Return sum of histograms
 
     Usage: df['hists'].apply(hist_sum) ; series.apply(hist_sum)
 
     :param pd.Series x: pandas series to extract histogram list from.
     :param str hist_name: name of column to extract histograms from. needs to be set with axis=1 (optional)
     :return: sum histogram
@@ -347,15 +347,15 @@
         return pd.Series(o)
 
     h_sum = np.sum(hist_list)
     o[hist_name] = h_sum
     return pd.Series(o)
 
 
-def roll_norm_hist_mean_cov(df, window, shift=1, *args, **kwargs):
+def roll_norm_hist_mean_cov(df, window, shift: int = 1, *args, **kwargs):
     """Apply rolling normalized_hist_mean_cov function
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe with column of histograms
     :param int window: size of rolling window
     :param int shift: shift of dataframe, default is 1 (optional)
@@ -364,15 +364,15 @@
     :return: dataframe with rolling normalized_hist_mean_cov results
     """
     return roll(df, window=window, shift=shift).apply(
         normalized_hist_mean_cov, axis=1, args=args, **kwargs
     )
 
 
-def expand_norm_hist_mean_cov(df, shift=1, *args, **kwargs):
+def expand_norm_hist_mean_cov(df, shift: int = 1, *args, **kwargs):
     """Apply expanding normalized_hist_mean_cov function
 
     Function can be used by ApplyFunc module.
 
     :param pd.DataFrame df: input pandas dataframe with column of histograms
     :param int shift: shift of dataframe, default is 1 (optional)
     :param args: args passed on to hist_sum function
@@ -380,15 +380,15 @@
     :return: dataframe with expanding normalized_hist_mean_cov results
     """
     return expand(df, shift=shift).apply(
         normalized_hist_mean_cov, axis=1, args=args, **kwargs
     )
 
 
-def normalized_hist_mean_cov(x, hist_name=""):
+def normalized_hist_mean_cov(x, hist_name: str = ""):
     """Mean normalized histogram and its covariance of list of input histograms
 
     Usage: df['hists'].apply(normalized_hist_mean_cov) ; series.apply(normalized_hist_mean_cov)
 
     :param pd.Series x: pandas series to extract histogram list from.
     :param str hist_name: name of column to extract histograms from. needs to be set with axis=1 (optional)
     :return: mean normalized histogram, covariance probability matrix
@@ -442,18 +442,18 @@
     o[hist_name + "_cov"] = normalized_hist_covariance
     o[hist_name + "_binning"] = binning
     return pd.Series(o)
 
 
 def relative_chi_squared(
     row,
-    hist_name="histogram",
-    suffix_mean="_mean",
-    suffix_cov="_cov",
-    suffix_binning="_binning",
+    hist_name: str = "histogram",
+    suffix_mean: str = "_mean",
+    suffix_cov: str = "_cov",
+    suffix_binning: str = "_binning",
 ):
     """Calculate chi squared of normalized histogram with pre-calculated mean normalized histogram
 
     :param pd.Series row: row to apply chi_squared function to.
     :param str hist_name: name of column to extract histograms from. default is 'histogram' (optional)
     :param str suffix_mean: suffix of mean. mean column = hist_name + suffix_mean (optional)
     :param str suffix_std: suffix of std. std column = hist_name + suffix_std (optional)
```

### Comparing `popmon-1.4.4/popmon/analysis/hist_numpy.py` & `popmon-1.4.5/popmon/analysis/hist_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import warnings
 
 import histogrammar
 import numpy as np
 from histogrammar.util import get_hist_props
 
@@ -98,15 +99,15 @@
 
     if hist.n_dim < n_dim:
         warnings.warn(
             f"Input histogram only has {hist.n_dim} dimensions (<{n_dim}). Returning empty grid."
         )
         return grid
 
-    def flatten(histogram, keys, grid, dim=0, prefix=None):
+    def flatten(histogram, keys, grid, dim: int = 0, prefix=None):
         if prefix is None:
             prefix = []
 
         if len(keys) == len(prefix):
             grid[tuple(prefix)] = histogram.entries
         elif hasattr(histogram, "bins"):
             for k, h in histogram.bins.items():
@@ -133,15 +134,15 @@
     :param list xkeys: list with unique x keys
     :param list ykeys: list with unique y keys
     :return: filled 2d numpy grid
     """
     return set_ndgrid(hist, keys, n_dim=2)
 
 
-def get_ndgrid(hist, get_bin_labels=False, n_dim=2):
+def get_ndgrid(hist, get_bin_labels: bool = False, n_dim: int = 2):
     """Get filled n-d grid of first n dimensions of input histogram
 
     :param hist: input histogrammar histogram
     :return: grid of first n dimensions of input histogram
     """
     if hist.n_dim < n_dim:
         warnings.warn(
@@ -154,24 +155,26 @@
 
     if get_bin_labels:
         return grid, keys
 
     return grid
 
 
-def get_2dgrid(hist, get_bin_labels=False):
+def get_2dgrid(hist, get_bin_labels: bool = False):
     """Get filled x,y grid of first two dimensions of input histogram
 
     :param hist: input histogrammar histogram
     :return: x,y grid of first two dimensions of input histogram
     """
     return get_ndgrid(hist, get_bin_labels, n_dim=2)
 
 
-def get_consistent_numpy_ndgrids(hist_list=None, get_bin_labels=False, dim=3):
+def get_consistent_numpy_ndgrids(
+    hist_list=None, get_bin_labels: bool = False, dim: int = 3
+):
     """Get list of consistent x,y grids of first n dimensions of (sparse) input histograms
 
     :param list hist_list: list of input histogrammar histograms
     :param bool get_bin_labels: if true, return x-keys and y-keys describing binnings of 2d-grid.
     :param int dim: number of dimension (>= 3)
     :return: list of consistent x,y grids of first two dimensions of each input histogram in list
     """
@@ -180,42 +183,44 @@
         raise ValueError("Input histogram list has zero length.")
     if hist_list[0].n_dim < dim:
         raise ValueError(
             f"Input histogram only has {hist_list[0].n_dim} dimensions (<{dim}). Cannot compute {dim}d-grid."
         )
     assert_similar_hists(hist_list)
 
-    keys = [set() for _ in range(dim)]
+    keys: list[set] = [set() for _ in range(dim)]
     for hist in hist_list:
         hist_keys = prepare_ndgrid(hist, n_dim=dim)
         for i, h_keys in enumerate(hist_keys):
             keys[i] |= set(h_keys)
-    keys = [sorted(k) for k in keys]
+    sorted_keys = [sorted(k) for k in keys]
 
-    gridnd_list = [set_ndgrid(hist, keys, n_dim=dim) for hist in hist_list]
+    gridnd_list = [set_ndgrid(hist, sorted_keys, n_dim=dim) for hist in hist_list]
 
     if get_bin_labels:
-        return gridnd_list, keys
+        return gridnd_list, sorted_keys
 
     return gridnd_list
 
 
-def get_consistent_numpy_2dgrids(hist_list=None, get_bin_labels=False):
+def get_consistent_numpy_2dgrids(hist_list=None, get_bin_labels: bool = False):
     """Get list of consistent x,y grids of first two dimensions of (sparse) input histograms
 
     :param list hist_list: list of input histogrammar histograms
     :param bool get_bin_labels: if true, return x-keys and y-keys describing binnings of 2d-grid.
     :return: list of consistent x,y grids of first two dimensions of each input histogram in list
     """
     if hist_list is None:
         hist_list = []
     return get_consistent_numpy_ndgrids(hist_list, get_bin_labels, dim=2)
 
 
-def get_consistent_numpy_1dhists(hist_list, get_bin_labels=False, crop_range=False):
+def get_consistent_numpy_1dhists(
+    hist_list, get_bin_labels: bool = False, crop_range: bool = False
+):
     """Get list of consistent numpy hists for list of sparse (or bin) input histograms
 
     Works for sparse and bin histograms.
     Note: for sparse histograms, all potential bins between low and high are picked up (also unfilled).
 
     Note: a numpy histogram is a union of lists of bin_edges and number of entries
     This gives the full range of bin_centers, including zeros, which is not robust against (extreme) outliers.
@@ -290,15 +295,15 @@
 
     if get_bin_labels:
         return nphist_list, bin_centers
     else:
         return nphist_list
 
 
-def get_consistent_numpy_entries(hist_list, get_bin_labels=False):
+def get_consistent_numpy_entries(hist_list, get_bin_labels: bool = False):
     """Get list of consistent numpy bin_entries for list of 1d input histograms
 
     Works for categorize, sparse and bin histograms.
     Note: for sparse histograms, *only* the filled bins are picked up.
     (this is not the case when calling get_consistent_numpy_1dhists(), which takes all bins b/n low and high.)
 
     :param list hist_list: list of input histogrammar histograms
@@ -341,15 +346,15 @@
 
     if get_bin_labels:
         return entries_list, labels
     else:
         return entries_list
 
 
-def get_contentType(hist):
+def get_contentType(hist) -> str:
     """Get content type of bins of histogram
 
     :param hist: input histogram
     :return: string describing content type
     """
     if isinstance(hist, histogrammar.Count):
         return "Count"
@@ -358,15 +363,17 @@
     elif isinstance(hist, histogrammar.SparselyBin):
         return "SparselyBin"
     elif isinstance(hist, histogrammar.Categorize):
         return "Categorize"
     return "Count"
 
 
-def check_similar_hists(hist_list, check_type=True, assert_type=used_hist_types):
+def check_similar_hists(
+    hist_list, check_type: bool = True, assert_type=used_hist_types
+) -> bool:
     """Check consistent list of input histograms
 
     Check that type and dimension of all histograms in input list are the same.
 
     :param list hist_list: list of input histogram objects to check on consistency
     :param bool check_type: if true, also check type consistency of histograms (besides n-dim and datatype).
     :return: bool indicating if lists are similar
@@ -474,15 +481,17 @@
         # iterate down
         if not check_similar_hists(sub_hist_list):
             return False
 
     return True
 
 
-def assert_similar_hists(hist_list, check_type=True, assert_type=used_hist_types):
+def assert_similar_hists(
+    hist_list, check_type: bool = True, assert_type=used_hist_types
+):
     """Assert consistent list of input histograms
 
     Assert that type and dimension of all histograms in input list are the same.
 
     :param list hist_list: list of input histogram objects to check on consistency
     :param bool assert_type: if true, also assert type consistency of histograms (besides n-dim and datatype).
     """
```

### Comparing `popmon-1.4.4/popmon/analysis/merge_statistics.py` & `popmon-1.4.5/popmon/analysis/merge_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class MergeStatistics(Module):
     """Merging dictionaries of features containing dataframes with statistics as its values."""
 
     _input_keys = ("read_keys",)
     _output_keys = ("store_key",)
 
-    def __init__(self, read_keys: list[str], store_key: str):
+    def __init__(self, read_keys: list[str], store_key: str) -> None:
         """Initialize an instance of MergeStatistics.
 
         :param list read_keys: list of keys of input data to read from the datastore
         :param str store_key: key of output data to store in the datastore
         """
         super().__init__()
         self.read_keys = read_keys
```

### Comparing `popmon-1.4.4/popmon/analysis/profiling/__init__.py` & `popmon-1.4.5/popmon/analysis/profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/analysis/profiling/hist_profiler.py` & `popmon-1.4.5/popmon/analysis/profiling/hist_profiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,18 @@
     def __init__(
         self,
         read_key,
         store_key,
         features=None,
         ignore_features=None,
         var_timestamp=None,
-        hist_col="histogram",
-        index_col="date",
+        hist_col: str = "histogram",
+        index_col: str = "date",
         stats_functions=None,
-    ):
+    ) -> None:
         super().__init__()
         self.read_key = read_key
         self.store_key = store_key
 
         self.features = features or []
         self.ignore_features = ignore_features or []
         self.var_timestamp = var_timestamp or []
```

### Comparing `popmon-1.4.4/popmon/analysis/profiling/profiles.py` & `popmon-1.4.5/popmon/analysis/profiling/profiles.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/analysis/profiling/pull_calculator.py` & `popmon-1.4.5/popmon/analysis/profiling/pull_calculator.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,21 +48,21 @@
     def __init__(
         self,
         func_mean,
         func_std,
         apply_to_key,
         assign_to_key=None,
         store_key=None,
-        suffix_mean="_mean",
-        suffix_std="_std",
-        suffix_pull="_pull",
+        suffix_mean: str = "_mean",
+        suffix_std: str = "_std",
+        suffix_pull: str = "_pull",
         features=None,
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of HistComparer.
 
         :param str func_mean: applied-function to calculate mean of profiled statistics
         :param str func_std: applied-function to calculate std of profiled statistics
         :param str apply_to_key: key of the input data to apply funcs to.
         :param str assign_to_key: key of the input data to assign function applied-output to. (optional)
         :param str store_key: key of the output data to store in the datastore (optional)
@@ -105,23 +105,23 @@
 class RollingPullCalculator(PullCalculator):
     """Pull calculation based on rolling mean and standard deviations"""
 
     def __init__(
         self,
         read_key,
         window,
-        shift=1,
+        shift: int = 1,
         features=None,
         store_key=None,
-        suffix_mean="_roll_mean",
-        suffix_std="_roll_std",
-        suffix_pull="_roll_pull",
+        suffix_mean: str = "_roll_mean",
+        suffix_std: str = "_roll_std",
+        suffix_pull: str = "_roll_pull",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of HistComparer.
 
         :param str read_key: key of input data to read from data store
         :param int window: size of rolling window
         :param int shift: shift of the window, default is 1.
         :param list features: list of features to calculate pull for.
         :param str store_key: key of the output data to store in the datastore (optional)
@@ -157,23 +157,23 @@
 
 class ExpandingPullCalculator(PullCalculator):
     """Pull calculation based on expanding mean and standard deviations"""
 
     def __init__(
         self,
         read_key,
-        shift=1,
+        shift: int = 1,
         features=None,
         store_key=None,
-        suffix_mean="_exp_mean",
-        suffix_std="_exp_std",
-        suffix_pull="_exp_pull",
+        suffix_mean: str = "_exp_mean",
+        suffix_std: str = "_exp_std",
+        suffix_pull: str = "_exp_pull",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of HistComparer.
 
         :param str read_key: key of input data to read from data store
         :param int shift: shift of the window, default is 1.
         :param list features: list of features to calculate pull for. (optional)
         :param str store_key: key of the output data to store in the datastore (optional)
         :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
@@ -210,20 +210,20 @@
 
     def __init__(
         self,
         reference_key,
         assign_to_key,
         store_key=None,
         features=None,
-        suffix_mean="_ref_mean",
-        suffix_std="_ref_std",
-        suffix_pull="_ref_pull",
+        suffix_mean: str = "_ref_mean",
+        suffix_std: str = "_ref_std",
+        suffix_pull: str = "_ref_pull",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of HistComparer.
 
         :param str reference_key: key of input data to read from data store
         :param str assign_to_key: key of output data to store in data store
         :param str store_key: key of the output data to store in the datastore (optional)
         :param list features: list of features to calculate pull for. (optional)
         :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
@@ -260,20 +260,20 @@
 
     def __init__(
         self,
         reference_key,
         assign_to_key,
         store_key=None,
         features=None,
-        suffix_mean="_ref_mean",
-        suffix_std="_ref_std",
-        suffix_pull="_ref_pull",
+        suffix_mean: str = "_ref_mean",
+        suffix_std: str = "_ref_std",
+        suffix_pull: str = "_ref_pull",
         *args,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance of HistComparer.
 
         :param str reference_key: key of input data to read from data store
         :param str assign_to_key: key of output data to store in data store
         :param str store_key: key of the output data to store in the datastore (optional)
         :param list features: list of features to calculate pull for.
         :param str suffix_mean: suffix of mean. mean column = metric + suffix_mean
```

### Comparing `popmon-1.4.4/popmon/base/__init__.py` & `popmon-1.4.5/popmon/base/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/base/module.py` & `popmon-1.4.5/popmon/base/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+from __future__ import annotations
 
 import logging
 from abc import ABCMeta
 from functools import wraps
 
 
 def datastore_helper(func):
@@ -84,18 +85,18 @@
     name = "".join(a.__name__ for a in args)
     return type(name, args, {})
 
 
 class Module(metaclass=combine_classes(ABCMeta, ModuleMetaClass)):
     """Abstract base class used for modules in a pipeline."""
 
-    _input_keys = None
-    _output_keys = None
+    _input_keys: tuple[str, ...] | None = None
+    _output_keys: tuple[str, ...] | None = None
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Module initialization"""
         self.logger = logging.getLogger()
         self.features = []
         self.feature_begins_with = []
         self.ignore_features = []
 
     def _get_values(self, keys):
@@ -109,18 +110,18 @@
 
     def get_inputs(self):
         return self._get_values(self._input_keys)
 
     def get_outputs(self):
         return self._get_values(self._output_keys)
 
-    def get_description(self):
+    def get_description(self) -> str:
         return ""
 
-    def set_logger(self, logger):
+    def set_logger(self, logger) -> None:
         """Set logger of module
 
         :param logger: input logger
         """
         self.logger = logger
 
     @staticmethod
@@ -167,26 +168,26 @@
         ]
         for feature in features_not_in_input:
             self.logger.warning(f'Feature "{feature}" not in input data; skipping.')
 
         features = [feature for feature in features if feature in all_features]
         return features
 
-    def transform(self, *args):
+    def transform(self, *args, **kwargs):
         """Central function of the module.
 
         Typically transform() takes something from the datastore, does something to it, and puts the results
         back into the datastore again, to be passed on to the next module in the pipeline.
 
         :param dict datastore: input datastore
         :return: updated output datastore
         :rtype: dict
         """
         raise NotImplementedError
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """String representation for modules when printing a pipeline/list of modules"""
         name = self.__class__.__name__
         input_keys = [f"{v}='{getattr(self, v)}'" for v in self._input_keys]
         output_keys = [f"{v}='{getattr(self, v)}'" for v in self._output_keys]
         params = ", ".join(input_keys + output_keys)
         return f"{name}({params})"
```

### Comparing `popmon-1.4.4/popmon/base/pipeline.py` & `popmon-1.4.5/popmon/base/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 
 import logging
 
 
 class Pipeline:
     """Base class used for to run modules in a pipeline."""
 
-    def __init__(self, modules, logger: logging.Logger | None = None):
+    def __init__(self, modules, logger: logging.Logger | None = None) -> None:
         """Initialization of the pipeline
 
         :param list modules: modules of the pipeline.
         :param logger: logger to be used by each module.
         """
         self.modules = modules
         self.set_logger(logger)
 
-    def set_logger(self, logger: logging.Logger | None):
+    def set_logger(self, logger: logging.Logger | None) -> None:
         """Set the logger to be used by each module
 
         :param logger: input logger
         """
         self.logger = logger or logging.getLogger()
         for module in self.modules:
             module.set_logger(self.logger)
 
-    def add_modules(self, modules):
+    def add_modules(self, modules) -> None:
         """Add more modules to existing list of modules.
 
         :param list modules: list of more modules
         """
         if len(modules):
             self.modules.extend(modules)
 
@@ -63,15 +63,15 @@
         """
 
         for module in self.modules:
             self.logger.debug(f"transform {module.__class__.__name__}")
             datastore = module.transform(datastore)
         return datastore
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """String representation for pipeline"""
         name = self.__class__.__name__
         ret = f"{name}: [\n"
         for m in self.modules:
             ret += "\t" + str(m).replace("\n", "\n\t") + "\n"
         ret += "]"
         return ret
```

### Comparing `popmon-1.4.4/popmon/base/registry.py` & `popmon-1.4.5/popmon/base/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
 from collections import defaultdict
-from typing import Callable
+from typing import Any, Callable
 
 
 class Registry:
     _properties = ("dim", "htype")
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._keys: list[str] = []
         self._descriptions: dict[str, str] = {}
-        self._properties_to_func = defaultdict(lambda: defaultdict(dict))
-        self._func_name_to_properties = {}
+        self._properties_to_func: defaultdict[
+            str, defaultdict[str, dict[Any, Any]]
+        ] = defaultdict(lambda: defaultdict(dict))
+        self._func_name_to_properties: dict[Any, Any] = {}
 
     def register(
         self,
         key: str | list[str] | tuple[str],
         description: str | list[str] | tuple[str],
         dim: int = -1,
         htype: str | None = None,
```

### Comparing `popmon-1.4.4/popmon/config.py` & `popmon-1.4.5/popmon/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,27 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from histogrammar.dfinterface.make_histograms import get_time_axes
-from pydantic import BaseModel, BaseSettings
+from pydantic import BaseModel
+from pydantic_settings import BaseSettings
 from typing_extensions import Literal
 
 # Global configuration for the joblib parallelization. Could be used to change the number of jobs, and/or change
 # the backend from default (loki) to 'multiprocessing' or 'threading'.
 # (see https://joblib.readthedocs.io/en/latest/generated/joblib.Parallel.html for details)
 parallel_args = {"n_jobs": 1}
 
 
 class ValidatedSettings(BaseSettings):
     class Config:
-        validate_all = True
+        validate_default = True
         validate_assignment = True
 
 
 class SectionModel(BaseModel):
     name: str
     """Name of the section in the report"""
 
@@ -350,15 +351,15 @@
     In the bin specs for x:y, x is not provided (here) and reverts to the 1-dim setting.
     The 'bin_width', 'bin_offset' notation makes an open-ended histogram (for that feature) with given bin width
     and offset. The notation 'num', 'low', 'high' gives a fixed range histogram from 'low' to 'high' with 'num'
     number of bins.
     """
 
     # Config utilities
-    def _ensure_features_time_axis(self):
+    def _ensure_features_time_axis(self) -> None:
         self.features = [
             c if c.startswith(self.time_axis) else f"{self.time_axis}:{c}"
             for c in self.features
         ]
 
     def _set_time_axis_dataframe(self, df):
         time_axes = get_time_axes(df)
@@ -370,15 +371,15 @@
                 "No obvious time-axes found. Cannot generate stability report."
             )
         else:
             raise ValueError(
                 f"Found {num} time-axes: {time_axes}. Set *one* time_axis manually!"
             )
 
-    def _set_time_axis_hists(self, hists):
+    def _set_time_axis_hists(self, hists) -> None:
         # auto guess the time_axis: find the most frequent first column name in the histograms list
         first_cols = [k.split(":")[0] for k in list(hists.keys())]
         self.time_axis = max(set(first_cols), key=first_cols.count)
 
     def _set_bin_specs_by_time_width_and_offset(
         self, time_width: Union[str, int, float], time_offset: Union[str, int, float]
     ):
```

### Comparing `popmon-1.4.4/popmon/decorators/__init__.py` & `popmon-1.4.5/popmon/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/decorators/pandas.py` & `popmon-1.4.5/popmon/decorators/pandas.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/decorators/spark.py` & `popmon-1.4.5/popmon/decorators/spark.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/extensions/__init__.py` & `popmon-1.4.5/popmon/stats/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,12 +14,10 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from popmon.extensions.profile_diptest import Diptest
+from popmon.stats.numpy import mean, median, quantile, std
 
-extensions = [Diptest()]
-for extension in extensions:
-    extension.check()
+__all__ = ["mean", "std", "median", "quantile"]
```

### Comparing `popmon-1.4.4/popmon/extensions/extension.py` & `popmon-1.4.5/popmon/io/json_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
 from __future__ import annotations
 
-import importlib.util
-from typing import Callable
+import json
+from pathlib import Path
+
+from popmon.io import FileReader
+
+
+class JsonReader(FileReader):
+    """Read json file's contents into the datastore."""
+
+    def __init__(self, file_path: str | Path, store_key: str) -> None:
+        """Initialize an instance.
 
+        :param str store_key: key of input data to be stored in the datastore
+        :param str file_path: the file path to read the data from
+        """
+        super().__init__(store_key, file_path, apply_func=json.loads)
 
-def is_installed(package):
-    is_present = importlib.util.find_spec(package)
-    return is_present is not None
-
-
-class Extension:
-    name: str
-    extension: Callable
-    # should also be added to `pyproject.toml` optional-dependencies
-    requirements: list[str]
-
-    def check(self):
-        if all(is_installed(package) for package in self.requirements):
-            func = self.extension
-            func = func.__func__
-            func()
+    def transform(self, *args):
+        return super().transform.__wrapped__(self, *args)
```

### Comparing `popmon-1.4.4/popmon/extensions/profile_diptest.py` & `popmon-1.4.5/popmon/extensions/profile_diptest.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 """
 import numpy as np
 
 from popmon.analysis import Profiles
 from popmon.extensions.extension import Extension
 
 
-def extension():
+def extension() -> None:
     from diptest import diptest
 
     @Profiles.register(
         key=["diptest_value", "diptest_pvalue"],
         description=[
             "diptest value for Hartigan & Hartigan's test for unimodality",
             "p-value for the diptest",
@@ -64,8 +64,7 @@
         dip, pval = diptest(sample_noise)
         return dip, pval
 
 
 class Diptest(Extension):
     name = "diptest"
     extension = extension
-    requirements = ["diptest"]
```

### Comparing `popmon-1.4.4/popmon/hist/__init__.py` & `popmon-1.4.5/popmon/hist/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/hist/filling/__init__.py` & `popmon-1.4.5/popmon/hist/filling/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/hist/hist_splitter.py` & `popmon-1.4.5/popmon/hist/hist_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 
     def __init__(
         self,
         read_key,
         store_key,
         features=None,
         ignore_features=None,
-        feature_begins_with="",
-        project_on_axes=True,
-        flatten_output=False,
-        short_keys=True,
+        feature_begins_with: str = "",
+        project_on_axes: bool = True,
+        flatten_output: bool = False,
+        short_keys: bool = True,
         var_timestamp=None,
-        index_col="date",
-        hist_col="histogram",
-        filter_empty_split_hists=True,
-    ):
+        index_col: str = "date",
+        hist_col: str = "histogram",
+        filter_empty_split_hists: bool = True,
+    ) -> None:
         """Initialize an instance.
 
         :param str read_key: key of input histogram-dict to read from data store
         :param str store_key: key of output data to store in data store
         :param list features: features of histograms to pick up from input data (optional)
         :param list ignore_features: ignore list of features to compare with reference, if present (optional)
         :param str feature_begins_with: require feature to begin with a given string (optional)
@@ -86,15 +86,15 @@
         self.filter_empty_split_hists = filter_empty_split_hists
 
         if self.flatten_output and self.short_keys:
             raise ValueError(
                 "flatten_output requires short_keys attribute to be False."
             )
 
-    def get_description(self):
+    def get_description(self) -> str:
         return ""
 
     def update_divided(self, divided, split, yname):
         if self.flatten_output:
             divided.update(split)
         else:
             divided[yname] = [
```

### Comparing `popmon-1.4.4/popmon/hist/hist_utils.py` & `popmon-1.4.5/popmon/hist/hist_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     TwoDimensionallyHistogramMethods,
     SparselyTwoDimensionallyHistogramMethods,
 )
 
 HG_FACTORY = histogrammar.Factory()
 
 
-def sum_entries(hist, default=True):
+def sum_entries(hist, default: bool = True):
     """Recursively get sum of entries of histogram
 
     Sometimes hist.entries gives zero as answer? This function always works though.
 
     :param hist: input histogrammar histogram
     :param bool default: if false, do not use default HG method for evaluating entries, but exclude nans, of, uf.
     :return: total sum of entries of histogram
@@ -160,15 +160,15 @@
         # loop over all counters and integrate
         for bi in hist.values:
             h_proj += bi
 
     return h_proj
 
 
-def project_split2dhist_on_axis(splitdict, axis="x"):
+def project_split2dhist_on_axis(splitdict, axis: str = "x"):
     """Project a split 2d-histogram onto one axis
 
     Project a 2d hist that's been split with function split_hist_along_first_dimension
     onto x or y axis.
 
     :param dict splitdict: input split histogram to be projected.
     :param str axis: name of axis to project on, should be x or y. default is x.
@@ -242,19 +242,19 @@
     else:  # categorize
         centers, values = hist.bin_labels(), hist.values
     return centers, values
 
 
 def split_hist_along_first_dimension(
     hist,
-    xname="x",
-    yname="y",
-    short_keys=True,
-    convert_time_index=True,
-    filter_empty_split_hists=True,
+    xname: str = "x",
+    yname: str = "y",
+    short_keys: bool = True,
+    convert_time_index: bool = True,
+    filter_empty_split_hists: bool = True,
 ):
     """Split (multi-dimensional) hist into sub-hists along x-axis
 
     Function to split a (multi-dimensional) histogram into sub-histograms
     along the first dimension encountered.
 
     :param str xname: name of x-axis. default is x.
```

### Comparing `popmon-1.4.4/popmon/io/__init__.py` & `popmon-1.4.5/popmon/io/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/io/file_reader.py` & `popmon-1.4.5/popmon/io/file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     def __init__(
         self,
         store_key: str,
         file_path: str | Path,
         apply_func: Callable | None = None,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance.
 
         :param str store_key: key of input data to be stored in the datastore
         :param str file_path: the file path to read the data from
         :param callable apply_func: function to be used for the transformation of data (optional)
         :param dict kwargs: additional keyword arguments which would be passed to `apply_func`
         """
```

### Comparing `popmon-1.4.4/popmon/io/file_writer.py` & `popmon-1.4.5/popmon/io/file_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __init__(
         self,
         read_key: str,
         store_key: str | None = None,
         file_path: str | Path | None = None,
         apply_func: Callable | None = None,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance.
 
         :param str read_key: key of input histogram-dict to read from data store
         :param str store_key: key of output data to store in data store (optional)
         :param str file_path: the file path where to output the report (optional)
         :param callable apply_func: function to be used for the transformation of data (optional)
         :param dict kwargs: additional keyword arguments which would be passed to `apply_func`
```

### Comparing `popmon-1.4.4/popmon/io/json_reader.py` & `popmon-1.4.5/popmon/extensions/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,28 +13,11 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-from __future__ import annotations
 
-import json
-from pathlib import Path
+from popmon.extensions.profile_diptest import Diptest
 
-from popmon.io import FileReader
-
-
-class JsonReader(FileReader):
-    """Read json file's contents into the datastore."""
-
-    def __init__(self, file_path: str | Path, store_key: str):
-        """Initialize an instance.
-
-        :param str store_key: key of input data to be stored in the datastore
-        :param str file_path: the file path to read the data from
-        """
-        super().__init__(store_key, file_path, apply_func=json.loads)
-
-    def transform(self, *args):
-        return super().transform.__wrapped__(self, *args)
+extensions = [Diptest()]
```

### Comparing `popmon-1.4.4/popmon/notebooks/popmon_tutorial_advanced.ipynb` & `popmon-1.4.5/popmon/notebooks/popmon_tutorial_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/notebooks/popmon_tutorial_basic.ipynb` & `popmon-1.4.5/popmon/notebooks/popmon_tutorial_basic.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/notebooks/popmon_tutorial_incremental_data.ipynb` & `popmon-1.4.5/popmon/notebooks/popmon_tutorial_incremental_data.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/notebooks/popmon_tutorial_reports.ipynb` & `popmon-1.4.5/popmon/notebooks/popmon_tutorial_reports.ipynb`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/pipeline/__init__.py` & `popmon-1.4.5/popmon/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/pipeline/amazing_pipeline.py` & `popmon-1.4.5/popmon/pipeline/amazing_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 from popmon import Settings, resources
 from popmon.base import Pipeline
 from popmon.io import JsonReader
 from popmon.pipeline.report_pipelines import SelfReference
 
 
 class AmazingPipeline(Pipeline):
-    def __init__(self, histogram_path: str, **kwargs):
+    def __init__(self, histogram_path: str, **kwargs) -> None:
         modules = [
             JsonReader(file_path=histogram_path, store_key=kwargs["hists_key"]),
             # Or ExternalReference, RollingReference etc.
             SelfReference(**kwargs),
         ]
         super().__init__(modules)
 
 
-def run():
+def run() -> None:
     """Example that run self-reference pipeline and produces monitoring report"""
     logging.basicConfig(
         level=logging.INFO, format="%(asctime)s %(levelname)s [%(module)s]: %(message)s"
     )
 
     settings = Settings(time_axis="date")
     settings.comparison.window = 20
```

### Comparing `popmon-1.4.4/popmon/pipeline/dataset_splitter.py` & `popmon-1.4.5/popmon/pipeline/dataset_splitter.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/pipeline/metrics.py` & `popmon-1.4.5/popmon/pipeline/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,17 @@
         datastore["ref_hists"] = reference
 
     return pipeline.transform(datastore)
 
 
 def df_stability_metrics(
     df,
-    settings: Settings = None,
+    settings: Settings | None = None,
     time_width=None,
-    time_offset=0,
+    time_offset: int = 0,
     var_dtype=None,
     reference=None,
     **kwargs,
 ):
     """Create a data stability monitoring html datastore for given pandas or spark dataframe.
 
     :param df: input pandas/spark dataframe to be profiled and monitored over time.
```

### Comparing `popmon-1.4.4/popmon/pipeline/metrics_pipelines.py` & `popmon-1.4.5/popmon/pipeline/metrics_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     return _metrics_pipeline_register[reference_type]
 
 
 def create_metrics_pipeline(
     settings: Settings,
     reference=None,
-    hists_key="hists",
+    hists_key: str = "hists",
     **kwargs,
 ):
     # configuration and datastore for report pipeline
     cfg = {
         "hists_key": hists_key,
         "settings": settings,
         **kwargs,
@@ -210,15 +210,15 @@
 
 
 class SelfReferenceMetricsPipeline(Pipeline):
     def __init__(
         self,
         settings: Settings,
         hists_key,
-    ):
+    ) -> None:
         """Example metrics pipeline for comparing test data with itself (full test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled self reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
@@ -265,17 +265,17 @@
         super().__init__(modules)
 
 
 class ExternalReferenceMetricsPipeline(Pipeline):
     def __init__(
         self,
         settings: Settings,
-        hists_key="test_hists",
-        ref_hists_key="ref_hists",
-    ):
+        hists_key: str = "test_hists",
+        ref_hists_key: str = "ref_hists",
+    ) -> None:
         """Example metrics pipeline for comparing test data with other (full) external reference set
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :param str ref_hists_key: key to reference histograms in datastore. default is 'ref_hists'
         :return: assembled external reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
@@ -328,16 +328,16 @@
         super().__init__(modules)
 
 
 class RollingReferenceMetricsPipeline(Pipeline):
     def __init__(
         self,
         settings: Settings,
-        hists_key="test_hists",
-    ):
+        hists_key: str = "test_hists",
+    ) -> None:
         """Example metrics pipeline for comparing test data with itself (rolling test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled rolling reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
 
@@ -387,16 +387,16 @@
         super().__init__(modules)
 
 
 class ExpandingReferenceMetricsPipeline(Pipeline):
     def __init__(
         self,
         settings: Settings,
-        hists_key="test_hists",
-    ):
+        hists_key: str = "test_hists",
+    ) -> None:
         """Example metrics pipeline for comparing test data with itself (expanding test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled expanding reference pipeline
         """
         from popmon.analysis.comparison import Comparisons
```

### Comparing `popmon-1.4.4/popmon/pipeline/report.py` & `popmon-1.4.5/popmon/pipeline/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,17 @@
 
     stability_report_result = StabilityReport(datastore=result)
     return stability_report_result
 
 
 def df_stability_report(
     df,
-    settings: Settings = None,
+    settings: Settings | None | None = None,
     time_width=None,
-    time_offset=0,
+    time_offset: int = 0,
     var_dtype=None,
     reference=None,
     split=None,
     **kwargs,
 ):
     """Create a data stability monitoring html report for given pandas or spark dataframe.
 
@@ -206,15 +206,15 @@
     """Representation layer of the report.
 
     Stability report module wraps the representation functionality of the report
     after running the pipeline and generating the report. Report can be represented
     as a HTML string, HTML file or Jupyter notebook's cell output.
     """
 
-    def __init__(self, datastore, read_key="html_report"):
+    def __init__(self, datastore, read_key: str = "html_report") -> None:
         """Initialize an instance of StabilityReport.
 
         :param str read_key: key of HTML report data to read from data store. default is html_report.
         """
         self.read_key = read_key
         self.datastore = datastore
         self.logger = logging.getLogger()
@@ -228,40 +228,40 @@
 
         :return HTML: HTML report in an iframe
         """
         from IPython.core.display import display
 
         return display(self.to_notebook_iframe())
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Override so that Jupyter Notebook does not print the object."""
         return ""
 
-    def to_html(self, escape=False):
+    def to_html(self, escape: bool = False):
         """HTML code representation of the report (represented as a string).
 
         :param bool escape: escape characters which could conflict with other HTML code. default: False
         :return str: HTML code of the report
         """
 
         if escape:
             import html
 
             return html.escape(self.html_report)
         return self.html_report
 
-    def to_file(self, filename):
+    def to_file(self, filename) -> None:
         """Store HTML report in the local file system.
 
         :param str filename: filename for the HTML report
         """
         with open(filename, "w+") as file:
             file.write(self.to_html())
 
-    def to_notebook_iframe(self, width="100%", height="100%"):
+    def to_notebook_iframe(self, width: str = "100%", height: str = "100%"):
         """HTML representation of the class (report) embedded in an iframe.
 
         :param str width: width of the frame to be shown
         :param str height: height of the frame to be shown
         :return HTML: HTML report in an iframe
         """
         from IPython.core.display import HTML
@@ -276,15 +276,15 @@
             )
         )
 
     def regenerate(
         self,
         store_key: str = "html_report",
         sections_key: str = "report_sections",
-        settings: Settings = None,
+        settings: Settings | None = None,
     ):
         """Regenerate HTML report with different plot settings
         :param str sections_key: key to store sections data in the datastore. default is 'report_sections'.
         :param str store_key: key to store the HTML report data in the datastore. default is 'html_report'
         :param Settings settings: configuration to regenerate the report
         :return HTML: HTML report in an iframe
         """
```

### Comparing `popmon-1.4.4/popmon/pipeline/report_pipelines.py` & `popmon-1.4.5/popmon/pipeline/report_pipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 class SelfReference(Pipeline):
     def __init__(
         self,
         settings: Settings,
         hists_key: str = "test_hists",
-    ):
+    ) -> None:
         """Example pipeline for comparing test data with itself (full test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled self reference pipeline
         """
         modules = [
             SelfReferenceMetricsPipeline(
@@ -89,15 +89,15 @@
 
 class ExternalReference(Pipeline):
     def __init__(
         self,
         settings: Settings,
         hists_key: str = "test_hists",
         ref_hists_key: str = "ref_hists",
-    ):
+    ) -> None:
         """Example pipeline for comparing test data with other (full) external reference set
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :param str ref_hists_key: key to reference histograms in datastore. default is 'ref_hists'
         :return: assembled external reference pipeline
         """
 
@@ -118,15 +118,15 @@
 
 
 class RollingReference(Pipeline):
     def __init__(
         self,
         settings: Settings,
         hists_key: str = "test_hists",
-    ):
+    ) -> None:
         """Example pipeline for comparing test data with itself (rolling test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled rolling reference pipeline
         """
         modules = [
             RollingReferenceMetricsPipeline(
@@ -144,15 +144,15 @@
 
 
 class ExpandingReference(Pipeline):
     def __init__(
         self,
         settings: Settings,
         hists_key: str = "test_hists",
-    ):
+    ) -> None:
         """Example pipeline for comparing test data with itself (expanding test set)
 
         :param str hists_key: key to test histograms in datastore. default is 'test_hists'
         :return: assembled expanding reference pipeline
         """
         modules = [
             ExpandingReferenceMetricsPipeline(
@@ -173,15 +173,15 @@
     """Pipeline of modules for generating sections and a final report."""
 
     def __init__(
         self,
         settings: Settings,
         sections_key: str = "report_sections",
         store_key: str = "html_report",
-    ):
+    ) -> None:
         """Initialize an instance of Report.
 
         :param Settings settings: the configuration object
         :param str sections_key: key to store sections data in the datastore
         :param str store_key: key to store the HTML report data in the datastore
         """
         self.store_key = store_key
@@ -240,15 +240,15 @@
             # generate report
             ReportGenerator(
                 read_key=sections_key, store_key=store_key, settings=settings.report
             ),
         ]
         if (
             isinstance(settings.report.report_filepath, (str, Path))
-            and len(settings.report.report_filepath) > 0
+            and len(str(settings.report.report_filepath)) > 0
         ):
             modules.append(
                 FileWriter(store_key, file_path=settings.report.report_filepath)
             )
 
         super().__init__(modules=modules)
```

### Comparing `popmon-1.4.4/popmon/pipeline/timing.py` & `popmon-1.4.5/popmon/pipeline/timing.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _input_keys = ()
     _output_keys = ("store_key",)
 
     def __init__(
         self,
         store_key: str,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize an instance.
 
         :param str store_key: key of input data to be stored in the datastore
         """
         super().__init__()
 
         self.store_key = store_key
```

### Comparing `popmon-1.4.4/popmon/resources.py` & `popmon-1.4.5/popmon/resources.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/stats/__init__.py` & `popmon-1.4.5/popmon/extensions/extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,15 @@
 #
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+from __future__ import annotations
 
+from typing import Callable
 
-from popmon.stats.numpy import mean, median, quantile, std
 
-__all__ = ["mean", "std", "median", "quantile"]
+class Extension:
+    name: str
+    extension: Callable
```

### Comparing `popmon-1.4.4/popmon/stats/numpy.py` & `popmon-1.4.5/popmon/stats/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import numpy as np
 import pandas as pd
 
 
-def mean(a, weights=None, axis=None, dtype=None, keepdims=False, ddof=0):
+def mean(a, weights=None, axis=None, dtype=None, keepdims: bool = False, ddof: int = 0):
     """
     Compute the weighted mean along the specified axis.
 
     :param a: Array containing numbers whose mean is desired. If `a` is not an array, a conversion is attempted.
     :param weights: Array containing weights for the elements of `a`. If `weights` is not an
         array, a conversion is attempted.
     :param axis: Axis or axes along which the means are computed. The default is to
@@ -43,15 +43,15 @@
         w = np.array(weights)
 
         return np.sum(w * np.array(a), axis=axis, dtype=dtype, keepdims=keepdims) / (
             np.sum(w, axis=axis, dtype=dtype, keepdims=keepdims) - ddof
         )
 
 
-def std(a, weights=None, axis=None, dtype=None, ddof=0, keepdims=False):
+def std(a, weights=None, axis=None, dtype=None, ddof: int = 0, keepdims: bool = False):
     """
     Compute the weighted standard deviation along the specified axis.
 
     :param a: Array containing numbers whose standard deviation is desired. If `a` is not an
         array, a conversion is attempted.
     :param weights: Array containing weights for the elements of `a`. If `weights` is not an
         array, a conversion is attempted.
@@ -69,15 +69,15 @@
         return np.std(a, axis=axis, dtype=dtype, ddof=ddof, keepdims=keepdims)
     else:
         m = mean(a, weights=weights, axis=axis, keepdims=True)
         v = mean((a - m) ** 2, weights=weights, axis=axis, keepdims=keepdims, ddof=ddof)
         return np.sqrt(v)
 
 
-def median(a, weights=None, axis=None, keepdims=False):
+def median(a, weights=None, axis=None, keepdims: bool = False):
     """
     Compute the weighted median along the specified axis.
 
     After https://en.wikipedia.org/wiki/Percentile#Weighted_percentile
 
     :param a: Array containing numbers whose median is desired. If `a` is not an
         array, a conversion is attempted.
@@ -220,15 +220,15 @@
             else:
                 covariance_matrix[i][j] = -(prob[i] * prob[j]) / n_entries
                 covariance_matrix[j][i] = covariance_matrix[i][j]
 
     return covariance_matrix
 
 
-def mad(a, c=0.6745, axis=0):
+def mad(a, c=0.6745, axis: int = 0):
     """Median Absolute Deviation along given axis of an array
 
     mad = median(abs(a - median(a)))/c
 
     Copyright statsmodels:
     Kindly taken from statsmodels package and then modified to work with dataframes as well.
     Reference: https://www.statsmodels.org/dev/_modules/statsmodels/robust/scale.html#mad
```

### Comparing `popmon-1.4.4/popmon/stitching/__init__.py` & `popmon-1.4.5/popmon/stitching/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/stitching/hist_stitcher.py` & `popmon-1.4.5/popmon/stitching/hist_stitcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     """Module stitches histograms by date"""
 
     _input_keys = ("read_key", "delta_key")
     _output_keys = ("store_key",)
 
     def __init__(
         self,
-        mode="add",
+        mode: str = "add",
         time_axis=None,
         time_bin_idx=None,
         read_key=None,
         delta_key=None,
         store_key=None,
-    ):
+    ) -> None:
         """Stitching histograms by first axis.
 
         :param str mode: options for histogram stitching: "add" or "replace". default is "add".
         :param str time_axis: name of the first axis, to stitch on.
         :param str time_bin_idx: value of delta dataset used for stitching,
             in case delta or first dataset is a batch without time_axis. Should be an ordered string or integer.
         :param str read_key: key of input histogram-dict to read from data store.
@@ -60,15 +60,15 @@
         self.mode = mode
         self.time_axis = time_axis
         self.time_bin_idx = time_bin_idx
         self.allowed_modes = ["add", "replace"]
         if self.mode not in self.allowed_modes:
             raise ValueError("mode should be either 'add' or 'replace'")
 
-    def get_description(self):
+    def get_description(self) -> str:
         return f"{self.mode}"
 
     def transform(self, hists_basis: dict, hists_delta: dict) -> dict:
         self.logger.info(
             f'Stitching histograms "{self.read_key}" and "{self.delta_key}" as "{self.store_key}"'
         )
         stitched = self.stitch_histograms(self.mode, hists_basis, hists_delta)
@@ -76,15 +76,15 @@
 
     def stitch_histograms(
         self,
         mode=None,
         hists_basis=None,
         hists_delta=None,
         hists_list=None,
-        time_axis="",
+        time_axis: str = "",
         time_bin_idx=None,
     ):
         """Stitching histograms by first axis.
 
         Histograms in hists_delta are added to those in hists_basis. Bins are summed or replaced, set this with 'mode'.
         'time_axis' specifies the name of the first axis. If the time_axis is not found, it is created, and
         histograms get inserted the time_bin_idx values.
```

### Comparing `popmon-1.4.4/popmon/test_data/data_generator_hists.json.gz` & `popmon-1.4.5/popmon/test_data/data_generator_hists.json.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/test_data/example_histogram.json` & `popmon-1.4.5/popmon/test_data/example_histogram.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/test_data/flight_delays.csv.gz` & `popmon-1.4.5/popmon/test_data/flight_delays.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/test_data/flight_delays_reference.csv.gz` & `popmon-1.4.5/popmon/test_data/flight_delays_reference.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/test_data/synthetic_histograms.json` & `popmon-1.4.5/popmon/test_data/synthetic_histograms.json`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/test_data/test.csv.gz` & `popmon-1.4.5/popmon/test_data/test.csv.gz`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/utils.py` & `popmon-1.4.5/popmon/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             m
             for m in metrics
             if any(fnmatch.fnmatch(m, pattern) for pattern in show_stats)
         ]
     return metrics
 
 
-def parallel(func: Callable, args_list, mode="args"):
+def parallel(func: Callable, args_list, mode: str = "args"):
     """
     Routine for parallel processing
     """
     from popmon.config import parallel_args
 
     if parallel_args["n_jobs"] == 1:
         results = [
```

### Comparing `popmon-1.4.4/popmon/visualization/__init__.py` & `popmon-1.4.5/popmon/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/alert_section_generator.py` & `popmon-1.4.5/popmon/visualization/alert_section_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         read_key,
         store_key,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
-        prefix="traffic_light_",
+        prefix: str = "traffic_light_",
         suffices=None,
         ignore_stat_endswith=None,
-    ):
+    ) -> None:
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
         :param list ignore_features: ignore list of features, if present (optional)
         :param str static_bounds: key to static traffic light bounds key in datastore (optional)
```

### Comparing `popmon-1.4.4/popmon/visualization/histogram_section.py` & `popmon-1.4.5/popmon/visualization/histogram_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         read_key,
         store_key,
         reference_type: str,
         settings: HistogramSectionModel,
         features=None,
         ignore_features=None,
         hist_names=None,
-        hist_name_starts_with="histogram",
-    ):
+        hist_name_starts_with: str = "histogram",
+    ) -> None:
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
         :param list ignore_features: ignore list of features, if present (optional)
         :param list hist_names: list of histogram names to plot
@@ -183,18 +183,15 @@
             if len(histogram) > 0:
                 plot_type_layouts["histogram"] = histogram["layout"]
                 histogram = [histogram]
             else:
                 histogram = []
 
             # filter out potential empty heatmap plots, then prepend them to the sorted histograms
-            hplots = []
-            for h in heatmaps:
-                if isinstance(h, dict) and len(h["plot"]):
-                    hplots.append(h)
+            hplots = [h for h in heatmaps if isinstance(h, dict) and len(h["plot"])]
 
             if len(hplots) > 0:
                 plot_type_layouts["heatmap"] = hplots[0]["layout"]
 
             plots = hplots + histogram
 
             features_w_metrics.append(
@@ -211,15 +208,15 @@
                 "section_description": self.description,
                 "features": features_w_metrics,
             }
         )
         return sections
 
 
-def _plot_histograms(feature, date, hc_list, hist_names, top_n, max_nbins=1000):
+def _plot_histograms(feature, date, hc_list, hist_names, top_n, max_nbins: int = 1000):
     """Split off plot histogram generation to allow for parallel processing
 
     :param str feature: feature
     :param str date: date of time slot
     :param list hc_list: histogram list
     :param list hist_names: names of histograms to show as labels
     :param int max_nbins: maximum number of histogram bins allowed for plot (default 1000)
```

### Comparing `popmon-1.4.4/popmon/visualization/overview_section.py` & `popmon-1.4.5/popmon/visualization/overview_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         reference_type,
         time_axis,
         bin_specs,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
-        prefix="traffic_light_",
+        prefix: str = "traffic_light_",
         suffices=None,
         ignore_stat_endswith=None,
-    ):
+    ) -> None:
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
         :param list ignore_features: ignore list of features, if present (optional)
         :param str static_bounds: key to static traffic light bounds key in datastore (optional)
```

### Comparing `popmon-1.4.4/popmon/visualization/report_generator.py` & `popmon-1.4.5/popmon/visualization/report_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
     """This module takes already prepared section data, renders HTML section template with the data and
     glues sections together into one compressed report which is created based on the provided template.
     """
 
     _input_keys = ("read_key",)
     _output_keys = ("store_key",)
 
-    def __init__(self, read_key, store_key, settings: Report):
+    def __init__(self, read_key, store_key, settings: Report) -> None:
         """Initialize an instance of ReportGenerator.
 
         :param str read_key: key of input sections data to read from the datastore
         :param str store_key: key for storing the html report code in the datastore
         :para bool online_report: if false (default), the plotly.js code is included in the html report, else the report takes js code from cdn server which requires internet connection
         """
         super().__init__()
         self.read_key = read_key
         self.store_key = store_key
         self.title = settings.title
         self.online_report = settings.online_report
         self.tl_colors = settings.tl_colors
 
-    def get_description(self):
+    def get_description(self) -> str:
         return "HTML Report"
 
     def transform(self, sections: list) -> str:
         # concatenate HTML sections' code
         sections_html = ""
         for i, section_info in enumerate(sections):
             sections_html += templates_env(
```

### Comparing `popmon-1.4.4/popmon/visualization/section_generator.py` & `popmon-1.4.5/popmon/visualization/section_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "expanding": "all preceding time slots",
 }
 group_descriptions = {
     key: f"Comparing each time slot to {value}." for key, value in references.items()
 }
 
 
-def get_stat_description(name: str):
+def get_stat_description(name: str) -> str:
     """Gets the description of a statistic.
 
     :param str name: the name of the statistic.
 
     :returns str: the description of the statistic. If not found, returns an empty string
     """
     if not isinstance(name, str):
@@ -66,16 +66,16 @@
 
     if name in profiles:
         return profiles[name]
 
     if name in "mean_trend10_zscore":
         return "Significance of (rolling) trend in means of features"
 
-    head, *tail = name.split("_")
-    tail = "_".join(tail)
+    head, *tails = name.split("_")
+    tail = "_".join(tails)
 
     if tail in comparisons and head in references:
         return comparisons[tail]
 
     return ""
 
 
@@ -94,19 +94,19 @@
         store_key,
         section_name,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
-        prefix="traffic_light_",
+        prefix: str = "traffic_light_",
         suffices=None,
         ignore_stat_endswith=None,
-        description="",
-    ):
+        description: str = "",
+    ) -> None:
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param str section_name: key of output data to store in the datastore
         :param list features: list of features to pick up from input data (optional)
         :param list ignore_features: ignore list of features, if present (optional)
```

### Comparing `popmon-1.4.4/popmon/visualization/templates/aggregated-overview.html` & `popmon-1.4.5/popmon/visualization/templates/aggregated-overview.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/css/bootstrap.min.css` & `popmon-1.4.5/popmon/visualization/templates/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/css/custom-style.css` & `popmon-1.4.5/popmon/visualization/templates/assets/css/custom-style.css`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/custom-script.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/custom-script.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.easing.min.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.easing.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/jquery.min.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/plotly.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/plotly.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/assets/js/scrolling-nav.js` & `popmon-1.4.5/popmon/visualization/templates/assets/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/card.html` & `popmon-1.4.5/popmon/visualization/templates/card.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,28 @@
                 <p class="card-text">
                     {{metric.description}}
                 </p>
                 {%- endif -%}
         </div>
         <div id="{{ card_id }}"> </div>
         {%- if metric.type in ['traffic_light', 'alert'] -%}
-            {{ metric.plot }}
+            {{ metric.plot | safe }}
         {%- else -%}
             <div class="skeleton-loader" id="{{ card_id }}-loading"></div>
             <script>
             rendered["{{ card_id }}"] = false;
             render_func["{{ card_id }}"] = (function(){
                 var layout = deepCopy(layouts["{{ section_index }}{{ curr }}-{{ metric.type }}"]);
                 {%- if metric.shapes | length -%}
-                    layout["shapes"] = {{ metric.shapes | json_plot}};
+                    layout["shapes"] = {{ metric.shapes | json_plot | safe }};
                 {%- endif -%}
                 {%- if metric.yaxis_range | length -%}
-                    layout["yaxis"]["range"] = {{ metric.yaxis_range | json_plot }};
+                    layout["yaxis"]["range"] = {{ metric.yaxis_range | json_plot | safe }};
                 {%- endif -%}
-                Plotly.newPlot(document.getElementById("{{ card_id }}"), {{ metric.plot | json_plot }}, layout, plotly_config).then(function() { document.getElementById("{{ card_id }}-loading").remove(); rendered["{{ card_id }}"] = true;});
+                Plotly.newPlot(document.getElementById("{{ card_id }}"), {{ metric.plot | json_plot | safe }}, layout, plotly_config).then(function() { document.getElementById("{{ card_id }}-loading").remove(); rendered["{{ card_id }}"] = true;});
             });
 
             var io = new IntersectionObserver(function(entries) {
                 var entry = entries[0];
                 if(entry.isIntersecting === true && rendered["{{ card_id }}"] === false){
                     if(document.readyState === "complete"){
                         render_func["{{ card_id }}"]();
```

### Comparing `popmon-1.4.4/popmon/visualization/templates/core.html` & `popmon-1.4.5/popmon/visualization/templates/core.html`

 * *Files 8% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     {%- include 'modal-popup.html' -%}
     <script>
     var rendered = {};
     var layouts = {};
     var render_func = {};
     </script>
     {%- include 'header.html' -%}
-    {{ sections }}
+    {{ sections | safe }}
     {%- include 'footer.html' -%}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 
 
 
 
 {%- if online_report %}
  {%- endif -%}
 {%- include 'modal-popup.html' -%}
- {%- include 'header.html' -%} {{ sections }} {%- include 'footer.html' -%}
+ {%- include 'header.html' -%} {{ sections | safe }} {%- include 'footer.html'
+-%}
```

### Comparing `popmon-1.4.4/popmon/visualization/templates/footer.html` & `popmon-1.4.5/popmon/visualization/templates/footer.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/header.html` & `popmon-1.4.5/popmon/visualization/templates/header.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/modal-popup.html` & `popmon-1.4.5/popmon/visualization/templates/modal-popup.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/templates/section.html` & `popmon-1.4.5/popmon/visualization/templates/section.html`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       <div class="section-description">{{section_description}}</div><hr>
     {%- endif -%}
     {%- if features | length -%}
       {%- for feature in features -%}
         <script> 
           {%- set curr = loop.index  -%}
         {%- for plot_type, layout in feature.plot_type_layouts.items() -%}
-            layouts["{{ section_index }}{{ curr }}-{{ plot_type }}"] = {{ layout | json_plot }};
+            layouts["{{ section_index }}{{ curr }}-{{ plot_type }}"] = {{ layout | json_plot | safe }};
         {%- endfor -%}
         </script>
         <div class="section_feature" data-section-feature="{{ feature.name }}">
           {%- if feature.plots is mapping -%}
             {%- for ref, plots in feature.plots.items() -%}
               <h3> {{ feature.titles.get(ref, ref) }} </h3>
               <div class="section-description">{{ feature.descriptions[ref] }}</div>
@@ -53,15 +53,15 @@
         </div>
       {%- endfor -%}
     {%- else -%}
         <div class="row" >
             {%- for metric in plots -%}
               <script> 
                 {%- set curr = loop.index  -%}
-                layouts["{{ section_index }}{{ curr }}-{{ metric.type }}"] = {{ metric.layout | json_plot }};
+                layouts["{{ section_index }}{{ curr }}-{{ metric.type }}"] = {{ metric.layout | json_plot | safe }};
               </script>
               {%- with metric=metric -%}
                 {%- include 'card.html' -%}
               {%- endwith -%}
             {%- endfor -%}
         </div>
     {%- endif -%}
```

### Comparing `popmon-1.4.4/popmon/visualization/templates/table.html` & `popmon-1.4.5/popmon/visualization/templates/table.html`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/popmon/visualization/traffic_light_section_generator.py` & `popmon-1.4.5/popmon/visualization/traffic_light_section_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,18 @@
         read_key,
         store_key,
         settings: Report,
         features=None,
         ignore_features=None,
         static_bounds=None,
         dynamic_bounds=None,
-        prefix="traffic_light_",
+        prefix: str = "traffic_light_",
         suffices=None,
         ignore_stat_endswith=None,
-    ):
+    ) -> None:
         """Initialize an instance of SectionGenerator.
 
         :param str read_key: key of input data to read from the datastore and use for plotting
         :param str store_key: key for output data to be stored in the datastore
         :param list features: list of features to pick up from input data (optional)
         :param list ignore_features: ignore list of features, if present (optional)
         :param str static_bounds: key to static traffic light bounds key in datastore (optional)
@@ -169,15 +169,15 @@
     metrics,
     dates,
     df,
     last_n,
     skip_first_n,
     skip_last_n,
     tl_colors,
-    style="heatmap",
+    style: str = "heatmap",
 ):
     # prune dates and values
     dates = _prune(dates, last_n, skip_first_n, skip_last_n)
 
     values = [
         _prune(df[metric], last_n, skip_first_n, skip_last_n) for metric in metrics
     ]
```

### Comparing `popmon-1.4.4/popmon/visualization/utils.py` & `popmon-1.4.5/popmon/visualization/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         logger.debug("unable to plot boundaries")
 
     plot = json.loads(fig.to_json())
     return plot
 
 
 def plot_traffic_lights_overview(feature, data, metrics: list[str], labels: list[str]):
-    colors = defaultdict(dict)
+    colors: defaultdict[str, dict[str, list[str]]] = defaultdict(dict)
     color_map = ["g", "y", "r"]
     for c1, metric in enumerate(metrics):
         for c2, label in enumerate(labels):
             colors[metric][label] = [color_map[data[c1][c2]]]
 
     return templates_env(
         "table.html",
@@ -361,15 +361,15 @@
     metrics = ["# green", "# yellow", "# red"]
     data = data.astype(int)
 
     green = hex_to_rgb(tl_colors["green"])
     yellow = hex_to_rgb(tl_colors["yellow"])
     red = hex_to_rgb(tl_colors["red"])
 
-    colors = defaultdict(dict)
+    colors: defaultdict[str, dict[str, list[str]]] = defaultdict(dict)
     for c1, metric in enumerate(metrics):
         row_max = np.max(data[c1])
         for c2, label in enumerate(labels):
             a = np.round(data[c1][c2] / row_max, 2) if row_max and row_max != 0 else 0
             if metric.endswith("green"):
                 background_rgba = (*green, a)
             elif metric.endswith("yellow"):
@@ -433,19 +433,19 @@
                 assert len(labels) == len(
                     values
                 ), f'labels and values have different array lengths: {len(labels):d} vs {len(values):d}. {plot["feature"]}'
 
 
 def plot_histogram_overlay(
     plots=None,
-    is_num=True,
-    is_ts=False,
-    is_static_reference=True,
-    top=20,
-    n_choices=2,
+    is_num: bool = True,
+    is_ts: bool = False,
+    is_static_reference: bool = True,
+    top: int = 20,
+    n_choices: int = 2,
 ):
     """Create and plot (overlapping/grouped) histogram(s) of column values.
 
     Copyright Eskapade:
     Kindly taken from Eskapade package and then modified. Reference link:
     https://github.com/KaveIO/Eskapade/blob/master/python/eskapade/visualization/vis_utils.py#L397
     License: https://github.com/KaveIO/Eskapade-Core/blob/master/LICENSE
@@ -792,15 +792,15 @@
         "name": hist_name,
         "type": "heatmap",
         "plot": plot["data"],
         "layout": plot["layout"],
     }
 
 
-def _prune(values, last_n=0, skip_first_n=0, skip_last_n=0):
+def _prune(values, last_n: int = 0, skip_first_n: int = 0, skip_last_n: int = 0):
     """inline function to select first or last items of input list
 
     :param values: input list to select from
     :param int last_n: select last 'n' items of values. default is 0.
     :param int skip_first_n: skip first n items of values. default is 0. last_n takes precedence.
     :param int skip_last_n: in plot skip last 'n' periods. last_n takes precedence (optional)
     :return: list of selected values
```

### Comparing `popmon-1.4.4/popmon.egg-info/PKG-INFO` & `popmon-1.4.5/popmon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popmon
-Version: 1.4.4
+Version: 1.4.5
 Summary: Monitor the stability of a pandas or spark dataset
 Author-email: ING Analytics Wholesale Banking <wbaa@ing.com>
 License: Copyright 2023 ING Analytics Wholesale Banking
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the Software without restriction, including without limitation
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and
```

### Comparing `popmon-1.4.4/popmon.egg-info/SOURCES.txt` & `popmon-1.4.5/popmon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popmon-1.4.4/pyproject.toml` & `popmon-1.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     "histogrammar>=1.0.32",
     "phik",
     "jinja2",
     "tqdm",
     "plotly>=5.8.0",
     "joblib>=0.14.0",
     "htmlmin",
-    "pydantic",
+    "pydantic>=2",
+    "pydantic-settings",
     "typing_extensions"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
@@ -71,15 +72,15 @@
 [project.scripts]
 popmon_run = "popmon.pipeline.amazing_pipeline:run"
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 namespace-packages = ["popmon"]
-select = ["ALL"]
+select = ["ALL", "CPY001"]
 ignore = [
     # COM812 is incompatible with COM819
     "COM",
 
     # Not sure if these are helpful
     "EM",
     "FBT",
@@ -101,14 +102,18 @@
     "PD901",
     "PLC1901",
     "PLR0912",
     "PLR0913",
     "TRY003",
     "E501",
     "DTZ",
+    "PERF203", #  `try`-`except` within a loop incurs performance overhead
+
+    # False positive
+    "PERF401", # Use a list comprehension to create a transformed list
 
     # Prefer autofix
     "PD011", # .to_numpy() instead of values
     "PD003", # `.isna` is preferred to `.isnull`; functionality is equivalent
     "PT018", # Assertion should be broken down into multiple parts
     "RET504", # Unnecessary variable assignment before `return` statement
     "RET506", # Unnecessary `else` after `raise` statement
@@ -135,26 +140,35 @@
     "E741",
     # implicit namespaces
     "INP001",
     # broad exceptions
     "PT011",
     # Too many statements
     "PLR0915",
+    # Copyright
+    "CPY001",
 ]
 
 # Sphinx config
 "docs/source/conf.py" = ["A001", "ARG001"]
 
 # Example
 "examples/*" = [
     # Print statement
     "T201",
 
     # implicit namespaces
     "INP001",
+
+    # Copyright
+    "CPY001",
+]
+
+"popmon/config.py" = [
+    "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar`
 ]
 
 # Notebooks & NBQA
 "popmon/notebooks/*" = [
     # Imports cannot be checked properly with NBQA
     # (It splits each cell into a .py file)
     "INP001", "E401", "E402", "F401", "I001",
@@ -163,18 +177,25 @@
      "T201",
 
     # Ignore magic value in comparison for now
     "PLR2004",
 
     # Found useless expression. Either assign it to a variable or remove it.
     "B018",
+
+    # Copyright
+    "CPY001",
 ]
 
+[tool.ruff.flake8-copyright]
+notice-rgx = """(?mis)Copyright \\(c\\) 2023 ING Analytics Wholesale Banking.+"""
+
 [tool.pytest.ini_options]
 markers = ["spark"]
+#filterwarnings = ["error"]
 
 [tool.pytest.ini_options.spark_options]
 "spark.executor.id" = "driver"
 "spark.app.name" = "PySparkShell"
 "spark.executor.instances" = 1
 "master" = "local[*]"
 "spark.driver.host" = "192.168.1.78"
```

