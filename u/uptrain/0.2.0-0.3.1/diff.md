# Comparing `tmp/uptrain-0.2.0.tar.gz` & `tmp/uptrain-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.2.0.tar", last modified: Mon May 15 17:53:03 2023, max compression
+gzip compressed data, was "uptrain-0.3.1.tar", last modified: Thu Jul  6 12:10:56 2023, max compression
```

## Comparing `uptrain-0.2.0.tar` & `uptrain-0.3.1.tar`

### file list

```diff
@@ -1,124 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.568987 uptrain-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 17:52:49.000000 uptrain-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-05-15 17:53:03.568987 uptrain-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-05-15 17:52:49.000000 uptrain-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 17:53:03.568987 uptrain-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-15 17:52:49.000000 uptrain-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.548987 uptrain-0.2.0/uptrain/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.548987 uptrain-0.2.0/uptrain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.548987 uptrain-0.2.0/uptrain/core/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.552987 uptrain-0.2.0/uptrain/core/classes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/algorithms/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/algorithms/popularity_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.552987 uptrain-0.2.0/uptrain/core/classes/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/abstract_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/cosine_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/distance_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/hamming_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/l2_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/distances/norm_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.552987 uptrain-0.2.0/uptrain/core/classes/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/finetuning/AbstractFinetune.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/finetuning/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18145 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.552987 uptrain-0.2.0/uptrain/core/classes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/helpers/annotation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/helpers/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/helpers/dataset_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/helpers/model_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.556987 uptrain-0.2.0/uptrain/core/classes/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/log_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/new_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/new_st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/new_st_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/logging/st_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.556987 uptrain-0.2.0/uptrain/core/classes/managers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/managers/check_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.556987 uptrain-0.2.0/uptrain/core/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/abstract_measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/feature_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/input_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/measurable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/output_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/recommendation_hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/measurables/scalar_from_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.560987 uptrain-0.2.0/uptrain/core/classes/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/abstract_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/abstract_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/edge_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/model_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/monitors/output_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.560987 uptrain-0.2.0/uptrain/core/classes/signals/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/signals/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.560987 uptrain-0.2.0/uptrain/core/classes/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/abstract_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/norm_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/statistics/old_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/core/classes/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/abstract_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/classes/visuals/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/core/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/encoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/core/lib/model_signal_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/ee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/ee/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/ee/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/classes/measurables/llm_measurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/ee/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/ee/lib/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.564987 uptrain-0.2.0/uptrain/io/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/io/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-15 17:52:49.000000 uptrain-0.2.0/uptrain/io/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:53:03.548987 uptrain-0.2.0/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-05-15 17:53:03.000000 uptrain-0.2.0/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-15 17:53:03.000000 uptrain-0.2.0/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:53:03.000000 uptrain-0.2.0/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-15 17:53:03.000000 uptrain-0.2.0/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 17:53:03.000000 uptrain-0.2.0/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.043221 uptrain-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 12:10:43.000000 uptrain-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-06 12:10:56.043221 uptrain-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-07-06 12:10:43.000000 uptrain-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/regression_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/regression_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-06 12:10:43.000000 uptrain-0.3.1/regression_testing/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:10:56.043221 uptrain-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-06 12:10:43.000000 uptrain-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-06 12:10:43.000000 uptrain-0.3.1/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/uptrain/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/dashboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/dashboard/st_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/dashboard/st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/dashboard/st_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/uptrain/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/framework/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/operators/code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/code/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/operators/code/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/code/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/code/sql/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/code/sql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/embs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/operators/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/io/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/operators/language/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/model_grade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/openai_evals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/language/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/operators/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/utilities/sql_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/utilities/sqlglot_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.027221 uptrain-0.3.1/uptrain/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/algorithms/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/algorithms/popularity_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/abstract_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/cosine_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/distance_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/hamming_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/l2_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/distances/norm_ratio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/finetuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/finetuning/AbstractFinetune.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/finetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/finetuning/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/helpers/annotation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/helpers/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/helpers/dataset_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/helpers/model_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.031221 uptrain-0.3.1/uptrain/v0/core/classes/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/io/runtime_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.035221 uptrain-0.3.1/uptrain/v0/core/classes/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/log_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/log_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/new_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/new_st_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/new_st_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/logging/st_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.035221 uptrain-0.3.1/uptrain/v0/core/classes/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/managers/check_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.035221 uptrain-0.3.1/uptrain/v0/core/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/abstract_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/feature_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/input_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/measurable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/output_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/measurables/scalar_from_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.035221 uptrain-0.3.1/uptrain/v0/core/classes/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/abstract_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/abstract_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/edge_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/feature_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/model_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/monitors/output_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/core/classes/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/signals/signal_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/core/classes/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/abstract_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/norm_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/statistics/old_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/core/classes/visuals/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/abstract_visual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/classes/visuals/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/core/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/encoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/core/lib/model_signal_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/ee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/ee/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/ee/classes/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/classes/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/classes/measurables/llm_measurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.039221 uptrain-0.3.1/uptrain/v0/ee/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/lib/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-06 12:10:43.000000 uptrain-0.3.1/uptrain/v0/ee/lib/ops_agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.023221 uptrain-0.3.1/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-06 12:10:56.000000 uptrain-0.3.1/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-06 12:10:56.000000 uptrain-0.3.1/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:10:56.000000 uptrain-0.3.1/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-06 12:10:56.000000 uptrain-0.3.1/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-06 12:10:56.000000 uptrain-0.3.1/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:56.043221 uptrain-0.3.1/validation_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 12:10:43.000000 uptrain-0.3.1/validation_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 12:10:43.000000 uptrain-0.3.1/validation_wrapper/validation_manager.py
```

### Comparing `uptrain-0.2.0/LICENSE` & `uptrain-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/PKG-INFO` & `uptrain-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-Metadata-Version: 2.1
-Name: uptrain
-Version: 0.2.0
-Summary: UpTrain - ML Observability and Retraining Framework
-Home-page: https://github.com/uptrain-ai/uptrain
-Maintainer: UpTrain AI Team
-Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0
-Keywords: uptrain ai retraining ML observability
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
 <h2>
   <p align="center">
-    <p align="center">An open-source framework to observe ML applications, built for engineers</p>
+    <p align="center">An open-source framework to evaluate, test and monitor LLM applications</p>
   </p>
 </h2>
 
 <p align="center">
 <a href="https://docs.uptrain.ai/docs/" rel="nofollow"><strong>Docs</strong></a>
+<!-- -
+<a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a> -->
 -
-<a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a>
--
-<a href="https://discord.com/invite/gVvZhhrQaQ/" rel="nofollow"><strong>Discord Community</strong></a>
+<a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg" rel="nofollow"><strong>Slack Community</strong></a>
 -
 <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=bug&template=bug_report.md&title=" rel="nofollow"><strong>Bug Report</strong></a>
 -
 <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=" rel="nofollow"><strong>Feature Request</strong></a>
 </p>
 
 <h4 align="center">
@@ -47,145 +27,148 @@
   </a>
   <a href='https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md'>
     <img alt='PRs Welcome' src='https://img.shields.io/badge/PRs-welcome-orange.svg?style=shields'/>
   </a>
   <a href="https://docs.uptrain.ai/docs/">
     <img src="https://img.shields.io/badge/Read-Docs-brightgreen" alt="Docs" />
   </a>
-  <a href="https://discord.com/invite/gVvZhhrQaQ">
-    <img src="https://img.shields.io/badge/Discord-Community-orange" alt="Community" />
+  <a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg">
+    <img src="https://img.shields.io/badge/Slack-Community-orange" alt="Community" />
   </a>
   <a href="https://uptrain.ai/">
     <img src="https://img.shields.io/badge/UpTrain-Website-yellow" alt="Website" />
   </a>
-  <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/">
+  <!-- <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/">
     <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-  </a>
+  </a> -->
 </h4>
 
-https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-4be1-83cf-408d5271518e.mp4
+<!-- https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-4be1-83cf-408d5271518e.mp4 -->
 
-**Read this in other languages**: 
+<!-- **Read this in other languages**: 
 <kbd>[<img title="English" alt="English language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/us.svg" width="22">](/README.md)</kbd>
 <kbd>[<img title="German" alt="German language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/de.svg" width="22">](/i18n/README.de.md)</kbd>
 <kbd>[<img title="Chinese" alt="Chinese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/cn.svg" width="22">](/i18n/README.zh-CN.md)</kbd>
 <kbd>[<img title="Hindi" alt="Hindi language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/in.svg" width="22">](/i18n/README.hi.md)</kbd>
 <kbd>[<img title="Spanish" alt="Spanish language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/es.svg" width="22">](/i18n/README.es.md)</kbd>
 <kbd>[<img title="French" alt="French language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/fr.svg" width="22">](/i18n/README.fr.md)</kbd>
 <kbd>[<img title="Japanese" alt="Japanese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/jp.svg" width="22">](/i18n/README.ja.md)</kbd>
-<kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd>
+<kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd> -->
 
 
-**[UpTrain](https://uptrain.ai)** is an open-source, data-secure tool for ML practitioners to observe and refine their ML models by monitoring their performance, checking for (data) distribution shifts, and collecting edge cases to retrain them upon. It integrates seamlessly with your existing production pipelines and takes minutes to get started ⚡.
+**[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM applications are performing reliably by allowing users to check aspects such as correctness, structural integrity, bias, hallucination, etc. UpTrain can be used to:
 
+1) Validate model's response and safeguard your users against hallucinations, bias, incorrect output formats, etc.
+2) Experiment across multiple model providers, prompt templates, and quantify model's performance.
+3) Monitor your model's performance in production and protect yourself against unwanted drifts
 
-# **[Key Features](https://uptrain.gitbook.io/docs/what-is-uptrain/key-features)** 💡
 
