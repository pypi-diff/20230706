# Comparing `tmp/alphastats-0.6.2.tar.gz` & `tmp/alphastats-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.6.2.tar", last modified: Thu Jun 22 13:02:10 2023, max compression
+gzip compressed data, was "alphastats-0.6.3.tar", last modified: Thu Jul  6 08:41:09 2023, max compression
```

## Comparing `alphastats-0.6.2.tar` & `alphastats-0.6.3.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-22 13:01:29.000000 alphastats-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 13:01:29.000000 alphastats-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-22 13:02:10.215180 alphastats-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-22 13:01:29.000000 alphastats-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.211180 alphastats-0.6.2/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/mzTabLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:02:10.215180 alphastats-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-22 13:01:30.000000 alphastats-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.253541 alphastats-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-06 08:40:27.000000 alphastats-0.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-06 08:40:27.000000 alphastats-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-06 08:41:09.253541 alphastats-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-06 08:40:27.000000 alphastats-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.229541 alphastats-0.6.3/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-07-06 08:40:27.000000 alphastats-0.6.3/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.249541 alphastats-0.6.3/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.249541 alphastats-0.6.3/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/GenericLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.249541 alphastats-0.6.3/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.249541 alphastats-0.6.3/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.253541 alphastats-0.6.3/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-06 08:40:28.000000 alphastats-0.6.3/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.233541 alphastats-0.6.3/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 08:41:09.000000 alphastats-0.6.3/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 08:41:09.253541 alphastats-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-06 08:40:28.000000 alphastats-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:41:09.253541 alphastats-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    37748 2023-07-06 08:40:28.000000 alphastats-0.6.3/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-06 08:40:28.000000 alphastats-0.6.3/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-06 08:40:28.000000 alphastats-0.6.3/tests/test_loaders.py
```

### Comparing `alphastats-0.6.2/LICENSE.txt` & `alphastats-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/PKG-INFO` & `alphastats-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.2
+Version: 0.6.3
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.2/README.md` & `alphastats-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/DataSet.py` & `alphastats-0.6.3/alphastats/DataSet.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import plotly
 
 from alphastats.loader.AlphaPeptLoader import AlphaPeptLoader
 from alphastats.loader.DIANNLoader import DIANNLoader
 from alphastats.loader.FragPipeLoader import FragPipeLoader
 from alphastats.loader.MaxQuantLoader import MaxQuantLoader
 from alphastats.loader.SpectronautLoader import SpectronautLoader
+from alphastats.loader.GenericLoader import GenericLoader
 from alphastats.loader.mzTabLoader import mzTabLoader
 
+
 from alphastats.DataSet_Plot import Plot
 from alphastats.DataSet_Preprocess import Preprocess
 from alphastats.DataSet_Pathway import Enrichment
 from alphastats.DataSet_Statistics import Statistics
 from alphastats.utils import LoaderError
 
 # remove warning from openpyxl
@@ -66,21 +68,26 @@
         self.evidence_df = loader.evidence_df
         self.gene_names = loader.gene_names
 
         # include filtering before
         self.create_matrix()
         self._check_matrix_values()
         self.metadata = None
+        
         if metadata_path is not None:
             self.sample = sample_column
             self.load_metadata(file_path=metadata_path)
             self._remove_misc_samples_in_metadata()
 
         else:
             self._create_metadata()
+        
+        if self.loader == "Generic":
+            intensity_column = loader._extract_sample_names(metadata=self.metadata, sample_column=self.sample)
+            self.intensity_column = intensity_column
 
         # save preprocessing settings
         self.preprocessing_info = self._save_dataset_info()
         self.preprocessed = False
 
         print("DataSet has been created.")
         self.overview()
@@ -93,15 +100,26 @@
     def _check_loader(self, loader):
         """Checks if the Loader is from class AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader
 
         Args:
             loader : loader
         """
         if not isinstance(
-            loader, (AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader, SpectronautLoader, mzTabLoader)
+
+            loader,
+            (
+                AlphaPeptLoader,
+                MaxQuantLoader,
+                DIANNLoader,
+                FragPipeLoader,
+                SpectronautLoader,
+                GenericLoader,
+                mzTabLoader
+            ),
+
         ):
             raise LoaderError(
                 "loader must be from class: AlphaPeptLoader, MaxQuantLoader, DIANNLoader, FragPipeLoader or SpectronautLoader"
             )
 
         if not isinstance(loader.rawinput, pd.DataFrame) or loader.rawinput.empty:
             raise ValueError(
@@ -132,22 +150,26 @@
 
     def create_matrix(self):
         """
         Creates a matrix of the Outputfile, with columns displaying features (Proteins) and
         rows the samples.
         """
 
-        regex_find_intensity_columns = self.intensity_column.replace("[sample]", ".*")
-        
         df = self.rawinput
         df = df.set_index(self.index_column)
-        df = df.filter(regex=(regex_find_intensity_columns), axis=1)
-        # remove Intensity so only sample names remain
-        substring_to_remove = regex_find_intensity_columns.replace(".*", "")
-        df.columns = df.columns.str.replace(substring_to_remove, "")
+
+        if isinstance(self.intensity_column, str):
+            regex_find_intensity_columns = self.intensity_column.replace("[sample]", ".*")
+            df = df.filter(regex=(regex_find_intensity_columns), axis=1)
+            # remove Intensity so only sample names remain
+            substring_to_remove = regex_find_intensity_columns.replace(".*", "")
+            df.columns = df.columns.str.replace(substring_to_remove, "")
+        
+        else:
+            df = df[self.intensity_column]
         # transpose dataframe
         mat = df.transpose()
         mat.replace([np.inf, -np.inf], np.nan, inplace=True)
         # remove proteins with only zero
         self.mat = mat.loc[:, (mat != 0).any(axis=0)]
         self.mat = self.mat.astype(float)
         # reset preproccessing info
@@ -195,14 +217,15 @@
             "Intensity used for analysis": self.intensity_column,
             "Log2-transformed": False,
             "Normalization": None,
             "Imputation": None,
             "Contaminations have been removed": False,
             "Contamination columns": self.filter_columns,
             "Number of removed ProteinGroups due to contaminaton": 0,
+            "Data completeness cut-off": 0,
         }
         return preprocessing_dict
 
     def overview(self):
         """Print overview of the DataSet"""
         dataset_overview = (
             "Attributes of the DataSet can be accessed using: \n"
```

### Comparing `alphastats-0.6.2/alphastats/DataSet_Pathway.py` & `alphastats-0.6.3/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/DataSet_Plot.py` & `alphastats-0.6.3/alphastats/DataSet_Plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import seaborn as sns
 import pandas as pd
 from scipy.spatial.distance import pdist, squareform
 import random
 import itertools
 import plotly.figure_factory
+from typing import Union
 
 from alphastats.plots.DimensionalityReduction import DimensionalityReduction
 from alphastats.plots.VolcanoPlot import VolcanoPlot
 from alphastats.plots.IntensityPlot import IntensityPlot
 from alphastats.plots.ClusterMap import ClusterMap
 from alphastats.plots.SampleHistogram import SampleHistogram
 from alphastats.utils import ignore_warning, check_for_missing_values
@@ -50,40 +51,46 @@
             "#A87F32",
         ],
     )
 )
 
 plotly.io.templates.default = "simple_white+alphastats_colors"
 
+
 class Plot:
     def _update_figure_attributes(self, figure_object, plotting_data, method=None):
         setattr(figure_object, "plotting_data", plotting_data)
         setattr(figure_object, "preprocessing", self.preprocessing_info)
         setattr(figure_object, "method", method)
         return figure_object
 
     @check_for_missing_values
-    def plot_pca(self, group=None, circle=False):
+    def plot_pca(self, group: str = None, circle: bool = False):
         """Plot Principal Component Analysis (PCA)
 
         Args:
             group (str, optional): column in metadata that should be used for coloring. Defaults to None.
             circle (bool, optional): draw circle around each group. Defaults to False.
 
         Returns:
             plotly.graph_objects._figure.Figure: PCA plot
         """
         dimensionality_reduction = DimensionalityReduction(
             dataset=self, group=group, method="pca", circle=circle
         )
         return dimensionality_reduction.plot
 
-
     @check_for_missing_values
-    def plot_tsne(self, group=None, circle=False, perplexity=5, n_iter=1000):
+    def plot_tsne(
+        self,
+        group: str = None,
+        circle: bool = False,
+        perplexity: int = 5,
+        n_iter: int = 1000,
+    ):
         """Plot t-distributed stochastic neighbor embedding (t-SNE)
 
         Args:
             group (str, optional): column in metadata that should be used for coloring. Defaults to None.
             circle (bool, optional): draw circle around each group. Defaults to False.
 
         Returns:
@@ -96,15 +103,15 @@
             circle=circle,
             perplexity=perplexity,
             n_iter=n_iter,
         )
         return dimensionality_reduction.plot
 
     @check_for_missing_values
-    def plot_umap(self, group=None, circle=False):
+    def plot_umap(self, group: str = None, circle: bool = False):
         """Plot Uniform Manifold Approximation and Projection for Dimension Reduction
 
         Args:
             group (str, optional): column in metadata that should be used for coloring. Defaults to None.
             circle (bool, optional): draw circle around each group. Defaults to False.
 
         Returns:
@@ -115,16 +122,16 @@
         )
         return dimensionality_reduction.plot
 
     
     @ignore_warning(RuntimeWarning)
     def plot_volcano(
         self,
-        group1,
-        group2,
+        group1: Union[str, list],
+        group2: Union[str, list],
         column:str=None,
         method:str="ttest",
         labels:bool=False,
         min_fc:float=1.0,
         alpha:float=0.05,
         draw_line:bool=True,
         perm:int=100, 
@@ -151,17 +158,19 @@
 
         Returns:
             plotly.graph_objects._figure.Figure: Volcano Plot
         """
 
         if compare_preprocessing_modes:
             params_for_func = locals()
-            results = self._compare_preprocessing_modes(func=VolcanoPlot,params_for_func=params_for_func)
+            results = self._compare_preprocessing_modes(
+                func=VolcanoPlot, params_for_func=params_for_func
+            )
             return results
-        
+
         else:
             volcano_plot = VolcanoPlot(
                 dataset=self,
                 group1=group1,
                 group2=group2,
                 column=column,
                 method=method,
@@ -172,29 +181,31 @@
                 perm=perm, 
                 fdr=fdr,
                 color_list=color_list
             )
 
             return volcano_plot.plot
 
-    def plot_correlation_matrix(self, method="pearson"):
+    def plot_correlation_matrix(self, method: str = "pearson"):
         """Plot Correlation Matrix
 
         Args:
             method (str, optional): orrelation coefficient "pearson", "kendall" (Kendall Tau correlation)
             or "spearman" (Spearman rank correlation). Defaults to "pearson".
 
         Returns:
             plotly.graph_objects._figure.Figure: Correlation matrix
         """
         corr_matrix = self.mat.transpose().corr(method=method)
         plot = px.imshow(corr_matrix)
         return plot
 
-    def plot_sampledistribution(self, method="violin", color=None, log_scale=False):
+    def plot_sampledistribution(
+        self, method: str = "violin", color: bool = None, log_scale: bool = False
+    ):
         """Plot Intensity Distribution for each sample. Either Violin or Boxplot
 
         Args:
             method (str, optional): Violinplot = "violin", Boxplot = "box". Defaults to "violin".
             color (str, optional): A metadata column used to color the boxes. Defaults to None.
             log_scale (bool, optional): yaxis in logarithmic scale. Defaults to False.
 
@@ -228,77 +239,83 @@
         fig = self._update_figure_attributes(
             figure_object=fig, plotting_data=df, method=method
         )
         return fig
 
     def plot_intensity(
         self,
-        protein_id,
-        group=None,
-        subgroups=None,
-        method="box",
-        add_significance=False,
-        log_scale=False,
-        compare_preprocessing_modes=False
+        protein_id: str,
+        group: str = None,
+        subgroups: list = None,
+        method: str = "box",
+        add_significance: bool = False,
+        log_scale: bool = False,
+        compare_preprocessing_modes: bool = False,
     ):
         """Plot Intensity of individual Protein/ProteinGroup
 
         Args:
-            ID (str): ProteinGroup ID
+            protein_id (str): ProteinGroup ID
             group (str, optional): A metadata column used for grouping. Defaults to None.
             subgroups (list, optional): Select variables from the group column. Defaults to None.
             method (str, optional):  Violinplot = "violin", Boxplot = "box", Scatterplot = "scatter" or "all". Defaults to "box".
             add_significance (bool, optional): add p-value bar, only possible when two groups are compared. Defaults False.
             log_scale (bool, optional): yaxis in logarithmic scale. Defaults to False.
 
         Returns:
             plotly.graph_objects._figure.Figure: Plotly Plot
         """
         if compare_preprocessing_modes:
             params_for_func = locals()
-            results = self._compare_preprocessing_modes(func=IntensityPlot,params_for_func=params_for_func)
+            results = self._compare_preprocessing_modes(
+                func=IntensityPlot, params_for_func=params_for_func
+            )
             return results
-        
+
         intensity_plot = IntensityPlot(
-            dataset = self,
+            dataset=self,
             protein_id=protein_id,
             group=group,
             subgroups=subgroups,
             method=method,
             add_significance=add_significance,
-            log_scale=log_scale
+            log_scale=log_scale,
         )
 
         return intensity_plot.plot
 
     @ignore_warning(UserWarning)
     @check_for_missing_values
     def plot_clustermap(
-        self, label_bar=None, only_significant=False, group=None, subgroups=None
+        self,
+        label_bar: str = None,
+        only_significant: bool = False,
+        group: str = None,
+        subgroups: list = None,
     ):
         """Plot a matrix dataset as a hierarchically-clustered heatmap
 
         Args:
             label_bar (str, optional): column/variable name described in the metadata. Will be plotted as bar above the heatmap to see wheteher groups are clustering together. Defaults to None.. Defaults to None.
             only_significant (bool, optional): performs ANOVA and only signficantly different proteins will be clustered (p<0.05). Defaults to False.
             group (str, optional): group containing subgroups that should be clustered. Defaults to None.
             subgroups (list, optional): variables in group that should be plotted. Defaults to None.
 
         Returns:
              ClusterGrid: Clustermap
         """
 
         clustermap = ClusterMap(
-            dataset = self,
+            dataset=self,
             label_bar=label_bar,
             only_significant=only_significant,
             group=group,
-            subgroups=subgroups
+            subgroups=subgroups,
         )
-        return  clustermap.plot
+        return clustermap.plot
 
     def plot_samplehistograms(self):
         """Plots the Denisty distribution of each sample
 
         Returns:
             plotly: Plotly Graph Object
         """
```

### Comparing `alphastats-0.6.2/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.3/alphastats/DataSet_Preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from alphastats.utils import ignore_warning
 from sklearn.experimental import enable_iterative_imputer
 import itertools
 
 
 
 class Preprocess:
-    def _remove_sampels(self, sample_list):
+    def _remove_sampels(self, sample_list: list):
         # exclude samples for analysis
         self.mat = self.mat.drop(sample_list)
         self.metadata = self.metadata[~self.metadata[self.sample].isin(sample_list)]
 
     def _subset(self):
         # filter matrix so only samples that are described in metadata
         # also found in matrix
@@ -25,14 +25,42 @@
         )
         return self.mat[self.mat.index.isin(self.metadata[self.sample].tolist())]
 
     def preprocess_print_info(self):
         """Print summary of preprocessing steps"""
         print(pd.DataFrame(self.preprocessing_info.items()))
 
+    def _remove_na_values(self, cut_off):
+        cut = 1 - cut_off
+        limit = self.mat.shape[0] * cut
+        
+        keep_list = list()
+        invalid = 0
+        for column_name in self.mat.columns:
+            column = self.mat[column_name]
+            # Get the count of Zeros in column 
+            count = (column == 0).sum()
+            try:
+                count = count.item()
+                if isinstance(count, int):
+                    if count < limit:
+                        keep_list += [column_name]
+                    
+            except ValueError:
+                invalid +=1
+                continue
+        
+        self.mat= self.mat[keep_list]
+        self.preprocessing_info.update(
+            {"Data completeness cut-off": cut_off}
+        )
+        percentage = cut_off * 100
+        print(f"Proteins with a data completeness across all samples of less than {percentage} % have been removed.")
+
+
     def _filter(self):
         if len(self.filter_columns) == 0:
             logging.info("No columns to filter.")
             return
 
         if self.preprocessing_info.get("Contaminations have been removed") == True:
             logging.info("Contaminatons have already been filtered.")
@@ -64,15 +92,15 @@
             f"Contaminations indicated in following columns: {self.filter_columns} were removed. "
             f"In total {str(len(protein_groups_to_remove))} observations have been removed."
         )
         logging.info(filter_info)
 
     @ignore_warning(RuntimeWarning)
     @ignore_warning(UserWarning)
-    def _imputation(self, method):
+    def _imputation(self, method: str):
         # remove ProteinGroups with only NA before
         protein_group_na = self.mat.columns[self.mat.isna().all()].tolist()
 
         if len(protein_group_na) > 0:
             self.mat = self.mat.drop(protein_group_na, axis=1)
             logging.info(
                 f" {len(protein_group_na)} Protein Groups were removed due to missing values."
@@ -125,16 +153,16 @@
         self.mat = pd.DataFrame(
             imputation_array, index=self.mat.index, columns=self.mat.columns
         )
         self.preprocessing_info.update({"Imputation": method})
 
     @ignore_warning(UserWarning)
     @ignore_warning(RuntimeWarning)
-    def _normalization(self, method):
-    
+    def _normalization(self, method: str):
+
         if method == "zscore":
             scaler = sklearn.preprocessing.StandardScaler()
             normalized_array = scaler.fit_transform(self.mat.values)
 
         elif method == "quantile":
             qt = sklearn.preprocessing.QuantileTransformer(random_state=0)
             normalized_array = qt.fit_transform(self.mat.values)
@@ -159,47 +187,44 @@
         )
 
         self.preprocessing_info.update({"Normalization": method})
 
     def reset_preprocessing(self):
         """ Reset all preprocessing steps
         """
-        # reset all preprocessing steps
+        #  reset all preprocessing steps
         self.create_matrix()
         print("All preprocessing steps are reset.")
     
     @ignore_warning(RuntimeWarning)
     def _compare_preprocessing_modes(self, func, params_for_func) -> list:
         dataset = self
-
-        #    normalization_methods = methods["normalization"]
-       # if isinstance(methods, dict):
-        #    imputation_methods = methods["imputation"]
-        
         imputation_methods = ["mean", "median", "knn", "randomforest"]
         normalization_methods = ["vst","zscore", "quantile" ]
         
         preprocessing_modes = list(itertools.product(normalization_methods, imputation_methods))
 
+
         results_list = []
 
         del params_for_func["compare_preprocessing_modes"]
         params_for_func["dataset"] = params_for_func.pop("self")
 
         for preprocessing_mode in preprocessing_modes:
             # reset preprocessing
             dataset.reset_preprocessing()
             print(f"Normalization {preprocessing_mode[0]}, Imputation {str(preprocessing_mode[1])}")
             dataset.mat.replace([np.inf, -np.inf], np.nan, inplace=True)
+
             dataset.preprocess(
                 subset=True,
-                normalization = preprocessing_mode[0],
-                imputation = preprocessing_mode[1]
+                normalization=preprocessing_mode[0],
+                imputation=preprocessing_mode[1],
             )
-            
+
             res = func(**params_for_func)
             results_list.append(res)
         
             print("\t")
 
         return results_list
 
