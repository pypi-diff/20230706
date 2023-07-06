# Comparing `tmp/quest_eras-1.6.4.3.tar.gz` & `tmp/quest_eras-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quest_eras-1.6.4.3.tar", last modified: Wed Mar 29 15:34:22 2023, max compression
+gzip compressed data, was "quest_eras-1.6.5.tar", last modified: Thu Jul  6 15:40:54 2023, max compression
```

## Comparing `quest_eras-1.6.4.3.tar` & `quest_eras-1.6.5.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.117292 quest_eras-1.6.4.3/
--rw-rw-r--   0 abera    (127551) 1049671531     1656 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/LICENSE
--rw-r--r--   0 abera    (127551) 1049671531      454 2023-03-29 15:34:22.117089 quest_eras-1.6.4.3/PKG-INFO
--rw-rw-r--   0 abera    (127551) 1049671531    30819 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/README.md
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.076380 quest_eras-1.6.4.3/quest_eras/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-02-15 19:37:20.000000 quest_eras-1.6.4.3/quest_eras/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.078113 quest_eras-1.6.4.3/quest_eras/es_gui/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.078436 quest_eras-1.6.4.3/quest_eras/es_gui/apps/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.081140 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    31284 2023-03-27 17:05:55.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/cost_savings.py
--rw-rw-r--   0 abera    (127551) 1049671531     4228 2023-03-27 17:08:15.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/home.py
--rw-rw-r--   0 abera    (127551) 1049671531     7315 2023-03-27 17:11:28.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/op_handler.py
--rw-rw-r--   0 abera    (127551) 1049671531    38030 2023-03-27 17:08:53.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/reporting.py
--rw-rw-r--   0 abera    (127551) 1049671531     5872 2023-03-27 17:09:03.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/results_viewer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.085245 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    60235 2023-03-27 17:10:30.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/data_manager.py
--rw-rw-r--   0 abera    (127551) 1049671531     3973 2023-03-27 17:10:34.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/home.py
--rw-rw-r--   0 abera    (127551) 1049671531    27098 2023-03-27 17:10:26.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/load.py
--rw-rw-r--   0 abera    (127551) 1049671531    15808 2023-03-27 17:12:26.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/nsrdb.py
--rw-rw-r--   0 abera    (127551) 1049671531    10595 2023-03-27 17:13:37.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/pv.py
--rw-rw-r--   0 abera    (127551) 1049671531    47475 2023-03-27 17:13:35.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/rate_structure.py
--rw-rw-r--   0 abera    (127551) 1049671531      778 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/utils.py
--rw-rw-r--   0 abera    (127551) 1049671531   146438 2023-03-27 17:13:33.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/widgets.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.087524 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531     4844 2023-03-27 17:13:58.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/home.py
--rw-rw-r--   0 abera    (127551) 1049671531    23951 2023-03-27 17:14:22.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/performance_sim.py
--rw-rw-r--   0 abera    (127551) 1049671531    12700 2023-03-27 17:14:24.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/performance_sim_handler.py
--rw-rw-r--   0 abera    (127551) 1049671531     7002 2023-03-27 17:14:36.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/results_viewer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.089989 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531     5960 2023-03-27 17:15:42.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/analysis.py
--rw-rw-r--   0 abera    (127551) 1049671531      636 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fAux.py
--rw-rw-r--   0 abera    (127551) 1049671531     5473 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fFeasibility.py
--rw-rw-r--   0 abera    (127551) 1049671531     2701 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fPlots.py
--rw-rw-r--   0 abera    (127551) 1049671531     2976 2023-03-27 17:15:41.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/home.py
--rw-rw-r--   0 abera    (127551) 1049671531     9822 2023-03-27 17:16:16.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/results_viewer.py
--rw-rw-r--   0 abera    (127551) 1049671531    14058 2023-03-27 17:16:14.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/tech_selection_wizard.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.094179 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    15613 2023-03-27 17:17:29.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/batchrunscreen.py
--rw-rw-r--   0 abera    (127551) 1049671531     6411 2023-03-27 17:17:27.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/home.py
--rw-rw-r--   0 abera    (127551) 1049671531    12378 2023-03-27 17:18:56.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/loaddatascreen.py
--rw-rw-r--   0 abera    (127551) 1049671531     8317 2023-03-27 17:18:54.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/op_handler.py
--rw-rw-r--   0 abera    (127551) 1049671531    23939 2023-03-27 17:18:44.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/reporting.py
--rw-rw-r--   0 abera    (127551) 1049671531     5843 2023-03-27 17:18:47.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/results_viewer.py
--rw-rw-r--   0 abera    (127551) 1049671531     5108 2023-03-27 17:18:41.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/setparametersscreen.py
--rw-rw-r--   0 abera    (127551) 1049671531     8296 2023-03-27 17:18:39.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/valuationscreen.py
--rw-rw-r--   0 abera    (127551) 1049671531    42080 2023-03-27 17:18:36.000000 quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/wizard.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.096953 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/
--rw-rw-r--   0 abera    (127551) 1049671531     4932 2023-03-27 17:19:23.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/ChartTestApp.py
--rw-rw-r--   0 abera    (127551) 1049671531      102 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    53107 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/charts.py
--rw-rw-r--   0 abera    (127551) 1049671531    13072 2023-03-27 17:19:29.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/data_importer.py
--rw-rw-r--   0 abera    (127551) 1049671531     1826 2023-03-27 17:19:24.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/data_importer_test_app.py
--rw-rw-r--   0 abera    (127551) 1049671531     3317 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/help_carousel.py
--rw-rw-r--   0 abera    (127551) 1049671531     1834 2023-03-27 17:19:34.000000 quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/help_carousel_test_app.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.097316 quest_eras-1.6.4.3/quest_eras/es_gui/resources/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/resources/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.097779 quest_eras-1.6.4.3/quest_eras/es_gui/resources/widgets/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/resources/widgets/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    32620 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/resources/widgets/common.py
--rw-rw-r--   0 abera    (127551) 1049671531      744 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/settings.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.099059 quest_eras-1.6.4.3/quest_eras/es_gui/tools/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.100461 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531     2058 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/btm_dms.py
--rw-rw-r--   0 abera    (127551) 1049671531    21943 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/btm_optimizer.py
--rw-rw-r--   0 abera    (127551) 1049671531     2992 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/constraints.py
--rw-rw-r--   0 abera    (127551) 1049671531    11202 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/readutdata.py
--rw-rw-r--   0 abera    (127551) 1049671531     5379 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/dms.py
--rw-rw-r--   0 abera    (127551) 1049671531     4328 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.102411 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/
--rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/__init__.py
--rw-rw-r--   0 abera    (127551) 1049671531    29319 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/constraints.py
--rw-rw-r--   0 abera    (127551) 1049671531    52211 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/utilities.py
--rw-rw-r--   0 abera    (127551) 1049671531    15749 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/valuation_dms.py
--rw-rw-r--   0 abera    (127551) 1049671531    32475 2022-12-01 18:24:52.000000 quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/valuation_optimizer.py
--rw-rw-r--   0 abera    (127551) 1049671531    48317 2023-03-29 15:25:42.000000 quest_eras-1.6.4.3/quest_eras/main.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.102722 quest_eras-1.6.4.3/quest_eras/quest_library/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.102929 quest_eras-1.6.4.3/quest_eras/quest_library/apps/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/apps/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.103836 quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531    16644 2023-03-08 23:02:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/op_handler.py
--rw-r--r--   0 abera    (127551) 1049671531     4647 2023-03-09 18:27:14.000000 quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/valuation_example.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.104300 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.105287 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     5491 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/dms.py
--rw-r--r--   0 abera    (127551) 1049671531     4471 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.105988 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/__init__.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.107543 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     8972 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     3685 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     4868 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    24645 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.108688 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     8794 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     3937 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     4843 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    18862 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.110136 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     8773 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     6208 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     3380 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    20649 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.111696 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     8604 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     7342 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     4009 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    20245 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.113605 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     8776 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     9258 2023-03-08 23:39:38.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     3193 2023-03-08 23:41:33.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    19794 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.114875 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     9253 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     7692 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     6332 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    20595 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.116434 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/
--rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/__init__.py
--rw-r--r--   0 abera    (127551) 1049671531     9244 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/constraints.py
--rw-r--r--   0 abera    (127551) 1049671531     4610 2023-03-09 00:14:36.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/data_processing_tools.py
--rw-r--r--   0 abera    (127551) 1049671531     3284 2023-03-09 00:05:06.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_dms.py
--rw-r--r--   0 abera    (127551) 1049671531    18993 2023-03-08 23:59:09.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_optimizer.py
--rw-r--r--   0 abera    (127551) 1049671531   140324 2023-03-08 22:11:23.000000 quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/valuation_optimizer.py
-drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-03-29 15:34:22.077743 quest_eras-1.6.4.3/quest_eras.egg-info/
--rw-r--r--   0 abera    (127551) 1049671531      454 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/PKG-INFO
--rw-r--r--   0 abera    (127551) 1049671531     6406 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/SOURCES.txt
--rw-r--r--   0 abera    (127551) 1049671531        1 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/dependency_links.txt
--rw-r--r--   0 abera    (127551) 1049671531       48 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/entry_points.txt
--rw-r--r--   0 abera    (127551) 1049671531      158 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/requires.txt
--rw-r--r--   0 abera    (127551) 1049671531       12 2023-03-29 15:34:22.000000 quest_eras-1.6.4.3/quest_eras.egg-info/top_level.txt
--rw-r--r--   0 abera    (127551) 1049671531       38 2023-03-29 15:34:22.117351 quest_eras-1.6.4.3/setup.cfg
--rw-rw-r--   0 abera    (127551) 1049671531     1397 2023-03-29 15:22:43.000000 quest_eras-1.6.4.3/setup.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.868071 quest_eras-1.6.5/
+-rw-rw-r--   0 abera    (127551) 1049671531     1656 2022-12-01 18:24:52.000000 quest_eras-1.6.5/LICENSE
+-rw-r--r--   0 abera    (127551) 1049671531      452 2023-07-06 15:40:54.867861 quest_eras-1.6.5/PKG-INFO
+-rw-rw-r--   0 abera    (127551) 1049671531    30819 2022-12-01 18:24:52.000000 quest_eras-1.6.5/README.md
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.827234 quest_eras-1.6.5/quest_eras/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-02-15 19:37:20.000000 quest_eras-1.6.5/quest_eras/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.829828 quest_eras-1.6.5/quest_eras/es_gui/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.830322 quest_eras-1.6.5/quest_eras/es_gui/apps/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.833134 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    31284 2023-03-27 17:05:55.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/cost_savings.py
+-rw-rw-r--   0 abera    (127551) 1049671531     4228 2023-03-27 17:08:15.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/home.py
+-rw-rw-r--   0 abera    (127551) 1049671531     7315 2023-03-27 17:11:28.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/op_handler.py
+-rw-rw-r--   0 abera    (127551) 1049671531    38030 2023-03-27 17:08:53.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/reporting.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5872 2023-03-27 17:09:03.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/btm/results_viewer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.836995 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    60235 2023-03-27 17:10:30.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/data_manager.py
+-rw-rw-r--   0 abera    (127551) 1049671531     3973 2023-03-27 17:10:34.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/home.py
+-rw-rw-r--   0 abera    (127551) 1049671531    27098 2023-03-27 17:10:26.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/load.py
+-rw-rw-r--   0 abera    (127551) 1049671531    15808 2023-03-27 17:12:26.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/nsrdb.py
+-rw-rw-r--   0 abera    (127551) 1049671531    10595 2023-03-27 17:13:37.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/pv.py
+-rw-rw-r--   0 abera    (127551) 1049671531    47475 2023-03-27 17:13:35.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/rate_structure.py
+-rw-rw-r--   0 abera    (127551) 1049671531      778 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/utils.py
+-rw-rw-r--   0 abera    (127551) 1049671531   146438 2023-03-27 17:13:33.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/widgets.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.839128 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531     4844 2023-03-27 17:13:58.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/home.py
+-rw-rw-r--   0 abera    (127551) 1049671531    23951 2023-03-27 17:14:22.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/performance_sim.py
+-rw-rw-r--   0 abera    (127551) 1049671531    12700 2023-03-27 17:14:24.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/performance_sim_handler.py
+-rw-rw-r--   0 abera    (127551) 1049671531     7002 2023-03-27 17:14:36.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/performance/results_viewer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.842256 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5960 2023-03-27 17:15:42.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/analysis.py
+-rw-rw-r--   0 abera    (127551) 1049671531      636 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fAux.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5473 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fFeasibility.py
+-rw-rw-r--   0 abera    (127551) 1049671531     2701 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fPlots.py
+-rw-rw-r--   0 abera    (127551) 1049671531     2976 2023-03-27 17:15:41.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/home.py
+-rw-rw-r--   0 abera    (127551) 1049671531     9833 2023-03-29 17:26:41.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/results_viewer.py
+-rw-rw-r--   0 abera    (127551) 1049671531    14058 2023-03-27 17:16:14.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/tech_selection_wizard.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.846288 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    15613 2023-03-27 17:17:29.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/batchrunscreen.py
+-rw-rw-r--   0 abera    (127551) 1049671531     6411 2023-03-27 17:17:27.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/home.py
+-rw-rw-r--   0 abera    (127551) 1049671531    12378 2023-03-27 17:18:56.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/loaddatascreen.py
+-rw-rw-r--   0 abera    (127551) 1049671531     8317 2023-03-27 17:18:54.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/op_handler.py
+-rw-rw-r--   0 abera    (127551) 1049671531    23939 2023-03-27 17:18:44.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/reporting.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5843 2023-03-27 17:18:47.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/results_viewer.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5108 2023-03-27 17:18:41.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/setparametersscreen.py
+-rw-rw-r--   0 abera    (127551) 1049671531     8296 2023-03-27 17:18:39.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/valuationscreen.py
+-rw-rw-r--   0 abera    (127551) 1049671531    42080 2023-03-27 17:18:36.000000 quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/wizard.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.848975 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/
+-rw-rw-r--   0 abera    (127551) 1049671531     4932 2023-03-27 17:19:23.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/ChartTestApp.py
+-rw-rw-r--   0 abera    (127551) 1049671531      102 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    53107 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/charts.py
+-rw-rw-r--   0 abera    (127551) 1049671531    13072 2023-03-27 17:19:29.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/data_importer.py
+-rw-rw-r--   0 abera    (127551) 1049671531     1826 2023-03-27 17:19:24.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/data_importer_test_app.py
+-rw-rw-r--   0 abera    (127551) 1049671531     3317 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/help_carousel.py
+-rw-rw-r--   0 abera    (127551) 1049671531     1834 2023-03-27 17:19:34.000000 quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/help_carousel_test_app.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.849377 quest_eras-1.6.5/quest_eras/es_gui/resources/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/resources/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.849904 quest_eras-1.6.5/quest_eras/es_gui/resources/widgets/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/resources/widgets/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    32631 2023-03-29 17:06:32.000000 quest_eras-1.6.5/quest_eras/es_gui/resources/widgets/common.py
+-rw-rw-r--   0 abera    (127551) 1049671531      744 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/settings.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.850942 quest_eras-1.6.5/quest_eras/es_gui/tools/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.852384 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531     2080 2023-03-29 17:22:31.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/btm_dms.py
+-rw-rw-r--   0 abera    (127551) 1049671531    21965 2023-03-29 17:22:44.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/btm_optimizer.py
+-rw-rw-r--   0 abera    (127551) 1049671531     2992 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/constraints.py
+-rw-rw-r--   0 abera    (127551) 1049671531    11202 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/btm/readutdata.py
+-rw-rw-r--   0 abera    (127551) 1049671531     5379 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/dms.py
+-rw-rw-r--   0 abera    (127551) 1049671531     4328 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.853963 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/
+-rw-rw-r--   0 abera    (127551) 1049671531        0 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/__init__.py
+-rw-rw-r--   0 abera    (127551) 1049671531    29319 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/constraints.py
+-rw-rw-r--   0 abera    (127551) 1049671531    52211 2022-12-01 18:24:52.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/utilities.py
+-rw-rw-r--   0 abera    (127551) 1049671531    15771 2023-03-29 17:20:13.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/valuation_dms.py
+-rw-rw-r--   0 abera    (127551) 1049671531    32497 2023-03-29 17:23:32.000000 quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/valuation_optimizer.py
+-rw-rw-r--   0 abera    (127551) 1049671531    48537 2023-03-30 16:26:24.000000 quest_eras-1.6.5/quest_eras/main.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.854428 quest_eras-1.6.5/quest_eras/quest_library/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.854570 quest_eras-1.6.5/quest_eras/quest_library/apps/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/apps/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.855371 quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531    16644 2023-03-08 23:02:23.000000 quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/op_handler.py
+-rw-r--r--   0 abera    (127551) 1049671531     4647 2023-03-09 18:27:14.000000 quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/valuation_example.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.855713 quest_eras-1.6.5/quest_eras/quest_library/utilities/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.856441 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     5491 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/dms.py
+-rw-r--r--   0 abera    (127551) 1049671531     4471 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.856966 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/__init__.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.858203 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     8972 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     3685 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     4868 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    24645 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.859450 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     8794 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     3937 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     4843 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    18862 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.860950 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     8773 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     6208 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     3380 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    20649 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.862279 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     8604 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     7342 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     4009 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    20245 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.864391 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     8776 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     9258 2023-03-08 23:39:38.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     3193 2023-03-08 23:41:33.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    19794 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.865866 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     9253 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     7692 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     6332 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    20595 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.867300 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/
+-rw-r--r--   0 abera    (127551) 1049671531        0 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/__init__.py
+-rw-r--r--   0 abera    (127551) 1049671531     9244 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/constraints.py
+-rw-r--r--   0 abera    (127551) 1049671531     4610 2023-03-09 00:14:36.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/data_processing_tools.py
+-rw-r--r--   0 abera    (127551) 1049671531     3284 2023-03-09 00:05:06.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_dms.py
+-rw-r--r--   0 abera    (127551) 1049671531    18993 2023-03-08 23:59:09.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_optimizer.py
+-rw-r--r--   0 abera    (127551) 1049671531   140324 2023-03-08 22:11:23.000000 quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/valuation_optimizer.py
+drwxr-xr-x   0 abera    (127551) 1049671531        0 2023-07-06 15:40:54.829401 quest_eras-1.6.5/quest_eras.egg-info/
+-rw-r--r--   0 abera    (127551) 1049671531      452 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/PKG-INFO
+-rw-r--r--   0 abera    (127551) 1049671531     6406 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/SOURCES.txt
+-rw-r--r--   0 abera    (127551) 1049671531        1 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/dependency_links.txt
+-rw-r--r--   0 abera    (127551) 1049671531       47 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/entry_points.txt
+-rw-r--r--   0 abera    (127551) 1049671531      158 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/requires.txt
+-rw-r--r--   0 abera    (127551) 1049671531       12 2023-07-06 15:40:54.000000 quest_eras-1.6.5/quest_eras.egg-info/top_level.txt
+-rw-r--r--   0 abera    (127551) 1049671531       38 2023-07-06 15:40:54.868137 quest_eras-1.6.5/setup.cfg
+-rw-rw-r--   0 abera    (127551) 1049671531     1394 2023-07-06 15:30:57.000000 quest_eras-1.6.5/setup.py
```

### Comparing `quest_eras-1.6.4.3/LICENSE` & `quest_eras-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/README.md` & `quest_eras-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/cost_savings.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/btm/cost_savings.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/home.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/btm/home.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/op_handler.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/btm/op_handler.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/reporting.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/btm/reporting.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/btm/results_viewer.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/btm/results_viewer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/data_manager.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/data_manager.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/home.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/home.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/load.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/load.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/nsrdb.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/nsrdb.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/pv.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/pv.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/rate_structure.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/rate_structure.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/utils.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/utils.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/data_manager/widgets.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/data_manager/widgets.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/home.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/performance/home.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/performance_sim.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/performance/performance_sim.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/performance_sim_handler.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/performance/performance_sim_handler.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/performance/results_viewer.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/performance/results_viewer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/analysis.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/analysis.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fAux.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fAux.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fFeasibility.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fFeasibility.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/fPlots.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/fPlots.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/home.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/home.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/results_viewer.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/results_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import
 
 import os
 import pandas as pd
 import webbrowser
