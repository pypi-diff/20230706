# Comparing `tmp/cosmotech-run-orchestrator-1.0.0.tar.gz` & `tmp/cosmotech-run-orchestrator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmotech-run-orchestrator-1.0.0.tar", last modified: Thu Jul  6 14:41:00 2023, max compression
+gzip compressed data, was "cosmotech-run-orchestrator-1.0.1.tar", last modified: Thu Jul  6 15:46:42 2023, max compression
```

## Comparing `cosmotech-run-orchestrator-1.0.0.tar` & `cosmotech-run-orchestrator-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1062 2023-06-12 12:23:13.000000 cosmotech-run-orchestrator-1.0.0/LICENCE.md
--rw-r--r--   0 afossart  (1001) afossart  (1001)       58 2023-07-06 14:39:00.000000 cosmotech-run-orchestrator-1.0.0/MANIFEST.in
--rw-r--r--   0 afossart  (1001) afossart  (1001)      267 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/PKG-INFO
--rw-r--r--   0 afossart  (1001) afossart  (1001)      269 2023-06-26 12:51:15.000000 cosmotech-run-orchestrator-1.0.0/README.md
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.683690 cosmotech-run-orchestrator-1.0.0/cosmotech/
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.683690 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/
--rw-r--r--   0 afossart  (1001) afossart  (1001)       18 2023-06-12 12:23:13.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/__init__.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 09:01:23.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     9592 2023-07-06 13:39:43.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     5023 2023-07-06 13:39:35.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)    19536 2023-07-06 13:47:07.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1588 2023-07-06 13:38:31.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/main.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     2775 2023-07-06 13:39:23.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/orchestrator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     6719 2023-07-06 13:39:23.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/parameters_generation.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4467 2023-07-06 13:39:23.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/run_step.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     7653 2023-07-06 13:38:48.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-07-06 12:57:57.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      889 2023-07-06 13:00:15.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/command_template.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1116 2023-07-06 12:58:02.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/environment.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4305 2023-07-06 14:01:01.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/orchestrator.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      554 2023-07-06 13:00:24.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/runner.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     5687 2023-07-06 13:00:29.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/step.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/schema/
--rw-r--r--   0 afossart  (1001) afossart  (1001)     4094 2023-07-06 08:43:07.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/schema/run_template_json_schema.json
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/
--rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 13:17:05.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/__init__.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)     2272 2023-07-06 09:44:35.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/api.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      434 2023-06-29 13:08:12.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/click.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      498 2023-06-15 13:17:17.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/decorators.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      465 2023-07-06 12:59:12.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/json.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      551 2023-06-26 15:10:36.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/logger.py
--rw-r--r--   0 afossart  (1001) afossart  (1001)      239 2023-07-06 12:59:31.000000 cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/singleton.py
-drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/
--rw-r--r--   0 afossart  (1001) afossart  (1001)      267 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/PKG-INFO
--rw-r--r--   0 afossart  (1001) afossart  (1001)     1539 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       90 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/entry_points.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 13:40:56.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/not-zip-safe
--rw-r--r--   0 afossart  (1001) afossart  (1001)      229 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/requires.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       10 2023-07-06 14:41:00.000000 cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/top_level.txt
--rw-r--r--   0 afossart  (1001) afossart  (1001)       38 2023-07-06 14:41:00.687690 cosmotech-run-orchestrator-1.0.0/setup.cfg
--rw-r--r--   0 afossart  (1001) afossart  (1001)      730 2023-07-06 13:40:28.000000 cosmotech-run-orchestrator-1.0.0/setup.py
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1260 2023-07-06 15:34:06.000000 cosmotech-run-orchestrator-1.0.1/LICENCE.md
+-rw-r--r--   0 afossart  (1001) afossart  (1001)       58 2023-07-06 14:39:00.000000 cosmotech-run-orchestrator-1.0.1/MANIFEST.in
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      285 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/PKG-INFO
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      269 2023-06-26 12:51:15.000000 cosmotech-run-orchestrator-1.0.1/README.md
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)       18 2023-07-06 15:46:22.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/__init__.py
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 09:01:23.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/__init__.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     9932 2023-07-06 15:34:44.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     5362 2023-07-06 15:34:41.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/download_cloud_steps.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)    19950 2023-07-06 15:34:51.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/legacy_json_generator.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1926 2023-07-06 15:34:57.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/main.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     3189 2023-07-06 15:35:13.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/orchestrator.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     7133 2023-07-06 15:35:18.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/parameters_generation.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     4881 2023-07-06 15:35:23.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/run_step.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     7993 2023-07-06 15:35:32.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-07-06 12:57:57.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/__init__.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1303 2023-07-06 15:35:44.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/command_template.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1440 2023-07-06 15:35:53.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/environment.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     4719 2023-07-06 15:35:59.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/orchestrator.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      968 2023-07-06 15:36:04.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/runner.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     6101 2023-07-06 15:36:13.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/step.py
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     4094 2023-07-06 08:43:07.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/run_template_json_schema.json
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.047530 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)        0 2023-06-15 13:17:05.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/__init__.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     2686 2023-07-06 15:36:22.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/api.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      848 2023-07-06 15:36:30.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/click.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      912 2023-07-06 15:36:34.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/decorators.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      879 2023-07-06 15:36:41.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/json.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      970 2023-07-06 15:36:53.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/logger.py
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      653 2023-07-06 15:37:00.000000 cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/singleton.py
+drwxr-xr-x   0 afossart  (1001) afossart  (1001)        0 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      285 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1539 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 afossart  (1001) afossart  (1001)       90 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/entry_points.txt
+-rw-r--r--   0 afossart  (1001) afossart  (1001)        1 2023-07-06 13:40:56.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 afossart  (1001) afossart  (1001)      229 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/requires.txt
+-rw-r--r--   0 afossart  (1001) afossart  (1001)       10 2023-07-06 15:46:42.000000 cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/top_level.txt
+-rw-r--r--   0 afossart  (1001) afossart  (1001)       38 2023-07-06 15:46:42.051530 cosmotech-run-orchestrator-1.0.1/setup.cfg
+-rw-r--r--   0 afossart  (1001) afossart  (1001)     1185 2023-07-06 15:40:44.000000 cosmotech-run-orchestrator-1.0.1/setup.py
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/adx_scenario_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-# Copyright (c) Cosmo Tech corporation.
-# Licensed under the MIT license.
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import pathlib
 import time
 from collections import defaultdict
 
 from CosmoTech_Acceleration_Library.Accelerators.adx_wrapper import ADXQueriesWrapper
 from CosmoTech_Acceleration_Library.Accelerators.adx_wrapper import IngestionStatus
 from azure.kusto.data.response import KustoResponseDataSet
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/download_cloud_steps.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/download_cloud_steps.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-# Copyright (c) Cosmo Tech corporation.
-# Licensed under the MIT license.
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
 
 import pathlib
 from zipfile import BadZipfile
 from zipfile import ZipFile
 
 import cosmotech_api
 from azure.identity import DefaultAzureCredential
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/legacy_json_generator.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/legacy_json_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import json
 
 from cosmotech_api.api.solution_api import RunTemplate
 from cosmotech_api.api.solution_api import Solution
 
 from cosmotech.orchestrator.core.orchestrator import Orchestrator
 from cosmotech.orchestrator.core.step import Step
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/parameters_generation.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/parameters_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import pathlib
 
 from cosmotech_api.api.solution_api import RunTemplate
 from cosmotech_api.api.solution_api import Solution
 
 from cosmotech.orchestrator.console_scripts.scenario_data_downloader import write_parameters
 from cosmotech.orchestrator.utils.api import get_solution
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/run_step.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/run_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import os
 import pathlib
 import subprocess
 import sys
 import venv
 
 from cosmotech.orchestrator.utils.click import click
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/console_scripts/scenario_data_downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-# Copyright (c) Cosmo Tech corporation.
-# Licensed under the MIT license.
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import json
 import os
 import pathlib
 from csv import DictWriter
 from distutils.dir_util import copy_tree
 
 from CosmoTech_Acceleration_Library.Accelerators.scenario_download.scenario_downloader import ScenarioDownloader
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/environment.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import os
 from dataclasses import dataclass
 from dataclasses import field
