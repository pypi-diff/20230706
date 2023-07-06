# Comparing `tmp/veta-0.7.7.tar.gz` & `tmp/veta-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veta-0.7.7.tar", last modified: Sun Jun  4 20:58:26 2023, max compression
+gzip compressed data, was "veta-0.7.8.tar", last modified: Thu Jul  6 21:53:05 2023, max compression
```

## Comparing `veta-0.7.7.tar` & `veta-0.7.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.973071 veta-0.7.7/
--rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.7/.gitignore
--rw-r--r--   0 pbarbosa   (503) staff       (20)      600 2023-01-13 02:44:49.000000 veta-0.7.7/Dockerfile
--rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.7/LICENSE
--rw-r--r--   0 pbarbosa   (503) staff       (20)    35110 2023-06-04 20:58:26.971825 veta-0.7.7/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34977 2023-06-04 20:46:42.000000 veta-0.7.7/README.md
--rw-r--r--   0 pbarbosa   (503) staff       (20)      484 2022-12-30 18:52:40.000000 veta-0.7.7/conda_environment.yml
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-06-04 20:46:42.000000 veta-0.7.7/pyproject.toml
--rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-06-04 20:58:26.973418 veta-0.7.7/setup.cfg
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.836107 veta-0.7.7/src/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    24480 2023-06-04 20:46:42.000000 veta-0.7.7/src/base.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22309 2023-01-13 02:18:40.000000 veta-0.7.7/src/benchmark.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.838228 veta-0.7.7/src/config/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.7/src/config/__init__.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.913746 veta-0.7.7/src/config/example_imgs/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/.gitkeep
--rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/benchmark_af.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/benchmark_dist.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/benchmark_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/benchmark_thresholds.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/heatmap.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/inspect_ratios.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/inspect_ratios2.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/logo.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/ml_fi.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/ml_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/pearson_corr.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.7/src/config/example_imgs/per_bin_score.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.7/src/config/example_imgs/per_bin_score_split_ss.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/roc_analysis.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/roc_curves.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1381 2023-06-04 20:46:42.000000 veta-0.7.7/src/config/tools_config.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)    14407 2023-04-28 14:55:43.000000 veta-0.7.7/src/interrogate.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.933590 veta-0.7.7/src/plots/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/plots/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    23298 2023-05-17 14:26:55.000000 veta-0.7.7/src/plots/plots_benchmark_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     8896 2023-04-28 14:55:43.000000 veta-0.7.7/src/plots/plots_interrogate_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15452 2023-02-08 17:08:39.000000 veta-0.7.7/src/plots/plots_intronic_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.7/src/plots/plots_machine_learning.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.7/src/plots/plots_threshold_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.7/src/plots/plots_utils.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.950294 veta-0.7.7/src/predictions/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/predictions/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2023-05-24 00:01:45.000000 veta-0.7.7/src/predictions/apply.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     9481 2023-06-04 20:46:42.000000 veta-0.7.7/src/predictions/filters.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    16825 2022-12-30 18:52:40.000000 veta-0.7.7/src/predictions/introns.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    21143 2023-06-04 20:46:42.000000 veta-0.7.7/src/predictions/metapredictions.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2022-08-25 13:25:47.000000 veta-0.7.7/src/predictions/metrics.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2022-12-29 18:11:14.000000 veta-0.7.7/src/predictions/thresholds.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.7/src/predictions/utils_classifiers.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.963503 veta-0.7.7/src/preprocessing/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/preprocessing/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.7/src/preprocessing/clinvar.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2023-06-04 20:46:42.000000 veta-0.7.7/src/preprocessing/location.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.7/src/preprocessing/osutils.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.7/src/preprocessing/tables.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22802 2023-06-04 20:46:42.000000 veta-0.7.7/src/preprocessing/utils_tools.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.7/src/preprocessing/vcf.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.969899 veta-0.7.7/src/veta.egg-info/
--rw-r--r--   0 pbarbosa   (503) staff       (20)    35110 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/SOURCES.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/dependency_links.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/entry_points.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/requires.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/top_level.txt
--rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.7/src/veta.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.259320 veta-0.7.8/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.8/.gitignore
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1185 2023-07-06 21:34:31.000000 veta-0.7.8/Dockerfile
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.8/LICENSE
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35063 2023-07-06 21:53:05.258794 veta-0.7.8/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    34932 2023-07-03 10:02:42.000000 veta-0.7.8/README.md
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      466 2023-07-06 15:59:29.000000 veta-0.7.8/conda_environment.yml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-07-06 15:57:07.000000 veta-0.7.8/pyproject.toml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-07-06 21:53:05.259415 veta-0.7.8/setup.cfg
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.198739 veta-0.7.8/src/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.8/src/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    24480 2023-06-04 20:46:42.000000 veta-0.7.8/src/base.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22297 2023-07-06 12:32:48.000000 veta-0.7.8/src/benchmark.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.200188 veta-0.7.8/src/config/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.8/src/config/__init__.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.233758 veta-0.7.8/src/config/example_imgs/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/.gitkeep
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/benchmark_af.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/benchmark_dist.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.8/src/config/example_imgs/benchmark_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.8/src/config/example_imgs/benchmark_thresholds.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/heatmap.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/inspect_ratios.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.8/src/config/example_imgs/inspect_ratios2.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/logo.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/ml_fi.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/ml_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/pearson_corr.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.8/src/config/example_imgs/per_bin_score.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.8/src/config/example_imgs/per_bin_score_split_ss.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.8/src/config/example_imgs/roc_analysis.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.8/src/config/example_imgs/roc_curves.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1381 2023-06-04 20:46:42.000000 veta-0.7.8/src/config/tools_config.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    14407 2023-04-28 14:55:43.000000 veta-0.7.8/src/interrogate.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.242216 veta-0.7.8/src/plots/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.8/src/plots/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    23271 2023-07-06 14:36:25.000000 veta-0.7.8/src/plots/plots_benchmark_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     8896 2023-04-28 14:55:43.000000 veta-0.7.8/src/plots/plots_interrogate_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15443 2023-07-06 14:58:36.000000 veta-0.7.8/src/plots/plots_intronic_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.8/src/plots/plots_machine_learning.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.8/src/plots/plots_threshold_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.8/src/plots/plots_utils.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.248969 veta-0.7.8/src/predictions/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.8/src/predictions/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2023-05-24 00:01:45.000000 veta-0.7.8/src/predictions/apply.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     9481 2023-06-04 20:46:42.000000 veta-0.7.8/src/predictions/filters.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    16796 2023-07-06 12:34:49.000000 veta-0.7.8/src/predictions/introns.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    21143 2023-06-04 20:46:42.000000 veta-0.7.8/src/predictions/metapredictions.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2023-07-06 12:32:25.000000 veta-0.7.8/src/predictions/metrics.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2023-07-06 09:43:19.000000 veta-0.7.8/src/predictions/thresholds.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.8/src/predictions/utils_classifiers.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.254505 veta-0.7.8/src/preprocessing/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.8/src/preprocessing/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.8/src/preprocessing/clinvar.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2023-06-04 20:46:42.000000 veta-0.7.8/src/preprocessing/location.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.8/src/preprocessing/osutils.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.8/src/preprocessing/tables.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22802 2023-06-04 20:46:42.000000 veta-0.7.8/src/preprocessing/utils_tools.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.8/src/preprocessing/vcf.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-07-06 21:53:05.258029 veta-0.7.8/src/veta.egg-info/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35063 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/SOURCES.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/dependency_links.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/entry_points.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/requires.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-07-06 21:53:05.000000 veta-0.7.8/src/veta.egg-info/top_level.txt
+-rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.8/src/veta.py
```

### Comparing `veta-0.7.7/LICENSE` & `veta-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/PKG-INFO` & `veta-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.7
+Version: 0.7.8
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
@@ -30,14 +30,18 @@
    * It does not run any model/prediction tool within the package. 
    * It does not annotate VCFs. For that you have [VEP](https://www.ensembl.org/info/docs/tools/vep/index.html), [vcfanno](https://github.com/brentp/vcfanno) or [bcftools annotate](http://samtools.github.io/bcftools/bcftools.html). 
 
 **Citing VETA:**
 
    * Paper: [Clinical significance of genetic variation in hypertrophic cardiomyopathy: comparison of computational tools to prioritize missense variants.](https://www.frontiersin.org/articles/10.3389/fcvm.2022.975478/full). The analysis performed with VETA for the paper is stored in a [jupyter notebook](https://github.com/PedroBarbosa/paper_HCM_benchmark/blob/main/run_benchmarks.ipynb), where multiple running examples are presented.
 
+**Contact:**
+
+psbpedrobarbosa@gmail.com\
+pbarbosa@lasige.di.fc.ul.pt
 
 # Table of Contents
 - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Input requirements](#input-requirements)
   - [Running on reference datasets](#running-on-reference-datasets)
     - [Clinvar](#clinvar)
@@ -344,9 +348,7 @@
 
 <a name="AF"></a>
 ### Note on allele frequency
 
 If the input data has a field that somehow measures allele frequency, that information can be taken into account by VETA by additionally plotting allele frequencies between the variants belonging to each label (benchmark mode, figure below). For example, if gnomAD frequencies are represented in the VCF with the `gnomAD_AF` INFO field, one can set the `--allele_frequency gnomAD_AF` so that information is included in the analysis. More info in the help: ```veta benchmark --help```. If the analysis is done with a Clinvar file and `AF*` is not present in the output, try to delete the `tsv` file a redo analysis from the original VCF file.
 
 <img src="src/config/example_imgs/benchmark_af.png" height="300"/>
-
-If you find bugs or have suggestions, feel free to get in touch  psbpedrobarbosa@gmail.com or by opening an issue.
```

### Comparing `veta-0.7.7/README.md` & `veta-0.7.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,18 @@
    * It does not run any model/prediction tool within the package. 
    * It does not annotate VCFs. For that you have [VEP](https://www.ensembl.org/info/docs/tools/vep/index.html), [vcfanno](https://github.com/brentp/vcfanno) or [bcftools annotate](http://samtools.github.io/bcftools/bcftools.html). 
 
 **Citing VETA:**
 
    * Paper: [Clinical significance of genetic variation in hypertrophic cardiomyopathy: comparison of computational tools to prioritize missense variants.](https://www.frontiersin.org/articles/10.3389/fcvm.2022.975478/full). The analysis performed with VETA for the paper is stored in a [jupyter notebook](https://github.com/PedroBarbosa/paper_HCM_benchmark/blob/main/run_benchmarks.ipynb), where multiple running examples are presented.
 
+**Contact:**
+
+psbpedrobarbosa@gmail.com\
+pbarbosa@lasige.di.fc.ul.pt
 
 # Table of Contents
 - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Input requirements](#input-requirements)
   - [Running on reference datasets](#running-on-reference-datasets)
     - [Clinvar](#clinvar)
@@ -331,9 +335,7 @@
 
 <a name="AF"></a>
 ### Note on allele frequency
 
 If the input data has a field that somehow measures allele frequency, that information can be taken into account by VETA by additionally plotting allele frequencies between the variants belonging to each label (benchmark mode, figure below). For example, if gnomAD frequencies are represented in the VCF with the `gnomAD_AF` INFO field, one can set the `--allele_frequency gnomAD_AF` so that information is included in the analysis. More info in the help: ```veta benchmark --help```. If the analysis is done with a Clinvar file and `AF*` is not present in the output, try to delete the `tsv` file a redo analysis from the original VCF file.
 
 <img src="src/config/example_imgs/benchmark_af.png" height="300"/>
-
-If you find bugs or have suggestions, feel free to get in touch  psbpedrobarbosa@gmail.com or by opening an issue.
```

### Comparing `veta-0.7.7/pyproject.toml` & `veta-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "veta"
 description = "Simple variant prediction evaluation"
 authors = [
     {name = "Pedro Barbosa", email = "psbpedrobarbosa@gmail.com"},
 ]
 
-version = "0.7.7"
+version = "0.7.8"
 readme = "README.md"
 requires-python = "~=3.8"
 dependencies = [
     "matplotlib==3.5.1",
     "numpy==1.23.5",
     "pandas==1.4.2",
     "seaborn==0.11.2",
```

### Comparing `veta-0.7.7/src/base.py` & `veta-0.7.8/src/base.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/benchmark.py` & `veta-0.7.8/src/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
                     except KeyError:
                         pass
                 
                 stats_all_df = pd.DataFrame(statistics)
     
                 if roc_metrics_per_tool:
                     roc_m = pd.DataFrame([[x[0], x[-1]] for x in roc_metrics_per_tool], columns=['tool', 'auROC'])
-                    pr_m = pd.DataFrame([[x[0], x[-1]] for x in pr_metrics_per_tool], columns=['tool', 'average_precision'])
+                    pr_m = pd.DataFrame([[x[0], x[-1]] for x in pr_metrics_per_tool], columns=['tool', 'auPRC'])
                     stats_all_df = stats_all_df.merge(roc_m, on='tool', how='left').merge(pr_m, on='tool', how='left')
 
                 # draw plots
                 out_stats = os.path.join(outdir, "results_tsv", "statistics_{}_{}.tsv").format(var_type, _location)
                 out_ranks = os.path.join(outdir, "results_tsv", "tools_ranking_{}_{}.tsv").format(var_type, _location)
 
                 af_plot = os.path.join(outdir, "allele_frequency", "AF_{}_{}.pdf".format(var_type, _location))
```

### Comparing `veta-0.7.7/src/config/example_imgs/benchmark_af.png` & `veta-0.7.8/src/config/example_imgs/benchmark_af.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/benchmark_dist.png` & `veta-0.7.8/src/config/example_imgs/benchmark_dist.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/benchmark_performance.png` & `veta-0.7.8/src/config/example_imgs/benchmark_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/benchmark_thresholds.png` & `veta-0.7.8/src/config/example_imgs/benchmark_thresholds.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/heatmap.png` & `veta-0.7.8/src/config/example_imgs/heatmap.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/inspect_ratios.png` & `veta-0.7.8/src/config/example_imgs/inspect_ratios.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/inspect_ratios2.png` & `veta-0.7.8/src/config/example_imgs/inspect_ratios2.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/logo.png` & `veta-0.7.8/src/config/example_imgs/logo.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/ml_fi.png` & `veta-0.7.8/src/config/example_imgs/ml_fi.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/ml_performance.png` & `veta-0.7.8/src/config/example_imgs/ml_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/pearson_corr.png` & `veta-0.7.8/src/config/example_imgs/pearson_corr.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/per_bin_score.png` & `veta-0.7.8/src/config/example_imgs/per_bin_score.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/per_bin_score_split_ss.png` & `veta-0.7.8/src/config/example_imgs/per_bin_score_split_ss.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/roc_analysis.png` & `veta-0.7.8/src/config/example_imgs/roc_analysis.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/example_imgs/roc_curves.png` & `veta-0.7.8/src/config/example_imgs/roc_curves.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/config/tools_config.txt` & `veta-0.7.8/src/config/tools_config.txt`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/interrogate.py` & `veta-0.7.8/src/interrogate.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/plots/plots_benchmark_mode.py` & `veta-0.7.8/src/plots/plots_benchmark_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,46 +513,46 @@
     os.makedirs(os.path.dirname(fname), exist_ok=True)
  
     data = [x for x in data if len(x) > 0]
     
     if data:
         if is_roc:
             colnames = ['tool', 'fraction_nan', 'label', 'thresholds', 'True Positive Rate (TPR)',
-                        'False Positive Rate (FPR)', 'roc_auc']
+                        'False Positive Rate (FPR)', 'auROC']
             to_explode = ['thresholds', 'True Positive Rate (TPR)', 'False Positive Rate (FPR)']
         else:
-            colnames = ['tool', 'fraction_nan', 'label', 'thresholds', 'Recall', 'Precision', 'ap_score']
+            colnames = ['tool', 'fraction_nan', 'label', 'thresholds', 'Recall', 'Precision', 'auPRC']
             to_explode = ['thresholds', 'Recall', 'Precision']
 
         df_metrics = pd.DataFrame.from_records(data, columns=colnames)
         df_metrics = df_metrics[df_metrics.thresholds.notna()]
         df_metrics = df_metrics.explode(to_explode).reset_index()
 
         if is_roc:
             df_metrics['True Positive Rate (TPR)'] = pd.to_numeric(df_metrics['True Positive Rate (TPR)'])
             df_metrics['False Positive Rate (FPR)'] = pd.to_numeric(df_metrics['False Positive Rate (FPR)'])
-            df_metrics["tool_with_roc_auc"] = df_metrics["label"] + " auROC=" + \
-                                            df_metrics["roc_auc"].round(3).map(str) + ")"
-            hue = "tool_with_roc_auc"
+            df_metrics["tool_with_auROC"] = df_metrics["label"] + " auROC=" + \
+                                            df_metrics["auROC"].round(3).map(str) + ")"
+            hue = "tool_with_auROC"
             x = "False Positive Rate (FPR)"
             y = "True Positive Rate (TPR)"
-            df_metrics = df_metrics.sort_values('roc_auc', ascending=False)
+            df_metrics = df_metrics.sort_values('auROC', ascending=False)
             
             no_min_scored = df_metrics[df_metrics['fraction_nan'] > max_nan_allowed].tool.unique().tolist()
             if no_min_scored:
                 logging.info('ROC curves will not be drawn for the following tool(s) (more than {} fraction of missing predictions): {}'.format(max_nan_allowed, ','.join(no_min_scored)))
         else:
             df_metrics['Recall'] = pd.to_numeric(df_metrics['Recall'])
             df_metrics['Precision'] = pd.to_numeric(df_metrics['Precision'])
-            df_metrics["tool_with_ap_score"] = df_metrics["label"] + " AP=" + \
-                                            df_metrics["ap_score"].round(3).map(str) + ")"
-            hue = "tool_with_ap_score"
+            df_metrics["tool_with_auPRC"] = df_metrics["label"] + " auPRC=" + \
+                                            df_metrics["auPRC"].round(3).map(str) + ")"
+            hue = "tool_with_auPRC"
             x = "Recall"
             y = "Precision"
-            df_metrics = df_metrics.sort_values('ap_score', ascending=False)
+            df_metrics = df_metrics.sort_values('auPRC', ascending=False)
 
         df_metrics = df_metrics[df_metrics['fraction_nan'] <= max_nan_allowed]
 
         # Since S-CAP has several different reference
         # threshold, S-CAP is removed from these analyses
         df_metrics = df_metrics[~df_metrics.tool.str.contains("S-CAP")]
 
@@ -577,15 +577,15 @@
         plt.ylim(0, 1.05)
         plt.tight_layout()
 
         plt.savefig(fname, bbox_inches='tight')
         plt.close()
         sns.reset_defaults()
         
-        _metric = 'roc_auc' if is_roc else 'ap_score'   
+        _metric = 'auROC' if is_roc else 'auPRC'   
         df_metrics = df_metrics[['tool', _metric]].drop_duplicates()
         return dict(zip(df_metrics.tool, df_metrics[_metric])) 
 
 ###############################
 ## Heatmap related functions ##
 ###############################
 GT_LABEL = '(*)True labels'
```

### Comparing `veta-0.7.7/src/plots/plots_interrogate_mode.py` & `veta-0.7.8/src/plots/plots_interrogate_mode.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/plots/plots_intronic_analysis.py` & `veta-0.7.8/src/plots/plots_intronic_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -302,44 +302,44 @@
     bins_with_scores = df.bin.unique().tolist()
 
     bins_to_exclude = ['1-2', '3-10'] if aggregate_classes else ['1-10']
     bins_to_exclude.extend(["all_intronic", "all_except_1-2", "all_except_1-10"])
     variant_class = df.name
     
     df['fraction_scored'] = 1 - df.fraction_nan
-    df['weighted_roc_auc'] = df.apply(lambda x: None if x.roc_auc is None else x.fraction_scored * x.roc_auc, axis = 1)
-    df['weighted_ap_score'] = df.apply(lambda x: None if x.ap_score is None else x.fraction_scored * x.ap_score, axis = 1)
+    df['weighted_auROC'] = df.apply(lambda x: None if x.auROC is None else x.fraction_scored * x.auROC, axis = 1)
+    df['weighted_auPRC'] = df.apply(lambda x: None if x.auPRC is None else x.fraction_scored * x.auPRC, axis = 1)
     
     # Keep only tools with auc and ap scores in all bins
-    na_rows = df.loc[df.isnull()['weighted_roc_auc'] | df.isnull()['weighted_ap_score']]
+    na_rows = df.loc[df.isnull()['weighted_auROC'] | df.isnull()['weighted_auPRC']]
     tools_to_remove = na_rows.tool.unique()
     
     _df = df[~df.tool.isin(tools_to_remove)]
-    _avg = _df.groupby('tool').agg({'weighted_roc_auc': 'mean',
-                                   'weighted_ap_score': 'mean'})
-    _avg = _avg.rename(columns={'weighted_roc_auc': 'avg_weighted_roc_auc_all_bins',
-                                'weighted_ap_score': 'avg_weighted_ap_score_all_bins'})
+    _avg = _df.groupby('tool').agg({'weighted_auROC': 'mean',
+                                   'weighted_auPRC': 'mean'})
+    _avg = _avg.rename(columns={'weighted_auROC': 'avg_weighted_auROC_all_bins',
+                                'weighted_auPRC': 'avg_weighted_auPRC_all_bins'})
     
     metrics = {"F1": "F1_Score",
                "weighted_F1": "F1 score (weighted)",
                "fraction_scored": "Fraction scored",
-               "roc_auc": "auROC",
-               "weighted_roc_auc": "auROC (weighted)",
-               "weighted_roc_auc_all_bins": "auROC (weighted)",
-               "ap_score": "Average precision",
-               "weighted_ap_score": "Average precision (weighted)",
-               "weighted_ap_score_all_bins": "Average precision (weighted)"}
+               "auROC": "area under ROC curve",
+               "weighted_auROC": "area under ROC curve (weighted)",
+               "weighted_auROC_all_bins": "area under ROC curve (weighted)",
+               "auPRC": "area under PR curve",
+               "weighted_auPRC": "area under PR curve (weighted)",
+               "weighted_auPRC_all_bins": "area under PR curve (weighted)"}
     
     avg = df.groupby('tool').agg({'F1':'mean',
                              'weighted_F1': 'mean',
                              'fraction_scored': 'mean',
-                             'roc_auc': 'mean',
-                             'ap_score': 'mean',
-                             'weighted_roc_auc': 'mean',
-                             'weighted_ap_score': 'mean'})
+                             'auROC': 'mean',
+                             'auPRC': 'mean',
+                             'weighted_auROC': 'mean',
+                             'weighted_auPRC': 'mean'})
     
     avg = avg.round(3)
     avg.columns = ["avg_{}".format(x) for x in avg.columns]
     df = pd.merge(df, avg, on="tool", how='left').merge(_avg, on='tool', how='left')
 
     n_tools = df.tool.unique().size 
     if n_tools > 10:
```

### Comparing `veta-0.7.7/src/plots/plots_machine_learning.py` & `veta-0.7.8/src/plots/plots_machine_learning.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/plots/plots_threshold_analysis.py` & `veta-0.7.8/src/plots/plots_threshold_analysis.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/plots/plots_utils.py` & `veta-0.7.8/src/plots/plots_utils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/apply.py` & `veta-0.7.8/src/predictions/apply.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/filters.py` & `veta-0.7.8/src/predictions/filters.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/introns.py` & `veta-0.7.8/src/predictions/introns.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,31 +432,31 @@
             
             if roc_m:
                 stats_df = pd.merge(stats_df, pd.DataFrame.from_dict(roc_m, orient='index', columns=['auROC']), how = 'left', left_on = 'tool', right_index = True)
             else:
                 stats_df['auROC'] = None
             
             if pr_m:
-                stats_df = pd.merge(stats_df, pd.DataFrame.from_dict(pr_m, orient='index', columns=['average_precision']), how = 'left', left_on = 'tool', right_index = True)
+                stats_df = pd.merge(stats_df, pd.DataFrame.from_dict(pr_m, orient='index', columns=['auPRC']), how = 'left', left_on = 'tool', right_index = True)
             else:
-                stats_df['average_precision'] = None
+                stats_df['auPRC'] = None
 
             stats_df.drop(["filter"], axis=1).to_csv(stats_out, sep="\t", index=False)
             
         df_metrics_per_bin = pd.DataFrame(
             [[k] + i for k, v in self.metrics_per_bin.items() for i in v],
             columns=[
                 "tool",
                 "variant_class",
                 "bin",
                 "F1",
                 "weighted_F1",
                 "fraction_nan",
-                "roc_auc",
-                "ap_score"
+                "auROC",
+                "auPRC"
             ],
         )
 
         df_metrics_per_bin.groupby("variant_class").apply(
             plot_metrics_by_bin,
             os.path.join(out_all_bin_agg, "per_bin"),
             self.aggregate_classes,
```

### Comparing `veta-0.7.7/src/predictions/metapredictions.py` & `veta-0.7.8/src/predictions/metapredictions.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/metrics.py` & `veta-0.7.8/src/predictions/metrics.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/thresholds.py` & `veta-0.7.8/src/predictions/thresholds.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/predictions/utils_classifiers.py` & `veta-0.7.8/src/predictions/utils_classifiers.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/clinvar.py` & `veta-0.7.8/src/preprocessing/clinvar.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/location.py` & `veta-0.7.8/src/preprocessing/location.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/osutils.py` & `veta-0.7.8/src/preprocessing/osutils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/tables.py` & `veta-0.7.8/src/preprocessing/tables.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/utils_tools.py` & `veta-0.7.8/src/preprocessing/utils_tools.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/preprocessing/vcf.py` & `veta-0.7.8/src/preprocessing/vcf.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/veta.egg-info/PKG-INFO` & `veta-0.7.8/src/veta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.7
+Version: 0.7.8
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
@@ -30,14 +30,18 @@
    * It does not run any model/prediction tool within the package. 
    * It does not annotate VCFs. For that you have [VEP](https://www.ensembl.org/info/docs/tools/vep/index.html), [vcfanno](https://github.com/brentp/vcfanno) or [bcftools annotate](http://samtools.github.io/bcftools/bcftools.html). 
 
 **Citing VETA:**
 
    * Paper: [Clinical significance of genetic variation in hypertrophic cardiomyopathy: comparison of computational tools to prioritize missense variants.](https://www.frontiersin.org/articles/10.3389/fcvm.2022.975478/full). The analysis performed with VETA for the paper is stored in a [jupyter notebook](https://github.com/PedroBarbosa/paper_HCM_benchmark/blob/main/run_benchmarks.ipynb), where multiple running examples are presented.
 
+**Contact:**
+
+psbpedrobarbosa@gmail.com\
+pbarbosa@lasige.di.fc.ul.pt
 
 # Table of Contents
 - [Table of Contents](#table-of-contents)
   - [Installation](#installation)
   - [Input requirements](#input-requirements)
   - [Running on reference datasets](#running-on-reference-datasets)
     - [Clinvar](#clinvar)
@@ -344,9 +348,7 @@
 
 <a name="AF"></a>
 ### Note on allele frequency
 
 If the input data has a field that somehow measures allele frequency, that information can be taken into account by VETA by additionally plotting allele frequencies between the variants belonging to each label (benchmark mode, figure below). For example, if gnomAD frequencies are represented in the VCF with the `gnomAD_AF` INFO field, one can set the `--allele_frequency gnomAD_AF` so that information is included in the analysis. More info in the help: ```veta benchmark --help```. If the analysis is done with a Clinvar file and `AF*` is not present in the output, try to delete the `tsv` file a redo analysis from the original VCF file.
 
 <img src="src/config/example_imgs/benchmark_af.png" height="300"/>
-
-If you find bugs or have suggestions, feel free to get in touch  psbpedrobarbosa@gmail.com or by opening an issue.
```

### Comparing `veta-0.7.7/src/veta.egg-info/SOURCES.txt` & `veta-0.7.8/src/veta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veta-0.7.7/src/veta.py` & `veta-0.7.8/src/veta.py`

 * *Files identical despite different names*