-from es_gui.apps.tech_selection import fAux
+from quest_eras.es_gui.apps.tech_selection import fAux
 
 from kivy.app import App
 from kivy.uix.screenmanager import Screen
 
 from quest_eras.es_gui.resources.widgets.common import BASE_TRANSITION_DUR, WarningPopup, stnd_font
 from quest_eras.es_gui.apps.tech_selection import fPlots
```

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/tech_selection/tech_selection_wizard.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/tech_selection/tech_selection_wizard.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/batchrunscreen.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/batchrunscreen.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/home.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/home.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/loaddatascreen.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/loaddatascreen.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/op_handler.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/op_handler.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/reporting.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/reporting.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/results_viewer.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/results_viewer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/setparametersscreen.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/setparametersscreen.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/valuationscreen.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/valuationscreen.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/apps/valuation/wizard.py` & `quest_eras-1.6.5/quest_eras/es_gui/apps/valuation/wizard.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/ChartTestApp.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/ChartTestApp.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/charts.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/charts.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/data_importer.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/data_importer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/data_importer_test_app.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/data_importer_test_app.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/help_carousel.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/help_carousel.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/proving_grounds/help_carousel_test_app.py` & `quest_eras-1.6.5/quest_eras/es_gui/proving_grounds/help_carousel_test_app.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/resources/widgets/common.py` & `quest_eras-1.6.5/quest_eras/es_gui/resources/widgets/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from kivy.uix.recycleview.views import RecycleDataViewBehavior
 from kivy.uix.popup import Popup
 from kivy.uix.spinner import SpinnerOption, Spinner
 from kivy.uix.label import Label
 from kivy.uix.screenmanager import Screen
 from kivy.uix.togglebutton import ToggleButton
 
-from es_gui.proving_grounds.help_carousel import HelpCarouselModalView
+from quest_eras.es_gui.proving_grounds.help_carousel import HelpCarouselModalView
 
 cwd = os.getcwd()
 
 # Animation durations in seconds #
 BASE_TRANSITION_DUR = 0.600
 BUTTON_FLASH_DUR = 0.100
 ANIM_STAGGER = 0.200
```

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/settings.py` & `quest_eras-1.6.5/quest_eras/es_gui/settings.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/btm_dms.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/btm/btm_dms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import
 import logging
 import os
 import json
 
 import pandas as pd
 