@@ -207,15 +232,14 @@
         self.mat = np.log2(self.mat + 0.1)
         self.preprocessing_info.update({"Log2-transformed": True})
         print("Data has been log2-transformed.")
     
     def batch_correction(self, batch:str):
         """Correct for technical bias/batch effects
         Behdenna A, Haziza J, Azencot CA and Nordor A. (2020) pyComBat, a Python tool for batch effects correction in high-throughput molecular data using empirical Bayes methods. bioRxiv doi: 10.1101/2020.03.17.995431
-
         Args:
             batch (str): column name in the metadata describing the different batches
         """
         import combat
         from combat.pycombat import pycombat
         data = self.mat.transpose()
         series_of_batches = self.metadata.set_index(self.sample).reindex(data.columns.to_list())[batch]
@@ -223,14 +247,15 @@
 
     @ignore_warning(RuntimeWarning)
     def preprocess(
         self,
         log2_transform: bool=True,
         remove_contaminations: bool=False,
         subset: bool=False,
+        data_completeness: float=0,
         normalization: str=None,
         imputation: str=None,
         remove_samples: list=None,
     ):
         """Preprocess Protein data
 
         Removal of contaminations:
@@ -264,33 +289,37 @@
         Random Forest Imputation: https://scikit-learn.org/stable/auto_examples/impute/plot_iterative_imputer_variants_comparison.html
         https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html#sklearn.ensemble.RandomForestRegressor
 
         Args:
             remove_contaminations (bool, optional): remove ProteinGroups that are identified as contamination.
             log2_transform (bool, optional): Log2 transform data. Default to True.
             normalization (str, optional): method to normalize data: either "zscore", "quantile", "linear". Defaults to None.
+            data_completeness (float, optional): data completeness across all samples between 0-1. Defaults to 0.
             remove_samples (list, optional): list with sample ids to remove. Defaults to None.
             imputation (str, optional):  method to impute data: either "mean", "median", "knn" or "randomforest". Defaults to None.
             subset (bool, optional): filter matrix so only samples that are described in metadata found in matrix. Defaults to False.
         """
         if remove_contaminations:
             self._filter()
         
         if remove_samples is not None:
             self._remove_sampels(sample_list=remove_samples)
 
         if subset:
             self.mat = self._subset()
         
+
+        if data_completeness> 0:
+            self._remove_na_values(cut_off=data_completeness)
+
         if log2_transform and self.preprocessing_info.get("Log2-transformed") is False:
             self._log2_transform()
 
         if normalization is not None:
             self._normalization(method=normalization)
             self.mat = self.mat.replace([np.inf, -np.inf], np.nan)
-            #self.mat[:] = np.nan_to_num(self.mat)
-
+            
         if imputation is not None:
             self._imputation(method=imputation)
 
         self.mat = self.mat.loc[:, (self.mat != 0).any(axis=0)]
         self.preprocessed = True
```

### Comparing `alphastats-0.6.2/alphastats/DataSet_Statistics.py` & `alphastats-0.6.3/alphastats/DataSet_Statistics.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import pingouin
 from alphastats.utils import ignore_warning
 from tqdm import tqdm
 from functools import lru_cache
 from typing import Union
 
+from alphastats.statistics.MultiCovaAnalysis import MultiCovaAnalysis
 from alphastats.statistics.DifferentialExpressionAnalysis import DifferentialExpressionAnalysis
 from alphastats.statistics.Anova import Anova
 
 
 class Statistics:
     def _calculate_foldchange(self, mat_transpose:pd.DataFrame, group1_samples:list, group2_samples:list) -> pd.DataFrame:
         mat_transpose += 0.00001
@@ -83,15 +84,14 @@
             * ``'qval'``: multiple testing - corrected p-value
             * ``'log2fc'``: log2(foldchange)
             * ``'grad'``: the gradient of the log-likelihood
             * ``'coef_mle'``: the maximum-likelihood estimate of coefficient in liker-space
             * ``'coef_sd'``: the standard deviation of the coefficient in liker-space
             * ``'ll'``: the log-likelihood of the estimation
         """
-
         df = DifferentialExpressionAnalysis(
             dataset=self, 
             group1=group1, 
             group2=group2, 
             column=column, method=method,
             perm=perm, 
             fdr=fdr
@@ -184,7 +184,43 @@
             * ``'p-unc'``: Uncorrected p-values
             * ``'np2'``: Partial eta-squared
         """
         df = self.mat[protein_id].reset_index().rename(columns={"index": self.sample})
         df = self.metadata.merge(df, how="inner", on=[self.sample])
         ancova_df = pingouin.ancova(df, dv=protein_id, covar=covar, between=between)
         return ancova_df
+
+    @ignore_warning(RuntimeWarning)
+    def multicova_analysis(
+        self,
+        covariates: list,
+        n_permutations: int = 3,
+        fdr: float = 0.05,
+        s0: float = 0.05,
+        subset: dict = None,
+    ) -> Union[pd.DataFrame, list]:
+        """Perform Multicovariat Analysis
+        will return a pandas DataFrame with the results and a list of volcano plots (for each covariat)
+
+        Args:
+            covariates (list): list of covariates, column names in metadata
+            n_permutations (int, optional): number of permutations. Defaults to 3.
+            fdr (float, optional): False Discovery Rate. Defaults to 0.05.
+            s0 (float, optional): . Defaults to 0.05.
+            subset (dict, optional): for categorical covariates . Defaults to None.
+
+        Returns:
+            pd.DataFrame: Multicova Analysis results
+        """
+        
+        res, plot_list= MultiCovaAnalysis(
+            dataset=self,
+            covariates=covariates,
+            n_permutations=n_permutations,
+            fdr=fdr,
+            s0=s0,
+            subset=subset,
+            plot=True
+        ).calculate()
+        return res, plot_list
+
+
```

### Comparing `alphastats-0.6.2/alphastats/__init__.py` & `alphastats-0.6.3/alphastats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.6.2/alphastats/data/contaminations.txt` & `alphastats-0.6.3/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.3/alphastats/gui/AlphaPeptStats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import streamlit as st
+
 st.set_page_config(layout="wide")
 
 try:
     from alphastats.gui.utils.ui_helper import sidebar_info, img_to_bytes
 except ModuleNotFoundError:
     from utils.ui_helper import sidebar_info, img_to_bytes
 import os
-#from PIL import Image
+
+# from PIL import Image
 
 # centering with streamlit is not really centered
 
 from streamlit.runtime import get_instance
 from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
 
 runtime = get_instance()
