# Comparing `tmp/pollination-annual-daylight.full-0.10.6.tar.gz` & `tmp/pollination-annual-daylight.full-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pollination-annual-daylight.full-0.10.6.tar", last modified: Sun Jun 25 21:23:32 2023, max compression
+gzip compressed data, was "pollination-annual-daylight.full-0.10.7.tar", last modified: Thu Jul  6 12:34:30 2023, max compression
```

## Comparing `pollination-annual-daylight.full-0.10.6.tar` & `pollination-annual-daylight.full-0.10.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.449226 pollination-annual-daylight.full-0.10.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.449226 pollination-annual-daylight.full-0.10.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.449226 pollination-annual-daylight.full-0.10.6/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_prepare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_raytracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-25 21:23:32.000000 pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:32.453226 pollination-annual-daylight.full-0.10.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-25 21:22:40.000000 pollination-annual-daylight.full-0.10.6/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.468236 pollination-annual-daylight.full-0.10.7/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_prepare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 12:34:30.000000 pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:34:30.472236 pollination-annual-daylight.full-0.10.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-06 12:33:41.000000 pollination-annual-daylight.full-0.10.7/tests/validation_test.py
```

### Comparing `pollination-annual-daylight.full-0.10.6/.github/workflows/ci.yaml` & `pollination-annual-daylight.full-0.10.7/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     runs-on: ubuntu-latest
     needs: [deploy, deploy-to-staging]
     if: ${{ github.ref == 'refs/heads/master' && github.repository_owner == 'pollination' && contains(needs.deploy.outputs.tag, '.') }}
     strategy:
       fail-fast: true
       matrix:
         branch: [full, viz]
+      max-parallel: 1
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ matrix.branch }}
           fetch-depth: 0
       - name: rebase ${{ matrix.branch }} branch
         run: |
@@ -146,14 +147,15 @@
     runs-on: ubuntu-latest
     needs: [deploy-to-production]
     if: github.ref == 'refs/heads/production' && github.repository_owner == 'pollination'
     strategy:
       fail-fast: true
       matrix:
         branch: [full, viz]
+      max-parallel: 1
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ matrix.branch }}
           fetch-depth: 0
       - name: rebase ${{ matrix.branch }} branch
         run: |
```

### Comparing `pollination-annual-daylight.full-0.10.6/.github/workflows/tests.yaml` & `pollination-annual-daylight.full-0.10.7/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.6/LICENSE` & `pollination-annual-daylight.full-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.6/PKG-INFO` & `pollination-annual-daylight.full-0.10.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.full
-Version: 0.10.6
+Version: 0.10.7
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
@@ -12,14 +12,23 @@
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 License-File: LICENSE
 
 # annual-daylight
-Annual daylight recipe for Pollination
+Annual daylight recipe for Pollination.
 
 Use this recipe to calculate annual daylight for a HBJSON model.
 