-from es_gui.tools.dms import DataManagementSystem
-from es_gui.tools.btm.readutdata import *
+from quest_eras.es_gui.tools.dms import DataManagementSystem
+from quest_eras.es_gui.tools.btm.readutdata import *
 
 
 class BtmDMS(DataManagementSystem):
     """
     A class for managing data for the behind-the-meter energy storage functions. Class methods for each type of file to be loaded are included, extending from the get_data() method of the superclass. Each of these methods uses get_data() to retrieve the relevant data and loads the file and adds it to the DMS if the data is not loaded. An optional class method for calling each of the individual data methods can be included to, e.g., form the necessary arguments and return the desired variables.
 
     :param home_path: A string indicating the relative path to where data is saved.
```

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/btm_optimizer.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/btm/btm_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 
 from pyomo.environ import *
 import pandas as pd
 import numpy as np
 import os
 
-from es_gui.tools import optimizer
-from es_gui.tools.btm.constraints import ExpressionsBlock
+from quest_eras.es_gui.tools import optimizer
+from quest_eras.es_gui.tools.btm.constraints import ExpressionsBlock
 
 
 class BtmOptimizer(optimizer.Optimizer):
     """A framework wrapper class for creating Pyomo ConcreteModels for behind the meter valuation."""
 
     def __init__(self, tou_energy_schedule = None, tou_energy_rate=None, 
                  tou_demand_schedule=None, tou_demand_rate=None, flat_demand_rate=None,
```

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/constraints.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/btm/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/btm/readutdata.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/btm/readutdata.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/dms.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/optimizer.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/constraints.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/utilities.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/utilities.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/valuation_dms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import absolute_import
 import logging
 import os
 import json
 
 import pandas as pd
 
-from es_gui.tools.dms import DataManagementSystem
-from es_gui.tools.valuation.utilities import *
+from quest_eras.es_gui.tools.dms import DataManagementSystem
+from quest_eras.es_gui.tools.valuation.utilities import *
 
 
 class ValuationDMS(DataManagementSystem):
     """
     A class for managing data for the energy storage valuation optimization functions. Class methods for each type of file to be loaded are included, extending from the get_data() method of the superclass. Each of these methods uses get_data() to retrieve the relevant data and loads the file and adds it to the DMS if the data is not loaded. An optional class method for calling each of the individual data methods can be included to, e.g., form the necessary arguments and return the desired variables.
 
     :param home_path: A string indicating the relative path to where data is saved.