-- **[Data Drift Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-drift)** - Identify distribution shifts in your model inputs.
-- **[Performance Monitoring](https://docs.uptrain.ai/docs/uptrain-monitors/concept-drift)** - Track the performance of your models in realtime and get degradation alerts.
-- **[Embeddings Support](https://github.com/uptrain-ai/uptrain/blob/main/examples/text_summarization/run.ipynb)** - Specialized dashboards to understand model-inferred embeddings.
-- **[Edge Case Signals](https://docs.uptrain.ai/docs/uptrain-monitors/edge-case-detection)** - User-defined signals and statistical techniques to detect out-of-distribution data-points.
-- **[Data Integrity Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-integrity)** - Checks for missing or inconsistent data, duplicate records, data quality, etc. 
-- **[Customizable metrics](https://docs.uptrain.ai/docs/monitoring-custom-metrics)** - Define custom metrics that make sense for your use case.
-- **[Automated Retraining](https://github.com/uptrain-ai/uptrain/blob/main/examples/human_orientation_classification/deepdive_examples/uptrain_check_all.ipynb)** - Automate model retraining by attaching your training and inference pipelines.
-- **[Model Bias](https://docs.uptrain.ai/docs/uptrain-monitors/model-bias)** - Track bias in your ML model's predictions.
-- **[AI Explainability](https://docs.uptrain.ai/docs/uptrain-visuals/shap-explainability)** - Understand relative importance of multiple features on predictions.
-- **Data Security** - Your data never goes out of your machine.
-- **Slack Integration** - Get alerts on Slack.
-- **Realtime Dashboards** - To visualize your model's health live.
-
-## 🚨Coming soon🚨
-
-- **Label Shift** - Identify drifts in your predictions. Specially useful in cases when ground truth is unavailable.
-- **Model confidence interval** - Confidence intervals for model predictions 
-- **Advanced drift detection techniques** - Outlier-based drift detection methods
-- **Advanced feature slicing** - Ability to slice statistical properties
-- **Kolmogorov-Smirnov Test** - For detecting distribution shifts
-- **Prediction Stability** - Filter cases where model prediction is not stable.
-- **Adversarial Checks** - Combat adversarial attacks
+# Key Features 💡
 
-And more.
 
+- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
+- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
+- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
+- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
+- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
+- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
+- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
+- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
+- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
+- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
 
 # Get started 🙌
 
-You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F).
+<!-- You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). -->
 
-To run it in your machine, follow the steps below:
+To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
 ### Install the package through pip:
-```console
+```bash
 pip install uptrain
 ```
 
-### Run your first example:
-```console
-git clone git@github.com:uptrain-ai/uptrain.git
-cd uptrain/examples
-pip install jupyterlab
-jupyter lab
+### How to define checks:
+Say we want to check whether our model's responses contain any grammatical mistakes or not.
+
+```python
+# Define your checkset - list of simple checks, dataset file, 
+# and api_keys
+
+checkset = CheckSet(
+    checks = Check(
+        name = "grammar_score",
+        operators = [
+            GrammarScore(
+                col_in_text = "model_response",
+                col_out = "grammar_score"
+            ),
+        ],
+        plots = PlotlyChart.Table(title="Grammar scores"),
+    ),
+    source = JsonReader(fpath = '...')
+)
+settings = Settings(openai_api_key = '...')
+
+checkset.setup(settings)
+checkset.run()
 ```
 
-For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial).
+<!-- For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial). -->
 
 <h4> </h4>
 
-# UpTrain in [action](https://github.com/uptrain-ai/uptrain/blob/main/examples/text_summarization/run.ipynb) 🎬
+# Integrations
 
-One of the most common use cases of ML today is language models, be it text summarization, NER, chatbots, language translation, etc. UpTrain provides ways to visualize differences in the training and real-world data via UMAP clustering of text embeddings (inferred from BERT). Following are some replays from the UpTrain dashboard.
+| Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | 
+| ------------- | ------------- | ------------- | ------------- | 
+| OpenAI Evals ✅ | GPT-3.5-turbo ✅ | Langchain 🔜 | HuggingFace 🔜 |
+| EleutherAI LM Eval 🔜 | GPT-4 ✅  | Llama Index 🔜 |  Replicate 🔜 |
+| BIG-Bench 🔜 | Claude 🔜 | AutoGPT 🔜 |
+| | Cohere 🔜 | 
 
-### AI Explainability out-of-the-box
 
-<h1 align="center">
-<img alt="umap_gif" width="60%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/ride_estimation/4_Explanability_recording.gif">
-</h1>
+# UpTrain in Action
 
-### Live Model Performance Monitoring and Data Integrity Checks
+## Experimentation
 
-<h1 align="center">
-<img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/fraud_detection/concept_drift_avg_acc.gif"> <img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/finetuning_llms/data_integrity.gif">
-</h1>
+You can use the UpTrain framework to run and compare LLM responses for different prompts, models, LLM chains, etc. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
 
-### UMAP Dimensionality Reduction and Visualization
+## Validation
 
-<h1 align="center">
-<img alt="umap_gif" width="60%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/text_summarization/umap.gif">
-</h1>
+You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
 
+## Monitoring
 
-### Edge-case Collection for Finetuning the Model later
+You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
 
-<h1 align="center">
-<img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/finetuning_llms/edge_cases.gif">
-</h1>
 
 # Why UpTrain 🤔?
 
-Machine learning (ML) models are widely used to make critical business decisions. Still, no ML model is 100% accurate, and, further, their accuracy deteriorates over time 😣. For example, Sales prediction becomes inaccurate over time due to a shift in consumer buying habits. Additionally, due to the black box nature of ML models, it's challenging to identify and fix their problems.
+Large language models are trained over billions of data points and perform really well over a wide variety of tasks. But one thing these models are not good at is being deterministic. Even with the most well-crafted prompts, the model can misbehave for certain inputs, be it hallucinations, wrong output structure, toxic or biased response, irrelevant response, and error modes can be immense. 
 
-UpTrain solves this. We make it easy for data scientists and ML engineers to understand where their models are going wrong and help them fix them before others complain 🗣️.
+To ensure your LLM applications work reliably and correctly, UpTrain makes it easy for developers to evaluate the responses of their applications on multiple criteria. UpTrain's evaluation framework can be used to:
 
-UpTrain can be used for a wide variety of Machine learning models such as LLMs, recommendation models, prediction models, Computer vision models, etc.
+1) Validate (and correct) the response of the model before showing it to the user
+2) Get quantitative measures to experiment across multiple prompts, model providers, etc.
+3) Do unit testing to ensure no buggy prompt or code gets pushed into your production
+4) Monitor your LLM applications in real time and understand when they are going wrong in order to fix them before users complain.
 
 We are constantly working to make UpTrain better. Want a new feature or need any integrations? Feel free to [create an issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the repository.
 
-<h1 align="center">
-<img alt="Meme" width="40%" src="https://user-images.githubusercontent.com/108270398/215209245-4d6b1f47-7af9-4db8-8d8c-63dcc610571c.jpg">
-</h1>
-
 # License 💻
 
-This repo is published under Apache 2.0 license, with the exception of the ee directory which will contain premium features requiring an enterprise license in the future. We're currently focused on developing non-enterprise offerings that should cover most use cases by adding more features and extending to more models. We also working towards adding a hosted offering - [contact us](mailto:tech@uptrain.ai) if you are interested.
+This repo is published under Apache 2.0 license. We are also working towards adding a hosted offering to make setting off eval runs easier - please fill **[this form](https://docs.google.com/forms/d/e/1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/viewform?usp=sf_link)** to get a waitlist slot.
 
 # Stay Updated ☎️
 We are continuously adding tons of features and use cases. Please support us by giving the project a star ⭐!
 
 # Provide feedback (Harsher the better 😉) 
 
-We are building UpTrain in public. Help us improve by giving your feedback **[here](https://forms.gle/PXd89D5LiFubro9o9)**.
+We are building UpTrain in public. Help us improve by giving your feedback **[here](https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**.
 
 # Contributors 🖥️
 
 We welcome contributions to UpTrain. Please see our [contribution guide](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for details.
 
 <a href="https://github.com/uptrain-ai/uptrain/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=uptrain-ai/uptrain" />
```

#### html2text {}

```diff
@@ -1,110 +1,88 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.2.0 Summary: UpTrain - ML
-Observability and Retraining Framework Home-page: https://github.com/uptrain-
-ai/uptrain Maintainer: UpTrain AI Team Maintainer-email: uptrain.ai@gmail.com
-License: Apache License 2.0 Keywords: uptrain ai retraining ML observability
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
                                *** [uptrain] ***
-***** An open-source framework to observe ML applications, built for engineers
+***** An open-source framework to evaluate, test and monitor LLM applications
 *****
-     Docs - Try_it_out - Discord_Community - Bug_Report - Feature_Request
+            Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
-           Welcome] [Docs] [Community] [Website] [Open_In_Colab] ***
-https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-
-4be1-83cf-408d5271518e.mp4 **Read this in other languages**: [[English
-language]](/README.md) [[German language]](/i18n/README.de.md) [[Chinese
-language]](/i18n/README.zh-CN.md) [[Hindi language]](/i18n/README.hi.md) [
-[Spanish language]](/i18n/README.es.md) [[French language]](/i18n/README.fr.md)
-[[Japanese language]](/i18n/README.ja.md) [[Russian language]](/i18n/
-README.ru.md) **[UpTrain](https://uptrain.ai)** is an open-source, data-secure
-tool for ML practitioners to observe and refine their ML models by monitoring
-their performance, checking for (data) distribution shifts, and collecting edge
-cases to retrain them upon. It integrates seamlessly with your existing
-production pipelines and takes minutes to get started â¡. # **[Key Features]
-(https://uptrain.gitbook.io/docs/what-is-uptrain/key-features)** ð¡ - **[Data
-Drift Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-drift)** -
-Identify distribution shifts in your model inputs. - **[Performance Monitoring]
-(https://docs.uptrain.ai/docs/uptrain-monitors/concept-drift)** - Track the
-performance of your models in realtime and get degradation alerts. - **
-[Embeddings Support](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-text_summarization/run.ipynb)** - Specialized dashboards to understand model-
-inferred embeddings. - **[Edge Case Signals](https://docs.uptrain.ai/docs/
-uptrain-monitors/edge-case-detection)** - User-defined signals and statistical
-techniques to detect out-of-distribution data-points. - **[Data Integrity
-Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-integrity)** -
-Checks for missing or inconsistent data, duplicate records, data quality, etc.
-- **[Customizable metrics](https://docs.uptrain.ai/docs/monitoring-custom-
-metrics)** - Define custom metrics that make sense for your use case. - **
-[Automated Retraining](https://github.com/uptrain-ai/uptrain/blob/main/
-examples/human_orientation_classification/deepdive_examples/
-uptrain_check_all.ipynb)** - Automate model retraining by attaching your
-training and inference pipelines. - **[Model Bias](https://docs.uptrain.ai/
-docs/uptrain-monitors/model-bias)** - Track bias in your ML model's
-predictions. - **[AI Explainability](https://docs.uptrain.ai/docs/uptrain-
-visuals/shap-explainability)** - Understand relative importance of multiple
-features on predictions. - **Data Security** - Your data never goes out of your
-machine. - **Slack Integration** - Get alerts on Slack. - **Realtime
-Dashboards** - To visualize your model's health live. ## ð¨Coming soonð¨ -
-**Label Shift** - Identify drifts in your predictions. Specially useful in
-cases when ground truth is unavailable. - **Model confidence interval** -
-Confidence intervals for model predictions - **Advanced drift detection
-techniques** - Outlier-based drift detection methods - **Advanced feature
-slicing** - Ability to slice statistical properties - **Kolmogorov-Smirnov
-Test** - For detecting distribution shifts - **Prediction Stability** - Filter
-cases where model prediction is not stable. - **Adversarial Checks** - Combat
-adversarial attacks And more. # Get started ð You can quickly get started
-with [Google Colab here](https://colab.research.google.com/drive/
-1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). To run it in your machine,
-follow the steps below: ### Install the package through pip: ```console pip
-install uptrain ``` ### Run your first example: ```console git clone
-git@github.com:uptrain-ai/uptrain.git cd uptrain/examples pip install
-jupyterlab jupyter lab ``` For a quick walkthrough of how UpTrain works, check
-out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/
-quickstart-tutorial).
-# UpTrain in [action](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-text_summarization/run.ipynb) ð¬ One of the most common use cases of ML today
-is language models, be it text summarization, NER, chatbots, language
-translation, etc. UpTrain provides ways to visualize differences in the
-training and real-world data via UMAP clustering of text embeddings (inferred
-from BERT). Following are some replays from the UpTrain dashboard. ### AI
-Explainability out-of-the-box
-                           ****** [umap_gif] ******
-### Live Model Performance Monitoring and Data Integrity Checks
-                      ****** [perf_gif] [perf_gif] ******
-### UMAP Dimensionality Reduction and Visualization
-                           ****** [umap_gif] ******
-### Edge-case Collection for Finetuning the Model later
-                           ****** [perf_gif] ******
-# Why UpTrain ð¤? Machine learning (ML) models are widely used to make
-critical business decisions. Still, no ML model is 100% accurate, and, further,
-their accuracy deteriorates over time ð£. For example, Sales prediction
-becomes inaccurate over time due to a shift in consumer buying habits.
-Additionally, due to the black box nature of ML models, it's challenging to
-identify and fix their problems. UpTrain solves this. We make it easy for data
-scientists and ML engineers to understand where their models are going wrong
-and help them fix them before others complain ð£ï¸. UpTrain can be used for
-a wide variety of Machine learning models such as LLMs, recommendation models,
-prediction models, Computer vision models, etc. We are constantly working to
-make UpTrain better. Want a new feature or need any integrations? Feel free to
-[create an issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute]
-(https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to
-the repository.
-                             ****** [Meme] ******
-# License ð» This repo is published under Apache 2.0 license, with the
-exception of the ee directory which will contain premium features requiring an
-enterprise license in the future. We're currently focused on developing non-
-enterprise offerings that should cover most use cases by adding more features
-and extending to more models. We also working towards adding a hosted offering
-- [contact us](mailto:tech@uptrain.ai) if you are interested. # Stay Updated
-âï¸ We are continuously adding tons of features and use cases. Please
-support us by giving the project a star â­! # Provide feedback (Harsher the
-better ð) We are building UpTrain in public. Help us improve by giving your
-feedback **[here](https://forms.gle/PXd89D5LiFubro9o9)**. # Contributors
-ð¥ï¸ We welcome contributions to UpTrain. Please see our [contribution
-guide](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for
-details. [https://contrib.rocks/image?repo=uptrain-ai/uptrain]
+                  Welcome] [Docs] [Community] [Website]  ***
+  **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
+applications are performing reliably by allowing users to check aspects such as
+correctness, structural integrity, bias, hallucination, etc. UpTrain can be
+used to: 1) Validate model's response and safeguard your users against
+hallucinations, bias, incorrect output formats, etc. 2) Experiment across
+multiple model providers, prompt templates, and quantify model's performance.
+3) Monitor your model's performance in production and protect yourself against
+unwanted drifts # Key Features ð¡ - **[ChatGPT Grading](https://uptrain-
+ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to
+grade your model outputs. - **[Custom Grading Checks](https://uptrain-
+ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom
+grading prompts. - **[Embeddings Similarity Check](https://uptrain-
+ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity
+between prompt and response embeddings - **[Output Validation](https://
+github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** -
+Safeguard your users against inappropriate responses - **[Prompt A/B Testing]
+(https://github.com/uptrain-ai/uptrain/blob/main/examples/
+prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and
+compare them quantatively. - **[UMAP Visualization and Clustering](https://
+uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding
+space using tools like UMAP and t-SNE. - **[Hallucination Checks]()** - Use
+metrics like custom grading, text similarity, and embedding similarity to check
+for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
+outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
+Built-in pivoting functionalities for data dice and slice to pinpoint low-
+performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
+performance in realtime. # Get started ð  To run it on your machine,
+checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
+quickstart): ### Install the package through pip: ```bash pip install uptrain
+``` ### How to define checks: Say we want to check whether our model's
+responses contain any grammatical mistakes or not. ```python # Define your
+checkset - list of simple checks, dataset file, # and api_keys checkset =
+CheckSet( checks = Check( name = "grammar_score", operators = [ GrammarScore
+( col_in_text = "model_response", col_out = "grammar_score" ), ], plots =
+PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader(fpath =
+'...') ) settings = Settings(openai_api_key = '...') checkset.setup(settings)
+checkset.run() ```
+# Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
+frameworks | | ------------- | ------------- | ------------- | ------------- |
+| OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
+EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
+BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
+Action ## Experimentation You can use the UpTrain framework to run and compare
+LLM responses for different prompts, models, LLM chains, etc. Check out the
+[experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/
+examples/prompt_experiments_tutorial.ipynb) to learn more. ## Validation You
+can use the UpTrain Validation Manager to define checks, retry logic and
+validate your LLM responses before showing it to your users. Check out the
+[tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/
+validation_tutorial.ipynb). ## Monitoring You can use the UpTrain framework to
+continuously monitor your model's performance and get real-time insights on how
+well it is doing on a variety of evaluation metrics. Check out the monitoring
+tutorial to learn more. # Why UpTrain ð¤? Large language models are trained
+over billions of data points and perform really well over a wide variety of
+tasks. But one thing these models are not good at is being deterministic. Even
+with the most well-crafted prompts, the model can misbehave for certain inputs,
+be it hallucinations, wrong output structure, toxic or biased response,
+irrelevant response, and error modes can be immense. To ensure your LLM
+applications work reliably and correctly, UpTrain makes it easy for developers
+to evaluate the responses of their applications on multiple criteria. UpTrain's
+evaluation framework can be used to: 1) Validate (and correct) the response of
+the model before showing it to the user 2) Get quantitative measures to
+experiment across multiple prompts, model providers, etc. 3) Do unit testing to
+ensure no buggy prompt or code gets pushed into your production 4) Monitor your
+LLM applications in real time and understand when they are going wrong in order
+to fix them before users complain. We are constantly working to make UpTrain
+better. Want a new feature or need any integrations? Feel free to [create an
+issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://
+github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the
+repository. # License ð» This repo is published under Apache 2.0 license. We
+are also working towards adding a hosted offering to make setting off eval runs
+easier - please fill **[this form](https://docs.google.com/forms/d/e/
+1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/
+viewform?usp=sf_link)** to get a waitlist slot. # Stay Updated âï¸ We are
+continuously adding tons of features and use cases. Please support us by giving
+the project a star â­! # Provide feedback (Harsher the better ð) We are
+building UpTrain in public. Help us improve by giving your feedback **[here]
+(https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-
+jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**. # Contributors ð¥ï¸ We
+welcome contributions to UpTrain. Please see our [contribution guide](https://
+github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for details. [https://
+contrib.rocks/image?repo=uptrain-ai/uptrain]
```

### Comparing `uptrain-0.2.0/setup.py` & `uptrain-0.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 # read the contents of your README file
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+# sentence-tranformers deps (it installs torch-gpu by default)
+# pip install torch torchvision --index-url https://download.pytorch.org/whl/cpu
+
 setup(
     name="uptrain",
-    version="0.2.0",
+    version="0.3.1",
     description="UpTrain - ML Observability and Retraining Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # The project's main homepage.
     url="https://github.com/uptrain-ai/uptrain",
     # Author details
     maintainer="UpTrain AI Team",
@@ -36,28 +39,51 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="uptrain ai retraining ML observability",
     packages=find_packages(),
+    package_data={"": ["*.pyi"]},
     install_requires=[
+        # utilities
+        "tqdm>=4.0",
+        "pydantic<1.10.10",
+        "aiolimiter>=1.1",
+        "loguru",
+        "lazy_loader",
+        "networkx",
+        # datasets and transforms
+        "polars>=0.18",
+        "deltalake>=0.9",
         "numpy>=1.23.0",
-        "pandas>=1.0.0",
+        "pyarrow>=10.0.0",
+        # visualization
         "plotly>=5.0.0",
-        "pydantic>=1.9.0",
-        "river<=0.14",
-        "scikit_learn>=1.0.0",
-        "streamlit>=1.0.0",
-        "json-fix>=0.5.0",
-    ],
-    tests_require=[
-        "pytest>=7.0",
-        "torch",
-        "imgaug",
-        "gensim",
-        "xgboost",
-        "lightgbm",
-        "hdbscan",
-        "umap-learn",
+        "streamlit>=1.23",
+        # llm related
+        "openai>=0.27",
+        "evals==1.0.3.post1",
+        # "evals @ git+https://github.com/openai/evals.git@main",
+        # access to remote execution
+        "httpx>=0.24.1",
     ],
+    extras_require={
+        "v0": [
+            "pandas>=1.0.0",
+            "river",
+            "scikit_learn>=1.0.0",
+            "umap-learn",
+            "json-fix>=0.5.0",
+            "xgboost",
+        ],
+        "full": [
+            "river<0.18",
+            "scikit_learn>=1.0.0",
+            "umap-learn",
+            "rouge-score",
+            "sentence-transformers",
+            "InstructorEmbedding",
+        ],
+    },  # Optional
+    tests_require=["pytest>=7.0"],
 )
```

### Comparing `uptrain-0.2.0/uptrain/constants.py` & `uptrain-0.3.1/uptrain/v0/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from uptrain.core.lib.model_signal_funcs import *
+from uptrain.v0.core.lib.model_signal_funcs import *
 
 
 class AnnotationMethod(Enum):
     MASTER_FILE = 1
 
 
 class DataDriftAlgo(str, Enum):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/algorithms/clustering.py` & `uptrain-0.3.1/uptrain/v0/core/classes/algorithms/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import Any, List, Tuple, Union
 
-from uptrain.core.lib.helper_funcs import cluster_and_plot_data
+from uptrain.v0.core.lib.helper_funcs import cluster_and_plot_data
 
 
 class Clustering:
     def __init__(self, args) -> None:
         """
         Initializes the Clustering object with the specified arguments.
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/algorithms/popularity_bias.py` & `uptrain-0.3.1/uptrain/v0/core/classes/algorithms/popularity_bias.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/classes/distances/cosine_distance.py` & `uptrain-0.3.1/uptrain/v0/core/classes/distances/cosine_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import List, Union
 
-from uptrain.core.classes.distances import AbstractDistance
+from uptrain.v0.core.classes.distances import AbstractDistance
 
 
 class CosineDistance(AbstractDistance):
     """Class that computes cosine distance between base and reference vectors."""
 
     def calculate_norm(self, vector) -> float:
         if len(vector.shape) > 1:
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/distances/distance_resolver.py` & `uptrain-0.3.1/uptrain/v0/core/classes/distances/distance_resolver.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uptrain.core.classes.distances import (
+from uptrain.v0.core.classes.distances import (
     CosineDistance,
     L2Distance,
     NormRatio,
 )
 
 
 class DistanceResolver:
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/distances/hamming_distance.py` & `uptrain-0.3.1/uptrain/v0/core/classes/distances/hamming_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import List, Union
 
-from uptrain.core.classes.distances import AbstractDistance
+from uptrain.v0.core.classes.distances import AbstractDistance
 
 
 class HammingDistance(AbstractDistance):
     """Class that computes Hamming distance between base and reference vectors."""
 
     def check_valid_vector(self, vector) -> None:
         if not np.all(np.isin(vector, [0, 1])):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/distances/l2_distance.py` & `uptrain-0.3.1/uptrain/v0/core/classes/distances/l2_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import List, Union
 
-from uptrain.core.classes.distances import AbstractDistance
+from uptrain.v0.core.classes.distances import AbstractDistance
 
 
 class L2Distance(AbstractDistance):
     """Class that computes L2 distance between base and reference vectors."""
 
     def compute_distance(
         self, base: Union[List, np.ndarray], reference: Union[List, np.ndarray]
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/distances/norm_ratio.py` & `uptrain-0.3.1/uptrain/v0/core/classes/distances/norm_ratio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import List, Union
 
-from uptrain.core.classes.distances import AbstractDistance
+from uptrain.v0.core.classes.distances import AbstractDistance
 
 
 class NormRatio(AbstractDistance):
     """Class that computes the normalized ratio between base and reference vectors."""
 
     def __init__(self, norm_min: float = 1e-6):
         self.norm_min = norm_min
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/finetuning/finetuning.py` & `uptrain-0.3.1/uptrain/v0/core/classes/finetuning/finetuning.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     import torch
     TORCH_PRESENT = True
 except:
     TORCH_PRESENT = False
 
 
-from uptrain.core.classes.monitors import AbstractCheck
+from uptrain.v0.core.classes.monitors import AbstractCheck
 
 
 class Finetune(AbstractCheck):
 
     def base_init(self, fw, check):
         self.optimizer = check["optimizer"]
         self.train_dataloader = check["train_dataloader"]
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/framework.py` & `uptrain-0.3.1/uptrain/v0/core/classes/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 from threading import Thread
 from typing import Optional
 
 import pandas as pd
 import numpy as np
 from sklearn.preprocessing import normalize
 
-from uptrain.core.classes.helpers import DatasetHandler, ModelHandler, config_handler
-from uptrain.core.classes.logging import LogHandler
-from uptrain.core.classes.logging.new_log_handler import LogHandler as NewLogHandler
-from uptrain.core.classes.managers import CheckManager
-from uptrain.core.lib.helper_funcs import (
+from uptrain.v0.core.classes.helpers import DatasetHandler, ModelHandler, config_handler
+from uptrain.v0.core.classes.logging import LogHandler
+from uptrain.v0.core.classes.logging.new_log_handler import LogHandler as NewLogHandler
+from uptrain.v0.core.classes.managers import CheckManager
+from uptrain.v0.core.classes.io import RunTimeManager
+from uptrain.v0.core.lib.helper_funcs import (
     read_json,
     extract_data_points_from_batch,
     add_data_to_warehouse,
     get_df_indices_from_ids,
     get_feature_names_list,
     load_list_from_df,
     clear_directory,
@@ -75,14 +76,15 @@
                 daemon=True,
                 name="Background Log Consumer",
             )
             daemon.start()
         else:
             training_args = cfg.training_args
             evaluation_args = cfg.evaluation_args
+            self.reader_args = cfg.reader_args
 
             self.orig_training_file = training_args.orig_training_file
             self.fold_name = cfg.retraining_folder
             if os.path.exists(self.fold_name):
                 print("Deleting contents of the folder: ", self.fold_name)
                 clear_directory(self.fold_name)
             else:
@@ -123,14 +125,18 @@
             if evaluation_args.golden_testing_dataset:
                 self.set_golden_testing_dataset(evaluation_args.golden_testing_dataset)
             if training_args.training_func:
                 self.set_training_func(training_args.training_func)
             if evaluation_args.inference_func:
                 self.set_inference_func(evaluation_args.inference_func)
 
+            if self.reader_args.mode == 'continuous':
+                self.runtime_manager = RunTimeManager(self.reader_args, self)
+
+
     def reset_retraining(self):
         self.version += 1
         self.selected_count = 0
         self.smart_data_ids = []
         retrain_folder = os.path.join(self.fold_name, str(self.version))
         if not os.path.exists(retrain_folder):
             os.mkdir(retrain_folder)
@@ -425,14 +431,19 @@
 
     def convert_dict_values_to_numpy_values(self, inputs: dict) -> dict:
         data = {}
         for key, value in inputs.items():
             data.update({key: np.array(value)})
         return data
 
+
+    def run_endlessly(self):
+        self.runtime_manager.run_endlessly()
+
+
     def log(
         self,
         inputs=None,
         outputs=None,
         gts=None,
         identifiers=None,
         extra=None,
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/helpers/annotation_helper.py` & `uptrain-0.3.1/uptrain/v0/core/classes/helpers/annotation_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uptrain.core.lib.helper_funcs import read_json
+from uptrain.v0.core.lib.helper_funcs import read_json
 
 
 class AnnotationHelper:
     """
     Helper class to integrate different annotation methods
 
     ...
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/helpers/config_handler.py` & `uptrain-0.3.1/uptrain/v0/core/classes/helpers/config_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import typing
 from datetime import datetime
 
 from pydantic import BaseModel
 import numpy as np
 
-from uptrain.constants import AnnotationMethod
+from uptrain.v0.constants import AnnotationMethod
 
 
 class AnnotationArgs(BaseModel):
     method: AnnotationMethod
     args: typing.Dict = {}
 
 
@@ -28,22 +28,33 @@
 
 class LoggingArgs(BaseModel):
     slack_webhook_url: str = None
     dashboard_port: int = None
     log_folder: str = "uptrain_logs"
     log_data: bool = True
     st_logging: bool = False
+    postgres_logging: bool = False
+    database: str = None
     run_background_streamlit: bool = True
     use_new_handler: bool = False
 
 
 class LicenseArgs(BaseModel):
     openai_key: str = None
 
 
+class ReaderArgs(BaseModel):
+    mode: str = 'default'
+    frequency_in_seconds: typing.Optional[typing.Union[float, int]] = None
+    num_backlog: typing.Optional[int] = 1
+    type: str = None
+    sql_query: str = None
+    sql_variables_dictn: typing.Optional[dict] = None
+    database: str = None
+
 class Config(BaseModel):
     training_args: TrainingArgs = TrainingArgs()
     evaluation_args: EvaluationArgs = EvaluationArgs()
     logging_args: LoggingArgs = LoggingArgs()
     license_args: LicenseArgs = LicenseArgs()
     data_identifier: str = "id"
     checks: typing.List[typing.Dict] = []
@@ -52,14 +63,15 @@
     retraining_folder: str = "uptrain_smart_data"
     data_id: str = "id"
     feat_name_list: list = None
     cluster_visualize_func: typing.Callable = None
     use_cache: bool = False
     run_background_log_consumer: bool = False
     running_ee: bool = False
+    reader_args: ReaderArgs = ReaderArgs()
 
 
 # class InputArgs(BaseModel):
 #     data: dict
 #     id: typing.Optional[typing.Union[list, np.ndarray]]
 
 #     class Config:
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/helpers/dataset_handler.py` & `uptrain-0.3.1/uptrain/v0/core/classes/helpers/dataset_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
-from uptrain.core.classes.helpers import AnnotationHelper
-from uptrain.core.lib.helper_funcs import read_json, write_json, cluster_and_plot_data
-from uptrain.constants import AnnotationMethod
+from uptrain.v0.core.classes.helpers import AnnotationHelper
+from uptrain.v0.core.lib.helper_funcs import read_json, write_json, cluster_and_plot_data
+from uptrain.v0.constants import AnnotationMethod
 
 
 class DatasetHandler:
     """
     Handler class to help with all the dataset related functionalities
 
     ...
@@ -25,15 +25,15 @@
     set_annotation_method(method):
         Set the annotation method
     """
 
     def __init__(self, framework=None, cfg=None, transformation_func=(lambda x: x)):
         self.transformation_func = transformation_func
         self.cluster_plot_func = cfg.cluster_visualize_func
-        self.log_handler = framework.log_handler 
+        self.log_handler = framework.log_handler
         np.random.seed(10)
 
     def add_annotations(self, dataset):
         """Adds gt to the dataset file by calling appropriate funcs on the annotation helper based on attached annotation method"""
 
         if self.annotation_method == AnnotationMethod.MASTER_FILE:
             annotated_data = self.annotation_helper.annotations_from_master_file(
@@ -73,15 +73,17 @@
         write_json(dataset_location + "/cleaned_dataset.json", new_data)
 
         if self.cluster_plot_func is not None:
             cluster_and_plot_data(
                 np.array([x["kps"] for x in new_data]),
                 9,
                 cluster_plot_func=self.cluster_plot_func,
-                plot_save_name=self.log_handler.get_plot_save_name("collected_edge_cases_clusters.png", "edge_cases"),
+                plot_save_name=self.log_handler.get_plot_save_name(
+                    "collected_edge_cases_clusters.png", "edge_cases"
+                ),
             )
 
         new_data = self.add_annotations(dataset_location + "/cleaned_dataset.json")
         write_json(dataset_location + "/annotated_dataset.json", new_data)
         write_json(
             dataset_location + "/training_dataset.json",
             self.merge_training_datasets(
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/helpers/model_handler.py` & `uptrain-0.3.1/uptrain/v0/core/classes/helpers/model_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/log_handler.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/log_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import os
 import shutil
 import urllib3
 import json
 
-from uptrain.core.lib.helper_funcs import clear_directory
+from uptrain.v0.core.lib.helper_funcs import clear_directory
 
 
 class LogHandler:
     def __init__(self, framework=None, cfg=None):
         self.fw = framework
         log_folder = cfg.logging_args.log_folder
         self.path_all_data = framework.path_all_data
 
         if os.path.exists(log_folder):
             print("Deleting contents of the folder: ", log_folder)
             clear_directory(log_folder)
 
         self.st_writer = None
+        self.postgres_writer = None
         if cfg.logging_args.st_logging:
-            from uptrain.core.classes.logging.log_streamlit import StreamlitLogs
+            from uptrain.v0.core.classes.logging.log_streamlit import StreamlitLogs
 
             self.st_log_folder = os.path.join(log_folder, "st_data")
             os.makedirs(self.st_log_folder, exist_ok=True)
             self.st_writer = StreamlitLogs(
                 self.st_log_folder, port=cfg.logging_args.dashboard_port
             )
+        elif cfg.logging_args.postgres_logging:
+            from uptrain.v0.core.classes.logging.log_postgres import PostgresLogs
+
+            self.postgres_database = cfg.logging_args.database
+            self.postgres_writer = PostgresLogs(
+                self.postgres_database
+            )
 
         # Get Webhook URL for alerting on slack
         self.webhook_url = cfg.logging_args.slack_webhook_url
 
         # Saving config to get model metadata
         self.cfg_metadata = {}
         if len(cfg.checks) > 0:
@@ -74,56 +82,66 @@
         count,
         dashboard_name,
         features={},
         models={},
         file_name=None,
         update_val=False,
     ):
-        if self.st_writer is None:
-            return
         dashboard_name, plot_name = self.dir_friendly_name([dashboard_name, plot_name])
         dictn.update(features)
         dictn.update(models)
         new_dictn = dict(
             zip(
                 self.dir_friendly_name(list(dictn.keys())),
                 dictn.values(),
             )
         )
-        dashboard_dir = os.path.join(self.st_log_folder, dashboard_name)
-        plot_folder = os.path.join(dashboard_dir, "line_plots", plot_name)
-        os.makedirs(plot_folder, exist_ok=True)
         new_dictn.update({"x_count": count})
-        if file_name is None:
-            file_name = plot_name
-        self.st_writer.add_scalars(
-            new_dictn, plot_folder, file_name=file_name, update_val=update_val
-        )
+
+        if self.st_writer is not None:
+            dashboard_dir = os.path.join(self.st_log_folder, dashboard_name)
+            plot_folder = os.path.join(dashboard_dir, "line_plots", plot_name)
+            os.makedirs(plot_folder, exist_ok=True)
+            if file_name is None:
+                file_name = plot_name
+            if self.st_writer is not None:
+                self.st_writer.add_scalars(
+                    new_dictn, plot_folder, file_name=file_name, update_val=update_val
+                )
+        if self.postgres_writer is not None:
+            plot_table = dashboard_name + "_line_plots_" + plot_name
+            self.postgres_writer.add_scalars(
+                new_dictn, plot_table, update_val=update_val
+            )
 
     def add_histogram(
         self,
         plot_name,
         data,
         dashboard_name,
         features=None,
         models=None,
         file_name=None,
     ):
+        if self.postgres_writer is not None:
+            raise Exception("Postgres Log writer not supported for Histogram")
         dashboard_name, plot_name = self.dir_friendly_name([dashboard_name, plot_name])
         if self.st_writer:
             dashboard_dir = os.path.join(self.st_log_folder, dashboard_name)
             plot_folder = os.path.join(dashboard_dir, "histograms", plot_name)
             os.makedirs(plot_folder, exist_ok=True)
             if file_name is None:
                 file_name = plot_name
             self.st_writer.add_histogram(
                 data, plot_folder, features=features, models=models, file_name=file_name
             )
 
     def add_bar_graphs(self, plot_name, data, dashboard_name, count=-1, hover_data={}):
+        if self.postgres_writer is not None:
+            raise Exception("Postgres Log writer not supported for Bar Graphs")
         if self.st_writer is None:
             return
         dashboard_name, plot_name = self.dir_friendly_name([dashboard_name, plot_name])
         dashboard_dir = os.path.join(self.st_log_folder, dashboard_name)
         plot_folder = os.path.join(dashboard_dir, "bar_graphs", plot_name)
         os.makedirs(plot_folder, exist_ok=True)
         self.st_writer.add_bar_graphs(data, plot_folder, count, hover_data=hover_data)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/log_streamlit.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/log_streamlit.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.log_folder = log_folder
 
         # remote_st_py_file = "https://raw.githubusercontent.com/uptrain-ai/uptrain/main/uptrain/core/classes/logging/st_run.py"
         # remote_st_py_file = "../../uptrain/core/classes/logging/st_run.py"
 
         path_uptrain_init: str = importlib.util.find_spec("uptrain").origin  # type: ignore
         remote_st_py_file = os.path.join(
-            os.path.dirname(path_uptrain_init), "core/classes/logging/st_run.py"
+            os.path.dirname(path_uptrain_init), "v0/core/classes/logging/st_run.py"
         )
 
         if port is None:
             cmd = "streamlit run " + remote_st_py_file + " -- " + self.log_folder
         else:
             port = get_free_port(int(port))
             cmd = (
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/new_log_handler.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/new_log_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import csv, _csv
 import os
 import shutil
 import json
 from typing import IO, TYPE_CHECKING, Protocol
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.framework import Framework
-    from uptrain.core.classes.helpers.config_handler import Config
+    from uptrain.v0.core.classes.framework import Framework
+    from uptrain.v0.core.classes.helpers.config_handler import Config
 
-from uptrain.core.lib.helper_funcs import make_dir_friendly_name, clear_directory
-from uptrain.core.encoders import NumpyEncoder
-from uptrain.core.classes.logging.new_st_setup import StreamlitRunner
+from uptrain.v0.core.lib.helper_funcs import make_dir_friendly_name, clear_directory
+from uptrain.v0.core.encoders import NumpyEncoder
+from uptrain.v0.core.classes.logging.new_st_setup import StreamlitRunner
 
 
 # -----------------------------------------------------------
 # Implement LogWriters for different file formats
 # -----------------------------------------------------------
 def get_logs_addr_for_check(
     log_folder: str, dashboard_name: str, distance_type: str, reference: str
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/new_st_run.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/new_st_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import streamlit as st
 import pandas as pd
 import plotly.graph_objects as go
 import numpy as np
 import plotly.express as px
 
-from uptrain.core.lib.helper_funcs import make_dir_friendly_name
+from uptrain.v0.core.lib.helper_funcs import make_dir_friendly_name
 
 # -----------------------------------------------------------
 # Set up layout of the dashboard and the sidebar
 # -----------------------------------------------------------
 
 st.set_page_config(
     page_title="UpTrain Dashboard",
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/new_st_setup.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/new_st_setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     launch_cmd: str
 
     def __init__(self, log_folder: str, port: Optional[int] = None):
         self.log_folder = log_folder
 
         path_uptrain_init: str = importlib.util.find_spec("uptrain").origin  # type: ignore
         path_st_run = os.path.join(
-            os.path.dirname(path_uptrain_init), "core/classes/logging/new_st_run.py"
+            os.path.dirname(path_uptrain_init), "v0/core/classes/logging/new_st_run.py"
         )
         port_arg = "" if port is None else f"--server.port {port}"
         self.launch_cmd = f"streamlit run {path_st_run} {port_arg} -- {self.log_folder}"
 
     def start(self):
         t = threading.Thread(target=lambda: os.system(self.launch_cmd), args=([]))
         t.start()
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/logging/st_run.py` & `uptrain-0.3.1/uptrain/v0/core/classes/logging/st_run.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/classes/managers/check_manager.py` & `uptrain-0.3.1/uptrain/v0/core/classes/managers/check_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import numpy as np
 from copy import deepcopy
 
-from uptrain.constants import Monitor, Statistic, Visual, MeasurableType
-from uptrain.core.classes.monitors import (
+from uptrain.v0.constants import Monitor, Statistic, Visual, MeasurableType
+from uptrain.v0.core.classes.monitors import (
     Accuracy,
     ConceptDrift,
     DataDrift,
     FeatureDrift,
     CustomMonitor,
     ModelBias,
     DataIntegrity,
     EdgeCase,
     OutputComparison,
 )
-from uptrain.core.classes.statistics import (
+from uptrain.v0.core.classes.statistics import (
     Distance,
     Convergence,
     Distribution,
     NormEmbedding,
 )
-from uptrain.core.classes.visuals import (
+from uptrain.v0.core.classes.visuals import (
     DimensionalityReduction,
     Shap,
     Plot,
 )
-from uptrain.core.classes.finetuning import Finetune
+from uptrain.v0.core.classes.finetuning import Finetune
 
 
 class CheckManager:
     def __init__(self, framework, checks=[]):
         self.monitors_to_check = []
         self.statistics_to_check = []
         self.visuals_to_check = []
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/__init__.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/abstract_measurable.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/abstract_measurable.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/accuracy.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/accuracy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import Measurable
 
 
 class AccuracyMeasurable(Measurable):
     """Class that computes the accuracy from predictions and ground truths.
 
     Returns a list of values where a value is:
     - True, if prediction equals ground truth
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/condition.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict
 
-from uptrain.core.classes.measurables import Measurable, FeatureMeasurable
+from uptrain.v0.core.classes.measurables import Measurable, FeatureMeasurable
 
 
 class ConditionMeasurable(Measurable):
     """Class that computes a boolean condition on a measurable feature."""
 
     def __init__(
         self, framework, underlying: Dict[str, Any], condition: Dict[str, Any]
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/custom.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/custom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
 from typing import Any, Dict
 
-from uptrain.core.classes.measurables import Measurable
-from uptrain.core.classes.signals import SignalManager
+from uptrain.v0.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.signals import SignalManager
 
 
 class CustomMeasurable(Measurable):
     """Class that computes a custom metric measurable using a user-defined signal formula."""
 
     def __init__(self, framework, custom_args: Dict[str, Any] = {}) -> None:
         """Constructor for CustomMeasurable class.
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/distance.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, List, Union
 
-from uptrain.core.classes.distances import DistanceResolver
-from uptrain.core.classes.measurables import Measurable
-from uptrain.core.classes.measurables import InputFeatureMeasurable
+from uptrain.v0.core.classes.distances import DistanceResolver
+from uptrain.v0.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import InputFeatureMeasurable
 
 
 class DistanceMeasurable(Measurable):
     """Class that computes and logs distance based on chosen distance metric."""
 
     def __init__(self, framework, base, reference, distance_types) -> None:
         """Constructor for DistanceMeasurable class.
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/feature.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from uptrain.core.classes.measurables import (
+from uptrain.v0.core.classes.measurables import (
     Measurable,
     InputFeatureMeasurable,
     OutputFeatureMeasurable,
 )
 
 
 class FeatureMeasurable(Measurable):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/feature_concat.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/feature_concat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 import numpy as np
 
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import Measurable
 
 
 class FeatureConcatMeasurable(Measurable):
     """Class that returns the input feature corresponding to the feature name."""
 
     def __init__(self, framework, feat_name_list) -> None:
         super().__init__(framework)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/input_feature.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/input_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import Measurable
 
 
 class InputFeatureMeasurable(Measurable):
     """Class that returns the input feature corresponding to the feature name."""
 
     def __init__(self, framework, feature_name) -> None:
         super().__init__(framework)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/measurable.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/measurable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 
 from typing import Any
 
-from uptrain.core.lib.helper_funcs import (
+from uptrain.v0.core.lib.helper_funcs import (
     extract_data_points_from_batch,
     combine_data_points_for_batch,
 )
-from uptrain.core.classes.measurables import AbstractMeasurable
+from uptrain.v0.core.classes.measurables import AbstractMeasurable
 
 
 class Measurable(AbstractMeasurable):
     """Class that contains the core logic for computation/logging of a measurable.
 
     This class is a subclass of AbstractMeasurable and implements the computation
     and logging of a measurable or evaluatable object. It can optionally use a
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/measurable_resolver.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/measurable_resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from uptrain.core.classes.measurables import (
+from uptrain.v0.core.classes.measurables import (
     Measurable,
     InputFeatureMeasurable,
     OutputFeatureMeasurable,
     FeatureMeasurable,
     FeatureConcatMeasurable,
     ConditionMeasurable,
     CustomMeasurable,
     AccuracyMeasurable,
     MAEMeasurable,
     MAPEMeasurable,
     ScalarFromEmbeddingMeasurable,
     DistanceMeasurable,
     RecHitRateMeasurable,
 )
-from uptrain.ee.classes.measurables import (
+from uptrain.v0.ee.classes.measurables import (
     GrammerScoreMeasurable,
 )
 
-from uptrain.constants import MeasurableType
+from uptrain.v0.constants import MeasurableType
 
 
 class MeasurableResolver:
     """Class that resolves a measurable key to a measurable class instance."""
 
     def __init__(self, args) -> None:
         super().__init__()
@@ -76,11 +76,12 @@
                 resolve_args["base"],
                 resolve_args["reference"],
                 resolve_args["distance_types"],
             )
         elif measurable_type == MeasurableType.REC_HIT_RATE:
             return RecHitRateMeasurable(framework)
         elif measurable_type == MeasurableType.GRAMMAR_SCORE:
-            return GrammerScoreMeasurable(framework,
-                                          resolve_args.get("feature_name", None))
+            return GrammerScoreMeasurable(
+                framework, resolve_args.get("feature_name", None)
+            )
         else:
             raise Exception("Resolver not defined")
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/output_feature.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/output_feature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import Measurable
 
 
 class OutputFeatureMeasurable(Measurable):
     """Class that returns the output feature corresponding to the feature name."""
 
     def __init__(self, framework) -> None:
         super().__init__(framework)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/recommendation_hit_rate.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/recommendation_hit_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from typing import Any
 
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.classes.measurables import Measurable
 
 
 class RecHitRateMeasurable(Measurable):
     """Class that computes the recommendation hit-rate of a model's predictions."""
 
     def __init__(self, framework) -> None:
         super().__init__(framework)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/measurables/scalar_from_embedding.py` & `uptrain-0.3.1/uptrain/v0/core/classes/measurables/scalar_from_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from uptrain.core.classes.measurables import (
+from uptrain.v0.core.classes.measurables import (
     Measurable,
     InputFeatureMeasurable,
 )
 
 
 class ScalarFromEmbeddingMeasurable(Measurable):
     """Class that extracts a scalar from a measurable embedding."""
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/abstract_check.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/abstract_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 from abc import ABC
 import os
 
-from uptrain.core.classes.measurables import MeasurableResolver
+from uptrain.v0.core.classes.measurables import MeasurableResolver
 
 class AbstractCheck(ABC):
 
     def __init__(self, fw, check) -> None:
         super().__init__()
         self.log_handler = fw.log_handler
         self.dashboard_name = check["type"]
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/abstract_monitor.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/abstract_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractCheck
+from uptrain.v0.core.classes.monitors import AbstractCheck
 
 class AbstractMonitor(AbstractCheck):
     monitor_type = None
 
     def need_ground_truth(self):
         return False
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/accuracy.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/accuracy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import MeasurableType
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Monitor
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.constants import MeasurableType
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Monitor
+
 
 class Accuracy(AbstractMonitor):
     dashboard_name = "accuracy"
     monitor_type = Monitor.ACCURACY
-    
+
     def base_init(self, fw, check):
         if check.get("measurable_args", None):
             self.measurable = MeasurableResolver(check["measurable_args"]).resolve(fw)
-            self.plot_name = check["measurable_args"]['type']
+            self.plot_name = check["measurable_args"]["type"]
         else:
-            self.measurable = MeasurableResolver(
-                {"type": MeasurableType.MAE}).resolve(fw)
+            self.measurable = MeasurableResolver({"type": MeasurableType.MAE}).resolve(
+                fw
+            )
         self.abs_err_arr = np.array([])
         self.avg_acc = 0
         self.log_handler = fw.log_handler
 
     def need_ground_truth(self):
         return True
-    
+
     def base_check(self, inputs, outputs, gts=None, extra_args={}):
-        batch_abs_error = self.measurable.compute_and_log(inputs, outputs, gts, extra_args)
+        batch_abs_error = self.measurable.compute_and_log(
+            inputs, outputs, gts, extra_args
+        )
         self.abs_err_arr = np.append(self.abs_err_arr, batch_abs_error)
 
         self.log_handler.add_scalars(
             self.plot_name,
             {"y_" + self.plot_name: np.mean(self.abs_err_arr)},
             len(self.abs_err_arr),
             self.dashboard_name,
-        )
+        )
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/concept_drift.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/concept_drift.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import numpy as np
 
 from river import drift
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import DataDriftAlgo, MeasurableType
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Monitor
-from uptrain.core.lib.helper_funcs import add_data_to_warehouse
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.constants import DataDriftAlgo, MeasurableType
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Monitor
+from uptrain.v0.core.lib.helper_funcs import add_data_to_warehouse
 
 
 class ConceptDrift(AbstractMonitor):
     monitor_type = Monitor.CONCEPT_DRIFT
 
     def base_init(self, fw, check):
         if check.get("measurable_args", None):
             self.measurable = MeasurableResolver(check["measurable_args"]).resolve(fw)
         else:
-            self.measurable = MeasurableResolver({"type": MeasurableType.ACCURACY}).resolve(fw)
+            self.measurable = MeasurableResolver(
+                {"type": MeasurableType.ACCURACY}
+            ).resolve(fw)
 
         self.avg_acc = 0
         self.drift_alerted = False
         self.algorithm = check["algorithm"]
         self.counter = 0
         self.plot_name = f"avg_accuracy_{self.measurable.col_name()}"
         self.feat_slicing = check.get("feat_slicing", False)
@@ -32,15 +34,17 @@
             self.algo = drift.DDM(warm_start, warn_threshold, alarm_threshold)
         elif self.algorithm == DataDriftAlgo.ADWIN:
             delta = check.get("delta", 0.002)
             clock = check.get("clock", 32)
             max_buckets = check.get("max_buckets", 5)
             min_window_length = check.get("min_window_length", 5)
             grace_period = check.get("grace_period", 5)
-            self.algo = drift.ADWIN(delta, clock, max_buckets, min_window_length, grace_period)
+            self.algo = drift.ADWIN(
+                delta, clock, max_buckets, min_window_length, grace_period
+            )
         else:
             raise Exception("Data drift algo type not supported")
 
     def need_ground_truth(self):
         return True
 
     def base_check(self, inputs, outputs, gts=None, extra_args={}):
@@ -66,27 +70,21 @@
                 self.drift_alerted = True
 
             self.avg_acc = (self.avg_acc * self.counter + acc) / (self.counter + 1)
             self.counter += 1
             models = dict(
                 zip(
                     self.model_names,
-                    [
-                        all_models[jdx][i]
-                        for jdx in range(len(self.model_names))
-                    ],
+                    [all_models[jdx][i] for jdx in range(len(self.model_names))],
                 )
             )
             features = dict(
                 zip(
                     self.feature_names,
-                    [
-                        all_features[jdx][i]
-                        for jdx in range(len(self.feature_names))
-                    ],
+                    [all_features[jdx][i] for jdx in range(len(self.feature_names))],
                 )
             )
             self.log_handler.add_scalars(
                 self.plot_name,
                 {"y_avg_accuracy": self.avg_acc},
                 self.counter,
                 self.dashboard_name,
@@ -95,15 +93,17 @@
             )
 
             if isinstance(alert, str):
                 self.log_handler.add_alert(
                     "Model Performance Degradation Alert 🚨", alert, self.dashboard_name
                 )
         if self.feat_slicing:
-            add_data_to_warehouse({"id": inputs["id"],
-                self.dashboard_name: batch_acc}, self.path_dashboard_data)
-    
-    def _preprocess (self, batch):
+            add_data_to_warehouse(
+                {"id": inputs["id"], self.dashboard_name: batch_acc},
+                self.path_dashboard_data,
+            )
+
+    def _preprocess(self, batch):
         if self.algorithm == DataDriftAlgo.DDM:
             return np.array([0 if x else 1 for x in batch])
         else:
             return np.array(batch)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/custom_monitor.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/custom_monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import Monitor
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.constants import Monitor
 
 
 class CustomMonitor(AbstractMonitor):
     monitor_type = Monitor.CUSTOM_MONITOR
 
     def base_init(self, fw, check):
         self.dashboard_name = check.get("dashboard_name", "custom_measure")
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/data_drift.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/data_drift.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 import numpy as np
 import copy
 import pandas as pd
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import Monitor
-from uptrain.core.lib.helper_funcs import read_json
-from uptrain.core.lib.algorithms import estimate_earth_moving_cost
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.core.classes.algorithms import Clustering
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.constants import Monitor
+from uptrain.v0.core.lib.helper_funcs import read_json
+from uptrain.v0.core.lib.algorithms import estimate_earth_moving_cost
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.core.classes.algorithms import Clustering
+
 
 class DataDrift(AbstractMonitor):
     dashboard_name = "data_drift"
     monitor_type = Monitor.DATA_DRIFT
     is_embedding = None
     mode = None
     NUM_BUCKETS = 20
     INITIAL_SKIP = 2000
 
     def model_choices(self, check):
-        self.is_embedding = check.get('is_embedding', None)
+        self.is_embedding = check.get("is_embedding", None)
         if self.is_embedding == None:
             return [{"is_embedding": False}, {"is_embedding": True}]
         else:
-            return [{"is_embedding": check['is_embedding']}]
+            return [{"is_embedding": check["is_embedding"]}]
 
     def base_init(self, fw, check):
         self.reference_dataset = check["reference_dataset"]
         self.cluster_plot_func = fw.dataset_handler.cluster_plot_func
         self.save_edge_cases = check.get("save_edge_cases", True)
         self.NUM_BUCKETS = check.get("num_buckets", self.NUM_BUCKETS)
-        
+
         # Also the step in calculating drift
         self.INITIAL_SKIP = check.get("initial_skip", self.INITIAL_SKIP)
         self.outlier_idxs = check.get("outlier_idxs", [])
         self.do_low_density_check = check.get("do_low_density_check", False)
-        self.hover_measurable = MeasurableResolver(check.get("hover_label_args", None)).resolve(fw)
+        self.hover_measurable = MeasurableResolver(
+            check.get("hover_label_args", None)
+        ).resolve(fw)
         self.count = 0
         self.bucket_labelling_info = {
-            'latest_idxs_added_to_clusters': np.array([None] * self.NUM_BUCKETS),
-            'idxs_closest_to_clusters': np.array([None] * self.NUM_BUCKETS),
-            'closest_idxs_distance': np.array([None] * self.NUM_BUCKETS),
-            'hover_vals_for_reference_clusters': np.array([' '] * self.NUM_BUCKETS),
-            'hover_vals_for_production_clusters': np.array([' '] * self.NUM_BUCKETS)
+            "latest_idxs_added_to_clusters": np.array([None] * self.NUM_BUCKETS),
+            "idxs_closest_to_clusters": np.array([None] * self.NUM_BUCKETS),
+            "closest_idxs_distance": np.array([None] * self.NUM_BUCKETS),
+            "hover_vals_for_reference_clusters": np.array([" "] * self.NUM_BUCKETS),
+            "hover_vals_for_production_clusters": np.array([" "] * self.NUM_BUCKETS),
         }
         self.prod_dist_counts_arr = []
         clustering_args = {
             "num_buckets": self.NUM_BUCKETS,
-            'is_embedding': self.is_embedding,
-            'plot_save_name': self.log_handler.get_plot_save_name("training_dataset_clusters.png", self.dashboard_name),
-            'cluster_plot_func': self.cluster_plot_func,
-            'find_low_density_regions': self.do_low_density_check
+            "is_embedding": self.is_embedding,
+            "plot_save_name": self.log_handler.get_plot_save_name(
+                "training_dataset_clusters.png", self.dashboard_name
+            ),
+            "cluster_plot_func": self.cluster_plot_func,
+            "find_low_density_regions": self.do_low_density_check,
         }
         self.clustering_helper = Clustering(clustering_args)
         if self.is_embedding:
             self.plot_name = "Embeddings_" + self.measurable.col_name()
             self.emd_threshold = check.get("emd_threshold", 1)
         else:
             self.plot_name = "Scalar_" + self.measurable.col_name()
@@ -66,17 +71,20 @@
         return False
 
     def check(self, inputs, outputs, gts=None, extra_args={}):
         if len(self.children) > 0:
             feats = self.measurable.compute_and_log(
                 inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
             )
-            if sum(list(feats.shape)[1:])/max(1,len(list(feats.shape)[1:])) <= 1:
+            if sum(list(feats.shape)[1:]) / max(1, len(list(feats.shape)[1:])) <= 1:
                 self.children = [self.children[0]]
-            [x.check(inputs, outputs, gts=gts, extra_args=extra_args) for x in self.children]
+            [
+                x.check(inputs, outputs, gts=gts, extra_args=extra_args)
+                for x in self.children
+            ]
         else:
             self.count += len(extra_args["id"])
 
             self.feats = self.measurable.compute_and_log(
                 inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
             )
             feats_shape = list(self.feats.shape)
@@ -84,68 +92,114 @@
             if len(feats_shape) == 2:
                 feats_shape.insert(2, 1)
             self.feats = np.reshape(self.feats, tuple(feats_shape))
 
             if self.is_embedding:
                 self.feats = self.feats / np.expand_dims(self.max_along_axis, 0)
 
-            self.this_datapoint_cluster, self.prod_dist_counts = self.clustering_helper.infer_cluster_assignment(self.feats, self.prod_dist_counts)
-            #TODO: Extend for feature-wise clusters
+            (
+                self.this_datapoint_cluster,
+                self.prod_dist_counts,
+            ) = self.clustering_helper.infer_cluster_assignment(
+                self.feats, self.prod_dist_counts
+            )
+            # TODO: Extend for feature-wise clusters
             if (self.hover_measurable is not None) and self.is_embedding:
-                hover_measurable_vals = np.array(self.hover_measurable.compute_and_log(
-                    inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
-                ))
-                uniq_clusters, uniq_indexs = np.unique(self.this_datapoint_cluster, return_index=True)
+                hover_measurable_vals = np.array(
+                    self.hover_measurable.compute_and_log(
+                        inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
+                    )
+                )
+                uniq_clusters, uniq_indexs = np.unique(
+                    self.this_datapoint_cluster, return_index=True
+                )
                 query_indexs = np.zeros(self.NUM_BUCKETS)
-                self.bucket_labelling_info['latest_idxs_added_to_clusters'][uniq_clusters] = uniq_indexs
+                self.bucket_labelling_info["latest_idxs_added_to_clusters"][
+                    uniq_clusters
+                ] = uniq_indexs
                 query_indexs[uniq_clusters] = uniq_indexs
                 query_indexs = np.array(query_indexs, dtype=int)
-                self.bucket_labelling_info['hover_vals_for_production_clusters'] = hover_measurable_vals[query_indexs]
+                self.bucket_labelling_info[
+                    "hover_vals_for_production_clusters"
+                ] = hover_measurable_vals[query_indexs]
 
             self.prod_dist_counts_arr.append(self.prod_dist_counts.copy())
 
             self.prod_dist = (
                 self.prod_dist_counts_arr[-1]
                 - self.prod_dist_counts_arr[
                     int(max(self.count - self.INITIAL_SKIP, 0) / len(extra_args["id"]))
                 ]
             ) / min(self.count, self.INITIAL_SKIP)
 
             if self.ref_dist.shape[0] == 1:
                 if self.is_embedding:
-                    bar_graph_buckets = ["cluster_" + str(idx) for idx in range(len(list(np.reshape(self.clusters,-1))))]
+                    bar_graph_buckets = [
+                        "cluster_" + str(idx)
+                        for idx in range(len(list(np.reshape(self.clusters, -1))))
+                    ]
                 else:
-                    bar_graph_buckets = list(np.reshape(self.clusters,-1))
+                    bar_graph_buckets = list(np.reshape(self.clusters, -1))
 
                 self.log_handler.add_bar_graphs(
                     self.plot_name,
                     {
-                        "reference": dict(zip(bar_graph_buckets, list(np.reshape(np.array(self.ref_dist[0]), -1)))),
-                        "production": dict(zip(bar_graph_buckets, list(np.reshape(np.array(self.prod_dist[0]), -1)))),
+                        "reference": dict(
+                            zip(
+                                bar_graph_buckets,
+                                list(np.reshape(np.array(self.ref_dist[0]), -1)),
+                            )
+                        ),
+                        "production": dict(
+                            zip(
+                                bar_graph_buckets,
+                                list(np.reshape(np.array(self.prod_dist[0]), -1)),
+                            )
+                        ),
                     },
                     self.dashboard_name,
-                    hover_data = {
-                        "reference": dict(zip(bar_graph_buckets, list(self.bucket_labelling_info['hover_vals_for_reference_clusters']))),
-                        "production": dict(zip(bar_graph_buckets, list(self.bucket_labelling_info['hover_vals_for_production_clusters'])))
-                    }
+                    hover_data={
+                        "reference": dict(
+                            zip(
+                                bar_graph_buckets,
+                                list(
+                                    self.bucket_labelling_info[
+                                        "hover_vals_for_reference_clusters"
+                                    ]
+                                ),
+                            )
+                        ),
+                        "production": dict(
+                            zip(
+                                bar_graph_buckets,
+                                list(
+                                    self.bucket_labelling_info[
+                                        "hover_vals_for_production_clusters"
+                                    ]
+                                ),
+                            )
+                        ),
+                    },
                 )
 
             if self.count < self.INITIAL_SKIP:
                 self.drift_detected = False
                 return
             else:
                 self.psis = np.zeros(self.ref_dist.shape[0])
                 self.costs = np.zeros(self.ref_dist.shape[0])
                 drift_detected = False
                 for idx in range(self.ref_dist.shape[0]):
                     if self.is_embedding:
                         self.costs[idx] = estimate_earth_moving_cost(
                             self.prod_dist[idx], self.ref_dist[idx], self.clusters[idx]
                         )
-                        drift_detected = drift_detected or (self.costs[idx] > self.emd_threshold)
+                        drift_detected = drift_detected or (
+                            self.costs[idx] > self.emd_threshold
+                        )
                     else:
                         this_psi = sum(
                             [
                                 (self.prod_dist[idx][jdx] - self.ref_dist[idx][jdx])
                                 * np.log(
                                     max(self.prod_dist[idx][jdx], 0.0001)
                                     / self.ref_dist[idx][jdx]
@@ -153,47 +207,56 @@
                                 for jdx in range(self.ref_dist.shape[1])
                             ]
                         )
                         self.psis[idx] = this_psi
                         drift_detected = drift_detected or (this_psi > 0.3)
                 self.drift_detected = drift_detected
                 if self.drift_detected:
-                    alert = "Data Drift last detected at " + str(self.count) + " for Embeddings with Earth moving distance = " + str(float(self.costs[0]))
+                    alert = (
+                        "Data Drift last detected at "
+                        + str(self.count)
+                        + " for Embeddings with Earth moving distance = "
+                        + str(float(self.costs[0]))
+                    )
                     self.log_handler.add_alert(
-                        "Data Drift Alert 🚨",
-                        alert,
-                        self.dashboard_name
+                        "Data Drift Alert 🚨", alert, self.dashboard_name
                     )
 
             if self.is_embedding:
                 dict_emc = dict(
                     zip(
-                        ["y_" + self.measurable.col_name() for x in range(self.costs.shape[0])],
+                        [
+                            "y_" + self.measurable.col_name()
+                            for x in range(self.costs.shape[0])
+                        ],
                         [float(x) for x in list(self.costs)],
                     )
                 )
                 # dict_emc.update({"threshold": self.emd_threshold})
                 self.log_handler.add_scalars(
                     self.measurable.col_name() + " - earth_moving_costs",
                     dict_emc,
                     self.count,
                     self.dashboard_name,
-                    file_name="embeddings"
+                    file_name="embeddings",
                 )
                 self.log_handler.add_scalars(
                     self.measurable.col_name() + " - earth_moving_costs",
                     {list(dict_emc.keys())[0]: self.emd_threshold},
                     self.count,
                     self.dashboard_name,
-                    file_name="threshold"
+                    file_name="threshold",
                 )
             else:
                 dict_psi = dict(
                     zip(
-                        ["y_" + self.measurable.col_name() + "_" + str(x) for x in range(self.psis.shape[0])],
+                        [
+                            "y_" + self.measurable.col_name() + "_" + str(x)
+                            for x in range(self.psis.shape[0])
+                        ],
                         [float(x) for x in list(self.psis)],
                     )
                 )
                 dict_psi.update({"threshold": 0.3})
                 self.log_handler.add_scalars(
                     self.measurable.col_name() + " - population_stability_index_scalar",
                     dict_psi,
@@ -202,35 +265,54 @@
                 )
 
     def base_is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
         is_interesting = np.array([False] * len(extra_args["id"]))
         reasons = ["None"] * len(extra_args["id"])
 
         if self.do_low_density_check and (len(self.low_density_regions) > 0):
-            dists_from_low_density_regions = np.min(np.sum(np.abs(self.feats - np.expand_dims(self.low_density_regions, axis=0)),axis=2),axis=1)
+            dists_from_low_density_regions = np.min(
+                np.sum(
+                    np.abs(
+                        self.feats - np.expand_dims(self.low_density_regions, axis=0)
+                    ),
+                    axis=2,
+                ),
+                axis=1,
+            )
             min_cluster_var = np.min(self.cluster_vars)
             is_close = dists_from_low_density_regions < min_cluster_var
             is_interesting = np.logical_or(is_close, is_interesting)
             for lkdx in range(len(is_close)):
                 if is_close[lkdx]:
-                    reasons[lkdx] = "Lies_to_Low_Density_Regions_In_Training_Distribution"
+                    reasons[
+                        lkdx
+                    ] = "Lies_to_Low_Density_Regions_In_Training_Distribution"
 
         if len(self.outliers):
-            dists_from_outliers = np.min(np.sum(np.abs(self.feats - np.expand_dims(self.outliers, axis=0)),axis=2),axis=1)
+            dists_from_outliers = np.min(
+                np.sum(
+                    np.abs(self.feats - np.expand_dims(self.outliers, axis=0)), axis=2
+                ),
+                axis=1,
+            )
             min_cluster_var = np.min(self.cluster_vars)
             is_close = dists_from_outliers < 0.5 * min_cluster_var
             is_interesting = np.logical_or(is_close, is_interesting)
             for lkdx in range(len(is_close)):
                 if is_close[lkdx]:
                     if dists_from_outliers[lkdx] < 0.0000001:
                         reasons[lkdx] = "Outlier_annotated_by_the_user"
                     else:
                         reasons[lkdx] = "Close_to_User_annotated_Outliers"
 
-        if self.save_edge_cases and self.drift_detected and not isinstance(self.feats[0,0,0], str):
+        if (
+            self.save_edge_cases
+            and self.drift_detected
+            and not isinstance(self.feats[0, 0, 0], str)
+        ):
             feats_shape = list(self.feats.shape)
             del feats_shape[1]
             self.feats = np.reshape(self.feats, tuple(feats_shape))
             for idx in range(self.ref_dist.shape[0]):
                 if self.is_embedding:
                     dist_from_cluster = (
                         np.sum(
@@ -273,55 +355,61 @@
                             min_dist_from_clusters > 1
                         )
                         if min_dist_from_clusters > 1:
                             reasons[jdx] = "Away_from_all_training_clusters"
 
         return is_interesting, reasons
 
-
     def bucket_reference_dataset(self):
         self.ref_dist = []
         self.prod_dist = []
         self.ref_dist_counts = []
         self.prod_dist_counts = []
-        if self.reference_dataset.split('.')[-1] == 'json':
+        if self.reference_dataset.split(".")[-1] == "json":
             data = read_json(self.reference_dataset)
             all_inputs = np.array(
                 [self.measurable.extract_val_from_training_data(x) for x in data]
             )
-        elif self.reference_dataset.split('.')[-1] == 'csv':
+        elif self.reference_dataset.split(".")[-1] == "csv":
             data = pd.read_csv(self.reference_dataset).to_dict()
             for key in data:
                 data[key] = list(data[key].values())
             all_inputs = np.array(self.measurable.extract_val_from_training_data(data))
         else:
             raise Exception("Reference data file type not recognized.")
-        
+
         all_inputs_shape = list(all_inputs.shape)
         if len(all_inputs_shape) == 1:
             all_inputs_shape.insert(1, 1)
             all_inputs = np.reshape(all_inputs, all_inputs_shape)
 
         clustering_results = self.clustering_helper.cluster_data(all_inputs)
 
-        self.buckets = np.array(clustering_results['buckets'])
-        self.clusters = np.array(clustering_results['clusters'])
-        self.cluster_vars = np.array(clustering_results['cluster_vars'])
-
-        self.ref_dist = np.array(clustering_results['dist'])
-        self.ref_dist_counts = np.array(clustering_results['dist_counts'])
-        self.max_along_axis = clustering_results['max_along_axis']
-        self.low_density_regions = clustering_results['low_density_regions']
+        self.buckets = np.array(clustering_results["buckets"])
+        self.clusters = np.array(clustering_results["clusters"])
+        self.cluster_vars = np.array(clustering_results["cluster_vars"])
+
+        self.ref_dist = np.array(clustering_results["dist"])
+        self.ref_dist_counts = np.array(clustering_results["dist_counts"])
+        self.max_along_axis = clustering_results["max_along_axis"]
+        self.low_density_regions = clustering_results["low_density_regions"]
 
         if self.hover_measurable is not None:
             all_hover_vals = np.array(
                 [self.hover_measurable.extract_val_from_training_data(x) for x in data]
             )
-            hover_label_idxs = [x[0] for x in list(clustering_results['idxs_closest_to_cluster_centroids'].values())]
-            self.bucket_labelling_info['hover_vals_for_reference_clusters'] = all_hover_vals[hover_label_idxs]
+            hover_label_idxs = [
+                x[0]
+                for x in list(
+                    clustering_results["idxs_closest_to_cluster_centroids"].values()
+                )
+            ]
+            self.bucket_labelling_info[
+                "hover_vals_for_reference_clusters"
+            ] = all_hover_vals[hover_label_idxs]
 
         self.prod_dist = np.zeros(self.ref_dist.shape)
         self.prod_dist_counts = np.zeros(self.ref_dist_counts.shape)
 
         self.prod_dist_counts_arr.append(copy.deepcopy(self.prod_dist_counts))
         if len(self.outlier_idxs):
-            self.outliers = all_inputs[np.array(self.outlier_idxs)]
+            self.outliers = all_inputs[np.array(self.outlier_idxs)]
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/data_integrity.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/data_integrity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import pandas as pd
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.ee.classes.measurables import GrammerScoreMeasurable
-from uptrain.constants import Monitor
-from uptrain.core.lib.helper_funcs import read_json
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.ee.classes.measurables import GrammerScoreMeasurable
+from uptrain.v0.constants import Monitor
+from uptrain.v0.core.lib.helper_funcs import read_json
 
 from scipy.stats import zscore
 
+
 class DataIntegrity(AbstractMonitor):
     dashboard_name = "data_integrity"
     monitor_type = Monitor.DATA_INTEGRITY
 
     def base_init(self, fw, check):
         self.integrity_type = check["integrity_type"]
         # Threshold value for data integrity check
@@ -19,45 +20,45 @@
         self.outliers_alert_thres = check.get("outliers_alert_thres", 2)
         self.count = 0
         self.num_issues = 0
         self.has_reference_dataset = "reference_dataset" in check
         if self.has_reference_dataset:
             self.reference_dataset = check["reference_dataset"]
             self.ref_mean, self.ref_std = self.get_ref_data_stats()
-            
+
     def base_check(self, inputs, outputs, gts=None, extra_args={}):
         signal_value = self.measurable.compute_and_log(
             inputs, outputs, gts=gts, extra=extra_args
         )
-        signal_value = np.squeeze(np.array(signal_value))
+        signal_value = np.reshape(np.array(signal_value), -1)
 
         if self.integrity_type == "non_null":
-            self.has_issue = signal_value == None
+            self.has_issue = [x == None for x in signal_value]
         elif self.integrity_type == "less_than":
             self.has_issue = signal_value > self.threshold
         elif self.integrity_type == "equal_to":
             self.has_issue = signal_value == self.threshold
         elif self.integrity_type == "greater_than":
             self.has_issue = signal_value < self.threshold
         elif self.integrity_type == "minus_one":
             self.has_issue = signal_value == -1
         elif self.integrity_type == "z_score":
             if self.threshold is None:
                 self.threshold = 3
-            
+
             # Calculating Z-scores w.r.t. the reference dataset
             if self.has_reference_dataset:
                 z_score = (signal_value - self.ref_mean) / self.ref_std
             # Calculating Z-scores w.r.t. the current dataset
             else:
                 z_score = zscore(signal_value)
             self.has_issue = np.abs(z_score) > self.threshold
             outliers = signal_value[self.has_issue]
             valid_signal = signal_value[~self.has_issue]
-            
+
             feat_name = self.measurable.col_name()
             plot_name = f"z_score_feature_{feat_name}"
             self.log_handler.add_histogram(
                 plot_name=plot_name,
                 data=valid_signal,
                 dashboard_name=self.dashboard_name,
                 file_name=f"valid_z_scores",
@@ -68,59 +69,63 @@
                     plot_name=plot_name,
                     data=outliers,
                     dashboard_name=self.dashboard_name,
                     file_name=f"outliers",
                 )
                 perc = round(percentage_outliers, 1)
                 self.log_handler.add_alert(
-                    alert_name = f"Z-score outliers detected for {feat_name} 🚨",
-                    alert = f"{len(outliers)} of {len(z_score)} samples have Z-Score > {self.threshold} ({perc}%)",
-                    dashboard_name = self.dashboard_name
+                    alert_name=f"Z-score outliers detected for {feat_name} 🚨",
+                    alert=f"{len(outliers)} of {len(z_score)} samples have Z-Score > {self.threshold} ({perc}%)",
+                    dashboard_name=self.dashboard_name,
                 )
         elif self.integrity_type == "grammar_check":
             self.has_issue = signal_value < self.threshold
         else:
             raise NotImplementedError(
                 "Data integrity check {} not implemented".format(self.integrity_type)
-            )            
+            )
         self.count += len(signal_value)
         self.num_issues += np.sum(np.array(self.has_issue))
 
         self.log_handler.add_scalars(
             self.integrity_type + "_outliers_ratio",
             {"y_outliers": self.num_issues / self.count},
             self.count,
             self.dashboard_name,
             file_name=self.measurable.col_name(),
         )
 
     def need_ground_truth(self):
         return False
-    
+
     def base_is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
         if self.integrity_type == "grammar_check":
             reasons = ["None"] * len(extra_args["id"])
             for idx in range(len(extra_args["id"])):
                 if self.has_issue[idx]:
-                    reasons.append("Data Integrity Issue, Type: {}".format(self.integrity_type))
+                    reasons.append(
+                        "Data Integrity Issue, Type: {}".format(self.integrity_type)
+                    )
             return self.has_issue, reasons
         else:
-            return np.array([False] * len(extra_args["id"])), np.array(['None'] * len(extra_args["id"]))
+            return np.array([False] * len(extra_args["id"])), np.array(
+                ["None"] * len(extra_args["id"])
+            )
 
     def get_ref_data_stats(self):
         """
         Find the mean and std for z-score in ref_arr. The data can be numerical or categorical.
         """
-        if self.reference_dataset.split('.')[-1] == 'json':
+        if self.reference_dataset.split(".")[-1] == "json":
             data = read_json(self.reference_dataset)
             all_inputs = np.array(
                 [self.measurable.extract_val_from_training_data(x) for x in data]
             )
-        elif self.reference_dataset.split('.')[-1] == 'csv':
+        elif self.reference_dataset.split(".")[-1] == "csv":
             data = pd.read_csv(self.reference_dataset).to_dict()
             for key in data:
                 data[key] = list(data[key].values())
             all_inputs = np.array(self.measurable.extract_val_from_training_data(data))
         else:
             raise Exception("Reference data file type not recognized.")
-        
+
         return np.mean(all_inputs), np.std(all_inputs)
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/edge_case.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/edge_case.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.core.classes.signals import SignalManager
-from uptrain.constants import Monitor
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.core.classes.signals import SignalManager
+from uptrain.v0.constants import Monitor
 
 
 class EdgeCase(AbstractMonitor):
     dashboard_name = "edge_cases"
     monitor_type = Monitor.EDGE_CASE
 
     def base_init(self, fw, check):
         self.signal_manager = SignalManager()
-        self.signal_manager.add_signal_formulae(check['signal_formulae'])
+        self.signal_manager.add_signal_formulae(check["signal_formulae"])
         self.num_preds = 0
         self.num_selected = 0
 
     def base_check(self, inputs, outputs, gts=None, extra_args={}):
         return
 
     def base_is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/feature_drift.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/feature_drift.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import scipy
 import pandas as pd
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import Monitor
-from uptrain.core.lib.helper_funcs import read_json
-from uptrain.core.classes.algorithms import Clustering
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.constants import Monitor
+from uptrain.v0.core.lib.helper_funcs import read_json
+from uptrain.v0.core.classes.algorithms import Clustering
 
 
 class FeatureDrift(AbstractMonitor):
     dashboard_name = "feature_drift"
 
     def model_choices(self, check):
         return [{"is_embedding": False}]
@@ -22,39 +22,38 @@
         self.prod_dist_counts_arr = []
         self.all_count = 0
         self.plot_name = "Feature " + self.measurable.col_name()
         self.feats = np.array([])
         self.psis = []
 
         self.train_dist, self.train_bins = self.get_ref_data_stats()
-        
+
         # convert the array self.train_bins into tuples of (min, max) values
         self.bar_vals = []
-        for i in range(len(self.train_bins)-1):
+        for i in range(len(self.train_bins) - 1):
             start_str = "{:.2f}".format(self.train_bins[i])
-            end_str = "{:.2f}".format(self.train_bins[i+1])
-            self.bar_vals.append(start_str + '-' + end_str)
-            
+            end_str = "{:.2f}".format(self.train_bins[i + 1])
+            self.bar_vals.append(start_str + "-" + end_str)
 
     def check(self, inputs, outputs, gts=None, extra_args={}):
         """
         Find the population stability index between the reference and
-        production distribtions by assigning them into 
-        reference buckets. 
+        production distribtions by assigning them into
+        reference buckets.
         """
 
         feats = self.measurable.compute_and_log(
             inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
         )
         self.all_count += len(feats)
         self.feats = np.append(self.feats, np.squeeze(np.array(feats)))
 
         if len(self.feats) >= self.step:
             prod_dist, _ = np.histogram(self.feats, bins=self.train_bins)
-            prod_dist = prod_dist/sum(prod_dist)
+            prod_dist = prod_dist / sum(prod_dist)
 
             # Find the PSI between the two distributions
             psi = self.get_psi(self.train_dist, prod_dist)
             self.psis.append(psi)
 
             self.log_handler.add_bar_graphs(
                 self.plot_name,
@@ -62,54 +61,54 @@
                     "reference": dict(zip(self.bar_vals, list(self.train_dist))),
                     "production": dict(zip(self.bar_vals, list(prod_dist))),
                 },
                 self.dashboard_name,
             )
 
             self.log_handler.add_scalars(
-                'psi',
-                {'y_psi': psi},
+                "psi",
+                {"y_psi": psi},
                 self.all_count,
                 self.dashboard_name,
                 file_name=self.measurable.col_name(),
             )
             feat_name = self.measurable.feature_name
 
             # High PSI alerts the user to a feature drift
             if psi > self.psi_threshold:
                 alert = f"Feature Drift last detected at {self.all_count} for {feat_name} with PSI = {psi}"
                 self.log_handler.add_alert(
-                        f"Feature Drift Alert for {feat_name} 🚨",
-                        alert,
-                        self.dashboard_name
-                    )
+                    f"Feature Drift Alert for {feat_name} 🚨", alert, self.dashboard_name
+                )
             self.feats = np.array([])
-        
+
     def get_ref_data_stats(self):
         """
         Find the bucketing scheme for data in ref_arr. The data can be numerical or categorical.
         """
-        if self.reference_dataset.split('.')[-1] == 'json':
+        if self.reference_dataset.split(".")[-1] == "json":
             data = read_json(self.reference_dataset)
             all_inputs = np.array(
                 [self.measurable.extract_val_from_training_data(x) for x in data]
             )
-        elif self.reference_dataset.split('.')[-1] == 'csv':
+        elif self.reference_dataset.split(".")[-1] == "csv":
             data = pd.read_csv(self.reference_dataset).to_dict()
             for key in data:
                 data[key] = list(data[key].values())
             all_inputs = np.array(self.measurable.extract_val_from_training_data(data))
         else:
             raise Exception("Reference data file type not recognized.")
-        
+
         prob = np.linspace(0, 1, self.NUM_BUCKETS + 1)
         bins = scipy.stats.mstats.mquantiles(all_inputs, prob)
         vals, bins = np.histogram(all_inputs, bins=bins)
-        return vals/sum(vals), bins
-    
+        return vals / sum(vals), bins
+
     def get_psi(self, ref_dist, prod_dist):
         """
         Find the population stability index between the two distributions.
         """
-        return np.sum(np.where(
-            ref_dist == 0, 0, (ref_dist - prod_dist) * np.log(ref_dist / prod_dist)
-        ))
+        return np.sum(
+            np.where(
+                ref_dist == 0, 0, (ref_dist - prod_dist) * np.log(ref_dist / prod_dist)
+            )
+        )
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/model_bias.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/model_bias.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.core.classes.algorithms import PopularityBias
-from uptrain.constants import BiasAlgo, Monitor
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.core.classes.algorithms import PopularityBias
+from uptrain.v0.constants import BiasAlgo, Monitor
 
 
 class ModelBias(AbstractMonitor):
     dashboard_name = "popularity_bias"
     monitor_type = Monitor.POPULARITY_BIAS
 
     def base_init(self, fw, check):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/monitors/output_comparison.py` & `uptrain-0.3.1/uptrain/v0/core/classes/monitors/output_comparison.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,59 @@
 import numpy as np
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Monitor, ComparisonModel, ComparisonMetric
+from uptrain.v0.core.classes.monitors import AbstractMonitor
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Monitor, ComparisonModel, ComparisonMetric
 
 
 class OutputComparison(AbstractMonitor):
     dashboard_name = "output_comparison"
     monitor_type = Monitor.OUTPUT_COMPARISON
 
     def base_init(self, fw, check):
-        self.comparison_model_base = check['comparison_model']
-        self.comparison_model_resolved = ComparisonModelResolver().resolve(check['comparison_model'])
-        self.comparison_model_inputs =  MeasurableResolver(check.get("comparison_model_input_args", None)).resolve(fw)
-        self.comparison_metric_base = check['comparison_metric']
-        self.comparison_metric_resolved = ComparisonMetricResolver().resolve(check['comparison_metric'])
-        self.threshold = check['threshold']
+        self.comparison_model_base = check["comparison_model"]
+        self.comparison_model_resolved = ComparisonModelResolver().resolve(
+            check["comparison_model"]
+        )
+        self.comparison_model_inputs = MeasurableResolver(
+            check.get("comparison_model_input_args", None)
+        ).resolve(fw)
+        self.comparison_metric_base = check["comparison_metric"]
+        self.comparison_metric_resolved = ComparisonMetricResolver().resolve(
+            check["comparison_metric"]
+        )
+        self.threshold = check["threshold"]
         self.count = 0
 
     def base_check(self, inputs, outputs, gts=None, extra_args={}):
         vals = self.measurable.compute_and_log(
             inputs, outputs, gts=gts, extra=extra_args
         )
 
         comparison_model_inputs = self.comparison_model_inputs.compute_and_log(
             inputs, outputs, gts=gts, extra=extra_args
         )
 
-        comparison_model_outputs = self.comparison_model_resolved(comparison_model_inputs)
+        comparison_model_outputs = self.comparison_model_resolved(
+            comparison_model_inputs
+        )
         batch_metrics = self.comparison_metric_resolved(vals, comparison_model_outputs)
         self.batch_metrics = batch_metrics
 
-        extra_args.update({self.comparison_model_base + " outputs": comparison_model_outputs, self.comparison_metric_base: batch_metrics})
+        extra_args.update(
+            {
+                self.comparison_model_base + " outputs": comparison_model_outputs,
+                self.comparison_metric_base: batch_metrics,
+            }
+        )
 
         feat_name = self.comparison_metric_base
-        plot_name = f"{feat_name} Comparison - Production vs {self.comparison_model_base}"
-        self.count += len(extra_args['id'])
+        plot_name = (
+            f"{feat_name} Comparison - Production vs {self.comparison_model_base}"
+        )
+        self.count += len(extra_args["id"])
 
         self.log_handler.add_scalars(
             plot_name,
             {"y_" + feat_name: np.mean(batch_metrics)},
             self.count,
             self.dashboard_name,
             file_name=plot_name,
@@ -51,29 +66,31 @@
         reasons = ["None"] * len(extra_args["id"])
         is_interesting = self.batch_metrics < self.threshold
         reasons = []
         for idx in range(len(extra_args["id"])):
             if is_interesting[idx] == 0:
                 reasons.append("None")
             else:
-                reasons.append(f"Different output compared to {self.comparison_model_base}")
+                reasons.append(
+                    f"Different output compared to {self.comparison_model_base}"
+                )
         return is_interesting, reasons
 
 
 class ComparisonModelResolver:
-
     def resolve(self, model):
         if model == ComparisonModel.FASTER_WHISPER:
-            from uptrain.ee.lib.algorithms import faster_whisper_speech_to_text
+            from uptrain.v0.ee.lib.algorithms import faster_whisper_speech_to_text
+
             return faster_whisper_speech_to_text
         else:
             raise Exception(f"{model} can't be resolved")
 
 
 class ComparisonMetricResolver:
-
     def resolve(self, metric):
         if metric == ComparisonMetric.ROGUE_L_F1:
-            from uptrain.ee.lib.algorithms import rogue_l_similarity
+            from uptrain.v0.ee.lib.algorithms import rogue_l_similarity
+
             return rogue_l_similarity
         else:
             raise Exception(f"{metric} can't be resolved")
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/signals/signal.py` & `uptrain-0.3.1/uptrain/v0/core/classes/signals/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import json_fix
 
-from uptrain.constants import MODEL_SIGNAL_TO_FN_MAPPING
+from uptrain.v0.constants import MODEL_SIGNAL_TO_FN_MAPPING
 
 
 class Signal:
     """
     Signal Class to identify edge cases
 
     ...
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/signals/signal_manager.py` & `uptrain-0.3.1/uptrain/v0/core/classes/signals/signal_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from uptrain.core.classes.signals import Signal
-from uptrain.constants import ModelSignal
+from uptrain.v0.core.classes.signals import Signal
+from uptrain.v0.constants import ModelSignal
 
 
 class SignalManager:
     """
     Manager class to help with signal evalutions
 
     ...
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/statistics/convergence.py` & `uptrain-0.3.1/uptrain/v0/core/classes/statistics/convergence.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 import numpy as np
 
-from uptrain.core.lib.helper_funcs import make_2d_np_array
-from uptrain.core.classes.distances import DistanceResolver
-from uptrain.core.classes.statistics import AbstractStatistic
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Statistic
-from uptrain.core.lib.cache import make_cache_container
+from uptrain.v0.core.lib.helper_funcs import make_2d_np_array
+from uptrain.v0.core.classes.distances import DistanceResolver
+from uptrain.v0.core.classes.statistics import AbstractStatistic
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Statistic
+from uptrain.v0.core.lib.cache import make_cache_container
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.new_log_handler import (
+    from uptrain.v0.core.classes.logging.new_log_handler import (
         LogHandler as NewLogHandler,
         LogWriter,
     )
-    from uptrain.core.classes.logging.log_handler import LogHandler
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler
 
-# from uptrain.core.classes.algorithms import Clustering
-# from uptrain.core.lib.algorithms import estimate_earth_moving_cost
+# from uptrain.v0.core.classes.algorithms import Clustering
+# from uptrain.v0.core.lib.algorithms import estimate_earth_moving_cost
 
 
 class Convergence(AbstractStatistic):
     log_handler: Union["LogHandler", "NewLogHandler"]
     log_writers: list["LogWriter"]
     dashboard_name = "convergence_stats"
     statistic_type = Statistic.CONVERGENCE_STATS
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/statistics/distance.py` & `uptrain-0.3.1/uptrain/v0/core/classes/statistics/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 import numpy as np
 
-from uptrain.core.classes.statistics import AbstractStatistic
-from uptrain.core.classes.distances import DistanceResolver
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Statistic
-from uptrain.core.lib.cache import make_cache_container
+from uptrain.v0.core.classes.statistics import AbstractStatistic
+from uptrain.v0.core.classes.distances import DistanceResolver
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Statistic
+from uptrain.v0.core.lib.cache import make_cache_container
 
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.new_log_handler import (
+    from uptrain.v0.core.classes.logging.new_log_handler import (
         LogHandler as NewLogHandler,
         LogWriter,
     )
-    from uptrain.core.classes.logging.log_handler import LogHandler
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler
 
 
 class Distance(AbstractStatistic):
     log_handler: Union["LogHandler", "NewLogHandler"]
     log_writers: list["LogWriter"]
     dashboard_name = "distance"
     statistic_type = Statistic.DISTANCE
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/statistics/distribution.py` & `uptrain-0.3.1/uptrain/v0/core/classes/statistics/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 """
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 import numpy as np
 import random
 
-from uptrain.core.lib.helper_funcs import make_2d_np_array
-from uptrain.core.classes.distances import DistanceResolver
-from uptrain.core.classes.statistics import AbstractStatistic
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Statistic
-from uptrain.core.lib.cache import make_cache_container
+from uptrain.v0.core.lib.helper_funcs import make_2d_np_array
+from uptrain.v0.core.classes.distances import DistanceResolver
+from uptrain.v0.core.classes.statistics import AbstractStatistic
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Statistic
+from uptrain.v0.core.lib.cache import make_cache_container
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.new_log_handler import (
+    from uptrain.v0.core.classes.logging.new_log_handler import (
         LogHandler as NewLogHandler,
         LogWriter,
     )
-    from uptrain.core.classes.logging.log_handler import LogHandler
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler
 
 
 class Distribution(AbstractStatistic):
     log_handler: Union["LogHandler", "NewLogHandler"]
     log_writers: list["LogWriter"]  # one for each distance type
     dashboard_name = "distribution_stats"
     statistic_type = Statistic.DISTRIBUTION_STATS
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/statistics/norm_embedding.py` & `uptrain-0.3.1/uptrain/v0/core/classes/statistics/norm_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import numpy as np
 
-from uptrain.core.classes.statistics import AbstractStatistic
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Statistic
+from uptrain.v0.core.classes.statistics import AbstractStatistic
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Statistic
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.new_log_handler import (
+    from uptrain.v0.core.classes.logging.new_log_handler import (
         LogHandler as NewLogHandler,
         LogWriter,
     )
-    from uptrain.core.classes.logging.log_handler import LogHandler
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler
 
 
 class NormEmbedding(AbstractStatistic):
     """Class that computes the norm of an embedding column."""
 
     log_handler: "NewLogHandler"
     log_writer: "LogWriter"
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/statistics/old_distribution.py` & `uptrain-0.3.1/uptrain/v0/core/classes/statistics/old_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import TYPE_CHECKING
 import numpy as np
 import random
 
-from uptrain.core.lib.helper_funcs import extract_data_points_from_batch
-from uptrain.core.classes.distances import DistanceResolver
-from uptrain.core.classes.statistics import AbstractStatistic
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Statistic
+from uptrain.v0.core.lib.helper_funcs import extract_data_points_from_batch
+from uptrain.v0.core.classes.distances import DistanceResolver
+from uptrain.v0.core.classes.statistics import AbstractStatistic
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.constants import Statistic
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.log_handler import LogHandler, CsvWriter
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler, CsvWriter
 
 
 class Distribution(AbstractStatistic):
     dashboard_name = "distribution_stats"
     statistic_type = Statistic.DISTRIBUTION_STATS
 
     def base_init(self, fw, check):
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/visuals/clustering.py` & `uptrain-0.3.1/uptrain/v0/core/classes/visuals/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 try:
     import hdbscan
 except:
     hdbscan = None
 from sklearn.cluster import DBSCAN
 from typing import Any, Dict, Union
 
-from uptrain.constants import ClusteringAlgorithm
-from uptrain.core.lib.helper_funcs import dependency_required
+from uptrain.v0.constants import ClusteringAlgorithm
+from uptrain.v0.core.lib.helper_funcs import dependency_required
 
 
 class Clustering(ABC):
     def __init__(self):
         super().__init__()
 
     def resolve(self, args: Dict[str, Any]) -> Any:
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/visuals/dimensionality_reduction.py` & `uptrain-0.3.1/uptrain/v0/core/classes/visuals/dimensionality_reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 try:
     import umap
 except:
     umap = None
 import numpy as np
 from sklearn.manifold import TSNE
 
-from uptrain.core.lib.helper_funcs import cluster_and_plot_data
-from uptrain.core.classes.visuals import AbstractVisual, ClusteringResolver
-from uptrain.constants import Visual, Statistic, MeasurableType, ClusteringAlgorithm
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.core.lib.helper_funcs import read_json, dependency_required
+from uptrain.v0.core.lib.helper_funcs import cluster_and_plot_data
+from uptrain.v0.core.classes.visuals import AbstractVisual, ClusteringResolver
+from uptrain.v0.constants import Visual, Statistic, MeasurableType, ClusteringAlgorithm
+from uptrain.v0.core.classes.measurables import MeasurableResolver
+from uptrain.v0.core.lib.helper_funcs import read_json, dependency_required
 
 if TYPE_CHECKING:
-    from uptrain.core.classes.logging.new_log_handler import (
+    from uptrain.v0.core.classes.logging.new_log_handler import (
         LogHandler as NewLogHandler,
         LogWriter,
     )
-    from uptrain.core.classes.logging.log_handler import LogHandler
+    from uptrain.v0.core.classes.logging.log_handler import LogHandler
 
 
 @dependency_required(umap, "umap-learn")
 class DimensionalityReduction(AbstractVisual):
     log_handler: Union["LogHandler", "NewLogHandler"]
     log_writer: Optional["LogWriter"]
 
@@ -35,15 +35,17 @@
             self.tsne_init(check)
         else:
             raise Exception("Dimensionality reduction type undefined.")
         self.framework = fw
         self.clustering_algorithm = ClusteringResolver(
             check.get("clustering_algorithm", ClusteringAlgorithm.HDBSCAN)
         ).resolve(check.get("clustering_args", {}))
-        self.label_measurables = [MeasurableResolver(x).resolve(fw) for x in check.get("label_args", [])]
+        self.label_measurables = [
+            MeasurableResolver(x).resolve(fw) for x in check.get("label_args", [])
+        ]
         label_names = [x.col_name() for x in self.label_measurables]
         self.labels = {"clusters": []}
         for label_name in label_names:
             self.labels[label_name] = []
         self.hover_measurables = [
             MeasurableResolver(x).resolve(fw) for x in check.get("hover_args", [])
         ]
@@ -74,15 +76,17 @@
         if self.initial_dataset is not None:
             data = read_json(self.initial_dataset)
             self.vals.extend(
                 [self.measurable.extract_val_from_training_data(x) for x in data]
             )
 
             for label_measurable in self.label_measurables:
-                label_data = [label_measurable.extract_val_from_training_data(x) for x in data]
+                label_data = [
+                    label_measurable.extract_val_from_training_data(x) for x in data
+                ]
                 self.labels[label_measurable.col_name()] = label_data
             if len(self.hover_measurables):
                 offset = 0
                 for data_point in data:
                     this_hovers = [
                         x.extract_val_from_training_data(data_point)
                         for x in self.hover_measurables
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/visuals/plot.py` & `uptrain-0.3.1/uptrain/v0/core/classes/visuals/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict
 
-from uptrain.core.classes.visuals import AbstractVisual
-from uptrain.constants import PlotType, Visual
+from uptrain.v0.core.classes.visuals import AbstractVisual
+from uptrain.v0.constants import PlotType, Visual
 
 
 class Plot(AbstractVisual):
     """Class to expose the plotting API."""
 
     visual_type = Visual.PLOT
```

### Comparing `uptrain-0.2.0/uptrain/core/classes/visuals/shap.py` & `uptrain-0.3.1/uptrain/v0/core/classes/visuals/shap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import pickle
 
 try:
     import shap
 except:
     shap = None
 
-from uptrain.core.classes.visuals import AbstractVisual
-from uptrain.constants import Visual
-from uptrain.core.lib.helper_funcs import dependency_required
+from uptrain.v0.core.classes.visuals import AbstractVisual
+from uptrain.v0.constants import Visual
+from uptrain.v0.core.lib.helper_funcs import dependency_required
 
 
 @dependency_required(shap, "shap")
 class Shap(AbstractVisual):
     visual_type = Visual.SHAP
     dashboard_name = "SHAP_explanation"
```

### Comparing `uptrain-0.2.0/uptrain/core/encoders/__init__.py` & `uptrain-0.3.1/uptrain/v0/core/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/lib/algorithms.py` & `uptrain-0.3.1/uptrain/v0/core/lib/algorithms.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/lib/cache.py` & `uptrain-0.3.1/uptrain/v0/core/lib/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         return output
 
 
 def make_cache_container(fw: Any, columns: dict[str, Type]) -> StateCache:
     """Create a state cache container for the given columns."""
     if fw.config_obj.running_ee:
         try:
-            from uptrain.ee.lib.cache import DuckDBStateCache
+            from uptrain.v0.ee.lib.cache import DuckDBStateCache
         except ImportError as exc:
             print(
                 "Error importing the uptrain-ee subpackage, Uptrain enterprise Edition not installed."
             )
             raise exc
 
         return DuckDBStateCache(fw, columns)
```

### Comparing `uptrain-0.2.0/uptrain/core/lib/datastores.py` & `uptrain-0.3.1/uptrain/v0/core/lib/datastores.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/core/lib/helper_funcs.py` & `uptrain-0.3.1/uptrain/v0/core/lib/helper_funcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime, timedelta, tzinfo
 from collections import OrderedDict
 import functools
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import KMeans
-from uptrain.core.encoders import UpTrainEncoder
+from uptrain.v0.core.encoders import UpTrainEncoder
 
 
 def cluster_and_plot_data(
     data,
     num_clusters,
     cluster_plot_func=None,
     plot_save_name="",
```

### Comparing `uptrain-0.2.0/uptrain/core/lib/model_signal_funcs.py` & `uptrain-0.3.1/uptrain/v0/core/lib/model_signal_funcs.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain/ee/classes/measurables/llm_measurables.py` & `uptrain-0.3.1/uptrain/v0/ee/classes/measurables/llm_measurables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
-from uptrain.core.lib.helper_funcs import read_json, dependency_required
-from uptrain.core.classes.measurables import Measurable
+from uptrain.v0.core.lib.helper_funcs import read_json, dependency_required
+from uptrain.v0.core.classes.measurables import Measurable
 
 try:
     import openai
 except:
     openai = None
```

### Comparing `uptrain-0.2.0/uptrain/ee/lib/algorithms.py` & `uptrain-0.3.1/uptrain/v0/ee/lib/algorithms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
-from uptrain.core.lib.helper_funcs import fn_dependency_required
+from uptrain.v0.core.lib.helper_funcs import fn_dependency_required
 
 try:
     import faster_whisper
 except:
     faster_whisper = None
 
 try:
     import rouge
 except:
     rouge = None
 
-@fn_dependency_required(faster_whisper, "faster_whisper")
+@fn_dependency_required(faster_whisper, "faster-whisper")
 def faster_whisper_speech_to_text(audio_files):
     model_size = "large-v2"
     model = faster_whisper.WhisperModel(model_size, device="cpu", compute_type="int8")
     prescribed_texts = []
     for audio_file in audio_files:
         segments, _ = model.transcribe(audio_file, beam_size=5)
         prescribed_text = ''
```

### Comparing `uptrain-0.2.0/uptrain/ee/lib/cache.py` & `uptrain-0.3.1/uptrain/v0/ee/lib/cache.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.2.0/uptrain.egg-info/PKG-INFO` & `uptrain-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrain
-Version: 0.2.0
+Version: 0.3.1
 Summary: UpTrain - ML Observability and Retraining Framework
 Home-page: https://github.com/uptrain-ai/uptrain
 Maintainer: UpTrain AI Team
 Maintainer-email: uptrain.ai@gmail.com
 License: Apache License 2.0
 Keywords: uptrain ai retraining ML observability
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,33 +12,35 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+Provides-Extra: v0
+Provides-Extra: full
 License-File: LICENSE
 
 <h4 align="center">
   <a href="https://uptrain.ai">
     <img width="300" src="https://user-images.githubusercontent.com/108270398/214240695-4f958b76-c993-4ddd-8de6-8668f4d0da84.png" alt="uptrain">
   </a>
 </h4>
 <h2>
   <p align="center">
-    <p align="center">An open-source framework to observe ML applications, built for engineers</p>
+    <p align="center">An open-source framework to evaluate, test and monitor LLM applications</p>
   </p>
 </h2>
 
 <p align="center">
 <a href="https://docs.uptrain.ai/docs/" rel="nofollow"><strong>Docs</strong></a>
+<!-- -
+<a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a> -->
 -
-<a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/" rel="nofollow"><strong>Try it out</strong></a>
--
-<a href="https://discord.com/invite/gVvZhhrQaQ/" rel="nofollow"><strong>Discord Community</strong></a>
+<a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg" rel="nofollow"><strong>Slack Community</strong></a>
 -
 <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=bug&template=bug_report.md&title=" rel="nofollow"><strong>Bug Report</strong></a>
 -
 <a href="https://github.com/uptrain-ai/uptrain/issues/new?assignees=&labels=enhancement&template=feature_request.md&title=" rel="nofollow"><strong>Feature Request</strong></a>
 </p>
 
 <h4 align="center">
@@ -47,145 +49,148 @@
   </a>
   <a href='https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md'>
     <img alt='PRs Welcome' src='https://img.shields.io/badge/PRs-welcome-orange.svg?style=shields'/>
   </a>
   <a href="https://docs.uptrain.ai/docs/">
     <img src="https://img.shields.io/badge/Read-Docs-brightgreen" alt="Docs" />
   </a>
-  <a href="https://discord.com/invite/gVvZhhrQaQ">
-    <img src="https://img.shields.io/badge/Discord-Community-orange" alt="Community" />
+  <a href="https://join.slack.com/t/uptraincommunity/shared_invite/zt-1yih3aojn-CEoR_gAh6PDSknhFmuaJeg">
+    <img src="https://img.shields.io/badge/Slack-Community-orange" alt="Community" />
   </a>
   <a href="https://uptrain.ai/">
     <img src="https://img.shields.io/badge/UpTrain-Website-yellow" alt="Website" />
   </a>
-  <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/">
+  <!-- <a href="https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing/">
     <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-  </a>
+  </a> -->
 </h4>
 
-https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-4be1-83cf-408d5271518e.mp4
+<!-- https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-4be1-83cf-408d5271518e.mp4 -->
 
-**Read this in other languages**: 
+<!-- **Read this in other languages**: 
 <kbd>[<img title="English" alt="English language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/us.svg" width="22">](/README.md)</kbd>
 <kbd>[<img title="German" alt="German language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/de.svg" width="22">](/i18n/README.de.md)</kbd>
 <kbd>[<img title="Chinese" alt="Chinese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/cn.svg" width="22">](/i18n/README.zh-CN.md)</kbd>
 <kbd>[<img title="Hindi" alt="Hindi language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/in.svg" width="22">](/i18n/README.hi.md)</kbd>
 <kbd>[<img title="Spanish" alt="Spanish language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/es.svg" width="22">](/i18n/README.es.md)</kbd>
 <kbd>[<img title="French" alt="French language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/fr.svg" width="22">](/i18n/README.fr.md)</kbd>
 <kbd>[<img title="Japanese" alt="Japanese language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/jp.svg" width="22">](/i18n/README.ja.md)</kbd>
-<kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd>
+<kbd>[<img title="Russian" alt="Russian language" src="https://cdn.staticaly.com/gh/hjnilsson/country-flags/master/svg/ru.svg" width="22">](/i18n/README.ru.md)</kbd> -->
 
 
-**[UpTrain](https://uptrain.ai)** is an open-source, data-secure tool for ML practitioners to observe and refine their ML models by monitoring their performance, checking for (data) distribution shifts, and collecting edge cases to retrain them upon. It integrates seamlessly with your existing production pipelines and takes minutes to get started ⚡.
+**[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM applications are performing reliably by allowing users to check aspects such as correctness, structural integrity, bias, hallucination, etc. UpTrain can be used to:
 
+1) Validate model's response and safeguard your users against hallucinations, bias, incorrect output formats, etc.
+2) Experiment across multiple model providers, prompt templates, and quantify model's performance.
+3) Monitor your model's performance in production and protect yourself against unwanted drifts
 
-# **[Key Features](https://uptrain.gitbook.io/docs/what-is-uptrain/key-features)** 💡
 
-- **[Data Drift Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-drift)** - Identify distribution shifts in your model inputs.
-- **[Performance Monitoring](https://docs.uptrain.ai/docs/uptrain-monitors/concept-drift)** - Track the performance of your models in realtime and get degradation alerts.
-- **[Embeddings Support](https://github.com/uptrain-ai/uptrain/blob/main/examples/text_summarization/run.ipynb)** - Specialized dashboards to understand model-inferred embeddings.
-- **[Edge Case Signals](https://docs.uptrain.ai/docs/uptrain-monitors/edge-case-detection)** - User-defined signals and statistical techniques to detect out-of-distribution data-points.
-- **[Data Integrity Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-integrity)** - Checks for missing or inconsistent data, duplicate records, data quality, etc. 
-- **[Customizable metrics](https://docs.uptrain.ai/docs/monitoring-custom-metrics)** - Define custom metrics that make sense for your use case.
-- **[Automated Retraining](https://github.com/uptrain-ai/uptrain/blob/main/examples/human_orientation_classification/deepdive_examples/uptrain_check_all.ipynb)** - Automate model retraining by attaching your training and inference pipelines.
-- **[Model Bias](https://docs.uptrain.ai/docs/uptrain-monitors/model-bias)** - Track bias in your ML model's predictions.
-- **[AI Explainability](https://docs.uptrain.ai/docs/uptrain-visuals/shap-explainability)** - Understand relative importance of multiple features on predictions.
-- **Data Security** - Your data never goes out of your machine.
-- **Slack Integration** - Get alerts on Slack.
-- **Realtime Dashboards** - To visualize your model's health live.
-
-## 🚨Coming soon🚨
-
-- **Label Shift** - Identify drifts in your predictions. Specially useful in cases when ground truth is unavailable.
-- **Model confidence interval** - Confidence intervals for model predictions 
-- **Advanced drift detection techniques** - Outlier-based drift detection methods
-- **Advanced feature slicing** - Ability to slice statistical properties
-- **Kolmogorov-Smirnov Test** - For detecting distribution shifts
-- **Prediction Stability** - Filter cases where model prediction is not stable.
-- **Adversarial Checks** - Combat adversarial attacks
+# Key Features 💡
 
-And more.
 
+- **[ChatGPT Grading](https://uptrain-ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to grade your model outputs.
+- **[Custom Grading Checks](https://uptrain-ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom grading prompts.
+- **[Embeddings Similarity Check](https://uptrain-ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity between prompt and response embeddings
+- **[Output Validation](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** - Safeguard your users against inappropriate responses
+- **[Prompt A/B Testing](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and compare them quantatively.
+- **[UMAP Visualization and Clustering](https://uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding space using tools like UMAP and t-SNE.
+- **[Hallucination Checks]()** - Use metrics like custom grading, text similarity, and embedding similarity to check for hallucinations.
+- **[Toxic Keywords Checks]()** - Make sure your model outputs are not biased or contain toxic keywords.
+- **[Feature Slicing]()** - Built-in pivoting functionalities for data dice and slice to pinpoint low-performing cohorts.
+- **[Realtime Dashboards]()** - Monitor your model's performance in realtime.
 
 # Get started 🙌
 
-You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F).
+<!-- You can quickly get started with [Google Colab here](https://colab.research.google.com/drive/1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). -->
 
-To run it in your machine, follow the steps below:
+To run it on your machine, checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/quickstart):
 
 ### Install the package through pip:
-```console
+```bash
 pip install uptrain
 ```
 
-### Run your first example:
-```console
-git clone git@github.com:uptrain-ai/uptrain.git
-cd uptrain/examples
-pip install jupyterlab
-jupyter lab
+### How to define checks:
+Say we want to check whether our model's responses contain any grammatical mistakes or not.
+
+```python
+# Define your checkset - list of simple checks, dataset file, 
+# and api_keys
+
+checkset = CheckSet(
+    checks = Check(
+        name = "grammar_score",
+        operators = [
+            GrammarScore(
+                col_in_text = "model_response",
+                col_out = "grammar_score"
+            ),
+        ],
+        plots = PlotlyChart.Table(title="Grammar scores"),
+    ),
+    source = JsonReader(fpath = '...')
+)
+settings = Settings(openai_api_key = '...')
+
+checkset.setup(settings)
+checkset.run()
 ```
 
-For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial).
+<!-- For a quick walkthrough of how UpTrain works, check out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/quickstart-tutorial). -->
 
 <h4> </h4>
 
-# UpTrain in [action](https://github.com/uptrain-ai/uptrain/blob/main/examples/text_summarization/run.ipynb) 🎬
+# Integrations
 
-One of the most common use cases of ML today is language models, be it text summarization, NER, chatbots, language translation, etc. UpTrain provides ways to visualize differences in the training and real-world data via UMAP clustering of text embeddings (inferred from BERT). Following are some replays from the UpTrain dashboard.
+| Eval Frameworks  | LLM Providers | LLM Packages | Serving frameworks | 
+| ------------- | ------------- | ------------- | ------------- | 
+| OpenAI Evals ✅ | GPT-3.5-turbo ✅ | Langchain 🔜 | HuggingFace 🔜 |
+| EleutherAI LM Eval 🔜 | GPT-4 ✅  | Llama Index 🔜 |  Replicate 🔜 |
+| BIG-Bench 🔜 | Claude 🔜 | AutoGPT 🔜 |
+| | Cohere 🔜 | 
 
-### AI Explainability out-of-the-box
 
-<h1 align="center">
-<img alt="umap_gif" width="60%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/ride_estimation/4_Explanability_recording.gif">
-</h1>
+# UpTrain in Action
 
-### Live Model Performance Monitoring and Data Integrity Checks
+## Experimentation
 
-<h1 align="center">
-<img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/fraud_detection/concept_drift_avg_acc.gif"> <img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/finetuning_llms/data_integrity.gif">
-</h1>
+You can use the UpTrain framework to run and compare LLM responses for different prompts, models, LLM chains, etc. Check out the [experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/examples/prompt_experiments_tutorial.ipynb) to learn more.
 
-### UMAP Dimensionality Reduction and Visualization
+## Validation
 
-<h1 align="center">
-<img alt="umap_gif" width="60%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/text_summarization/umap.gif">
-</h1>
+You can use the UpTrain Validation Manager to define checks, retry logic and validate your LLM responses before showing it to your users. Check out the [tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb).
 
+## Monitoring
 
-### Edge-case Collection for Finetuning the Model later
+You can use the UpTrain framework to continuously monitor your model's performance and get real-time insights on how well it is doing on a variety of evaluation metrics. Check out the monitoring tutorial to learn more.
 
-<h1 align="center">
-<img alt="perf_gif" width="40%" src="https://uptrain-demo.s3.us-west-1.amazonaws.com/finetuning_llms/edge_cases.gif">
-</h1>
 
 # Why UpTrain 🤔?
 
-Machine learning (ML) models are widely used to make critical business decisions. Still, no ML model is 100% accurate, and, further, their accuracy deteriorates over time 😣. For example, Sales prediction becomes inaccurate over time due to a shift in consumer buying habits. Additionally, due to the black box nature of ML models, it's challenging to identify and fix their problems.
+Large language models are trained over billions of data points and perform really well over a wide variety of tasks. But one thing these models are not good at is being deterministic. Even with the most well-crafted prompts, the model can misbehave for certain inputs, be it hallucinations, wrong output structure, toxic or biased response, irrelevant response, and error modes can be immense. 
 
-UpTrain solves this. We make it easy for data scientists and ML engineers to understand where their models are going wrong and help them fix them before others complain 🗣️.
+To ensure your LLM applications work reliably and correctly, UpTrain makes it easy for developers to evaluate the responses of their applications on multiple criteria. UpTrain's evaluation framework can be used to:
 
-UpTrain can be used for a wide variety of Machine learning models such as LLMs, recommendation models, prediction models, Computer vision models, etc.
+1) Validate (and correct) the response of the model before showing it to the user
+2) Get quantitative measures to experiment across multiple prompts, model providers, etc.
+3) Do unit testing to ensure no buggy prompt or code gets pushed into your production
+4) Monitor your LLM applications in real time and understand when they are going wrong in order to fix them before users complain.
 
 We are constantly working to make UpTrain better. Want a new feature or need any integrations? Feel free to [create an issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the repository.
 
-<h1 align="center">
-<img alt="Meme" width="40%" src="https://user-images.githubusercontent.com/108270398/215209245-4d6b1f47-7af9-4db8-8d8c-63dcc610571c.jpg">
-</h1>
-
 # License 💻
 
-This repo is published under Apache 2.0 license, with the exception of the ee directory which will contain premium features requiring an enterprise license in the future. We're currently focused on developing non-enterprise offerings that should cover most use cases by adding more features and extending to more models. We also working towards adding a hosted offering - [contact us](mailto:tech@uptrain.ai) if you are interested.
+This repo is published under Apache 2.0 license. We are also working towards adding a hosted offering to make setting off eval runs easier - please fill **[this form](https://docs.google.com/forms/d/e/1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/viewform?usp=sf_link)** to get a waitlist slot.
 
 # Stay Updated ☎️
 We are continuously adding tons of features and use cases. Please support us by giving the project a star ⭐!
 
 # Provide feedback (Harsher the better 😉) 
 
-We are building UpTrain in public. Help us improve by giving your feedback **[here](https://forms.gle/PXd89D5LiFubro9o9)**.
+We are building UpTrain in public. Help us improve by giving your feedback **[here](https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**.
 
 # Contributors 🖥️
 
 We welcome contributions to UpTrain. Please see our [contribution guide](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for details.
 
 <a href="https://github.com/uptrain-ai/uptrain/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=uptrain-ai/uptrain" />
```

#### html2text {}

```diff
@@ -1,110 +1,99 @@
-Metadata-Version: 2.1 Name: uptrain Version: 0.2.0 Summary: UpTrain - ML
+Metadata-Version: 2.1 Name: uptrain Version: 0.3.1 Summary: UpTrain - ML
 Observability and Retraining Framework Home-page: https://github.com/uptrain-
 ai/uptrain Maintainer: UpTrain AI Team Maintainer-email: uptrain.ai@gmail.com
 License: Apache License 2.0 Keywords: uptrain ai retraining ML observability
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-License-File: LICENSE
+Provides-Extra: v0 Provides-Extra: full License-File: LICENSE
                                *** [uptrain] ***
-***** An open-source framework to observe ML applications, built for engineers
+***** An open-source framework to evaluate, test and monitor LLM applications
 *****
-     Docs - Try_it_out - Discord_Community - Bug_Report - Feature_Request
+            Docs  - Slack_Community - Bug_Report - Feature_Request
    *** [https://img.shields.io/github/contributors/uptrain-ai/uptrain] [PRs
-           Welcome] [Docs] [Community] [Website] [Open_In_Colab] ***
-https://user-images.githubusercontent.com/43818888/229681912-a1d9733d-0c41-
-4be1-83cf-408d5271518e.mp4 **Read this in other languages**: [[English
-language]](/README.md) [[German language]](/i18n/README.de.md) [[Chinese
-language]](/i18n/README.zh-CN.md) [[Hindi language]](/i18n/README.hi.md) [
-[Spanish language]](/i18n/README.es.md) [[French language]](/i18n/README.fr.md)
-[[Japanese language]](/i18n/README.ja.md) [[Russian language]](/i18n/
-README.ru.md) **[UpTrain](https://uptrain.ai)** is an open-source, data-secure
-tool for ML practitioners to observe and refine their ML models by monitoring
-their performance, checking for (data) distribution shifts, and collecting edge
-cases to retrain them upon. It integrates seamlessly with your existing
-production pipelines and takes minutes to get started â¡. # **[Key Features]
-(https://uptrain.gitbook.io/docs/what-is-uptrain/key-features)** ð¡ - **[Data
-Drift Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-drift)** -
-Identify distribution shifts in your model inputs. - **[Performance Monitoring]
-(https://docs.uptrain.ai/docs/uptrain-monitors/concept-drift)** - Track the
-performance of your models in realtime and get degradation alerts. - **
-[Embeddings Support](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-text_summarization/run.ipynb)** - Specialized dashboards to understand model-
-inferred embeddings. - **[Edge Case Signals](https://docs.uptrain.ai/docs/
-uptrain-monitors/edge-case-detection)** - User-defined signals and statistical
-techniques to detect out-of-distribution data-points. - **[Data Integrity
-Checks](https://docs.uptrain.ai/docs/uptrain-monitors/data-integrity)** -
-Checks for missing or inconsistent data, duplicate records, data quality, etc.
-- **[Customizable metrics](https://docs.uptrain.ai/docs/monitoring-custom-
-metrics)** - Define custom metrics that make sense for your use case. - **
-[Automated Retraining](https://github.com/uptrain-ai/uptrain/blob/main/
-examples/human_orientation_classification/deepdive_examples/
-uptrain_check_all.ipynb)** - Automate model retraining by attaching your
-training and inference pipelines. - **[Model Bias](https://docs.uptrain.ai/
-docs/uptrain-monitors/model-bias)** - Track bias in your ML model's
-predictions. - **[AI Explainability](https://docs.uptrain.ai/docs/uptrain-
-visuals/shap-explainability)** - Understand relative importance of multiple
-features on predictions. - **Data Security** - Your data never goes out of your
-machine. - **Slack Integration** - Get alerts on Slack. - **Realtime
-Dashboards** - To visualize your model's health live. ## ð¨Coming soonð¨ -
-**Label Shift** - Identify drifts in your predictions. Specially useful in
-cases when ground truth is unavailable. - **Model confidence interval** -
-Confidence intervals for model predictions - **Advanced drift detection
-techniques** - Outlier-based drift detection methods - **Advanced feature
-slicing** - Ability to slice statistical properties - **Kolmogorov-Smirnov
-Test** - For detecting distribution shifts - **Prediction Stability** - Filter
-cases where model prediction is not stable. - **Adversarial Checks** - Combat
-adversarial attacks And more. # Get started ð You can quickly get started
-with [Google Colab here](https://colab.research.google.com/drive/
-1ZIITMB7XYotvhg5CNvGPFnBdM4SR2w4Q?usp=sharing%2F). To run it in your machine,
-follow the steps below: ### Install the package through pip: ```console pip
-install uptrain ``` ### Run your first example: ```console git clone
-git@github.com:uptrain-ai/uptrain.git cd uptrain/examples pip install
-jupyterlab jupyter lab ``` For a quick walkthrough of how UpTrain works, check
-out our [quickstart tutorial](https://docs.uptrain.ai/docs/uptrain-examples/
-quickstart-tutorial).
-# UpTrain in [action](https://github.com/uptrain-ai/uptrain/blob/main/examples/
-text_summarization/run.ipynb) ð¬ One of the most common use cases of ML today
-is language models, be it text summarization, NER, chatbots, language
-translation, etc. UpTrain provides ways to visualize differences in the
-training and real-world data via UMAP clustering of text embeddings (inferred
-from BERT). Following are some replays from the UpTrain dashboard. ### AI
-Explainability out-of-the-box
-                           ****** [umap_gif] ******
-### Live Model Performance Monitoring and Data Integrity Checks
-                      ****** [perf_gif] [perf_gif] ******
-### UMAP Dimensionality Reduction and Visualization
-                           ****** [umap_gif] ******
-### Edge-case Collection for Finetuning the Model later
-                           ****** [perf_gif] ******
-# Why UpTrain ð¤? Machine learning (ML) models are widely used to make
-critical business decisions. Still, no ML model is 100% accurate, and, further,
-their accuracy deteriorates over time ð£. For example, Sales prediction
-becomes inaccurate over time due to a shift in consumer buying habits.
-Additionally, due to the black box nature of ML models, it's challenging to
-identify and fix their problems. UpTrain solves this. We make it easy for data
-scientists and ML engineers to understand where their models are going wrong
-and help them fix them before others complain ð£ï¸. UpTrain can be used for
-a wide variety of Machine learning models such as LLMs, recommendation models,
-prediction models, Computer vision models, etc. We are constantly working to
-make UpTrain better. Want a new feature or need any integrations? Feel free to
-[create an issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute]
-(https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to
-the repository.
-                             ****** [Meme] ******
-# License ð» This repo is published under Apache 2.0 license, with the
-exception of the ee directory which will contain premium features requiring an
-enterprise license in the future. We're currently focused on developing non-
-enterprise offerings that should cover most use cases by adding more features
-and extending to more models. We also working towards adding a hosted offering
-- [contact us](mailto:tech@uptrain.ai) if you are interested. # Stay Updated
-âï¸ We are continuously adding tons of features and use cases. Please
-support us by giving the project a star â­! # Provide feedback (Harsher the
-better ð) We are building UpTrain in public. Help us improve by giving your
-feedback **[here](https://forms.gle/PXd89D5LiFubro9o9)**. # Contributors
-ð¥ï¸ We welcome contributions to UpTrain. Please see our [contribution
-guide](https://github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for
-details. [https://contrib.rocks/image?repo=uptrain-ai/uptrain]
+                  Welcome] [Docs] [Community] [Website]  ***
+  **[UpTrain](https://uptrain.ai)** is a Python framework that ensures your LLM
+applications are performing reliably by allowing users to check aspects such as
+correctness, structural integrity, bias, hallucination, etc. UpTrain can be
+used to: 1) Validate model's response and safeguard your users against
+hallucinations, bias, incorrect output formats, etc. 2) Experiment across
+multiple model providers, prompt templates, and quantify model's performance.
+3) Monitor your model's performance in production and protect yourself against
+unwanted drifts # Key Features ð¡ - **[ChatGPT Grading](https://uptrain-
+ai.github.io/uptrain/operators/language/OpenAIGradeScore/)** - Utilize LLMs to
+grade your model outputs. - **[Custom Grading Checks](https://uptrain-
+ai.github.io/uptrain/operators/language/ModelGradeScore/)** - Write your custom
+grading prompts. - **[Embeddings Similarity Check](https://uptrain-
+ai.github.io/uptrain/operators/CosineSimilarity/)** - Compute cosine similarity
+between prompt and response embeddings - **[Output Validation](https://
+github.com/uptrain-ai/uptrain/blob/main/examples/validation_tutorial.ipynb)** -
+Safeguard your users against inappropriate responses - **[Prompt A/B Testing]
+(https://github.com/uptrain-ai/uptrain/blob/main/examples/
+prompt_experiments_tutorial.ipynb)** - Experiment across multiple prompts and
+compare them quantatively. - **[UMAP Visualization and Clustering](https://
+uptrain-ai.github.io/uptrain/operators/UMAP/)** - Visualize your embedding
+space using tools like UMAP and t-SNE. - **[Hallucination Checks]()** - Use
+metrics like custom grading, text similarity, and embedding similarity to check
+for hallucinations. - **[Toxic Keywords Checks]()** - Make sure your model
+outputs are not biased or contain toxic keywords. - **[Feature Slicing]()** -
+Built-in pivoting functionalities for data dice and slice to pinpoint low-
+performing cohorts. - **[Realtime Dashboards]()** - Monitor your model's
+performance in realtime. # Get started ð  To run it on your machine,
+checkout the [Quickstart tutorial](https://docs.uptrain.ai/getting-started/
+quickstart): ### Install the package through pip: ```bash pip install uptrain
+``` ### How to define checks: Say we want to check whether our model's
+responses contain any grammatical mistakes or not. ```python # Define your
+checkset - list of simple checks, dataset file, # and api_keys checkset =
+CheckSet( checks = Check( name = "grammar_score", operators = [ GrammarScore
+( col_in_text = "model_response", col_out = "grammar_score" ), ], plots =
+PlotlyChart.Table(title="Grammar scores"), ), source = JsonReader(fpath =
+'...') ) settings = Settings(openai_api_key = '...') checkset.setup(settings)
+checkset.run() ```
+# Integrations | Eval Frameworks | LLM Providers | LLM Packages | Serving
+frameworks | | ------------- | ------------- | ------------- | ------------- |
+| OpenAI Evals â | GPT-3.5-turbo â | Langchain ð | HuggingFace ð | |
+EleutherAI LM Eval ð | GPT-4 â | Llama Index ð | Replicate ð | |
+BIG-Bench ð | Claude ð | AutoGPT ð | | | Cohere ð | # UpTrain in
+Action ## Experimentation You can use the UpTrain framework to run and compare
+LLM responses for different prompts, models, LLM chains, etc. Check out the
+[experimentation tutorial](https://github.com/uptrain-ai/uptrain/blob/main/
+examples/prompt_experiments_tutorial.ipynb) to learn more. ## Validation You
+can use the UpTrain Validation Manager to define checks, retry logic and
+validate your LLM responses before showing it to your users. Check out the
+[tutorial here](https://github.com/uptrain-ai/uptrain/blob/main/examples/
+validation_tutorial.ipynb). ## Monitoring You can use the UpTrain framework to
+continuously monitor your model's performance and get real-time insights on how
+well it is doing on a variety of evaluation metrics. Check out the monitoring
+tutorial to learn more. # Why UpTrain ð¤? Large language models are trained
+over billions of data points and perform really well over a wide variety of
+tasks. But one thing these models are not good at is being deterministic. Even
+with the most well-crafted prompts, the model can misbehave for certain inputs,
+be it hallucinations, wrong output structure, toxic or biased response,
+irrelevant response, and error modes can be immense. To ensure your LLM
+applications work reliably and correctly, UpTrain makes it easy for developers
+to evaluate the responses of their applications on multiple criteria. UpTrain's
+evaluation framework can be used to: 1) Validate (and correct) the response of
+the model before showing it to the user 2) Get quantitative measures to
+experiment across multiple prompts, model providers, etc. 3) Do unit testing to
+ensure no buggy prompt or code gets pushed into your production 4) Monitor your
+LLM applications in real time and understand when they are going wrong in order
+to fix them before users complain. We are constantly working to make UpTrain
+better. Want a new feature or need any integrations? Feel free to [create an
+issue](https://github.com/uptrain-ai/uptrain/issues) or [contribute](https://
+github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) directly to the
+repository. # License ð» This repo is published under Apache 2.0 license. We
+are also working towards adding a hosted offering to make setting off eval runs
+easier - please fill **[this form](https://docs.google.com/forms/d/e/
+1FAIpQLSf9h_SXoU0rJP2MUc4NIKOmOCqJ5J0xgephN1xgeoXscSHUSA/
+viewform?usp=sf_link)** to get a waitlist slot. # Stay Updated âï¸ We are
+continuously adding tons of features and use cases. Please support us by giving
+the project a star â­! # Provide feedback (Harsher the better ð) We are
+building UpTrain in public. Help us improve by giving your feedback **[here]
+(https://docs.google.com/forms/d/e/1FAIpQLSezGUkkC0JoEvx-0gCrRSmGutA-
+jqyb7kl2lomXv302_C3MnQ/viewform?usp=sf_link)**. # Contributors ð¥ï¸ We
+welcome contributions to UpTrain. Please see our [contribution guide](https://
+github.com/uptrain-ai/uptrain/blob/main/CONTRIBUTING.md) for details. [https://
+contrib.rocks/image?repo=uptrain-ai/uptrain]
```