-This recipe uses an enhanced 2-phase method for daylight simulation with accurate direct sunlight calculation.
+This recipe uses a 2-phase method for daylight simulation. If the accuracy of the direct sunlight is important, you can use the [annual-daylight-enhanced](https://github.com/pollination/annual-daylight-enhanced) recipe.
+
+### Versions
+There are three different versions of the recipe. All three versions use the same simulation methodology and workflow, although their outputs vary.
+| Version | Outputs | PyPI |
+|-|-|-|
+| annual-daylight | <ul><li>annual daylight metrics</li></ul> | [annual-daylight](https://pypi.org/project/pollination-annual-daylight/) |
+| annual-daylight.viz | <ul><li>annual daylight metrics</li><li>visualization</li></ul> | [annual-daylight.viz](https://pypi.org/project/pollination-annual-daylight.viz/) |
+| annual-daylight.full | <ul><li>annual daylight metrics</li><li>visualization</li><li>results folder</li></ul> | [annual-daylight.full](https://pypi.org/project/pollination-annual-daylight.full/) |
+
 
 For more information [see the recipe on Pollination](https://app.pollination.cloud/recipes/ladybug-tools/annual-daylight).
```

### Comparing `pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_post_process.py` & `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_post_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Post-process DAG for annual daylight."""
 from dataclasses import dataclass
 from pollination_dsl.dag import Inputs, GroupedDAG, task, Outputs
-from pollination.honeybee_radiance_postprocess.grid import MergeFolderData, \
-    MergeFolderMetrics
+from pollination.honeybee_radiance_postprocess.grid import MergeFolderMetrics
 from pollination.honeybee_display.translate import ModelToVis
 
 
 @dataclass
 class AnnualDaylightPostProcess(GroupedDAG):
     """Post-process for annual daylight."""
 
@@ -29,36 +28,15 @@
 
     grids_info = Inputs.file(
         description='Grid information file.',
         path='grids_info.json'
     )
 
     @task(
-        template=MergeFolderData,
-        sub_paths={
-            'input_folder': 'final'
-        }
-    )
-    def restructure_results(
-        self, input_folder=initial_results,
-        dist_info=dist_info,
-        extension='ill'
-    ):
-        return [
-            {
-                'from': MergeFolderData()._outputs.output_folder,
-                'to': 'results'
-            }
-        ]
-
-    @task(
-        template=MergeFolderMetrics,
-        sub_paths={
-            'input_folder': 'metrics'
-        }
+        template=MergeFolderMetrics
     )
     def restructure_metrics(
         self, input_folder=initial_results,
         dist_info=dist_info,
         grids_info=grids_info
     ):
         return [
@@ -84,12 +62,7 @@
         source='visualization.vsf',
         description='Annual daylight result visualization in VisualizationSet format.'
     )
 
     metrics = Outputs.folder(
         source='metrics', description='metrics folder.'
     )
-
-    results = Outputs.folder(
-        source='results', description='Folder with raw result files (.ill) that '
-        'contain illuminance matrices for each sensor at each timestep of the analysis.'
-    )
```

### Comparing `pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_prepare_folder.py` & `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_prepare_folder.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/_raytracing.py` & `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/_raytracing.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.6/pollination/annual_daylight/entry.py` & `pollination-annual-daylight.full-0.10.7/pollination/annual_daylight/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pollination_dsl.dag import Inputs, DAG, task, Outputs
 from dataclasses import dataclass
+from pollination.honeybee_radiance_postprocess.grid import MergeFolderData
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.wea import wea_input_timestep_check
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
@@ -155,30 +156,45 @@
         needs=[prepare_folder_annual_daylight, annual_daylight_raytracing],
         sub_paths={
             'dist_info': 'grid/_redist_info.json',
             'grids_info': 'grids_info.json'
         }
     )
     def post_process_annual_daylight(
-        self, initial_results='initial_results',
+        self, initial_results='initial_results/metrics',
         dist_info=prepare_folder_annual_daylight._outputs.resources,
         grids_info=prepare_folder_annual_daylight._outputs.results,
         model=model
         ):
         return [
             {
                 'from': AnnualDaylightPostProcess()._outputs.metrics,
                 'to': 'metrics'
             },
             {
                 'from': AnnualDaylightPostProcess()._outputs.visualization,
                 'to': 'visualization.vsf'
-            },
+            }
+        ]
+
+    @task(
+        template=MergeFolderData,
+        needs=[prepare_folder_annual_daylight, annual_daylight_raytracing],
+        sub_paths={
+            'dist_info': 'grid/_redist_info.json'
+        }
+    )
+    def restructure_results(
+        self, input_folder='initial_results/final',
+        dist_info=prepare_folder_annual_daylight._outputs.resources,
+        extension='ill'
+    ):
+        return [
             {
-                'from': AnnualDaylightPostProcess()._outputs.results,
+                'from': MergeFolderData()._outputs.output_folder,
                 'to': 'results'
             }
         ]
 
     visualization = Outputs.file(
         source='visualization.vsf',
         description='Result visualization in VisualizationSet format.'
```

### Comparing `pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/PKG-INFO` & `pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight.full
-Version: 0.10.6
+Version: 0.10.7
 Summary: Annual daylight recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
@@ -12,14 +12,23 @@
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-radiance
 Keywords: honeybee,radiance,ladybug-tools,daylight,annual-daylight
 Description-Content-Type: text/markdown
 Provides-Extra: viz
 License-File: LICENSE
 
 # annual-daylight
-Annual daylight recipe for Pollination
+Annual daylight recipe for Pollination.
 
 Use this recipe to calculate annual daylight for a HBJSON model.
 
-This recipe uses an enhanced 2-phase method for daylight simulation with accurate direct sunlight calculation.
+This recipe uses a 2-phase method for daylight simulation. If the accuracy of the direct sunlight is important, you can use the [annual-daylight-enhanced](https://github.com/pollination/annual-daylight-enhanced) recipe.
+
+### Versions
+There are three different versions of the recipe. All three versions use the same simulation methodology and workflow, although their outputs vary.
+| Version | Outputs | PyPI |
+|-|-|-|
+| annual-daylight | <ul><li>annual daylight metrics</li></ul> | [annual-daylight](https://pypi.org/project/pollination-annual-daylight/) |
+| annual-daylight.viz | <ul><li>annual daylight metrics</li><li>visualization</li></ul> | [annual-daylight.viz](https://pypi.org/project/pollination-annual-daylight.viz/) |
+| annual-daylight.full | <ul><li>annual daylight metrics</li><li>visualization</li><li>results folder</li></ul> | [annual-daylight.full](https://pypi.org/project/pollination-annual-daylight.full/) |
+
 
 For more information [see the recipe on Pollination](https://app.pollination.cloud/recipes/ladybug-tools/annual-daylight).
```

### Comparing `pollination-annual-daylight.full-0.10.6/pollination_annual_daylight.full.egg-info/SOURCES.txt` & `pollination-annual-daylight.full-0.10.7/pollination_annual_daylight.full.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight.full-0.10.6/setup.py` & `pollination-annual-daylight.full-0.10.7/setup.py`

 * *Files identical despite different names*