@@ -38,16 +40,15 @@
 icon = os.path.join(_this_directory, "alphapeptstats_logo.png")
 
 header_html = img_center + "<img src='data:image/png;base64,{}'>".format(
     img_to_bytes(icon)
 )
 
 st.markdown(
-    header_html,
-    unsafe_allow_html=True,
+    header_html, unsafe_allow_html=True,
 )
 
 ##
 st.markdown(
     """\n\n
 An open-source Python package for the analysis of mass spectrometry based proteomics data 
 from the [Mann Group at the University of Copenhagen](https://www.cpr.ku.dk/research/proteomics/mann/).
```

### Comparing `alphastats-0.6.2/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.3/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.3/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.3/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/gui.py` & `alphastats-0.6.3/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.3/alphastats/gui/pages/02_Import Data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import streamlit as st
 import sys
 import os
+import io
 
 try:
     from alphastats.gui.utils.ui_helper import sidebar_info
     from alphastats.gui.utils.analysis_helper import *
     from alphastats.gui.utils.software_options import software_options
     from alphastats.loader.MaxQuantLoader import MaxQuantLoader
     from alphastats.DataSet import DataSet
@@ -13,28 +14,30 @@
     from utils.ui_helper import sidebar_info
     from utils.analysis_helper import *
     from utils.software_options import software_options
     from alphastats import MaxQuantLoader
     from alphastats import DataSet
 
 
-
 import pandas as pd
 import plotly.express as px
 
 from streamlit.runtime import get_instance
 from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
 
 runtime = get_instance()
 session_id = get_script_run_ctx().session_id
 session_info = runtime._session_mgr.get_session_info(session_id)
 
 user_session_id = session_id
 st.session_state["user_session_id"] = user_session_id
 
+if "loader" not in st.session_state:
+    st.session_state["loader"] = None
+
 
 def load_options():
 
     from alphastats.gui.utils.options import plotting_options, statistic_options
 
     st.session_state["plotting_options"] = plotting_options
     st.session_state["statistic_options"] = statistic_options
@@ -78,43 +81,53 @@
         expected_columns = ["Protein"]
         if (set(expected_columns).issubset(set(df.columns.to_list()))) == False:
             st.error(
                 "This is not a valid FragPipe file. Please check:"
                 "https://fragpipe.nesvilab.org/docs/tutorial_fragpipe_outputs.html#combined_proteintsv"
             )
 
-
-def print_software_import_info(software):
-    import_file = software_options.get(software).get("import_file")
-    string_output = f"Please upload {import_file} file from {software}."
-    return string_output
-
-
-def select_columns_for_loaders(software):
+def select_columns_for_loaders(software, software_df:None):
     """
     select intensity and index column depending on software
     will be saved in session state
     """
     st.write("\n\n")
     st.markdown("### 2. Select columns used for further analysis.")
     st.markdown("Select intensity columns for further analysis")
 
-    st.selectbox(
-        "Intensity Column",
-        options=software_options.get(software).get("intensity_column"),
-        key="intensity_column",
-    )
+    if software != "Other":
+
+        st.selectbox(
+            "Intensity Column",
+            options=software_options.get(software).get("intensity_column"),
+            key="intensity_column",
+        )
 
-    st.markdown("Select index column (with ProteinGroups) for further analysis")
+        st.markdown("Select index column (with ProteinGroups) for further analysis")
 
-    st.selectbox(
-        "Index Column",
-        options=software_options.get(software).get("index_column"),
-        key="index_column",
-    )
+        st.selectbox(
+            "Index Column",
+            options=software_options.get(software).get("index_column"),
+            key="index_column",
+        )
+        
+    else:
+        st.multiselect(
+            "Intensity Columns",
+            options=software_df.columns.to_list(),
+            key="intensity_column",
+        )
+
+        st.markdown("Select index column (with ProteinGroups) for further analysis")
+
+        st.selectbox(
+            "Index Column",
+            options=software_df.columns.to_list(),
+            key="index_column",
+        )
 
 
 def load_proteomics_data(uploaded_file, intensity_column, index_column, software):
     """load software file into loader object from alphastats"""
     loader = software_options.get(software)["loader_function"](
         uploaded_file, intensity_column, index_column
     )
@@ -132,30 +145,30 @@
     if len(valid_sample_columns) == 0:
         st.error(
             f"Metadata does not match Proteomics data."
             f"Information for the samples: {samples_proteomics_data} is required."
         )
 
     st.write(
-        f"Select column that contains sample IDs matching the sample names described"
+        f"Select column that contains sample IDs matching the sample names described "
         + f"in {software_options.get(software).get('import_file')}"
     )
 
     with st.form("sample_column"):
         st.selectbox("Sample Column", options=valid_sample_columns, key="sample_column")
         submitted = st.form_submit_button("Create DataSet")
 
     if submitted:
         return True
 
 
 def upload_softwarefile(software):
 
     softwarefile = st.file_uploader(
-        print_software_import_info(software=software),
+        software_options.get(software).get("import_file"),
         type=["csv", "tsv", "txt", "hdf"],
     )
 
     if softwarefile is not None:
 
         softwarefile_df = read_uploaded_file_into_df(softwarefile)
         # display head a protein data
@@ -164,39 +177,57 @@
 
         st.write(
             f"File successfully uploaded. Number of rows: {softwarefile_df.shape[0]}"
             f", Number of columns: {softwarefile_df.shape[1]}.\nPreview:"
         )
         st.dataframe(softwarefile_df.head(5))
 
-        select_columns_for_loaders(software=software)
+        select_columns_for_loaders(software=software, software_df=softwarefile_df)
 
         if (
             "intensity_column" in st.session_state
             and "index_column" in st.session_state
         ):
             loader = load_proteomics_data(
                 softwarefile_df,
                 intensity_column=st.session_state.intensity_column,
                 index_column=st.session_state.index_column,
                 software=software,
             )
             st.session_state["loader"] = loader
 
 
+def create_metadata_file():
+    dataset = DataSet(loader=st.session_state.loader)
+    st.session_state["metadata_columns"] = ["sample"]
+    metadata = dataset.metadata
+    buffer = io.BytesIO()
+
+    with pd.ExcelWriter(buffer, engine='xlsxwriter') as writer:
+        # Write each dataframe to a different worksheet.
+        metadata.to_excel(writer, sheet_name='Sheet1', index=False)
+        # Close the Pandas Excel writer and output the Excel file to the buffer
+        writer.close()
+
+        st.download_button(
+            label="Download metadata template as Excel",
+            data=buffer,
+            file_name='metadata.xlsx',
+            mime='application/vnd.ms-excel'
+        )
+
 def upload_metadatafile(software):
 
     st.write("\n\n")
-    st.markdown("### 3. Upload corresponding metadata.")
-    st.file_uploader(
-        "Upload metadata file. with information about your samples",
-        key="metadatafile",
+    st.markdown("### 3. Prepare Metadata.")
+    metadatafile_upload = st.file_uploader(
+        "Upload metadata file. with information about your samples", key="metadatafile",
     )
 
-    if st.session_state.metadatafile is not None:
+    if metadatafile_upload is not None and  st.session_state.loader is not None:
 
         metadatafile_df = read_uploaded_file_into_df(st.session_state.metadatafile)
         # display metadata
         st.write(
             f"File successfully uploaded. Number of rows: {metadatafile_df.shape[0]}"
             f", Number of columns: {metadatafile_df.shape[1]}. \nPreview:"
         )
@@ -212,38 +243,50 @@
             )
             st.session_state["metadata_columns"] = metadatafile_df.columns.to_list()
 
             load_options()
 
             display_loaded_dataset()
 
-    if st.button("Create a DataSet without metadata"):
-        st.session_state["dataset"] = DataSet(loader=st.session_state.loader)
-        st.session_state["metadata_columns"] = ["sample"]
+    if st.session_state.loader is not None:
+        create_metadata_file()
+        st.write("Download the template file and add additional information as "
+                 + "columns to your samples such as disease group. "
+                 + "Upload the updated metadata file.")
+    
+    if st.session_state.loader is not None:
+        if st.button("Create a DataSet without metadata"):
+            st.session_state["dataset"] = DataSet(loader=st.session_state.loader)
+            st.session_state["metadata_columns"] = ["sample"]
 
-        load_options()
+            load_options()
 
-        display_loaded_dataset()
+            display_loaded_dataset()
 
 
 def load_sample_data():
     _this_file = os.path.abspath(__file__)
     _this_directory = os.path.dirname(_this_file)
     _parent_directory = os.path.dirname(_this_directory)     
     folder_to_load = os.path.join(_parent_directory, 'sample_data')
     
     filepath= os.path.join(folder_to_load, "proteinGroups.txt")
     metadatapath= os.path.join(folder_to_load, "metadata.xlsx")
 
-
     loader = MaxQuantLoader(file=filepath)
     ds = DataSet(
         loader=loader, metadata_path=metadatapath, sample_column="sample"
     )
-    
+    metadatapath = os.path.join(_this_directory, "sample_data/metadata.xlsx").replace(
+        "pages/", ""
+    )
+
+    loader = MaxQuantLoader(file=filepath)
+    ds = DataSet(loader=loader, metadata_path=metadatapath, sample_column="sample")
+
     ds.metadata = ds.metadata[
         [
             "sample",
             "disease",
             "Drug therapy (procedure) (416608005)",
             "Lipid-lowering therapy (134350008)",
         ]
@@ -253,28 +296,26 @@
     st.session_state["metadata_columns"] = ds.metadata.columns.to_list()
     st.session_state["dataset"] = ds
 
     load_options()
 
 
 def import_data():
+    options = ["<select>"] + list(software_options.keys())
 
     software = st.selectbox(
         "Select your Proteomics Software",
-        options=["<select>", "MaxQuant", "AlphaPept", "DIANN", "FragPipe", "Spectronaut"],
+        options=options,
     )
-
     session_state_empty = False
 
     if software != "<select>":
-        # if
-        # reset()
         upload_softwarefile(software=software)
 
-    if "loader" in st.session_state:
+    if st.session_state.loader is not None:
         upload_metadatafile(software)
 
 
 def display_loaded_dataset():
 
     st.info("Data was successfully imported")
     st.info("DataSet has been created")
@@ -313,17 +354,19 @@
     """
     for key in st.session_state.keys():
         del st.session_state[key]
     st.empty()
 
     from streamlit.runtime import get_instance
     from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
+
     user_session_id = get_script_run_ctx().session_id
     st.session_state["user_session_id"] = user_session_id
 
+
 sidebar_info()
 
 
 if "dataset" not in st.session_state:
     st.markdown("### Import Proteomics Data")
 
     st.markdown(
```

### Comparing `alphastats-0.6.2/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.3/alphastats/gui/pages/03_Data Overview.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import streamlit as st
 import pandas as pd
 import plotly.express as px
 
 
 @st.cache_data
-def convert_df(df, user_session_id = st.session_state.user_session_id):
+def convert_df(df, user_session_id=st.session_state.user_session_id):
     return df.to_csv().encode("utf-8")
 
 
 @st.cache_data
-def get_display_matrix(user_session_id = st.session_state.user_session_id):
+def get_display_matrix(user_session_id=st.session_state.user_session_id):
 
     processed_df = pd.DataFrame(
         st.session_state.dataset.mat.values,
         index=st.session_state.dataset.mat.index.to_list(),
     ).head(10)
 
     return processed_df
@@ -53,34 +53,35 @@
 
 
 
 if "dataset" in st.session_state:
     st.markdown("## DataSet overview")
 
     c1, c2 = st.columns(2)
-    
+
     with c1:
 
         st.markdown("**Intensity distribution raw data per sample**")
         st.plotly_chart(
             st.session_state.distribution_plot.update_layout(plot_bgcolor="white"),
-            use_container_width=True
+            use_container_width=True,
         )
-    
+
     with c2:
 
         st.markdown("**Intensity distribution data per sample used for analysis**")
         st.plotly_chart(
             get_intensity_distribution_processed(user_session_id = st.session_state.user_session_id)
                         .update_layout(plot_bgcolor="white"), use_container_width=True
         )
  
     st.plotly_chart(
         get_sample_histogram_matrix(user_session_id = st.session_state.user_session_id)
                     .update_layout(plot_bgcolor="white"), use_container_width=True
     )
 
+
     display_matrix()
 
 
 else:
     st.info("Import Data first")
```

### Comparing `alphastats-0.6.2/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.3/alphastats/gui/pages/03_Preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,21 @@
             )
 
             remove_samples = st.multiselect(
                 "Remove samples from analysis", 
                 options=st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list()
             )
 
+            data_completeness = st.number_input(
+                f"Data completeness across samples cut-off \n(0.7 -> protein has to be detected in at least 70% of the samples)",
+                value=0, min_value=0, max_value=1
+            )
+
             log2_transform = st.selectbox(
-                "Log2-transform dataset",
-                options=[True, False],
+                "Log2-transform dataset", options=[True, False],
             )
 
             normalization = st.selectbox(
                 "Normalization", options=[None, "zscore", "quantile", "vst", "linear"]
             )
 
             imputation = st.selectbox(
@@ -53,14 +57,15 @@
             if len(remove_samples) == 0:
                 remove_samples = None
             
             st.session_state.dataset.preprocess(
                 remove_contaminations=remove_contaminations,
                 log2_transform=log2_transform,
                 remove_samples = remove_samples,
+                data_completeness=data_completeness,
                 subset=subset,
                 normalization=normalization,
                 imputation=imputation,
             )
             preprocessing = st.session_state.dataset.preprocessing_info
             st.info(
                 "Data has been processed. "
@@ -98,23 +103,21 @@
             st.plotly_chart(fig_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
         
         else:
             st.markdown("**Intensity Distribution per sample**")
             fig_none_processed = st.session_state.dataset.plot_sampledistribution()
             st.plotly_chart(fig_none_processed.update_layout(plot_bgcolor="white"), use_container_width=True)
         
-    
+
     reset_steps = st.button("Reset all Preprocessing steps")
-        
+
     if reset_steps:
         reset_preprocessing()
 
 
-
-
 def reset_preprocessing():
     st.session_state.dataset.create_matrix()
     preprocessing = st.session_state.dataset.preprocessing_info
     st.info(
         "Data has been reset. " + datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
     )
     st.dataframe(
@@ -124,16 +127,15 @@
 
 
 def main_preprocessing():
 
     if "dataset" in st.session_state:
 
         preprocessing()
-        
-        
+
     else:
         st.info("Import Data first")
 
 
 st.markdown("### Preprocessing")
```

### Comparing `alphastats-0.6.2/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.3/alphastats/gui/pages/04_Analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 import pandas as pd
 import io
 
 
 try:
     from alphastats.gui.utils.ui_helper import sidebar_info
-    from alphastats.gui.utils.analysis_helper import (
-    get_analysis,
-)  
+    from alphastats.gui.utils.analysis_helper import get_analysis
 
 except ModuleNotFoundError:
     from utils.ui_helper import sidebar_info
-    from utils.analysis_helper import (
-    get_analysis,
-)  
+    from utils.analysis_helper import get_analysis
+
 
 def check_if_options_are_loaded(f):
     """
     decorator to check whether analysis options are loaded
     """
 
     def inner(*args, **kwargs):
@@ -72,29 +69,25 @@
     else:
         plot.savefig(buffer, format=format)
 
     st.download_button(label="Download as " + format, data=buffer, file_name=filename)
 
 
 @st.cache_data
-def convert_df(df, user_session_id = st.session_state.user_session_id):
+def convert_df(df, user_session_id=st.session_state.user_session_id):
     return df.to_csv().encode("utf-8")
 
 
 def download_preprocessing_info(plot):
     preprocesing_dict = plot[1].preprocessing
     df = pd.DataFrame(preprocesing_dict.items())
     filename = "plot" + plot[0] + "preprocessing_info.csv"
     csv = convert_df(df)
     st.download_button(
-        "Download DataSet Info as .csv",
-        csv,
-        filename,
-        "text/csv",
-        key="preprocessing",
+        "Download DataSet Info as .csv", csv, filename, "text/csv", key="preprocessing",
     )
 
 
 @check_if_options_are_loaded
 def select_analysis():
     """
     select box
@@ -130,104 +123,96 @@
 
 if "plot_list" not in st.session_state:
     st.session_state["plot_list"] = []
 
 
 if "dataset" in st.session_state:
 
-    c1, c2 = st.columns((1,2))
+    c1, c2 = st.columns((1, 2))
 
     plot_to_display = False
     df_to_display = False
 
     with c1:
 
         method = select_analysis()
 
         if method in st.session_state.plotting_options.keys():
 
             analysis_result = get_analysis(
                 method=method, options_dict=st.session_state.plotting_options
             )
             plot_to_display = True
-        
+
         elif method in st.session_state.statistic_options.keys():
 
             analysis_result = get_analysis(
                 method=method, options_dict=st.session_state.statistic_options
             )
             df_to_display = True
 
         st.markdown("")
         st.markdown("")
         st.markdown("")
         st.markdown("")
-        
 
     with c2:
 
         # --- Plot -------------------------------------------------------
 
         if analysis_result is not None and method != "Clustermap" and plot_to_display:
-            
+
             display_figure(analysis_result)
 
             save_plot_to_session_state(analysis_result, method)
 
             method_plot = [method, analysis_result]
 
-            
         elif method == "Clustermap":
 
             st.write("Download Figure to see full size.")
 
             display_figure(analysis_result)
 
             save_plot_to_session_state(analysis_result, method)
 
-
         # --- STATISTICAL ANALYSIS -------------------------------------------------------
 
         elif analysis_result is not None and df_to_display:
 
             display_df(analysis_result)
 
             filename = method + ".csv"
             csv = convert_df(analysis_result)
 
-            
-    
     if analysis_result is not None and method != "Clustermap" and plot_to_display:
         col1, col2, col3 = st.columns([1, 1, 1])
 
         with col1:
             download_figure(method_plot, format="pdf")
 
         with col2:
             download_figure(method_plot, format="svg")
 
         with col3:
             download_preprocessing_info(method_plot)
 
-    
     elif analysis_result is not None and df_to_display:
         col1, col2, col3 = st.columns([1, 1, 1])
 
         with col1:
             download_figure(method_plot, format="pdf", plotting_library="seaborn")
 
         with col2:
             download_figure(method_plot, format="svg", plotting_library="seaborn")
 
         with col3:
-             download_preprocessing_info(method_plot)
-    
+            download_preprocessing_info(method_plot)
+
     elif analysis_result is not None and df_to_display:
         st.download_button(
-                "Download as .csv", csv, filename, "text/csv", key="download-csv"
+            "Download as .csv", csv, filename, "text/csv", key="download-csv"
         )
-            
-
 
 
 else:
     st.info("Import Data first")
```

### Comparing `alphastats-0.6.2/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.3/alphastats/gui/pages/06_Results.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     plot[1].write_image(file=buffer, format=format)
     st.download_button(
         label="Download as " + format, data=buffer, file_name=plot[0] + "." + format
     )
 
 
 @st.cache_data
-def convert_df(df, user_session_id = st.session_state.user_session_id):
+def convert_df(df, user_session_id=st.session_state.user_session_id):
     return df.to_csv().encode("utf-8")
 
 
 def download_preprocessing_info(plot, count):
     preprocesing_dict = plot[1].preprocessing
     df = pd.DataFrame(preprocesing_dict.items())
     filename = "plot" + plot[0] + "preprocessing_info.csv"
```

### Comparing `alphastats-0.6.2/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.3/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.3/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.3/alphastats/gui/utils/analysis_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,62 +75,60 @@
 def gui_volcano_plot_differential_expression_analysis(
         chosen_parameter_dict, user_session_id = st.session_state.user_session_id
     ):
     """
     initalize volcano plot object with differential expression analysis results
     """
     volcano_plot = VolcanoPlot(
-        dataset=st.session_state.dataset, 
-        **chosen_parameter_dict, 
-        plot = False
+        dataset=st.session_state.dataset, **chosen_parameter_dict, plot=False
     )
     volcano_plot._perform_differential_expression_analysis()
     volcano_plot._add_hover_data_columns()
     return volcano_plot
 
+
 def gui_volcano_plot():
     """
     Draw Volcano Plot using the VolcanoPlot class
     """
     chosen_parameter_dict = helper_compare_two_groups()
     method = st.selectbox(
         "Differential Analysis using:",
         options=["ttest", "anova", "wald", "sam", "paired-ttest", "welch-ttest"],
     )
     chosen_parameter_dict.update({"method": method})
 
     # TODO streamlit doesnt allow nested columns check for updates
-    
+
     labels = st.checkbox("Add label")
 
     draw_line = st.checkbox("Draw line")
 
     alpha = st.number_input(
-            label="alpha", min_value=0.001, max_value=0.050, value=0.050
-        )
+        label="alpha", min_value=0.001, max_value=0.050, value=0.050
+    )
 
     min_fc = st.select_slider("Foldchange cutoff", range(0, 3), value=1)
- 
+
     plotting_parameter_dict = {
-            "labels": labels,
-            "draw_line": draw_line,
-            "alpha": alpha,
-            "min_fc": min_fc,
-        }
+        "labels": labels,
+        "draw_line": draw_line,
+        "alpha": alpha,
+        "min_fc": min_fc,
+    }
 
     if method == "sam":
         perm = st.number_input(
             label="Number of Permutations", min_value=1, max_value=1000, value=10
         )
         fdr = st.number_input(
             label="FDR cut off", min_value=0.005, max_value=0.1, value=0.050
         )
         chosen_parameter_dict.update({"perm": perm, "fdr": fdr})
 
-   
     submitted = st.button("Submit")
 
     if submitted:
         volcano_plot = gui_volcano_plot_differential_expression_analysis(
             chosen_parameter_dict, user_session_id = st.session_state.user_session_id
         )
         volcano_plot._update(plotting_parameter_dict)
@@ -259,14 +257,15 @@
     group = st.selectbox(
         "Grouping variable",
         options=["< None >"] + st.session_state.dataset.metadata.columns.to_list(),
     )
 
     if group != "< None >":
 
+
         unique_values = get_unique_values_from_column(group)
 
         group1 = st.selectbox("Group 1", options=unique_values)
 
         group2 = st.selectbox("Group 2", options=list(reversed(unique_values)))
 
         chosen_parameter_dict.update(
@@ -288,14 +287,15 @@
         group2 = st.multiselect(
                 "Group 2 samples:",
                 options=list(
                     reversed(st.session_state.dataset.metadata[st.session_state.dataset.sample].to_list())
                 ),
             )
 
+
         intersection_list = list(set(group1).intersection(set(group2)))
 
         if len(intersection_list) > 0:
             st.warning(
                 "Group 1 and Group 2 contain same samples: " + str(intersection_list)
             )
 
@@ -304,25 +304,30 @@
     return chosen_parameter_dict
 
 
 def get_sample_names_from_software_file():
     """
     extract sample names from software
     """
-    regex_find_intensity_columns = st.session_state.loader.intensity_column.replace(
-        "[sample]", ".*"
-    )
-
-    df = st.session_state.loader.rawinput
-    df = df.set_index(st.session_state.loader.index_column)
-    df = df.filter(regex=(regex_find_intensity_columns), axis=1)
-    # remove Intensity so only sample names remain
-    substring_to_remove = regex_find_intensity_columns.replace(".*", "")
-    df.columns = df.columns.str.replace(substring_to_remove, "")
-    return df.columns.to_list()
+    if isinstance(st.session_state.loader.intensity_column, str):
+        regex_find_intensity_columns = st.session_state.loader.intensity_column.replace(
+            "[sample]", ".*"
+        )
+        df = st.session_state.loader.rawinput
+        df = df.set_index(st.session_state.loader.index_column)
+        df = df.filter(regex=(regex_find_intensity_columns), axis=1)
+        # remove Intensity so only sample names remain
+        substring_to_remove = regex_find_intensity_columns.replace(".*", "")
+        df.columns = df.columns.str.replace(substring_to_remove, "")
+        sample_names = df.columns.to_list()
+    
+    else:
+        sample_names = st.session_state.loader.intensity_column
+    
+    return sample_names
 
 
 def get_analysis(method, options_dict):
 
     if method in options_dict.keys():
         obj = get_analysis_options_from_dict(method, options_dict=options_dict)
         return obj
@@ -338,24 +343,25 @@
         range(250, 2001),
         value=1000,
     )
     perplexity = st.select_slider("Perplexity", range(5, 51), value=30)
 
     submitted = st.button("Submit")
     chosen_parameter_dict.update(
-        {
-            "n_iter": n_iter,
-            "perplexity": perplexity,
-        }
+        {"n_iter": n_iter, "perplexity": perplexity,}
     )
 
     if submitted:
         with st.spinner("Calculating..."):
             return method_dict["function"](**chosen_parameter_dict)
 
 
 def load_options():
 
     from alphastats.gui.utils.options import plotting_options, statistic_options
 
     st.session_state["plotting_options"] = plotting_options
     st.session_state["statistic_options"] = statistic_options
+
+
+def gui_multicova_analysis():
+    pass
```

### Comparing `alphastats-0.6.2/alphastats/gui/utils/options.py` & `alphastats-0.6.3/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/gui/utils/software_options.py` & `alphastats-0.6.3/alphastats/gui/utils/software_options.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 from alphastats.loader.MaxQuantLoader import MaxQuantLoader
 from alphastats.loader.AlphaPeptLoader import AlphaPeptLoader
 from alphastats.loader.FragPipeLoader import FragPipeLoader
 from alphastats.loader.DIANNLoader import DIANNLoader
 from alphastats.loader.SpectronautLoader import SpectronautLoader
+from alphastats.loader.GenericLoader import GenericLoader
+from alphastats.loader.mzTabLoader import mzTabLoader
 
 software_options = {
     "MaxQuant": {
-        "import_file": "proteinGroups.txt",
-        "intensity_column": ["LFQ intensity [sample]"],
-        "index_column": ["Protein IDs"],
+        "import_file": "Please upload proteinGroups.txt",
+        "intensity_column": ["LFQ intensity [sample]", "Intensity [sample]"],
+        "index_column": ["Protein IDs", "Gene names", "Majority protein IDs", "Protein names"],
         "loader_function": MaxQuantLoader,
     },
     "AlphaPept": {
-        "import_file": "results_proteins.csv or results.hdf",
+        "import_file": "Please upload results_proteins.csv or results.hdf",
         "intensity_column": ["[sample]_LFQ"],
         "index_column": ["Unnamed: 0"],
         "loader_function": AlphaPeptLoader,
     },
     "DIANN": {
-        "import_file": "report.pg_matrix.tsv",
+        "import_file": "Please upload report.pg_matrix.tsv",
         "intensity_column": ["[sample]"],
         "index_column": ["Protein.Group"],
         "loader_function": DIANNLoader,
     },
     "FragPipe": {
-        "import_file": "combined_protein.tsv",
+        "import_file": "Please upload combined_protein.tsv file from FragPipe.",
         "intensity_column": ["[sample] MaxLFQ Intensity", "[sample] Intensity"],
         "index_column": ["Protein", "Protein ID"],
         "loader_function": FragPipeLoader,
     },
     "Spectronaut": {
-        "import_file": "spectronaut.tsv",
+        "import_file": "Please upload spectronaut.tsv",
         "intensity_column": ["PG.Quantity", "F.PeakArea", "PG.Log2Quantity"],
         "index_column": ["PG.ProteinGroups", "PEP.StrippedSequence"],
         "loader_function": SpectronautLoader,
     },
+     "Other": {
+        "import_file": "Please upload your proteomics file.",
+        "intensity_column": [],
+        "index_column": [],
+        "loader_function": GenericLoader,
+    },
+     "mzTab": {
+        "import_file": "Please upload your .mzTab file with quantitative proteomics data.",
+        "intensity_column": ["protein_abundance_[sample]"],
+        "index_column": ["accession"],
+        "loader_function": mzTabLoader,
+    },
 }
```

### Comparing `alphastats-0.6.2/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.3/alphastats/gui/utils/ui_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     <body>
         <div class="footer">Mann Group, 2022</div>
     </body>""",
         unsafe_allow_html=True,
     )
 
 
-
 def display_sidebar_html_table():
 
     if "dataset" not in st.session_state:
         return
 
     preprocessing_dict = st.session_state.dataset.preprocessing_info
```

### Comparing `alphastats-0.6.2/alphastats/load_data.py` & `alphastats-0.6.3/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.3/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/loader/BaseLoader.py` & `alphastats-0.6.3/alphastats/loader/BaseLoader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pandas as pd
 import logging
 import os
 import numpy as np
 from alphastats.utils import find_duplicates_in_list
 import pkg_resources
-
+from typing import Union
 
 class BaseLoader:
     """Parent class of Loaders"""
 
-    def __init__(self, file, intensity_column, index_column, sep):
-        """BaseLoader for AlphaPept, MaxQuant, Fragpipe and DIANNLoader
+    def __init__(self, file:Union[str, pd.DataFrame], intensity_column:Union[str, list], index_column:str, sep:str):
+        """BaseLoader for AlphaPept, MaxQuant, Fragpipe, Spectronau and DIANNLoader
 
         Args:
             file_path (str): path to file
             sep (str, optional): file separation. Defaults to "\t".
         """
 
-        # self._check_if_file_exists(file=file)
+
         if isinstance(file, pd.DataFrame):
             self.rawinput = file
         else:
             self.rawinput = pd.read_csv(file, sep=sep, low_memory=False)
         self.intensity_column = intensity_column
         self.index_column = index_column
         self.filter_columns = []
@@ -43,15 +43,15 @@
                 ", ".join(wrong_columns) + " columns do not exist.\n"
                 "Check the documtentation: \n"
                 "AlphaPept Format: https://github.com/MannLabs/alphapept \n"
                 "DIA-NN Format: https://github.com/vdemichev/DiaNN"
                 "FragPipe Format: https://fragpipe.nesvilab.org/docs/tutorial_fragpipe_outputs.html#combined_proteintsv"
                 "MaxQuant Format: http://www.coxdocs.org/doku.php?id=maxquant:table:proteingrouptable"
             )
-    
+
     def _read_all_columns_as_string(self):
         self.rawinput.columns = self.rawinput.columns.astype(str)
 
     def _check_if_indexcolumn_is_unique(self):
         duplicated_values = find_duplicates_in_list(self.rawinput[self.index_column].to_list())
         if len(duplicated_values) > 0:
             # error or warning, duplicates could be resolved with preprocessing/filtering
```

### Comparing `alphastats-0.6.2/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.3/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.3/alphastats/loader/FragPipeLoader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from alphastats.loader.BaseLoader import BaseLoader
 import pandas as pd
+from typing import Union
 
 # Philosopher
 # class name needs to be discussed whether MSFragger/Fragpipe/Philospher
 class FragPipeLoader(BaseLoader):
     """Loader for FragPipe-Philosopheroutputfiles
     https://fragpipe.nesvilab.org/docs/tutorial_fragpipe_outputs.html#combined_proteintsv
     """
 
     def __init__(
         self,
-        file,
-        intensity_column="[sample] MaxLFQ Intensity ",
-        index_column="Protein",
-        gene_names_column="Gene Names",
-        confidence_column="Protein Probability",
-        sep="\t",
+        file:Union[str, pd.DataFrame],
+        intensity_column:str="[sample] MaxLFQ Intensity ",
+        index_column:str="Protein",
+        gene_names_column:str="Gene Names",
+        confidence_column:str="Protein Probability",
+        sep:str="\t",
         **kwargs
     ):
 
         super().__init__(file, intensity_column, index_column, sep)
 
         if gene_names_column in self.rawinput.columns.to_list():
             self.gene_names = gene_names_column
```

### Comparing `alphastats-0.6.2/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.3/alphastats/loader/MaxQuantLoader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from alphastats.loader.BaseLoader import BaseLoader
 import pandas as pd
 import numpy as np
+from typing import Union
 
 
 class MaxQuantLoader(BaseLoader):
     """Loader for MaxQuant outputfiles"""
 
     def __init__(
         self,
         file,
-        intensity_column="LFQ intensity [sample]",
-        index_column="Protein IDs",
-        gene_names_column="Gene names",
-        filter_columns=["Only identified by site", "Reverse", "Potential contaminant"],
-        confidence_column="Q-value",
+        intensity_column:Union[str, list]="LFQ intensity [sample]",
+        index_column:str="Protein IDs",
+        gene_names_column:str="Gene names",
+        filter_columns:list=["Only identified by site", "Reverse", "Potential contaminant"],
+        confidence_column:str="Q-value",
         evidence_file=None,
-        sep="\t",
+        sep:str="\t",
         **kwargs
     ):
         """Loader MaxQuant output
 
         Args:
             file (str): ProteinGroups.txt file: http://www.coxdocs.org/doku.php?id=maxquant:table:proteingrouptable
             intensity_column (str, optional): columns with Intensity values for each sample. Defaults to "LFQ intentsity [experiment]".
```

### Comparing `alphastats-0.6.2/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.3/alphastats/loader/SpectronautLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,122 @@
 from alphastats.loader.BaseLoader import BaseLoader
 import pandas as pd
 import numpy as np
 import logging
 
 
-
 class SpectronautLoader(BaseLoader):
     """Loader for Spectronaut outputfiles 
     """
 
     def __init__(
         self,
         file,
         intensity_column="PG.Quantity",
-        index_column="PG.ProteinGroups", 
-        sample_column = "R.FileName",
+        index_column="PG.ProteinGroups",
+        sample_column="R.FileName",
         gene_names_column="PG.Genes",
-        filter_qvalue = True,
-        qvalue_cutoff = 0.01,
-        sep="\t"
+        filter_qvalue=True,
+        qvalue_cutoff=0.01,
+        sep="\t",
     ):
         """Loads Spectronaut output. Will add contamination column for further analysis.
 
         Args:
             file (str): path to Spectronaut outputfile or pandas.DataFrame 
             intensity_column (str, optional): columns where the intensity of the proteins are given. Defaults to "PG.Quantity".
             index_column (str, optional): column indicating the protein groups. Defaults to "PG.ProteinGroups".
             sample_column (str, optional): column that contains sample names used for downstream analysis. Defaults to "R.FileName".
             gene_names_column (str, optional): column with gene names. Defaults to "PG.Genes".
             filter_qvalue (bool, optional): will filter out the intensities that have greater than qvalue_cutoff in EG.Qvalue column. Those intensities will be replaced with zero and will be considered as censored missing values for imputation purpose.. Defaults to True.
             qvalue_cutoff (float, optional): cut off vaéie. Defaults to 0.01.
             sep (str, optional): file separation of file. Defaults to "\t".
         """
-        
+
         self.software = "Spectronaut"
         self.intensity_column = intensity_column
         self.index_column = index_column
         self.confidence_column = None
         self.filter_columns = []
-        self.evidence_df = None 
+        self.evidence_df = None
         self.gene_names = None
 
         self._read_spectronaut_file(file=file, sep=sep)
 
         if filter_qvalue:
             self._filter_qvalue(qvalue_cutoff=qvalue_cutoff)
 
-        self._reshape_spectronaut(sample_column=sample_column, gene_names_column=gene_names_column)
+        self._reshape_spectronaut(
+            sample_column=sample_column, gene_names_column=gene_names_column
+        )
         self._add_contamination_column()
         self._read_all_columns_as_string()
-              
 
     def _reshape_spectronaut(self, sample_column, gene_names_column):
         """
         other proteomics softwares use a wide format (column for each sample)
         reshape to a wider format
         """
-        self.rawinput["sample"] = self.rawinput[sample_column] + "_" + self.intensity_column
-        
+        self.rawinput["sample"] = (
+            self.rawinput[sample_column] + "_" + self.intensity_column
+        )
+
         indexing_columns = [self.index_column]
-        
+
         if gene_names_column in self.rawinput.columns.to_list():
             self.gene_names = gene_names_column
             indexing_columns += [self.gene_names]
-        
+
         keep_columns = [self.intensity_column, "sample"] + indexing_columns
-        
+
         df = self.rawinput[keep_columns].drop_duplicates()
-        df = df.pivot(columns='sample', index=indexing_columns, values=self.intensity_column)
+        df = df.pivot(
+            columns="sample", index=indexing_columns, values=self.intensity_column
+        )
         df.reset_index(inplace=True)
-        
+
         self.rawinput = df
-        
+
         self.intensity_column = "[sample]_" + self.intensity_column
 
     def _filter_qvalue(self, qvalue_cutoff):
         if "EG.Qvalue" not in self.rawinput.columns.to_list():
-            raise Warning("Column EG.Qvalue not found in file. File will not be filtered according to q-value.")
-        
+            raise Warning(
+                "Column EG.Qvalue not found in file. File will not be filtered according to q-value."
+            )
+
         rows_before_filtering = self.rawinput.shape[0]
         self.rawinput = self.rawinput[self.rawinput["EG.Qvalue"] < qvalue_cutoff]
         rows_after_filtering = self.rawinput.shape[0]
 
         rows_removed = rows_before_filtering - rows_after_filtering
-        logging.info(f"{rows_removed} identification with a qvalue below {qvalue_cutoff} have been removed")
-        
-    
+        logging.info(
+            f"{rows_removed} identification with a qvalue below {qvalue_cutoff} have been removed"
+        )
+
     def _read_spectronaut_file(self, file, sep):
         # some spectronaut files include european decimal separators
         if isinstance(file, pd.DataFrame):
             df = file
         else:
             df = pd.read_csv(file, sep=sep, low_memory=False)
 
             if df[self.intensity_column].dtype != np.float64:
                 # load european
                 df = pd.read_csv(file, sep=sep, decimal=",")
 
         self.rawinput = df
-        
-    
 
-#filter_with_Qvalue	
-#TRUE(default) will filter out the intensities that have greater than qvalue_cutoff in EG.Qvalue column. Those intensities will be replaced with zero and will be considered as censored missing values for imputation purpose.
 
-#qvalue_cutoff	
-#Cutoff for EG.Qvalue. default is 0.01.
+# filter_with_Qvalue
+# TRUE(default) will filter out the intensities that have greater than qvalue_cutoff in EG.Qvalue column. Those intensities will be replaced with zero and will be considered as censored missing values for imputation purpose.
+
+# qvalue_cutoff
+# Cutoff for EG.Qvalue. default is 0.01.
 
-# Protein Level
-# PG.Quantity
+#  Protein Level
+#  PG.Quantity
 # PG.ProteinGroups
 
 # Peptide Level
 # F.PeakArea
 # PEP.StrippedSequence
-
```

### Comparing `alphastats-0.6.2/alphastats/loader/mzTabLoader.py` & `alphastats-0.6.3/alphastats/loader/mzTabLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/multicova/multicova.py` & `alphastats-0.6.3/alphastats/multicova/multicova.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,39 +20,42 @@
 
 # code taken from Isabel Bludau - multicova
 
 def get_std(x):
     """
     Function to calculate the sample standard deviation.
     """
-    std_x = np.sqrt(np.sum((abs(x - x.mean())**2)/(len(x)-1)))
+    std_x = np.sqrt(np.sum((abs(x - x.mean()) ** 2) / (len(x) - 1)))
     return std_x
 
 
 def perform_ttest(x, y, s0):
     """
     Function to perform a independent two-sample t-test including s0
     adjustment.
     Assumptions: Equal or unequal sample sizes with similar variances.
     """
     mean_x = np.mean(x)
     mean_y = np.mean(y)
     # Get fold-change
-    fc = mean_x-mean_y
+    fc = mean_x - mean_y
     n_x = len(x)
     n_y = len(y)
     # pooled standard vatiation
     # assumes that the two distributions have the same variance
-    sp = np.sqrt((((n_x-1)*get_std(x)**2) + ((n_y-1)*(get_std(y)**2)))/(n_x+n_y-2))
+    sp = np.sqrt(
+        (((n_x - 1) * get_std(x) ** 2) + ((n_y - 1) * (get_std(y) ** 2)))
+        / (n_x + n_y - 2)
+    )
     # Get t-values
-    tval = fc/(sp * (np.sqrt((1/n_x)+(1/n_y))))
-    tval_s0 = fc/((sp * (np.sqrt((1/n_x)+(1/n_y))))+s0)
+    tval = fc / (sp * (np.sqrt((1 / n_x) + (1 / n_y))))
+    tval_s0 = fc / ((sp * (np.sqrt((1 / n_x) + (1 / n_y)))) + s0)
     # Get p-values
-    pval = 2*(1-stats.t.cdf(np.abs(tval), n_x+n_y-2))
-    pval_s0 = 2*(1-stats.t.cdf(np.abs(tval_s0), n_x+n_y-2))
+    pval = 2 * (1 - stats.t.cdf(np.abs(tval), n_x + n_y - 2))
+    pval_s0 = 2 * (1 - stats.t.cdf(np.abs(tval_s0), n_x + n_y - 2))
     return [fc, tval, pval, tval_s0, pval_s0]
 
 
 def permutate_vars(X, n_rand, seed=42):
     """
     Function to randomly permutate an array `n_rand` times.
     """
@@ -68,19 +71,21 @@
     Function to perform a t-test on all rows in a data frame.
     c1 specifies the column names with intensity values of the first condition.
     c2 specifies the column names with intensity values of the second
     condition. s0 is the tuning parameter that specifies the minimum
     fold-change to be trusted.
     """
     if parallelize:
-        res = df.swifter.progress_bar(False).apply(lambda row : perform_ttest(row[c1], row[c2], s0=s0), axis = 1)
+        res = df.swifter.progress_bar(False).apply(
+            lambda row: perform_ttest(row[c1], row[c2], s0=s0), axis=1
+        )
     else:
-        res = df.apply(lambda row : perform_ttest(row[c1], row[c2], s0=s0), axis = 1)
+        res = df.apply(lambda row: perform_ttest(row[c1], row[c2], s0=s0), axis=1)
 
-    res = pd.DataFrame(list(res), columns=['fc','tval','pval','tval_s0','pval_s0'])
+    res = pd.DataFrame(list(res), columns=["fc", "tval", "pval", "tval_s0", "pval_s0"])
 
     df_real = pd.concat([df, res], axis=1)
 
     return df_real
 
 
 def workflow_permutation_tvals(df, c1, c2, s0=1, n_perm=2, parallelize=False):
@@ -92,26 +97,36 @@
     condition. s0 is the tuning parameter that specifies the minimum
     fold-change to be trusted. n_perm specifies the number of random
     permutations to perform.
     """
     all_c = c1 + c2
     all_c_rand = permutate_vars(all_c, n_rand=n_perm)
     res_perm = list()
-    for i in np.arange(0,len(all_c_rand)):
+    for i in np.arange(0, len(all_c_rand)):
         if parallelize:
-            res_i = df.swifter.progress_bar(False).apply(lambda row : perform_ttest(row[all_c_rand[i][0:len(c1)]],
-                                                                row[all_c_rand[i][len(c1):len(c1)+len(c2)]],
-                                                                s0=s0),
-                                                                axis = 1)
+            res_i = df.swifter.progress_bar(False).apply(
+                lambda row: perform_ttest(
+                    row[all_c_rand[i][0 : len(c1)]],
+                    row[all_c_rand[i][len(c1) : len(c1) + len(c2)]],
+                    s0=s0,
+                ),
+                axis=1,
+            )
         else:
-            res_i = df.apply(lambda row : perform_ttest(row[all_c_rand[i][0:len(c1)]],
-                                                        row[all_c_rand[i][len(c1):len(c1)+len(c2)]],
-                                                        s0=s0),
-                                                        axis=1)
-        res_i = pd.DataFrame(list(res_i), columns=['fc','tval','pval','tval_s0','pval_s0'])
+            res_i = df.apply(
+                lambda row: perform_ttest(
+                    row[all_c_rand[i][0 : len(c1)]],
+                    row[all_c_rand[i][len(c1) : len(c1) + len(c2)]],
+                    s0=s0,
+                ),
+                axis=1,
+            )
+        res_i = pd.DataFrame(
+            list(res_i), columns=["fc", "tval", "pval", "tval_s0", "pval_s0"]
+        )
         res_perm.append(list(np.sort(np.abs(res_i.tval_s0.values))))
     return res_perm
 
 
 def get_tstat_cutoff(res_real, t_perm_avg, delta):
     # Extract all t-stats from the results of the 'real' data
     # and sort the absolute values.
@@ -124,15 +139,15 @@
     t_diff = t_real_abs - t_perm_avg
     # print(t_diff)
 
     # Find the minimum t-stat value for which the difference
     # between the observed and average random t-stat is
     # larger than the selected delta.
     t_max = t_real_abs[t_diff > delta]
-    if (t_max.shape[0] == 0):
+    if t_max.shape[0] == 0:
         t_max = np.ceil(np.max(t_real_abs))
     else:
         t_max = np.min(t_max)
     return t_max
 
 
 @nb.njit
@@ -190,32 +205,32 @@
             t_perm.append(r)
     t_perm_abs = np.sort(np.abs(t_perm))
 
     t_perm_25 = np.percentile(t_perm_abs, 25)
     t_perm_75 = np.percentile(t_perm_abs, 75)
 
     n_real_in_range = np.sum((t_real_abs >= t_perm_25) & (t_real_abs <= t_perm_75))
-    pi0 = n_real_in_range/(0.5*len(t_real_abs))
+    pi0 = n_real_in_range / (0.5 * len(t_real_abs))
 
     # pi0 can maximally be 1
     pi0 = np.min([pi0, 1])
 
     return pi0
 
 
 def get_fdr(n_pos, n_false_pos, pi0):
     """
     Compute the FDR by dividing the number of false positives by the number of
     true positives. The number of false positives are adjusted by pi0, the
     proportion of true null (unaffected) genes in the data set.
     """
-    n = n_false_pos*pi0
+    n = n_false_pos * pi0
     if n != 0:
         if n_pos != 0:
-            fdr = n/n_pos
+            fdr = n / n_pos
         else:
             fdr = 0
     else:
         if n_pos > 0:
             fdr = 0
         else:
             fdr = np.nan
@@ -230,15 +245,15 @@
     t_cut, n_pos, n_false_pos, pi0, n_false_pos_corr, fdr
     """
     perm_avg = np.mean(res_perm, axis=0)
     t_cut = get_tstat_cutoff(res_real, perm_avg, delta)
     n_pos = get_positive_count(res_real_tval_s0=np.array(res_real.tval_s0), t_cut=t_cut)
     n_false_pos = get_false_positive_count(np.array(res_perm), t_cut=t_cut)
     pi0 = get_pi0(res_real, res_perm)
-    n_false_pos_corr = n_false_pos*pi0
+    n_false_pos_corr = n_false_pos * pi0
     fdr = get_fdr(n_pos, n_false_pos, pi0)
     return [t_cut, n_pos, n_false_pos, pi0, n_false_pos_corr, fdr]
 
 
 def get_fdr_stats_across_deltas(res_real, res_perm):
     """
     Wrapper function that starts with the res_real and res_perm to derive
@@ -247,96 +262,122 @@
     res_stats = list()
     for d in np.arange(0, 10, 0.01):
         res_d = estimate_fdr_stats(res_real, res_perm, d)
         if np.isnan(res_d[5]):
             break
         else:
             res_stats.append(res_d)
-    res_stats_df = pd.DataFrame(res_stats,
-                                columns=['t_cut', 'n_pos', 'n_false_pos', 'pi0', 'n_false_pos_corr', 'fdr'])
+    res_stats_df = pd.DataFrame(
+        res_stats,
+        columns=["t_cut", "n_pos", "n_false_pos", "pi0", "n_false_pos_corr", "fdr"],
+    )
 
-    return(res_stats_df)
+    return res_stats_df
 
 
 def get_tstat_limit(stats, fdr=0.01):
     """
     Function to get tval_s0 at the specified FDR.
     """
     t_limit = np.min(stats[stats.fdr <= fdr].t_cut)
-    return(t_limit)
+    return t_limit
 
 
 def annotate_fdr_significance(res_real, stats, fdr=0.01):
     t_limit = np.min(stats[stats.fdr <= fdr].t_cut)
-    res_real['qval'] = [np.min(stats[stats.t_cut <= abs(x)].fdr) for x in res_real['tval_s0']]
-    res_real['FDR' + str(int(fdr*100)) + '%'] = ["sig" if abs(x) >= t_limit else "non_sig" for x in res_real['tval_s0']]
-    return(res_real)
+    res_real["qval"] = [
+        np.min(stats[stats.t_cut <= abs(x)].fdr) for x in res_real["tval_s0"]
+    ]
+    res_real["FDR" + str(int(fdr * 100)) + "%"] = [
+        "sig" if abs(x) >= t_limit else "non_sig" for x in res_real["tval_s0"]
+    ]
+    return res_real
 
 
 def perform_ttest_getMaxS(fc, s, s0, n_x, n_y):
     """
     Helper function to get ttest stats for specified standard errors s.
     Called from within get_fdr_line.
     """
     # Get t-values
-    tval = fc/s
-    tval_s0 = fc/(s+s0)
+    tval = fc / s
+    tval_s0 = fc / (s + s0)
 
     # Get p-values
-    pval = 2*(1-stats.t.cdf(np.abs(tval), n_x+n_y-2))
-    pval_s0 = 2*(1-stats.t.cdf(np.abs(tval_s0), n_x+n_y-2))
+    pval = 2 * (1 - stats.t.cdf(np.abs(tval), n_x + n_y - 2))
+    pval_s0 = 2 * (1 - stats.t.cdf(np.abs(tval_s0), n_x + n_y - 2))
 
     return [fc, tval, pval, tval_s0, pval_s0]
 
 
-def get_fdr_line(t_limit, s0, n_x, n_y, plot=False,
-                 fc_s=np.arange(0, 6, 0.01), s_s=np.arange(0.005, 6, 0.005)):
+def get_fdr_line(
+    t_limit,
+    s0,
+    n_x,
+    n_y,
+    plot=False,
+    fc_s=np.arange(0, 6, 0.01),
+    s_s=np.arange(0.005, 6, 0.005),
+):
     """
     Function to get the fdr line for a volcano plot as specified tval_s0
     limit, s0, n_x and n_y.
     """
     pvals = np.ones(len(fc_s))
     svals = np.zeros(len(fc_s))
     for i in np.arange(0, len(fc_s)):
         for j in np.arange(0, len(s_s)):
             res_s = perform_ttest_getMaxS(fc=fc_s[i], s=s_s[j], s0=s0, n_x=n_x, n_y=n_y)
             if res_s[3] >= t_limit:
                 if svals[i] < s_s[j]:
                     svals[i] = s_s[j]
                     pvals[i] = res_s[2]
 
-    s_df = pd.DataFrame(np.array([fc_s, svals, pvals]).T, columns=['fc_s','svals','pvals'])
+    s_df = pd.DataFrame(
+        np.array([fc_s, svals, pvals]).T, columns=["fc_s", "svals", "pvals"]
+    )
     s_df = s_df[s_df.pvals != 1]
 
     s_df_neg = s_df.copy()
     s_df_neg.fc_s = -s_df_neg.fc_s
 
     s_df = pd.concat([s_df, s_df_neg])
 
-    if (plot):
-        fig = px.scatter(x=s_df.fc_s,
-                         y=-np.log10(s_df.pvals),
-                         template='simple_white')
+    if plot:
+        fig = px.scatter(x=s_df.fc_s, y=-np.log10(s_df.pvals), template="simple_white")
         fig.show()
 
-    return(s_df)
+    return s_df
 
 
-
-def perform_ttest_analysis(df, c1, c2, s0=1, n_perm=2, fdr=0.01, id_col='Genes', plot_fdr_line=False, parallelize=False):
+def perform_ttest_analysis(
+    df,
+    c1,
+    c2,
+    s0=1,
+    n_perm=2,
+    fdr=0.01,
+    id_col="Genes",
+    plot_fdr_line=False,
+    parallelize=False,
+):
     """
     Workflow function for the entire T-test analysis including FDR
     estimation and visualizing a volcanoe plot.
     """
     ttest_res = workflow_ttest(df, c1, c2, s0, parallelize=parallelize)
-    ttest_perm_res = workflow_permutation_tvals(df, c1, c2, s0, n_perm, parallelize=parallelize)
+    ttest_perm_res = workflow_permutation_tvals(
+        df, c1, c2, s0, n_perm, parallelize=parallelize
+    )
     ttest_stats = get_fdr_stats_across_deltas(ttest_res, ttest_perm_res)
-    ttest_res = annotate_fdr_significance(res_real=ttest_res, stats=ttest_stats, fdr=fdr)
+    ttest_res = annotate_fdr_significance(
+        res_real=ttest_res, stats=ttest_stats, fdr=fdr
+    )
     t_limit = get_tstat_limit(stats=ttest_stats, fdr=fdr)
-    return(ttest_res, t_limit)
+    return (ttest_res, t_limit)
 
 
 def perform_regression(y, X, s0):
     """
     Function to perform multiple linear regression including the s0 parameter.
     """
     # Use LinearRegression from sklearn.linear_model
@@ -347,50 +388,50 @@
 
     # Add intercept column to X dataframe
     newX = pd.DataFrame({"Constant": np.ones(len(X))}).join(pd.DataFrame(X))
 
     # Calculate mean squared error (MSE) of observed y vs. prediction
     # MSE = squared_error/degrees_of_freedom
     # degrees_of_freedom = number_of_samples - number_of_betas (including beta0 = intercept)
-    MSE = (sum((y-predictions)**2))/(len(newX)-len(newX.columns))
+    MSE = (sum((y - predictions) ** 2)) / (len(newX) - len(newX.columns))
     # Calculate t-values and p-values
     ts_b, ps_b = get_tstats(newX, betas, MSE)
     # Adjust the MSE by the minimum fold change that we trust (s0)
     MSE_s0 = MSE + s0
     # Calculate t-values and p-values
     ts_b_s0, ps_b_s0 = get_tstats(newX, betas, MSE_s0)
     betas_std = list()
     for i in np.arange(0, len(betas)):
-        betas_std.append(betas[i]*(get_std(np.array(newX)[:, i])/get_std(y)))
+        betas_std.append(betas[i] * (get_std(np.array(newX)[:, i]) / get_std(y)))
     betas_std = np.array(betas_std)
     return betas, betas_std, predictions, MSE, ts_b, ps_b, MSE_s0, ts_b_s0, ps_b_s0
 
 
 def get_tstats(newX, betas, MSE):
     # Calculate standard deviation for each beta
     # This scales the error as estimated by MSE to each beta
     # (error on the betas might be different for different betas depending on
     # the variable)
-    var_b = MSE*(np.linalg.inv(np.dot(newX.T, newX)).diagonal())
+    var_b = MSE * (np.linalg.inv(np.dot(newX.T, newX)).diagonal())
     sd_b = np.sqrt(var_b)
     # Get t-values
-    ts_b = betas/sd_b
+    ts_b = betas / sd_b
     # Get p-values
-    #ps_b =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b]
-    #ps_b =[2*(1-nbs.t_cdf(np.abs(i),len(newX)-len(newX.columns),0,1)) for i in ts_b]
-    ps_b = get_cdf(ts_b, len(newX)-len(newX.columns))
+    # ps_b =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b]
+    # ps_b =[2*(1-nbs.t_cdf(np.abs(i),len(newX)-len(newX.columns),0,1)) for i in ts_b]
+    ps_b = get_cdf(ts_b, len(newX) - len(newX.columns))
     return ts_b, ps_b
 
 
 @nb.njit
 def get_cdf(ts, df):
     pvals = [0.0][1:]
     for t in ts:
-        pvals.append(2*(1-nbs.t_cdf(np.abs(t), df, 0, 1)))
-    return (pvals)
+        pvals.append(2 * (1 - nbs.t_cdf(np.abs(t), df, 0, 1)))
+    return pvals
 
 
 def filter_nan(y, X):
     """
     Find nan values in quantitative data y and remove corresponding samples
     from both X and y.
     """
@@ -407,118 +448,144 @@
     min_vars = list()
     for d in np.arange(0, X.shape[1]):
         test_vals = X[:, d]
         n_vars = len(set(test_vals))
         if n_vars > 2:
             min_vars.append(n_vars)
         else:
-            test_vals_0 = np.append(test_vals,[0,1]) # append 0 and 1 for counter
+            test_vals_0 = np.append(test_vals, [0, 1])  # append 0 and 1 for counter
             var_count = Counter(test_vals_0)
             min_vars.append(min(var_count.values()))
 
     return min_vars
 
 
 def regression_workflow(y, X, s0):
     y_new, X_new = filter_nan(y, X)
     # Removed min_var filtering after standard scaling of variable.
     # @ToDo: Include sanity check that sufficient categories are covered!
     # The following counts the minimum number of observations for each covariate
-    #min_vars = get_min_vars(X_new)
+    # min_vars = get_min_vars(X_new)
     # A min(min_vars) value < 2 means essentially no values for at least one covariate were observed
     # A beta of zero and p-values of 1 are returned for these cases
-    #if min(min_vars) < 2:
+    # if min(min_vars) < 2:
     #    betas, betas_std, tvals, pvals, tvals_s0, pvals_s0 = 0, 0, 0, 1, 0, 1
-    #else:
+    # else:
     #    betas, betas_std, predictions, MSE, tvals, pvals, MSE_s0, tvals_s0, pvals_s0 = perform_regression(np.array(y_new), np.array(X_new), s0)
-    betas, betas_std, predictions, MSE, tvals, pvals, MSE_s0, tvals_s0, pvals_s0 = perform_regression(np.array(y_new), np.array(X_new), s0)
+    (
+        betas,
+        betas_std,
+        predictions,
+        MSE,
+        tvals,
+        pvals,
+        MSE_s0,
+        tvals_s0,
+        pvals_s0,
+    ) = perform_regression(np.array(y_new), np.array(X_new), s0)
     return betas, betas_std, tvals, pvals, tvals_s0, pvals_s0
 
 
 def regression_workflow_permutation(y, X_rand, s0):
     res_rand = list()
     for X_r in X_rand:
         res_rand.append(regression_workflow(y, X_r, s0))
     # num_cores = multiprocessing.cpu_count()
     # res_rand = Parallel(n_jobs=num_cores-1)(delayed(regression_workflow)(y=y, X=X_r, s0=s0) for X_r in X_rand)
     return res_rand
 
 
-def get_fdr_line_regression(t_limits, s0, X, plot = False,
-                            fc_s = np.arange(0,6,0.01), s_s = np.arange(0.005,6,0.005)):
+def get_fdr_line_regression(
+    t_limits,
+    s0,
+    X,
+    plot=False,
+    fc_s=np.arange(0, 6, 0.01),
+    s_s=np.arange(0.005, 6, 0.005),
+):
     """
     Function to get the fdr line for a volcano plot as specified tval_s0 limit, s0, n_x and n_y.
     """
-    #pvals = [list(np.ones(len(fc_s)))] * X.shape[1]
-    pvals = [list(np.ones(len(fc_s))) for i in range(0,X.shape[1])]
-    #print(pvals)
-    #svals = [list(np.zeros(len(fc_s)))] * X.shape[1]
-    svals = [list(np.zeros(len(fc_s))) for i in range(0,X.shape[1])]
-    #print(svals)
-    for i in np.arange(0,len(fc_s)):
-        for j in np.arange(0,len(s_s)):
+    # pvals = [list(np.ones(len(fc_s)))] * X.shape[1]
+    pvals = [list(np.ones(len(fc_s))) for i in range(0, X.shape[1])]
+    # print(pvals)
+    # svals = [list(np.zeros(len(fc_s)))] * X.shape[1]
+    svals = [list(np.zeros(len(fc_s))) for i in range(0, X.shape[1])]
+    # print(svals)
+    for i in np.arange(0, len(fc_s)):
+        for j in np.arange(0, len(s_s)):
             res_s = perform_ttest_getMaxS_regression(fc=fc_s[i], s=s_s[j], s0=s0, X=X)
-            for k in np.arange(0,X.shape[1]):
+            for k in np.arange(0, X.shape[1]):
                 t_limit = t_limits[k]
                 if (res_s[k][3] >= t_limit) and (svals[k][i] < s_s[j]):
                     svals[k][i] = s_s[j]
                     pvals[k][i] = res_s[k][2]
     s_df_list = list()
     for k in np.arange(0, X.shape[1]):
-        s_df = pd.DataFrame(np.array([fc_s,svals[k],pvals[k]]).T, columns=['fc_s','svals','pvals'])
+        s_df = pd.DataFrame(
+            np.array([fc_s, svals[k], pvals[k]]).T, columns=["fc_s", "svals", "pvals"]
+        )
         s_df = s_df[s_df.pvals != 1]
 
         s_df_neg = s_df.copy()
         s_df_neg.fc_s = -s_df_neg.fc_s
 
         s_df = pd.concat([s_df, s_df_neg])
 
-        if (plot):
-            fig = px.scatter(x=s_df.fc_s,
-                             y=-np.log10(s_df.pvals),
-                             template='simple_white')
+        if plot:
+            fig = px.scatter(
+                x=s_df.fc_s, y=-np.log10(s_df.pvals), template="simple_white"
+            )
             fig.show()
 
         s_df_list.append(s_df)
 
-    return(s_df_list)
+    return s_df_list
 
 
 def perform_ttest_getMaxS_regression(fc, s, s0, X):
     """
     Helper function to get ttest stats for specified standard errors s.
     Called from within get_fdr_line_regression.
     """
-    newX = pd.DataFrame({"Constant":np.ones(len(X))}).join(pd.DataFrame(X))
-    fc=np.repeat(fc,newX.shape[1])
-    #print(fc)
-    var_b = s*(np.linalg.inv(np.dot(newX.T,newX)).diagonal())
+    newX = pd.DataFrame({"Constant": np.ones(len(X))}).join(pd.DataFrame(X))
+    fc = np.repeat(fc, newX.shape[1])
+    # print(fc)
+    var_b = s * (np.linalg.inv(np.dot(newX.T, newX)).diagonal())
     sd_b = np.sqrt(var_b)
-    ts_b = fc/sd_b
-    #ps_b =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b]
-    ps_b = get_cdf(ts_b, len(newX)-len(newX.columns))
-    var_b_s0 = (s+s0)*(np.linalg.inv(np.dot(newX.T,newX)).diagonal())
+    ts_b = fc / sd_b
+    # ps_b =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b]
+    ps_b = get_cdf(ts_b, len(newX) - len(newX.columns))
+    var_b_s0 = (s + s0) * (np.linalg.inv(np.dot(newX.T, newX)).diagonal())
     sd_b_s0 = np.sqrt(var_b_s0)
-    ts_b_s0 = fc/sd_b_s0
-    #ps_b_s0 =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b_s0]
-    ps_b_s0 = get_cdf(ts_b_s0, len(newX)-len(newX.columns))
-    res = [[fc[x], ts_b[x], ps_b[x], ts_b_s0[x], ps_b_s0[x]] for x in np.arange(1,newX.shape[1])]
+    ts_b_s0 = fc / sd_b_s0
+    # ps_b_s0 =[2*(1-stats.t.cdf(np.abs(i),len(newX)-len(newX.columns))) for i in ts_b_s0]
+    ps_b_s0 = get_cdf(ts_b_s0, len(newX) - len(newX.columns))
+    res = [
+        [fc[x], ts_b[x], ps_b[x], ts_b_s0[x], ps_b_s0[x]]
+        for x in np.arange(1, newX.shape[1])
+    ]
     return res
 
+
 def generate_perms(n, n_rand, seed=42):
     """
     Generate n_rand permutations of indeces ranging from 0 to n.
     """
     np.random.seed(seed)
     idx_v = np.arange(0, n)
     rand_v = list()
     n_rand_i = 0
-    n_rand_max = math.factorial(n)-1
+    n_rand_max = math.factorial(n) - 1
     if n_rand_max <= n_rand:
-        print("{} random permutations cannot be created. The maximum of n_rand={} is used instead.".format(n_rand, n_rand_max))
+        print(
+            "{} random permutations cannot be created. The maximum of n_rand={} is used instead.".format(
+                n_rand, n_rand_max
+            )
+        )
         n_rand = n_rand_max
     while n_rand_i < n_rand:
         rand_i = list(np.random.permutation(idx_v))
         if np.all(rand_i == idx_v):
             next
         else:
             if rand_i in rand_v:
@@ -543,250 +610,338 @@
         idx_a = np.transpose(idx_a)
         X_rand.append(np.take_along_axis(X, indices=idx_a, axis=0))
 
     return X_rand
 
 
 def get_res_parallel(y_i, X, s0):
-    betas, betas_std, tvals, pvals, tvals_s0, pvals_s0 = regression_workflow(y=y_i, X = X, s0 = s0)
+    betas, betas_std, tvals, pvals, tvals_s0, pvals_s0 = regression_workflow(
+        y=y_i, X=X, s0=s0
+    )
     res = pd.DataFrame()
-    res["fc"], res["fc_std"], res["tval"], res["pval"], res["tval_s0"], res["pval_s0"] = [betas, betas_std, tvals, pvals, tvals_s0, pvals_s0]
+    (
+        res["fc"],
+        res["fc_std"],
+        res["tval"],
+        res["pval"],
+        res["tval_s0"],
+        res["pval_s0"],
+    ) = [betas, betas_std, tvals, pvals, tvals_s0, pvals_s0]
     return res
 
 
 def get_perm_res_parallel(y_i, X_rand, s0):
     res_perm_list = regression_workflow_permutation(y_i, X_rand, s0=s0)
     return res_perm_list
 
 
-def full_regression_analysis(quant_data, annotation, covariates, sample_column='sample_name', n_permutations=4, fdr=0.05, s0=0.05, seed=42):
+def full_regression_analysis(
+    quant_data,
+    annotation,
+    covariates,
+    sample_column="sample_name",
+    n_permutations=4,
+    fdr=0.05,
+    s0=0.05,
+    seed=42,
+):
     data_cols = annotation[sample_column].values
     quant_data = quant_data.dropna().reset_index(drop=True)
-    y = quant_data[data_cols].to_numpy().astype('float')
+    y = quant_data[data_cols].to_numpy().astype("float")
     # @ToDo make sure that columns are sorted correctly!!!
     X = np.array(annotation[covariates])
 
     # standardize X:
     X_scaled = StandardScaler().fit_transform(X)
 
     num_cores = multiprocessing.cpu_count()
-    res_list = Parallel(n_jobs=num_cores-1)(delayed(get_res_parallel)(y_i=y_i, X=X_scaled, s0=s0) for y_i in y)
+    res_list = Parallel(n_jobs=num_cores - 1)(
+        delayed(get_res_parallel)(y_i=y_i, X=X_scaled, s0=s0) for y_i in y
+    )
 
     t_limit_dict = {}
 
     for test_index in np.arange(0, len(covariates)):
         test_covariate = covariates[test_index]
         print(test_covariate)
-        X_rand = permutate_multi_vars(X_scaled, rand_index=test_index, n_rand=n_permutations, seed=seed)
-        res_perm_list = Parallel(n_jobs=num_cores-1)(delayed(get_perm_res_parallel)(y_i=y_i, X_rand=X_rand, s0=s0) for y_i in y)
+        X_rand = permutate_multi_vars(
+            X_scaled, rand_index=test_index, n_rand=n_permutations, seed=seed
+        )
+        res_perm_list = Parallel(n_jobs=num_cores - 1)(
+            delayed(get_perm_res_parallel)(y_i=y_i, X_rand=X_rand, s0=s0) for y_i in y
+        )
 
         i = test_index + 1
         res_i = [r.iloc[[i]] for r in res_list]
         res_i = pd.concat(res_i)
 
         # get tvals_s0 list of permutations for covariate i
         res_i_rand = [[0] * len(res_perm_list) for i in range(len(res_perm_list[0]))]
-        for a in np.arange(0,len(res_perm_list)):
+        for a in np.arange(0, len(res_perm_list)):
             for b in np.arange(0, len(res_perm_list[a])):
-                #print(res_perm_list[a][b][3])
+                # print(res_perm_list[a][b][3])
                 res_i_rand[b][a] = res_perm_list[a][b][4][i]
 
         res_i_rand = [list(np.sort(np.abs(r))) for r in res_i_rand]
         fdr_d_i = get_fdr_stats_across_deltas(res_real=res_i, res_perm=res_i_rand)
         res_i = annotate_fdr_significance(res_real=res_i, stats=fdr_d_i, fdr=fdr)
         t_limit_i = get_tstat_limit(stats=fdr_d_i, fdr=fdr)
         t_limit_dict[test_covariate] = t_limit_i
 
         # @ToDo: This multiple testing should potentially be done across all covariates together?
-        res_i['qval_BH'] = multipletests(res_i.pval, method='fdr_bh')[1]
-        res_i['BH_FDR ' + str(int(fdr*100)) + '%'] = ["sig" if abs(x)<=fdr else "non_sig" for x in res_i["qval_BH"]]
-        res_i['qval_BH_s0'] = multipletests(res_i.pval_s0, method='fdr_bh')[1]
-        res_i['BH_FDR_s0 ' + str(int(fdr*100)) + '%'] = ["sig" if abs(x)<=fdr else "non_sig" for x in res_i["qval_BH_s0"]]
+        res_i["qval_BH"] = multipletests(res_i.pval, method="fdr_bh")[1]
+        res_i["BH_FDR " + str(int(fdr * 100)) + "%"] = [
+            "sig" if abs(x) <= fdr else "non_sig" for x in res_i["qval_BH"]
+        ]
+        res_i["qval_BH_s0"] = multipletests(res_i.pval_s0, method="fdr_bh")[1]
+        res_i["BH_FDR_s0 " + str(int(fdr * 100)) + "%"] = [
+            "sig" if abs(x) <= fdr else "non_sig" for x in res_i["qval_BH_s0"]
+        ]
 
         res_i = res_i.add_prefix(covariates[test_index] + "_")
 
-        quant_data = pd.concat([quant_data.reset_index(drop=True), res_i.reset_index(drop=True)], axis=1)
+        quant_data = pd.concat(
+            [quant_data.reset_index(drop=True), res_i.reset_index(drop=True)], axis=1
+        )
 
     return [quant_data, t_limit_dict]
 
 
-def add_random_covariate(annotation, name='random', n_random=50, seed=42):
+def add_random_covariate(annotation, name="random", n_random=50, seed=42):
     annotation_test = annotation.copy()
     annotation_test.reset_index(drop=True, inplace=True)
     annotation_test[name] = 0
     random.seed(seed)
     rand_true = random.sample(range(0, annotation_test.shape[0]), n_random)
     annotation_test.loc[rand_true, name] = 1
     return annotation_test
 
 
 def plot_evaluate_seed_and_perm(df, covariates):
-    config = {'toImageButtonOptions': {'format': 'svg',
-                                      'filename': 'permutation_test',
-                                      'scale': 1
-                                      }
-             }
+    config = {
+        "toImageButtonOptions": {
+            "format": "svg",
+            "filename": "permutation_test",
+            "scale": 1,
+        }
+    }
     for c in covariates:
-        fig = px.line(df, x="permutations",
-                      y=c,
-                      line_dash="seed",
-                      line_group="seed",
-                      template="simple_white",
-                      color_discrete_sequence=['lightgrey'])
-        fig.update_traces(mode='lines+markers')
+        fig = px.line(
+            df,
+            x="permutations",
+            y=c,
+            line_dash="seed",
+            line_group="seed",
+            template="simple_white",
+            color_discrete_sequence=["lightgrey"],
+        )
+        fig.update_traces(mode="lines+markers")
         fig.update_layout(width=620, height=350)
         fig.show(config=config)
 
 
-def evaluate_seed_and_perm(quant_data,
-                           annotation,
-                           covariates,
-                           perms,
-                           seeds,
-                           sample_column='sample_name',
-                           fdr=0.05,
-                           s0=0.05):
-    resDF = pd.DataFrame({'seed': np.repeat(seeds, len(perms)),
-                          'permutations': np.tile(perms, len(seeds))})
-    resDF[covariates] = pd.DataFrame([np.repeat(0, len(covariates))],
-                                     index=resDF.index)
-
-    for i in np.arange(0,resDF.shape[0]):
-        res, tlim = full_regression_analysis(quant_data=quant_data,
-                                             annotation=annotation,
-                                             covariates=covariates,
-                                             n_permutations=resDF.permutations[i],
-                                             sample_column=sample_column,
-                                             fdr=fdr,
-                                             s0=s0,
-                                             seed=resDF.seed[i])
+def evaluate_seed_and_perm(
+    quant_data,
+    annotation,
+    covariates,
+    perms,
+    seeds,
+    sample_column="sample_name",
+    fdr=0.05,
+    s0=0.05,
+):
+    resDF = pd.DataFrame(
+        {
+            "seed": np.repeat(seeds, len(perms)),
+            "permutations": np.tile(perms, len(seeds)),
+        }
+    )
+    resDF[covariates] = pd.DataFrame([np.repeat(0, len(covariates))], index=resDF.index)
+
+    for i in np.arange(0, resDF.shape[0]):
+        res, tlim = full_regression_analysis(
+            quant_data=quant_data,
+            annotation=annotation,
+            covariates=covariates,
+            n_permutations=resDF.permutations[i],
+            sample_column=sample_column,
+            fdr=fdr,
+            s0=s0,
+            seed=resDF.seed[i],
+        )
 
         for c in covariates:
-            resDF.loc[i,c] = res[res[c + "_FDR " + str(int(fdr*100)) + "%"] == "sig"].shape[0]
+            resDF.loc[i, c] = res[
+                res[c + "_FDR " + str(int(fdr * 100)) + "%"] == "sig"
+            ].shape[0]
     plot_evaluate_seed_and_perm(resDF, covariates=covariates)
     return resDF
 
 
 def plot_evaluate_s0s(df, covariates):
     for c in covariates:
-        fig = px.line(df, x="s0", y=c, title=c, template="simple_white", color_discrete_sequence=['lightgrey'])
-        fig.update_traces(mode='lines+markers')
+        fig = px.line(
+            df,
+            x="s0",
+            y=c,
+            title=c,
+            template="simple_white",
+            color_discrete_sequence=["lightgrey"],
+        )
+        fig.update_traces(mode="lines+markers")
         fig.update_layout(width=800, height=500)
         fig.show()
 
 
-def evaluate_s0s(quant_data,
-                           annotation,
-                           covariates,
-                           s0s,
-                           sample_column='sample_name',
-                           n_permutations=5,
-                           seed=42,
-                           fdr=0.01):
-    resDF = pd.DataFrame({'s0':s0s})
+def evaluate_s0s(
+    quant_data,
+    annotation,
+    covariates,
+    s0s,
+    sample_column="sample_name",
+    n_permutations=5,
+    seed=42,
+    fdr=0.01,
+):
+    resDF = pd.DataFrame({"s0": s0s})
     resDF[covariates] = pd.DataFrame([np.repeat(0, len(covariates))], index=resDF.index)
 
-    for i in np.arange(0,resDF.shape[0]):
-        res, tlim = full_regression_analysis(quant_data=quant_data,
-                                             annotation=annotation,
-                                             covariates=covariates,
-                                             sample_column=sample_column,
-                                             n_permutations=n_permutations,
-                                             fdr=fdr,
-                                             s0=resDF.s0[i],
-                                             seed=seed)
+    for i in np.arange(0, resDF.shape[0]):
+        res, tlim = full_regression_analysis(
+            quant_data=quant_data,
+            annotation=annotation,
+            covariates=covariates,
+            sample_column=sample_column,
+            n_permutations=n_permutations,
+            fdr=fdr,
+            s0=resDF.s0[i],
+            seed=seed,
+        )
 
         for c in covariates:
-            resDF.loc[i,c] = res[res[c + "_FDR " + str(int(fdr*100)) + "%"] == "sig"].shape[0]
+            resDF.loc[i, c] = res[
+                res[c + "_FDR " + str(int(fdr * 100)) + "%"] == "sig"
+            ].shape[0]
 
     plot_evaluate_s0s(resDF, covariates=covariates)
 
     return resDF
 
 
-def plot_pval_dist(df, covariates, mode='separate'):
-    config = {'toImageButtonOptions': {'format': 'svg',
-                                       'filename': 'pvalue_histogram',
-                                       'scale': 1
-                                      }
-             }
-    if (mode == 'separate'):
+def plot_pval_dist(df, covariates, mode="separate"):
+    config = {
+        "toImageButtonOptions": {
+            "format": "svg",
+            "filename": "pvalue_histogram",
+            "scale": 1,
+        }
+    }
+    if mode == "separate":
         for c in covariates:
-            fig = px.histogram(df,
-                               x=c+"_pval",
-                               title=c,
-                               nbins=50,
-                               template='simple_white',
-                               color_discrete_sequence=['lightgrey'])
+            fig = px.histogram(
+                df,
+                x=c + "_pval",
+                title=c,
+                nbins=50,
+                template="simple_white",
+                color_discrete_sequence=["lightgrey"],
+            )
             fig.update_layout(width=400, height=300)
             fig.show(config=config)
-    elif (mode == 'joined'):
+    elif mode == "joined":
         df_cov = pd.DataFrame()
         for c in covariates:
-            df_c = pd.DataFrame({'p-value': df[c+"_pval"], 'covariate': c})
+            df_c = pd.DataFrame({"p-value": df[c + "_pval"], "covariate": c})
             df_cov = pd.concat([df_cov, df_c])
-        fig = px.histogram(df_cov, x='p-value',
-                           color='covariate',
-                           barmode='overlay',
-                           opacity=0.6,
-                           nbins=50,
-                           template='simple_white')
+        fig = px.histogram(
+            df_cov,
+            x="p-value",
+            color="covariate",
+            barmode="overlay",
+            opacity=0.6,
+            nbins=50,
+            template="simple_white",
+        )
         fig.update_layout(width=620, height=350)
         fig.show(config=config)
     else:
-        raise ValueError("The mode parameter needs to be either 'separate' or 'joined'.")
+        raise ValueError(
+            "The mode parameter needs to be either 'separate' or 'joined'."
+        )
 
 
 def plot_beta_dist(df, covariates):
     for c in covariates:
-        fig = px.histogram(df, x=c+"_fc", title=c, template='simple_white', color_discrete_sequence=['lightgrey'])
+        fig = px.histogram(
+            df,
+            x=c + "_fc",
+            title=c,
+            template="simple_white",
+            color_discrete_sequence=["lightgrey"],
+        )
         fig.update_layout(width=800, height=500)
         fig.show()
 
 
 def get_replacement_vals(df, threshold, mean_all, sd_all, ds_f):
     """
     Helper function for missing value imputation.
     """
     if df.percent_valid_vals == 100:
         # print(100)
         rep = []
     elif df.percent_valid_vals > threshold:
         # print(70)
-        rep = np.random.normal(df.int_mean-(ds_f*df.int_sd), df.int_sd, df.invalid_vals)
+        rep = np.random.normal(
+            df.int_mean - (ds_f * df.int_sd), df.int_sd, df.invalid_vals
+        )
     else:
         # print(0)
-        rep = np.random.normal(mean_all-(ds_f*sd_all), sd_all, df.invalid_vals)
-    return(rep)
+        rep = np.random.normal(mean_all - (ds_f * sd_all), sd_all, df.invalid_vals)
+    return rep
+
 
-def impute_missing_values(data, percent_impute=20, percent_self_impute=70, downshift_factor=1.8):
+def impute_missing_values(
+    data, percent_impute=20, percent_self_impute=70, downshift_factor=1.8
+):
     """
     Function for missing value imputation. Proteins with less than
     'percent_impute' valid values are removed.
     For proteins with less than 'percent_self_impute' valid values, global mean
     and sd values are used for imputation.
     For proteins with more than 'percent_self_impute' valid values, mean and sd
     values for each specific protein are used.
     The 'downshift_factor' determines by how many standard deviations the mean
     of the imputed distribution is shifted.
     """
 
-    data['int_mean'] = data.filter(regex=("Quantity")).mean(axis=1)
-    data['int_sd'] = data.filter(regex=("Quantity")).std(axis=1)
-    data['valid_vals'] = data.filter(regex=("Quantity")).count(axis=1)
-    data['invalid_vals'] = data.filter(regex=("Quantity")).shape[1]-data.filter(regex=("Quantity")).count(axis=1)
-    data['percent_valid_vals'] = 100/data.filter(regex=("Quantity")).shape[1]*data['valid_vals']
+    data["int_mean"] = data.filter(regex=("Quantity")).mean(axis=1)
+    data["int_sd"] = data.filter(regex=("Quantity")).std(axis=1)
+    data["valid_vals"] = data.filter(regex=("Quantity")).count(axis=1)
+    data["invalid_vals"] = data.filter(regex=("Quantity")).shape[1] - data.filter(
+        regex=("Quantity")
+    ).count(axis=1)
+    data["percent_valid_vals"] = (
+        100 / data.filter(regex=("Quantity")).shape[1] * data["valid_vals"]
+    )
 
     data = data[data.percent_valid_vals >= percent_impute]
 
     overall_mean = np.mean(data.int_mean)
     overall_sd = np.mean(data.int_sd)
 
     nan_idx = np.where(data.isna())
 
-    replacement = data.apply(get_replacement_vals, threshold=percent_self_impute, mean_all=overall_mean, sd_all=overall_sd, ds_f = downshift_factor, axis=1)
+    replacement = data.apply(
+        get_replacement_vals,
+        threshold=percent_self_impute,
+        mean_all=overall_mean,
+        sd_all=overall_sd,
+        ds_f=downshift_factor,
+        axis=1,
+    )
     replacement = [val for sublist in replacement for val in sublist]
 
     for i in np.arange(0, len(nan_idx[0])):
         data.iloc[nan_idx[0][i], nan_idx[1][i]] = replacement[i]
 
     return data
```

### Comparing `alphastats-0.6.2/alphastats/plots/ClusterMap.py` & `alphastats-0.6.3/alphastats/plots/ClusterMap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from alphastats.plots.PlotUtils import PlotUtils, seaborn_object
 
 import seaborn as sns
 import random
 
 
 class ClusterMap(PlotUtils):
-    def __init__(
-        self,
-        dataset,
-        label_bar,
-        only_significant,
-        group,
-        subgroups
-        ):
+    def __init__(self, dataset, label_bar, only_significant, group, subgroups):
         self.dataset = dataset
         self.label_bar = label_bar
         self.only_significant = only_significant
         self.group = group
         self.subgroups = subgroups
 
         self._prepare_df()
         self._plot()
 
-
     def _prepare_df(self):
         df = self.dataset.mat.loc[:, (self.dataset.mat != 0).any(axis=0)]
 
         if self.group is not None and self.subgroups is not None:
             metadata_df = self.dataset.metadata[
-                self.dataset.metadata[self.group].isin(self.subgroups + [self.dataset.sample])
+                self.dataset.metadata[self.group].isin(
+                    self.subgroups + [self.dataset.sample]
+                )
             ]
             samples = metadata_df[self.dataset.sample]
             df = df.filter(items=samples, axis=0)
 
         else:
             metadata_df = self.dataset.metadata
 
@@ -40,40 +34,39 @@
             anova_df = self.dataset.anova(column=self.group, tukey=False)
             significant_proteins = anova_df[anova_df["ANOVA_pvalue"] < 0.05][
                 self.dataset.index_column
             ].to_list()
             df = df[significant_proteins]
 
         if self.label_bar is not None:
-            self._create_label_bar(
-               metadata_df
-            )
+            self._create_label_bar(metadata_df)
 
-        self.prepared_df = self.dataset.mat.loc[:, (self.dataset.mat != 0).any(axis=0)].transpose()
-  
+        self.prepared_df = self.dataset.mat.loc[
+            :, (self.dataset.mat != 0).any(axis=0)
+        ].transpose()
 
     def _plot(self):
         fig = sns.clustermap(self.prepared_df, col_colors=self.label_bar)
 
         if self.label_bar is not None:
-           fig = self._add_label_bar(fig)
+            fig = self._add_label_bar(fig)
 
         # set attributes
         setattr(fig, "plotting_data", self.prepared_df)
         setattr(fig, "preprocessing", self.dataset.preprocessing_info)
         setattr(fig, "method", "clustermap")
 
         self.plot = fig
 
     def _add_label_bar(self, fig):
         for label in self.s.unique():
-                fig.ax_col_dendrogram.bar(
-                    0, 0, color=self.lut[label], label=label, linewidth=0
-                )
-                fig.ax_col_dendrogram.legend(loc="center", ncol=6)
+            fig.ax_col_dendrogram.bar(
+                0, 0, color=self.lut[label], label=label, linewidth=0
+            )
+            fig.ax_col_dendrogram.legend(loc="center", ncol=6)
         return fig
 
     def _create_label_bar(self, metadata_df):
         colorway = [
             "#009599",
             "#005358",
             "#772173",
@@ -84,9 +77,7 @@
         ]
 
         self.s = metadata_df[self.label_bar]
         su = self.s.unique()
         colors = sns.light_palette(random.choice(colorway), len(su))
         self.lut = dict(zip(su, colors))
         self.label_bar = self.s.map(self.lut)
-
-
```

### Comparing `alphastats-0.6.2/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.3/alphastats/plots/DimensionalityReduction.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,20 +106,20 @@
         self.labels = {
             "0": "Dimension 1",
             "1": "Dimension 2",
         }
 
     def _umap(self):
 
-        # TODO umap import is reallly buggy 
+        # TODO umap import is reallly buggy
         try:
             import umap.umap_ as umap
         except ModuleNotFoundError:
             import umap
-        
+
         umap_2d = umap.UMAP(n_components=2, init="random", random_state=0)
         self.components = umap_2d.fit_transform(self.prepared_df)
         self.labels = {
             "0": "",
             "1": "",
         }
 
@@ -148,15 +148,15 @@
 
         #  save plotting data in figure object
         fig = plotly_object(fig)
         fig = self._update_figure_attributes(
             figure_object=fig,
             plotting_data=pd.DataFrame(components),
             method=self.method,
-            preprocessing_info=self.dataset.preprocessing_info
+            preprocessing_info=self.dataset.preprocessing_info,
         )
 
         # draw circles around plotted groups
         if self.circle is True and self.group is not None:
             fig = self._add_circles_to_scatterplot(fig)
 
         if self.group:
```

### Comparing `alphastats-0.6.2/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.3/alphastats/plots/IntensityPlot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import logging
 import scipy
 import numpy as np
 import plotly.graph_objects as go
 import plotly.express as px
 import plotly
 
@@ -26,15 +25,16 @@
     )
 )
 
 plotly.io.templates.default = "simple_white+alphastats_colors"
 
 
 class IntensityPlot(PlotUtils):
-    def __init__(self,
+    def __init__(
+        self,
         dataset,
         protein_id,
         group,
         subgroups,
         method,
         add_significance,
         log_scale,
@@ -45,15 +45,14 @@
         self.subgroups = subgroups
         self.method = method
         self.add_significance = add_significance
         self.log_scale = log_scale
 
         self._prepare_data()
         self._plot()
- 
 
     @staticmethod
     def _add_significance(plot):
         # add sginficance pvalue, and stars to pairwise intensity plot
         plot_dict = plot.to_plotly_json()
         data = plot_dict.get("data")
 
@@ -69,21 +68,21 @@
         pvalue = scipy.stats.ttest_ind(y_array1, y_array2).pvalue
 
         pvalue_text = "<i>p=" + str(round(pvalue, 4)) + "</i>"
 
         if pvalue < 0.001:
             significance_level = "***"
             pvalue_text = "<i>p<0.001</i>"
-        
+
         elif pvalue < 0.01:
             significance_level = "**"
-       
+
         elif pvalue < 0.05:
             significance_level = "*"
-       
+
         else:
             significance_level = "-"
 
         y_max = np.concatenate((y_array1, y_array2)).max()
         # add connecting bar for pvalue
         plot.add_trace(
             go.Scatter(
@@ -117,24 +116,32 @@
             y=1.002,
             showarrow=False,
             font=dict(size=12, color="black"),
         )
 
         plot.update_layout(width=600, height=700)
         return plot
-    
+
     def _prepare_data(self):
         #  TODO use difflib to find similar ProteinId if ProteinGroup is not present
-        df = self.dataset.mat[[self.protein_id]].reset_index().rename(columns={"index": self.dataset.sample})
+        df = (
+            self.dataset.mat[[self.protein_id]]
+            .reset_index()
+            .rename(columns={"index": self.dataset.sample})
+        )
         df = df.merge(self.dataset.metadata, how="inner", on=[self.dataset.sample])
 
         if self.subgroups is not None:
             df = df[df[self.group].isin(self.subgroups)]
 
-        self.y_label = self.protein_id + " - " + self.dataset.intensity_column.replace("[sample]", "")
+        self.y_label = (
+            self.protein_id
+            + " - "
+            + self.dataset.intensity_column.replace("[sample]", "")
+        )
         self.prepared_df = df
 
     def _plot(self):
         if self.method == "violin":
             fig = px.violin(
                 self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
                 template="simple_white+alphastats_colors"
@@ -168,13 +175,14 @@
             fig.update_layout(yaxis=dict(type="log"))
 
         if self.add_significance:
             fig = self._add_significance(fig)
 
         fig = plotly_object(fig)
         fig = self._update_figure_attributes(
-            figure_object=fig, plotting_data= self.prepared_df, preprocessing_info=self.dataset.preprocessing_info,  method=self.method
+            figure_object=fig,
+            plotting_data=self.prepared_df,
+            preprocessing_info=self.dataset.preprocessing_info,
+            method=self.method,
         )
 
         self.plot = fig
-
-
```

### Comparing `alphastats-0.6.2/alphastats/plots/PlotUtils.py` & `alphastats-0.6.3/alphastats/plots/PlotUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import plotly
 import seaborn as sns
 import plotly.graph_objects as go
 
+
 plotly.io.templates["alphastats_colors"] = plotly.graph_objects.layout.Template(
     layout=plotly.graph_objects.Layout(
         paper_bgcolor="rgba(0,0,0,0)",
         plot_bgcolor="rgba(0,0,0,0)",
         colorway=[
             "#009599",
             "#005358",
@@ -18,14 +19,15 @@
             "#A87F32",
         ],
     )
 )
 
 plotly.io.templates.default = "simple_white+alphastats_colors"
 
+
 class PlotUtils:
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def _update_colors_plotly(fig, color_dict):
         # plotly doesnt allow to assign color to certain group
@@ -36,15 +38,17 @@
         for count, group in enumerate(data_dict_list):
             group_variable = group.get("legendgroup")
             group_color = color_dict.get(group_variable)
             fig_dict["data"][count]["marker"]["color"] = group_color
         # convert dict back to plotly figure
         return go.Figure(fig_dict)
 
-    def _update_figure_attributes(self, figure_object, plotting_data, preprocessing_info, method=None):
+    def _update_figure_attributes(
+        self, figure_object, plotting_data, preprocessing_info, method=None
+    ):
         setattr(figure_object, "plotting_data", plotting_data)
         setattr(figure_object, "preprocessing", preprocessing_info)
         setattr(figure_object, "method", method)
         return figure_object
 
 
 class plotly_object(plotly.graph_objs._figure.Figure):
```

### Comparing `alphastats-0.6.2/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.3/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.3/alphastats/plots/VolcanoPlot.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.draw_line = draw_line
         self.hover_data = None
         self.res = None
         self.pvalue_column = None
         self.perm=perm
         self.color_list = color_list
         self._check_input()
-       
+
         if plot:
             self._perform_differential_expression_analysis()
             self._annotate_result_df()
             self._add_hover_data_columns()
             self._plot()
 
     def _check_input(self):
@@ -74,16 +74,16 @@
                 "Column containing group1 and group2 needs to be specified"
             )
 
     def _update(self, updated_attributes):
         """
         update attributes using dict
         """
-        for key,value in updated_attributes.items():
-            setattr(self,key,value)
+        for key, value in updated_attributes.items():
+            setattr(self, key, value)
 
     @ignore_warning(UserWarning)
     @ignore_warning(RuntimeWarning)
     def _perform_differential_expression_analysis(self):
         """
         wrapper for diff analysis
         """
@@ -100,74 +100,102 @@
             self._welch_ttest()
         
         elif self.method == "paired-ttest":
             self._pairedttest()
         
         elif self.method == "sam":
             self._sam()
-        
-        # elif self.method == "Multi Covariates":
-        #    raise NotImplementedError
 
         else:
             raise ValueError(
                 f"{self.method} is not available."
-                + "Please select from 'ttest', 'sam' or 'anova' for anova with follow up tukey or 'wald' for wald-test."
+                + "Please select from 'ttest', 'sam', 'paired-ttest' or 'anova' for anova with follow up tukey or 'wald' for wald-test."
             )
 
     @lru_cache(maxsize=20)
     def _sam_calculate_fdr_line(self):
         from alphastats.multicova import multicova
 
-        self.fdr_line= multicova.get_fdr_line(
-                t_limit=self.tlim_ttest,
-                s0=0.05,
-                n_x=len(list(self.dataset.metadata[self.dataset.metadata[self.column]==self.group1][self.dataset.sample])),
-                n_y=len(list(self.dataset.metadata[self.dataset.metadata[self.column]==self.group2][self.dataset.sample])),
-                fc_s = np.arange(0,np.max(np.abs(self.res.log2fc)),np.max(np.abs(self.res.log2fc))/200),
-                s_s = np.arange(0.005, 6, 0.0025),
-                plot=False
-            )
-    
+        self.fdr_line = multicova.get_fdr_line(
+            t_limit=self.tlim_ttest,
+            s0=0.05,
+            n_x=len(
+                list(
+                    self.dataset.metadata[
+                        self.dataset.metadata[self.column] == self.group1
+                    ][self.dataset.sample]
+                )
+            ),
+            n_y=len(
+                list(
+                    self.dataset.metadata[
+                        self.dataset.metadata[self.column] == self.group2
+                    ][self.dataset.sample]
+                )
+            ),
+            fc_s=np.arange(
+                0,
+                np.max(np.abs(self.res.log2fc)),
+                np.max(np.abs(self.res.log2fc)) / 200,
+            ),
+            s_s=np.arange(0.005, 6, 0.0025),
+            plot=False,
+        )
+
     @lru_cache(maxsize=20)
     def _sam(self):
         from alphastats.multicova import multicova
 
-        print(
-            "Calculating t-test and permuation based FDR (SAM)... "
-        )
+        print("Calculating t-test and permuation based FDR (SAM)... ")
 
         transposed = self.dataset.mat.transpose()
 
         if self.dataset.preprocessing_info["Normalization"] is None:
-             # needs to be lpog2 transformed for fold change calculations
+            # needs to be lpog2 transformed for fold change calculations
             transposed = transposed.transform(lambda x: np.log2(x))
 
         transposed[self.dataset.index_column] = transposed.index
         transposed = transposed.reset_index(drop=True)
 
         res_ttest, tlim_ttest = multicova.perform_ttest_analysis(
             transposed,
-            c1 =list(self.dataset.metadata[self.dataset.metadata[self.column]==self.group1][self.dataset.sample]),                                      
-            c2 =list(self.dataset.metadata[self.dataset.metadata[self.column]==self.group2][self.dataset.sample]), 
-            s0=0.05, 
+            c1=list(
+                self.dataset.metadata[
+                    self.dataset.metadata[self.column] == self.group1
+                ][self.dataset.sample]
+            ),
+            c2=list(
+                self.dataset.metadata[
+                    self.dataset.metadata[self.column] == self.group2
+                ][self.dataset.sample]
+            ),
+            s0=0.05,
             n_perm=self.perm,
             fdr=self.fdr,
             id_col=self.dataset.index_column,
-            parallelize=True
+            parallelize=True,
         )
-        
-        fdr_column = "FDR"  + str(int(self.fdr*100)) + "%"
-        self.res = res_ttest[[self.dataset.index_column, 'fc', 'tval', 'pval', 'tval_s0', 'pval_s0', 'qval']]
+
+        fdr_column = "FDR" + str(int(self.fdr * 100)) + "%"
+        self.res = res_ttest[
+            [
+                self.dataset.index_column,
+                "fc",
+                "tval",
+                "pval",
+                "tval_s0",
+                "pval_s0",
+                "qval",
+            ]
+        ]
         self.res["log2fc"] = res_ttest["fc"]
         self.res["FDR"] = res_ttest[fdr_column]
         self.tlim_ttest = tlim_ttest
         self.pvalue_column = "pval"
 
-
     @lru_cache(maxsize=20)
     def _wald(self):
 
         print(
             "Calculating differential expression analysis using wald test. Fitting generalized linear model..."
         )
         self.res = self.dataset.diff_expression_analysis(
@@ -231,72 +259,80 @@
         ][self.dataset.sample].tolist()
 
         group2_samples = self.dataset.metadata[
             self.dataset.metadata[self.column] == self.group2
         ][self.dataset.sample].tolist()
 
         mat_transpose = self.dataset.mat.transpose()
-        fc = self.dataset._calculate_foldchange(mat_transpose, group1_samples, group2_samples)
+        fc = self.dataset._calculate_foldchange(
+            mat_transpose, group1_samples, group2_samples
+        )
 
         #  check how column is ordered
         self.pvalue_column = self.group1 + " vs. " + self.group2 + " Tukey Test"
 
         if self.pvalue_column not in result_df.columns:
             self.pvalue_column = self.group2 + " vs. " + self.group1 + " Tukey Test"
 
-        self.res = result_df.reset_index().merge(fc.reset_index(), on=self.dataset.index_column)
+        self.res = result_df.reset_index().merge(
+            fc.reset_index(), on=self.dataset.index_column
+        )
 
     def _add_hover_data_columns(self):
         # additional labeling with gene names
         self.hover_data = [self.dataset.index_column]
 
         if self.dataset.gene_names is not None:
             self.res = pd.merge(
                 self.res,
-                self.dataset.rawinput[[self.dataset.gene_names, self.dataset.index_column]],
+                self.dataset.rawinput[
+                    [self.dataset.gene_names, self.dataset.index_column]
+                ],
                 on=self.dataset.index_column,
                 how="left",
             )
             self.hover_data.append(self.dataset.gene_names)
 
-
     def _annotate_result_df(self):
         """
         convert pvalue to log10
         add color labels for up and down regulates
         """
         self.res = self.res[(self.res["log2fc"] < 20) & (self.res["log2fc"] > -20)]
         self.res["-log10(p-value)"] = -np.log10(self.res[self.pvalue_column])
-        
+
         self.alpha = -np.log10(self.alpha)
         # add color variable to plot
 
         if self.method != "sam":
-        
+
             condition = [
-                (self.res["log2fc"] < -self.min_fc) & (self.res["-log10(p-value)"] > self.alpha),
-                (self.res["log2fc"] > self.min_fc) & (self.res["-log10(p-value)"] > self.alpha),
+                (self.res["log2fc"] < -self.min_fc)
+                & (self.res["-log10(p-value)"] > self.alpha),
+                (self.res["log2fc"] > self.min_fc)
+                & (self.res["-log10(p-value)"] > self.alpha),
             ]
 
         else:
 
             condition = [
                 (self.res["log2fc"] < 0) & (self.res["FDR"] == "sig"),
                 (self.res["log2fc"] > 0) & (self.res["FDR"] == "sig"),
             ]
 
-
         value = ["down", "up"]
+
         self.res["color"] = np.select(condition, value, default="non_sig")   
 
         if len(self.color_list) > 0:
             self.res["color"] = np.where(self.res[self.dataset.index_column].isin(self.color_list), 
                                           "color", "no_color")   
         
 
+
     def _add_labels_plot(self):
         """
         add gene names as hover data if they are given
         """
 
         if self.dataset.gene_names is not None:
             label_column = self.dataset.gene_names
@@ -333,71 +369,71 @@
         )
 
     def _draw_fdr_line(self):
         """
         Draw fdr line if SAM was applied
         """
         self._sam_calculate_fdr_line()
-        
-        self.plot.add_trace(go.Scatter(
-            x=self.fdr_line[self.fdr_line.fc_s > 0].fc_s,
-            y=-np.log10(self.fdr_line[self.fdr_line.fc_s > 0].pvals),
-            line_color="black",
-            line_shape='spline',
-            showlegend=False)
-        )
-        self.plot.add_trace(go.Scatter(
-            x=self.fdr_line[self.fdr_line.fc_s < 0].fc_s,
-            y=-np.log10(self.fdr_line[self.fdr_line.fc_s < 0].pvals),
-            line_color="black",
-            line_shape='spline',
-            showlegend=False)
+
+        self.plot.add_trace(
+            go.Scatter(
+                x=self.fdr_line[self.fdr_line.fc_s > 0].fc_s,
+                y=-np.log10(self.fdr_line[self.fdr_line.fc_s > 0].pvals),
+                line_color="black",
+                line_shape="spline",
+                showlegend=False,
+            )
+        )
+        self.plot.add_trace(
+            go.Scatter(
+                x=self.fdr_line[self.fdr_line.fc_s < 0].fc_s,
+                y=-np.log10(self.fdr_line[self.fdr_line.fc_s < 0].pvals),
+                line_color="black",
+                line_shape="spline",
+                showlegend=False,
+            )
         )
     
     def _color_data_points(self):
          # update coloring
         if len(self.color_list) == 0:
             color_dict = {"non_sig": "#404040", "up": "#B65EAF", "down": "#009599"}
     
         else:
             color_dict = {"no_color": "#404040", "color": "#B65EAF"}
         
         self.plot = self._update_colors_plotly(self.plot, color_dict=color_dict)
 
 
-
     def _plot(self):
         self.plot = px.scatter(
             self.res,
             x="log2fc",
             y="-log10(p-value)",
             color="color",
             hover_data=self.hover_data,
             template= "simple_white+alphastats_colors"
         )
-        
+
         # update coloring
         self._color_data_points()
 
         if self.labels:
             self._add_labels_plot()
-        
+
         if self.draw_line:
             if self.method == "sam":
                 self._draw_fdr_line()
             else:
                 self._draw_lines_plot()
 
         self.plot.update_layout(showlegend=False)
         self.plot.update_layout(width=600, height=700)
 
         #  save plotting data in figure object
         self.plot = plotly_object(self.plot)
         self.plot = self._update_figure_attributes(
-            figure_object=self.plot, 
-            plotting_data=self.res, 
-            preprocessing_info=self.dataset.preprocessing_info, 
-            method=self.method
+            figure_object=self.plot,
+            plotting_data=self.res,
+            preprocessing_info=self.dataset.preprocessing_info,
+            method=self.method,
         )
-    
-
-
```

### Comparing `alphastats-0.6.2/alphastats/statistics/Anova.py` & `alphastats-0.6.3/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.3/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.2/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.3/alphastats/statistics/StatisticUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as no
+
 class StatisticUtils:
     def __init__(self) -> None:
         pass
     
     def _add_metadata_column(self, group1_list: list, group2_list: list):
 
         # create new column in metadata with defined groups
```

### Comparing `alphastats-0.6.2/alphastats/utils.py` & `alphastats-0.6.3/alphastats/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,27 @@
     def inner(*args, **kwargs):
         if args[0].empty is True:
             raise ValueError("DataFrame is empty. No significant GO-terms found.")
         return f(*args, **kwargs)
 
     return inner
 
+
 def list_to_tuple(function):
     """
     list are not hashable not suitable for caching 
     convert to tuple
     """
+
     def wrapper(*args):
         args = [tuple(x) if type(x) == list else x for x in args]
         result = function(*args)
         result = tuple(result) if type(result) == list else result
         return result
+
     return wrapper
 
 def find_duplicates_in_list(l:list) -> list:
     """Find duplicates in a list
 
     Args:
         l (list): list
@@ -95,8 +98,8 @@
     duplicates = []
     ys = sorted(l)
 
     for n in range(1, len(l)):
         if ys[n] == ys[n-1]:
             duplicates.append(ys[n])
     return duplicates
-    
+
```

### Comparing `alphastats-0.6.2/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.3/alphastats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.2
+Version: 0.6.3
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
```

### Comparing `alphastats-0.6.2/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.3/alphastats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 alphastats/gui/utils/options.py
 alphastats/gui/utils/software_options.py
 alphastats/gui/utils/ui_helper.py
 alphastats/loader/AlphaPeptLoader.py
 alphastats/loader/BaseLoader.py
 alphastats/loader/DIANNLoader.py
 alphastats/loader/FragPipeLoader.py
+alphastats/loader/GenericLoader.py
 alphastats/loader/MaxQuantLoader.py
 alphastats/loader/SpectronautLoader.py
 alphastats/loader/__init__.py
 alphastats/loader/mzTabLoader.py
 alphastats/multicova/__init__.py
 alphastats/multicova/multicova.py
 alphastats/plots/ClusterMap.py
```

### Comparing `alphastats-0.6.2/setup.py` & `alphastats-0.6.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 def get_long_description():
     with open("README.md", "r") as readme_file:
         long_description = readme_file.read()
     return long_description
 
 
 def get_requirements():
-    with open('requirements.txt') as f:
+    with open("requirements.txt") as f:
         required = f.read().splitlines()
     return required
-    
+
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.6.2",
+        version="0.6.3",
         license="Apache",
         description="An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@gmail.com",
         url="https://github.com/MannLabs/alphastats",
@@ -52,24 +52,24 @@
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
             "Programming Language :: Python :: 3",
             "Topic :: Scientific/Engineering :: Bio-Informatics",
         ],
         packages=[
-            "alphastats", 
-            "alphastats.plots", 
+            "alphastats",
+            "alphastats.plots",
             "alphastats.multicova",
-            "alphastats.gui", 
-            "alphastats.data", 
+            "alphastats.gui",
+            "alphastats.data",
             "alphastats.gui.pages",
             "alphastats.gui",
             "alphastats.gui.sample_data",
             "alphastats.gui.utils",
-            "alphastats.loader"
+            "alphastats.loader",
         ],
         include_package_data=True,
         entry_points={"console_scripts": "alphastats=alphastats.gui.gui:run",},
         install_requires=requirements,
         python_requires=">=3.8,<4",
     )
```

### Comparing `alphastats-0.6.2/tests/test_DataSet.py` & `alphastats-0.6.3/tests/test_DataSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 import pandas as pd
 import plotly
 from contextlib import contextmanager
 import shutil
 import os
 import copy
 import dictdiffer
+
 # from pandas.api.types import is_object_dtype, is_numeric_dtype, is_bool_dtype
 
 from alphastats.loader.BaseLoader import BaseLoader
 from alphastats.loader.DIANNLoader import DIANNLoader
 from alphastats.loader.MaxQuantLoader import MaxQuantLoader
 from alphastats.loader.AlphaPeptLoader import AlphaPeptLoader
 from alphastats.loader.FragPipeLoader import FragPipeLoader
 from alphastats.loader.SpectronautLoader import SpectronautLoader
+from alphastats.loader.GenericLoader import GenericLoader
 from alphastats.DataSet import DataSet
 
 from alphastats.DataSet_Statistics import Statistics
 from alphastats.DataSet_Plot import Plot
 from alphastats.utils import LoaderError
 
 
@@ -180,18 +182,18 @@
             self.assertIsInstance(plot, plotly.graph_objects.Figure)
             # convert plotly objec to dict
             plot_dict = plot.to_plotly_json()
             # check if plotly object is not empty
             self.assertEqual(len(plot_dict.get("data")), 1)
             #  check if it is logscale
             self.assertEqual(plot_dict.get("layout").get("yaxis").get("type"), "log")
-        
+
         def test_reset_preprocessing(self):
             self.assertEqual(self.obj.mat.shape, self.matrix_dim)
-            
+
             self.obj.preprocess(remove_contaminations=True)
             self.assertEqual(self.obj.mat.shape, self.matrix_dim_filtered)
 
             self.obj.reset_preprocessing()
             self.assertEqual(self.obj.mat.shape, self.matrix_dim)
 
 
@@ -253,94 +255,94 @@
         sample_list = ["A"]
         self.obj.preprocess(remove_samples=sample_list)
         self.assertEqual(self.obj.mat.shape, (1, 3781))
 
     def test_preprocess_normalize_zscore(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # zscore Normalization
-        self.obj.preprocess(log2_transform=False,normalization="zscore")
+        self.obj.preprocess(log2_transform=False, normalization="zscore")
         expected_mat = pd.DataFrame(
             {
                 "a": [-1.33630621, 1.06904497, 0.26726124],
                 "b": [1.41421356, -0.70710678, -0.70710678],
                 "c": [-1.38873015, 0.9258201, 0.46291005],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_normalize_quantile(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Quantile Normalization
-        self.obj.preprocess(log2_transform=False,normalization="quantile")
+        self.obj.preprocess(log2_transform=False, normalization="quantile")
         expected_mat = pd.DataFrame(
             {"a": [0.0, 1.0, 0.5], "b": [1.0, 0.0, 0.0], "c": [0.0, 1.0, 0.5]}
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_normalize_linear(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Linear Normalization
-        self.obj.preprocess(log2_transform=False,normalization="linear")
+        self.obj.preprocess(log2_transform=False, normalization="linear")
         expected_mat = pd.DataFrame(
             {
                 "a": [0.37139068, 0.42107596, 0.40824829],
                 "b": [0.92847669, 0.33686077, 0.40824829],
                 "c": [0.0, 0.84215192, 0.81649658],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_normalize_vst(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Linear Normalization
-        self.obj.preprocess(log2_transform=False,normalization="vst")
+        self.obj.preprocess(log2_transform=False, normalization="vst")
         expected_mat = pd.DataFrame(
             {
                 "a": [ 3.19059101,  11.591763, 8.365096],
                 "b": [0.084829, 0.084829, 0.084829],
                 "c": [0.000000, 7.850074, 6.435102],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat.round(2), expected_mat.round(2))
 
     def test_preprocess_imputation_mean_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
-        self.obj.preprocess(log2_transform=False,imputation="mean")
+        self.obj.preprocess(log2_transform=False, imputation="mean")
         expected_mat = pd.DataFrame(
             {"a": [2.0, 3.0, 4.0], "b": [5.0, 4.0, 4.0], "c": [10.0, 10.0, 10.0]}
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_imputation_median_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
-        self.obj.preprocess(log2_transform=False,imputation="median")
+        self.obj.preprocess(log2_transform=False, imputation="median")
         expected_mat = pd.DataFrame(
             {"a": [2.0, 3.0, 4.0], "b": [5.0, 4.0, 4.0], "c": [10.0, 10.0, 10.0]}
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_imputation_knn_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
-        self.obj.preprocess(log2_transform=False,imputation="knn")
+        self.obj.preprocess(log2_transform=False, imputation="knn")
         expected_mat = pd.DataFrame(
             {"a": [2.0, 3.0, 4.0], "b": [5.0, 4.0, 4.0], "c": [10.0, 10.0, 10.0]}
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_imputation_randomforest_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
-        self.obj.preprocess(log2_transform=False,imputation="randomforest")
+        self.obj.preprocess(log2_transform=False, imputation="randomforest")
         expected_mat = pd.DataFrame(
             {
                 "a": [2.00000000e00, -9.22337204e12, 4.00000000e00],
                 "b": [5.00000000e00, 4.00000000e00, 4.0],
                 "c": [-9.22337204e12, 1.00000000e01, -9.22337204e12],
             }
         )
@@ -400,26 +402,28 @@
         self.matrix_dim_filtered = (312, 2397)
         self.comparison_column = "disease"
 
     def test_load_evidence_wrong_sample_names(self):
         with self.assertRaises(ValueError):
             loader = MaxQuantLoader(
                 file="testfiles/maxquant/proteinGroups.txt",
-                evidence_file="testfiles/maxquant_go/evidence.txt"
+                evidence_file="testfiles/maxquant_go/evidence.txt",
             )
             DataSet(
-                loader=loader,
-                metadata_path=self.metadata_path,
-                sample_column="sample",
+                loader=loader, metadata_path=self.metadata_path, sample_column="sample",
             )
 
     def test_plot_pca_group(self):
         pca_plot = self.obj.plot_pca(group=self.comparison_column)
         # 5 different disease
         self.assertEqual(len(pca_plot.to_plotly_json().get("data")), 5)
+    
+    def test_data_completeness(self):
+        self.obj.preprocess(log2_transform=False, data_completeness=0.7)
+        self.assertEqual(self.obj.mat.shape[1], 517)
 
     def test_plot_pca_circles(self):
         pca_plot = self.obj.plot_pca(group=self.comparison_column, circle=True)
         # are there 5 circles drawn - for each group
         number_of_groups = len(pca_plot.to_plotly_json().get("layout").get("shapes"))
         self.assertEqual(number_of_groups, 5)
 
@@ -444,24 +448,26 @@
     def test_plot_volcano_with_grouplist_wrong_names(self):
         with self.assertRaises(ValueError):
             self.obj.plot_volcano(
                 method="ttest",
                 group1=["wrong_sample_name", "1_42_D9", "1_57_E8"],
                 group2=["1_71_F10", "1_73_F12"],
             )
-    
+
     def test_plot_volcano_compare_preprocessing_modes(self):
         result_list = self.obj.plot_volcano(
             method="ttest",
             group1=["1_31_C6", "1_32_C7", "1_57_E8"],
             group2=["1_71_F10", "1_73_F12"],
-            compare_preprocessing_modes=True
+            compare_preprocessing_modes=True,
         )
+
         self.assertEqual(len(result_list), 12)               
 
+
     def test_preprocess_subset(self):
         self.obj.preprocess(subset=True, log2_transform=False)
         self.assertEqual(self.obj.mat.shape, (48, 1364))
 
     @patch.object(Statistics, "tukey_test")
     def test_anova_without_tukey(self, mock):
         anova_results = self.obj.anova(column="disease", protein_ids="all", tukey=False)
@@ -501,17 +507,15 @@
         # with one protein id
         protein_id = "A0A024R4J8;Q92876"
         results = self.obj.anova(column="disease", protein_ids=protein_id, tukey=True)
         self.assertEqual(results.shape[1], 10)
 
     def test_tukey_test(self):
         protein_id = "K7ERI9;A0A024R0T8;P02654;K7EJI9;K7ELM9;K7EPF9;K7EKP1"
-        tukey_df = self.obj.tukey_test(
-            protein_id=protein_id, group="disease", df=None
-        )
+        tukey_df = self.obj.tukey_test(protein_id=protein_id, group="disease", df=None)
         self.assertEqual(tukey_df["p-tukey"][0], 0.674989009816342)
 
     def test_ancova(self):
         ancova_df = self.obj.ancova(
             protein_id="K7ERI9;A0A024R0T8;P02654;K7EJI9;K7ELM9;K7EPF9;K7EKP1",
             covar="Triglycerides measurement (14740000)",
             between="disease",
@@ -534,29 +538,34 @@
         #self.assertTrue(n_labels > 20)
 
     def test_plot_volcano_wald(self):
         """
         Volcano Plot with wald test and list of samples
         """
         self.obj.preprocess(imputation="knn")
-        self.obj.plot_volcano(group1 = ["1_31_C6", "1_32_C7", "1_33_C8"],
-                    group2 = ["1_78_G5", "1_77_G4", "1_76_G3"], method="ttest")
+        self.obj.plot_volcano(
+            group1=["1_31_C6", "1_32_C7", "1_33_C8"],
+            group2=["1_78_G5", "1_77_G4", "1_76_G3"],
+            method="ttest",
+        )
 
         column_added = "_comparison_column" in self.obj.metadata.columns.to_list()
-        self.assertTrue(column_added)  
+        self.assertTrue(column_added)
 
     def test_plot_volcano_sam(self):
-        self.obj.preprocess(log2_transform=False, imputation="knn", normalization="zscore")
+        self.obj.preprocess(
+            log2_transform=False, imputation="knn", normalization="zscore"
+        )
         plot = self.obj.plot_volcano(
-            column = "disease",
-            group1="type 2 diabetes mellitus", 
-            group2 ="type 2 diabetes mellitus|non-alcoholic fatty liver disease",
+            column="disease",
+            group1="type 2 diabetes mellitus",
+            group2="type 2 diabetes mellitus|non-alcoholic fatty liver disease",
             method="sam",
-            draw_line =True,
-            perm= 10
+            draw_line=True,
+            perm=10,
         )
 
         # fdr lines get drawn
         line_1 = plot.to_plotly_json()["data"][3].get("line").get("shape")
         line_2 = plot.to_plotly_json()["data"][4].get("line").get("shape")
 
         self.assertEqual(line_1, "spline")
@@ -566,17 +575,17 @@
         self.obj.preprocess(imputation="mean")
         plot = self.obj.plot_volcano( method="ttest",
             group1=["1_31_C6", "1_32_C7", "1_57_E8"],
             group2=["1_71_F10", "1_73_F12"],
             color_list=self.obj.mat.columns.to_list()[0:20])
         self.assertEqual(len(plot.to_plotly_json()["data"][0]["x"]), 20)
 
-
     def test_plot_clustermap_significant(self):
         import sys
+
         sys.setrecursionlimit(100000)
         self.obj.preprocess(imputation="knn")
         plot = self.obj.plot_clustermap(
             label_bar=self.comparison_column,
             only_significant=True,
             group=self.comparison_column,
             subgroups=["healthy", "liver cirrhosis"],
@@ -625,66 +634,84 @@
         with self.assertRaises(ValueError):
             self.obj.diff_expression_analysis(
                 group1="healthy", group2="liver cirrhosis"
             )
 
     def test_diff_expression_analysis_list(self):
         self.obj.diff_expression_analysis(
-            group1 = ["1_31_C6", "1_32_C7", "1_33_C8"],
-            group2 = ["1_78_G5", "1_77_G4", "1_76_G3"], method="ttest")
+            group1=["1_31_C6", "1_32_C7", "1_33_C8"],
+            group2=["1_78_G5", "1_77_G4", "1_76_G3"],
+            method="ttest",
+        )
 
         column_added = "_comparison_column" in self.obj.metadata.columns.to_list()
-        self.assertTrue(column_added)  
+        self.assertTrue(column_added)
 
     def test_plot_intensity_non_sign(self):
         """
         No significant label is added to intensity plot
         """
-        plot = self.obj.plot_intensity(protein_id="S6BAR0", 
-            group="disease", 
+        plot = self.obj.plot_intensity(
+            protein_id="S6BAR0",
+            group="disease",
             subgroups=["liver cirrhosis", "healthy"],
-            add_significance=True)
+            add_significance=True,
+        )
 
-        annotation = plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        annotation = (
+            plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        )
         self.assertEqual(annotation, "-")
 
     def test_plot_intensity_sign(self):
         """
         Significant label * is added to intensity plot
         """
-        plot = self.obj.plot_intensity(protein_id="Q9UL94", 
-            group="disease", 
+        plot = self.obj.plot_intensity(
+            protein_id="Q9UL94",
+            group="disease",
             subgroups=["liver cirrhosis", "healthy"],
-            add_significance=True)
+            add_significance=True,
+        )
 
-        annotation = plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        annotation = (
+            plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        )
         self.assertEqual(annotation, "*")
 
     def test_plot_intensity_sign_01(self):
         """
         Significant label ** is added to intensity plot
         """
-        plot = self.obj.plot_intensity(protein_id="Q96JD0;Q96JD1;P01721", 
-            group="disease", 
+        plot = self.obj.plot_intensity(
+            protein_id="Q96JD0;Q96JD1;P01721",
+            group="disease",
             subgroups=["liver cirrhosis", "healthy"],
-            add_significance=True)
+            add_significance=True,
+        )
 
-        annotation = plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        annotation = (
+            plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        )
         self.assertEqual(annotation, "**")
 
     def test_plot_intensity_sign_001(self):
         """
         Highly significant label is added to intensity plot
         """
-        plot = self.obj.plot_intensity(protein_id="Q9BWP8", 
-            group="disease", 
+        plot = self.obj.plot_intensity(
+            protein_id="Q9BWP8",
+            group="disease",
             subgroups=["liver cirrhosis", "healthy"],
-            add_significance=True)
+            add_significance=True,
+        )
 
-        annotation = plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        annotation = (
+            plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
+        )
         self.assertEqual(annotation, "***")
 
     def test_plot_intensity_all(self):
         plot = self.obj.plot_intensity(protein_id="Q9BWP8", 
             group="disease", 
             subgroups=["liver cirrhosis", "healthy"],
             method="all",
@@ -696,22 +723,36 @@
         fig = self.obj.plot_samplehistograms().to_plotly_json()
         self.assertEqual(312, len(fig["data"]))
     
     def test_batch_correction(self):
         self.obj.preprocess(subset=True, imputation="knn", normalization="quantile")
         self.obj.batch_correction(batch="batch_artifical_added")
         first_value = self.obj.mat.values[0,0]
-        self.assertAlmostEqual(0.0111, first_value, places=2)
-
+        self.assertAlmostEqual(0.0111, first_value, places=2)   
 
+    def test_multicova_analysis(self):
+        self.obj.preprocess(imputation="knn", normalization="zscore", subset=True)
+        res, plot_list = self.obj.multicova_analysis(
+            covariates=["disease", "Alkaline phosphatase measurement"],
+            subset={"disease": ["healthy", "liver cirrhosis"]},
+        )
+        self.assertAlmostEqual(-0.3063, res['disease_fc'].iloc[1], places=2)
         
 
+    def test_multicova_analysis_invalid_covariates(self):
+        self.obj.preprocess(imputation="knn", normalization="zscore", subset=True)
+        res, _ = self.obj.multicova_analysis(
+            covariates=["disease", "Alkaline phosphatase measurement", "Body mass index ", "not here"],
+            subset={"disease": ["healthy", "liver cirrhosis"]},
+        )
+        self.assertEqual(res.shape[1], 45)
+
     # def test_perform_gsea(self):
-    #     df = self.obj.perform_gsea(column="disease", 
-    #                             group1="healthy", 
+    #     df = self.obj.perform_gsea(column="disease",
+    #                             group1="healthy",
     #                                     group2="liver cirrhosis",
     #                                     gene_sets= 'KEGG_2019_Human')
 
     #     cholesterol_enhanced = 'Cholesterol metabolism' in df.index.to_list()
     #     self.assertTrue(cholersterol_enhanced)
 
 
@@ -844,38 +885,80 @@
         self.matrix_dim_filtered = (20, 6)
         self.comparison_column = "grouping1"
 
 
 class TestSpectronautDataSet(BaseTestDataSet.BaseTest):
     @classmethod
     def setUpClass(cls):
-        
+
         if os.path.isfile("testfiles/spectronaut/results.tsv") == False:
-            shutil.unpack_archive("testfiles/spectronaut/results.tsv.zip", "testfiles/spectronaut/")
-        
-        cls.cls_loader = SpectronautLoader(file="testfiles/spectronaut/results.tsv", filter_qvalue=False)
+            shutil.unpack_archive(
+                "testfiles/spectronaut/results.tsv.zip", "testfiles/spectronaut/"
+            )
+
+        cls.cls_loader = SpectronautLoader(
+            file="testfiles/spectronaut/results.tsv", filter_qvalue=False
+        )
         cls.cls_metadata_path = "testfiles/spectronaut/metadata.xlsx"
         cls.cls_obj = DataSet(
             loader=cls.cls_loader,
             metadata_path=cls.cls_metadata_path,
-            sample_column="sample"
+            sample_column="sample",
         )
 
     def setUp(self):
         self.loader = copy.deepcopy(self.cls_loader)
         self.metadata_path = copy.deepcopy(self.cls_metadata_path)
         self.obj = copy.deepcopy(self.cls_obj)
-        self.matrix_dim = (9,2458)
+        self.matrix_dim = (9, 2458)
         self.matrix_dim_filtered = (9, 2453)
         self.comparison_column = "condition"
-    
+
     @classmethod
     def tearDownClass(cls):
         if os.path.isdir("testfiles/spectronaut/__MACOSX"):
             shutil.rmtree("testfiles/spectronaut/__MACOSX")
 
         os.remove("testfiles/spectronaut/results.tsv")
+    
+class TestGenericDataSet(BaseTestDataSet.BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        if os.path.isfile("testfiles/fragpipe/combined_proteins.tsv") == False:
+            shutil.unpack_archive(
+                "testfiles/fragpipe/combined_proteins.tsv.zip", "testfiles/fragpipe"
+            )
+
+        cls.cls_loader = GenericLoader(
+            file="testfiles/fragpipe/combined_proteins.tsv",
+            intensity_column=[
+                "S1 Razor Intensity",	"S2 Razor Intensity", "S3 Razor Intensity",
+                "S4 Razor Intensity",	"S5 Razor Intensity",	"S6 Razor Intensity", 
+                "S7 Razor Intensity", "S8 Razor Intensity"
+            ],
+            index_column="Protein",
+            sep="\t"
+        )
+        cls.cls_metadata_path = "testfiles/fragpipe/metadata2.xlsx"
+        cls.cls_obj = DataSet(
+            loader=cls.cls_loader,
+            metadata_path=cls.cls_metadata_path,
+            sample_column="analytical_sample external_id",
+        )
+      
+    def setUp(self):
+        self.loader = copy.deepcopy(self.cls_loader)
+        self.metadata_path = copy.deepcopy(self.cls_metadata_path)
+        self.obj = copy.deepcopy(self.cls_obj)
+        self.matrix_dim = (8, 5)
+        self.matrix_dim_filtered = (8, 5)
+        self.comparison_column = "grouping1"
 
+    @classmethod
+    def tearDownClass(cls):
+        if os.path.isdir("testfiles/fragpipe/__MACOSX"):
+            shutil.rmtree("testfiles/fragpipe/__MACOSX")
 
+       
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `alphastats-0.6.2/tests/test_DataSet_Pathway.py` & `alphastats-0.6.3/tests/test_DataSet_Pathway.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,20 +48,23 @@
                 self.obj.evidence_df = None
                 self.obj.go_abundance_correction(
                     fg_sample=self.fg_sample, bg_sample=self.bg_sample
                 )
 
         def test_go_abundance_correction_with_list(self):
             df = self.obj.go_abundance_correction(
-                bg_sample=self.bg_sample, fg_protein_list=self.obj.mat.columns.to_list()[200:300]
+                bg_sample=self.bg_sample,
+                fg_protein_list=self.obj.mat.columns.to_list()[200:300],
             )
             self.assertTrue(df.empty)
 
         def test_go_genome_list(self):
-            df = self.obj.go_genome(protein_list=self.obj.mat.columns.to_list()[600:700])
+            df = self.obj.go_genome(
+                protein_list=self.obj.mat.columns.to_list()[600:700]
+            )
             self.assertFalse(df.empty)
 
         def test_go_genome_sample(self):
             df = self.obj.go_genome(fg_sample=self.fg_sample)
             self.assertFalse(df.empty)
 
         def test_extract_protein_ids(self):
@@ -90,10 +93,9 @@
         self.obj = DataSet(
             loader=self.loader, metadata_path=metadata, sample_column="sample",
         )
         self.fg_sample = "AC399"
         self.bg_sample = "UT822"
 
 
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `alphastats-0.6.2/tests/test_loaders.py` & `alphastats-0.6.3/tests/test_loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 
     def test_set_filter_columns_to_true_false(self):
         # check if + has been replaced by TRUE FALSE
         self.assertEqual(self.obj.rawinput["Reverse"].dtype, "bool")
         self.assertEqual(self.obj.rawinput["Only identified by site"].dtype, "bool")
         self.assertEqual(self.obj.rawinput["Potential contaminant"].dtype, "bool")
 
+
 class TestDIANNLoader(BaseTestLoader.BaseTest):
     @classmethod
     def setUpClass(cls):
         cls.obj = DIANNLoader(file="testfiles/diann/report_final.pg_matrix.tsv")
         cls.df_dim = (10, 26)
 
     def add_tag_to_sample_columns(self):
@@ -187,57 +188,69 @@
 
 class TestFragPipeLoader(BaseTestLoader.BaseTest):
     @classmethod
     def setUpClass(cls):
         cls.obj = FragPipeLoader(file="testfiles/fragpipe/combined_proteins.tsv")
         cls.df_dim = (10, 37)
 
+
 class TestmzTabLoader(BaseTestLoader.BaseTest):
     @classmethod
     def setUpClass(cls):
         cls.obj = mzTabLoader(file="testfiles/mzTab/test.mztab")
         cls.df_dim = (283, 265)
 
 class TestSpectronautLoader(BaseTestLoader.BaseTest):
     @classmethod
     def setUpClass(cls):
-        
+
         if os.path.isfile("testfiles/spectronaut/results.tsv") == False:
-            shutil.unpack_archive("testfiles/spectronaut/results.tsv.zip", "testfiles/spectronaut/")
-        
-        cls.obj = SpectronautLoader(file="testfiles/spectronaut/results.tsv", filter_qvalue=False)
+            shutil.unpack_archive(
+                "testfiles/spectronaut/results.tsv.zip", "testfiles/spectronaut/"
+            )
+
+        cls.obj = SpectronautLoader(
+            file="testfiles/spectronaut/results.tsv", filter_qvalue=False
+        )
         cls.df_dim = (2458, 11)
 
     def test_reading_non_european_comma(self):
         """
         files with non european comma get read correctly
         """
-        s = SpectronautLoader(file="testfiles/spectronaut/results_non_european_comma.tsv", filter_qvalue=False)
-        mean = s.rawinput["20221015_EV_TP_40SPD_LITDIA_MS1_Rapid_MS2_Rapid_57w_100ng_03_PG.Quantity"].mean()
+        s = SpectronautLoader(
+            file="testfiles/spectronaut/results_non_european_comma.tsv",
+            filter_qvalue=False,
+        )
+        mean = s.rawinput[
+            "20221015_EV_TP_40SPD_LITDIA_MS1_Rapid_MS2_Rapid_57w_100ng_03_PG.Quantity"
+        ].mean()
 
     def test_qvalue_filtering(self):
-        obj = SpectronautLoader(file="testfiles/spectronaut/results.tsv", filter_qvalue=True, qvalue_cutoff=0.00000001)
+        obj = SpectronautLoader(
+            file="testfiles/spectronaut/results.tsv",
+            filter_qvalue=True,
+            qvalue_cutoff=0.00000001,
+        )
         self.assertEqual(obj.rawinput.shape, (2071, 10))
 
     def test_qvalue_filtering_warning(self):
         with self.assertWarns(Warning):
             df = pd.read_csv("testfiles/spectronaut/results.tsv", sep="\t", decimal=",")
-            df.drop(columns = ["EG.Qvalue"], axis=1) 
+            df.drop(columns=["EG.Qvalue"], axis=1)
             SpectronautLoader(file=df)
 
     def test_gene_name_column(self):
         df = pd.read_csv("testfiles/spectronaut/results.tsv", sep="\t", decimal=",")
         df["PG.Genes"] = 0
         s = SpectronautLoader(file=df, filter_qvalue=False)
-  
+
     @classmethod
     def tearDownClass(cls):
         if os.path.isdir("testfiles/spectronaut/__MACOSX"):
             shutil.rmtree("testfiles/spectronaut/__MACOSX")
 
         os.remove("testfiles/spectronaut/results.tsv")
-       
-        
 
 
 if __name__ == "__main__":
     unittest.main()
```