-from dataclasses import field
-from dataclasses import field
-from dataclasses import field
 
 
 @dataclass
 class EnvironmentVariable:
     name: str = field()
     defaultValue: str = field(default=None)
     value: str = field(default=None)
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/orchestrator.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/orchestrator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import json
 import pathlib
 
 import flowpipe
 import jsonschema
 
 from cosmotech.orchestrator.core.command_template import CommandTemplate
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/core/step.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/core/step.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import pathlib
 import subprocess
 import sys
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Union
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/schema/run_template_json_schema.json` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/schema/run_template_json_schema.json`

 * *Files identical despite different names*

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech/orchestrator/utils/api.py` & `cosmotech-run-orchestrator-1.0.1/cosmotech/orchestrator/utils/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# Copyright (C) - 2023 - 2023 - Cosmo Tech
+# This document and all information contained herein is the exclusive property -
+# including all intellectual property rights pertaining thereto - of Cosmo Tech.
+# Any use, reproduction, translation, broadcasting, transmission, distribution,
+# etc., to any person is prohibited unless it has been previously and
+# specifically authorized by written means by Cosmo Tech.
+
 import json
 import pathlib
 from typing import Optional
 
 import cosmotech_api
 import yaml
 from azure.identity import DefaultAzureCredential
```

### Comparing `cosmotech-run-orchestrator-1.0.0/cosmotech_run_orchestrator.egg-info/SOURCES.txt` & `cosmotech-run-orchestrator-1.0.1/cosmotech_run_orchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