```

### Comparing `quest_eras-1.6.4.3/quest_eras/es_gui/tools/valuation/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/es_gui/tools/valuation/valuation_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 
 from pyomo.environ import *
 import pandas as pd
 import numpy as np
 
-from es_gui.tools import optimizer
-from es_gui.tools.valuation.constraints import ExpressionsBlock
+from quest_eras.es_gui.tools import optimizer
+from quest_eras.es_gui.tools.valuation.constraints import ExpressionsBlock
 
 
 class ValuationOptimizer(optimizer.Optimizer):
     """A framework wrapper class for creating Pyomo ConcreteModels for energy storage valuation."""
 
     def __init__(self, price_electricity=None,
                  price_reg_up=None, price_reg_down=None,
```

### Comparing `quest_eras-1.6.4.3/quest_eras/main.py` & `quest_eras-1.6.5/quest_eras/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,43 +54,43 @@
 from quest_eras.es_gui.proving_grounds.help_carousel import HelpCarouselModalView
 
 dirname = os.path.dirname(__file__)
 
 # Import common widgets from look_and_feel
 Builder.load_file(os.path.join(dirname, 'es_gui', 'resources', 'widgets', 'common.kv'))
 
-from es_gui.settings import ESAppSettings
+from quest_eras.es_gui.settings import ESAppSettings
 
 # Data Manager
-from es_gui.apps.data_manager.home import DataManagerHomeScreen
-from es_gui.apps.data_manager.widgets import DataManagerRTOMOdataScreen
-from es_gui.apps.data_manager.rate_structure import RateStructureDataScreen
-from es_gui.apps.data_manager.load import DataManagerLoadHomeScreen, DataManagerCommercialLoadScreen, DataManagerResidentialLoadScreen
-from es_gui.apps.data_manager.pv import PVwattsSearchScreen
-from es_gui.apps.data_manager.nsrdb import NSRDBDataScreen
+from quest_eras.es_gui.apps.data_manager.home import DataManagerHomeScreen
+from quest_eras.es_gui.apps.data_manager.widgets import DataManagerRTOMOdataScreen
+from quest_eras.es_gui.apps.data_manager.rate_structure import RateStructureDataScreen
+from quest_eras.es_gui.apps.data_manager.load import DataManagerLoadHomeScreen, DataManagerCommercialLoadScreen, DataManagerResidentialLoadScreen
+from quest_eras.es_gui.apps.data_manager.pv import PVwattsSearchScreen
+from quest_eras.es_gui.apps.data_manager.nsrdb import NSRDBDataScreen
 
 # Valuation
-from es_gui.apps.valuation.home import ValuationHomeScreen
-from es_gui.apps.valuation.batchrunscreen import BatchRunScreen
-from es_gui.apps.valuation.results_viewer import ValuationResultsViewer
-from es_gui.apps.valuation.wizard import ValuationWizard
+from quest_eras.es_gui.apps.valuation.home import ValuationHomeScreen
+from quest_eras.es_gui.apps.valuation.batchrunscreen import BatchRunScreen
+from quest_eras.es_gui.apps.valuation.results_viewer import ValuationResultsViewer
+from quest_eras.es_gui.apps.valuation.wizard import ValuationWizard
 
 # Behind-the-meter
-from es_gui.apps.btm.home import BehindTheMeterHomeScreen
-from es_gui.apps.btm.cost_savings import CostSavingsWizard
-from es_gui.apps.btm.results_viewer import BtmResultsViewer
-
-from es_gui.apps.performance.home import PerformanceHomeScreen
-from es_gui.apps.performance.performance_sim import PerformanceSimRunScreen
-from es_gui.apps.performance.results_viewer import PerformanceResultsViewer
+from quest_eras.es_gui.apps.btm.home import BehindTheMeterHomeScreen
+from quest_eras.es_gui.apps.btm.cost_savings import CostSavingsWizard
+from quest_eras.es_gui.apps.btm.results_viewer import BtmResultsViewer
+
+from quest_eras.es_gui.apps.performance.home import PerformanceHomeScreen
+from quest_eras.es_gui.apps.performance.performance_sim import PerformanceSimRunScreen
+from quest_eras.es_gui.apps.performance.results_viewer import PerformanceResultsViewer
 
 # Technology selection
-from es_gui.apps.tech_selection.home import TechSelectionHomeScreen
-from es_gui.apps.tech_selection.tech_selection_wizard import TechSelectionWizard
-from es_gui.apps.tech_selection.results_viewer import TechSelectionFeasible
+from quest_eras.es_gui.apps.tech_selection.home import TechSelectionHomeScreen
+from quest_eras.es_gui.apps.tech_selection.tech_selection_wizard import TechSelectionWizard
+from quest_eras.es_gui.apps.tech_selection.results_viewer import TechSelectionFeasible
 
 # Font registration.
 LabelBase.register(name='Exo 2',
                    fn_regular=os.path.join('es_gui', 'resources', 'fonts', 'Exo_2', 'Exo2-Regular.ttf'),
                    fn_bold=os.path.join('es_gui', 'resources', 'fonts', 'Exo_2', 'Exo2-Bold.ttf'),
                    fn_italic=os.path.join('es_gui', 'resources', 'fonts', 'Exo_2', 'Exo2-Italic.ttf'))
```

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/op_handler.py` & `quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/op_handler.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/apps/valuation/valuation_example.py` & `quest_eras-1.6.5/quest_eras/quest_library/apps/valuation/valuation_example.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/caiso/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/ercot/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/isone/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/miso/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/nyiso/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/pjm/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/constraints.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/constraints.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/data_processing_tools.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/data_processing_tools.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_dms.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_dms.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/spp/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras/quest_library/utilities/pomo/valuation/valuation_optimizer.py` & `quest_eras-1.6.5/quest_eras/quest_library/utilities/pomo/valuation/valuation_optimizer.py`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/quest_eras.egg-info/SOURCES.txt` & `quest_eras-1.6.5/quest_eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quest_eras-1.6.4.3/setup.py` & `quest_eras-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 DISTNAME = "quest_eras"
-VERSION = "1.6.4.3"
+VERSION = "1.6.5"
 EXTENSIONS = []
 PYTHON_REQUIRES = ">=3.8"
 DESCRIPTION = "Sandia National Laboratories application suite for energy storage analysis and evaluation tools."
 LONG_DESCRIPTION = "Sandia National Laboratories application suite for energy storage analysis and evaluation tools."
 AUTHOR = "Sandia National Laboratories"
 MAINTAINER_EMAIL = "tunguy@sandia.gov"
 LICENSE = "BSD 3-clause"
@@ -41,13 +41,13 @@
     version=VERSION,
     packages=find_packages() + ['.'],
     ext_modules=EXTENSIONS,
     python_requires=PYTHON_REQUIRES,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author=AUTHOR,
-    entry_points = {'gui_scripts': ['quest = quest_eras.main:QuESt_App']} ,
+    entry_points = {'gui_scripts': ['quest = quest_eras.main:QuEStApp']} ,
     maintainer_email=MAINTAINER_EMAIL,
     license=LICENSE,
     url=URL,
     **setuptools_kwargs
 )
```

