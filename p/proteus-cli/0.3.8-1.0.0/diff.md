# Comparing `tmp/proteus_cli-0.3.8.tar.gz` & `tmp/proteus_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.3.8.tar", max compression
+gzip compressed data, was "proteus_cli-1.0.0.tar", max compression
```

## Comparing `proteus_cli-0.3.8.tar` & `proteus_cli-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,49 @@
--rw-r--r--   0        0        0     3083 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/buckets/commands.py
--rw-r--r--   0        0        0     2810 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/config.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.060060 proteus_cli-0.3.8/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      958 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3251 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    14707 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4944 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8656 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     5927 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2809 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9158 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-06-20 17:12:06.064059 proteus_cli-0.3.8/logging.ini
--rw-r--r--   0        0        0     1530 2023-06-20 17:12:06.068058 proteus_cli-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     3124 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2810 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/config.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1277 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0     6754 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0     1068 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/case.py
+-rw-r--r--   0        0        0     2381 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/common.py
+-rw-r--r--   0        0        0      142 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/cnn_pca/step.py
+-rw-r--r--   0        0        0      167 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/__init__.py
+-rw-r--r--   0        0        0     2762 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/case.py
+-rw-r--r--   0        0        0     1415 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/common.py
+-rw-r--r--   0        0        0      145 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/step.py
+-rw-r--r--   0        0        0      673 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    12408 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     7051 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0      411 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     8822 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0     1289 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     3895 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     6930 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.302471 proteus_cli-1.0.0/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/simulations/opm.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/__init__.py
+-rw-r--r--   0        0        0     8114 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/files.py
+-rw-r--r--   0        0        0      385 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/sssh.py
+-rw-r--r--   0        0        0     1917 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/cli/utils/sync.py
+-rw-r--r--   0        0        0      449 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/logging.ini
+-rw-r--r--   0        0        0     1528 2023-07-06 16:46:13.306470 proteus_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 proteus_cli-1.0.0/PKG-INFO
```

### Comparing `proteus_cli-0.3.8/cli/__init__.py` & `proteus_cli-1.0.0/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from cli.buckets.commands import buckets as buckets_commands
 from cli.config import config
 from cli.datasets.commands import datasets as datasets_commands
 from cli.debugger.commands import debugger as debugger_commands
 from cli.jobs.commands import jobs as jobs_commands
 from cli.runtime import proteus
 from cli.simulations.commands import simulations as simulations_commands
+from cli.utils import sssh  # noqa: F401
 
 ENTITY_INFO = next(
     (
         x.groupdict()
         for x in re.finditer(
             r"^/api/v[12]/(?P<entity_name>[^/]+)/(?P<entity_id>[a-fA-F0-9\-]+)/?$", config.ENTITY_URL or ""
         )
```

### Comparing `proteus_cli-0.3.8/cli/api/decorators.py` & `proteus_cli-1.0.0/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/api/hooks.py` & `proteus_cli-1.0.0/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/buckets/commands.py` & `proteus_cli-1.0.0/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/config.py` & `proteus_cli-1.0.0/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/datasets/commands.py` & `proteus_cli-1.0.0/cli/datasets/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     """
 
 
 @datasets.command()
 @click.option("--workers", prompt=config.PROMPT, default=config.WORKERS_COUNT)
 @click.option("--user", prompt=config.USERNAME is None, default=config.USERNAME)
 @click.option("--password", prompt=config.PASSWORD is None, default=config.PASSWORD, hide_input=True)
-@click.option("--replace/--no-replace", default=False)
 @click.option("--allow-missing-file", "-m", multiple=True)
 @click.option("--temp-folder-override", "-t", multiple=False)
 @click.argument("bucket")
 @click.argument("dataset_uuid")
 @may_fail_on_http_error(exit_code=1)
 @proteus.runs_authentified
 def upload(
```

### Comparing `proteus_cli-0.3.8/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-1.0.0/cli/datasets/preprocessor/config/well_model/case.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,78 @@
 import json
 import os
 
-from ..default import DefaultConfig
-from ...utils import RequiredFilePath
+from cli.datasets.preprocessor.config import BaseConfig, CaseStepConfig
+from cli.datasets.preprocessor.config.well_model import SMSPEC_WELL_KEYWORDS, SMSPEC_FIELD_KEYWORDS
+from cli.datasets.preprocessor.preprocess_functions import (
+    export_egrid_properties,
+    export_well_init_properties,
+    export_smspec,
+)
+from cli.utils.files import RequiredFilePath, OptionalFilePath
 
-SMSPEC_WELL_KEYWORDS = ["WOPR", "WOPRH", "WWPR", "WWPRH", "WGPR", "WWIR", "WBHP", "WBHPH"]
-SMSPEC_FIELD_KEYWORDS = ["FOPR", "FWPR", "FGPR", "FOPRH", "FWPRH", "FGPRH"]
 
+class WellModelCaseConfig(BaseConfig):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-class WellModelCaseConfig(DefaultConfig):
-    """Configuration generator for the cases"""
+        dir_path = os.path.dirname(os.path.abspath(__file__))
+        with open(os.path.join(dir_path, "../../well_init_keywords.json")) as file:
+            self.init_keywords = json.load(file)
 
     def step_1_grid_props(self):
-        """
-        List all cases and its steps to generate the .EGRID iterator
-
-        Args: -
 
-        Returns:
-            iterator: the list of steps to preprocess
-        """
-        return (
-            {
-                "input": [f'{case["root"]}/*.EGRID'],
-                "output": [f'{case["root"]}/grid.h5'],
-                "preprocessing": "export_egrid_properties",
-                "split": case["group"],
-                "case": case["number"],
-                "keep": True,
-            }
+        return tuple(
+            CaseStepConfig(
+                input=(
+                    RequiredFilePath(
+                        "*.EGRID", download_name="egrid", replace_with=RequiredFilePath("*.DATA", download_name="data")
+                    ),
+                ),
+                output=(RequiredFilePath("grid.h5"),),
+                root=case["root"],
+                preprocessing_fn=export_egrid_properties,
+                split=case["group"],
+                case=case["number"],
+                keep=False,
+                enabled=True,
+            )
             for case in self.cases
         )
 
     def step_2_init_props(self):
-        """
-        List all cases and its steps to generate the .INIT iterator
-
-        Args: -
 
-        Returns:
-            iterator: the list of steps to preprocess
-        """
-        init_keywords = []
-        dir_path = os.path.dirname(os.path.realpath(__file__))
-        with open(os.path.join(dir_path, "../../well_init_keywords.json")) as file:
-            init_keywords = json.load(file)
-
-        return (
-            {
-                "input": [
-                    RequiredFilePath(f'{case["root"]}/*.INIT', download_name="init"),
-                    RequiredFilePath(f'{case["root"]}/*.EGRID', download_name="grid"),
-                ],
-                "output": list(
-                    map(
-                        lambda output: f'{case["root"]}/{output.get("filename")}',
-                        init_keywords,
-                    )
+        return tuple(
+            CaseStepConfig(
+                input=(
+                    RequiredFilePath("*.INIT", download_name="init"),
+                    RequiredFilePath("*.EGRID", download_name="grid"),
                 ),
-                "preprocessing": "export_well_init_properties",
-                "split": case["group"],
-                "case": case["number"],
-                "keep": True,
-                "additional_info": {"get_endpoint": self._get_endpoint},
-            }
+                output=tuple(RequiredFilePath(output.get("filename")) for output in self.init_keywords),
+                root=case["root"],
+                preprocessing_fn=export_well_init_properties,
+                split=case["group"],
+                case=case["number"],
+                keep=False,
+                enabled=True,
+            )
             for case in self.cases
         )
 
     def step_3_smspec(self):
-        """
-        List all cases and its steps to generate the Summaries iterator
 
-        Args: -
-
-        Returns:
-            iterator: the list of steps to preprocess
-        """
-        return (
-            {
-                "input": [
-                    RequiredFilePath(f'{case["root"]}/*.SMSPEC', download_name="smspec"),
-                ]
-                + [
-                    RequiredFilePath(f'{case["root"]}/*.S{str(step).zfill(4)}', download_name="s")
+        return tuple(
+            CaseStepConfig(
+                input=(RequiredFilePath("*.SMSPEC", download_name="smspec"),)
+                + tuple(
+                    RequiredFilePath(f"*.S{str(step).zfill(4)}", download_name="s")
                     for step in range(case["initialStep"] + 1, case["finalStep"] + 1)
-                ],
-                "output": [f'{case["root"]}/{k}.h5' for k in SMSPEC_WELL_KEYWORDS + SMSPEC_FIELD_KEYWORDS],
-                "preprocessing": "export_smspec",
-                "split": case["group"],
-                "case": case["number"],
-            }
+                ),
+                output=tuple(OptionalFilePath(f"{k}.h5") for k in SMSPEC_WELL_KEYWORDS + SMSPEC_FIELD_KEYWORDS),
+                root=case["root"],
+                preprocessing_fn=export_smspec,
+                split=case["group"],
+                keep=False,
+                case=case["number"],
+            )
             for case in self.cases
         )
```

### Comparing `proteus_cli-0.3.8/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-1.0.0/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-1.0.0/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import json
 import os
 import pickle
+from threading import RLock
+from typing import Callable, Sequence
 
 import cwrap
 import h5py
 import numpy as np
 from ecl.eclfile import EclInitFile, EclFile
 from ecl.grid import EclGrid
 from ecl.summary import EclSum
+
+from cli.datasets.preprocessor.config.well_model import SMSPEC_WELL_KEYWORDS, SMSPEC_FIELD_KEYWORDS
+from cli.utils.files import upload_file, find_ext, PathMeta
 from preprocessing.deck import ecl_deck
 from preprocessing.deck.runspec import preprocess as preprocess_runspec
 from preprocessing.deck.section import find_section, get_includes
 from preprocessing.modular import dat
 from preprocessing.modular.data import WellSpecsProcessor
 from preprocessing.modular.egrid import preprocess as preprocess_egrid
 from preprocessing.modular.grdecl import preprocess as preprocess_grdecl
 from preprocessing.modular.init import preprocess as preprocess_init
 from preprocessing.modular.s import WellSummaryProcessor
 from preprocessing.modular.x import preprocess as preprocess_x
-
-from .config.case.well_model import SMSPEC_WELL_KEYWORDS, SMSPEC_FIELD_KEYWORDS
-from .utils import upload_file, find_ext, find_file, get_case_info
+from ..sources.local import LocalSource
 from ... import proteus
 
 DEFAULT_COMMON_PROPERTIES = {"max_pressure": -100000, "min_pressure": 100000}
 
 
 def extract_casename(case_loc):
     return os.path.basename(case_loc)
@@ -97,129 +100,95 @@
     return common_loc
 
 
 def export_deck(case_loc, case_dest_loc, _, source, cases_url, group, number):
     root_folder = case_dest_loc.split("/cases/")[0]
     ecl_deck_loc = os.path.join(root_folder, "ecl_deck.p")
 
-    case = get_case_info(f"{cases_url}/{group}/{number}")
-    min = int(case.get("initialStep")) - 1
-    max = case.get("finalStep")
-    props = {"size": max - min, "min": min, "max": max}
+    case = proteus.api.get(f"{cases_url}/{group}/{number}").json().get("case")
+
+    min_step = int(case.get("initialStep")) - 1
+    max_step = case.get("finalStep")
+    props = {"size": max_step - min_step, "min": min_step, "max": max_step}
     write_pickle_from_dict(props, ecl_deck_loc)
 
     return None, ecl_deck_loc, None
 
 
 def export_runspec(
-    case_loc,
-    case_dest_loc,
-    input_src,
-    source,
-    cases_url,
-    set_endpoint,
-    allow_missing_files=tuple(),
-    base_dir=None,
-    *_,
+    download_func: Callable,
+    output_source: LocalSource,
+    data: PathMeta,
+    init: PathMeta = None,
+    egrid: PathMeta = None,
+    smspec: PathMeta = None,
+    allow_missing_files: Sequence[str] = tuple(),
+    **_,
 ):
-    runspec_dest_loc = os.path.join(base_dir, "runspec.p")
-
-    data_file_loc = None
-    egrid_file_loc = None
-    smspec_file_loc = None
-    init_file_loc = None
-
-    if isinstance(input_src, dict):
-        data_file_loc = next(iter(input_src.get("data") or []), None)
-        init_file_loc = next(iter(input_src.get("init") or []), None)
-        egrid_file_loc = next(iter(input_src.get("grid") or []), None)
-        smspec_file_loc = next(iter(input_src.get("smspec") or []), None)
-
-    if data_file_loc is None:
-        data_file_loc = find_ext(case_loc, "DATA", required=True, one=True)
-    if egrid_file_loc is None:
-        egrid_file_loc = find_ext(case_loc, "EGRID", first=True, required=False)
-    if smspec_file_loc is None:
-        smspec_file_loc = find_ext(case_loc, "SMSPEC", first=True, required=False)
-    if init_file_loc is None:
-        init_file_loc = find_ext(case_loc, "INIT", required=False)
-
-    def download_func(source_path, destination_path):
-        from .utils import download_file
-
-        download_file(source_path, destination_path, source)
+    runspec_dest_loc = os.path.join(output_source.uri, "runspec.p")
 
     data = preprocess_runspec(
-        data_file_loc,
-        egrid_file_loc=egrid_file_loc,
-        smspec_file_loc=smspec_file_loc,
+        data.full_path,
+        egrid_file_loc=egrid and egrid.full_path,
+        smspec_file_loc=smspec and smspec.full_path,
+        init_file_loc=init and init.full_path,
         download_func=download_func,
-        init_file_loc=init_file_loc,
         allow_missing_files=allow_missing_files,
-        base_dir=base_dir,
     )
 
     multout = data.get("multout")
     del data["multout"]
     if not multout:
         proteus.logger.warning("MULTOUT not found in RUNSPEC section. This can lead to issues.")
 
     write_pickle_from_dict(data, runspec_dest_loc)
 
-    set_endpoint(data.get("endscale"))
-
-    return data_file_loc, runspec_dest_loc, None
-
 
 """ Cases preprocessing """
 
 
-def export_egrid_properties(case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=tuple(), base_dir=None):
+def export_egrid_properties(
+    download_func: Callable, output_source: LocalSource, data: PathMeta = None, egrid: PathMeta = None, **_
+):
+    if not data and not egrid:
+        raise RuntimeError("Either data or egrid files are needed")
 
-    if getattr(input_src, "download_name", None) == "data":
-        return _export_egrid_properties_from_data(
-            case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=allow_missing_files, base_dir=base_dir
-        )
+    if data:
+        _export_egrid_properties_from_data(data.full_path, download_func=download_func, base_dir=output_source.uri)
     else:
-        return _export_egrid_properties_from_egrid(case_loc, case_dest_loc, input_src, *_)
+        _export_egrid_properties_from_egrid(egrid.full_path, base_dir=output_source.uri)
 
 
 def _export_egrid_properties_from_data(
-    case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=tuple(), base_dir=None
+    input_src,
+    download_func,
+    base_dir=None,
+    allow_missing_files=tuple(),
 ):
-    def download_func(source_path, destination_path):
-        from .utils import download_file
 
-        download_file(source_path, destination_path, source)
-
-    get_includes(input_src.full_path, download_func, allow_missing_files=allow_missing_files, base_dir=base_dir)
+    get_includes(input_src, download_func, allow_missing_files=allow_missing_files)
 
     grid = ecl_deck.extract_actnum(input_src.full_path)
-    grid_dest_loc = os.path.join(case_dest_loc, "grid.h5")
+    grid_dest_loc = os.path.join(base_dir, "grid.h5")
     props = preprocess_egrid(grid)
     write_h5_from_dict(props, grid_dest_loc)
 
-    return None, grid_dest_loc, None
-
 
-def _export_egrid_properties_from_egrid(case_loc, case_dest_loc, input_src, *_):
-
-    if getattr(input_src, "full_path", None):
-        grid_src_loc = getattr(input_src, "full_path", None)
-    else:
-        grid_src_loc = find_ext(case_loc=case_loc, ext="EGRID", required=True, one=True)
+def _export_egrid_properties_from_egrid(
+    input_src,
+    base_dir=None,
+    allow_missing_files=tuple(),
+):
 
-    grid_dest_loc = os.path.join(case_dest_loc, "grid.h5")
+    grid_dest_loc = os.path.join(base_dir, "grid.h5")
 
-    grid = EclGrid(str(grid_src_loc))
+    grid = EclGrid(str(input_src))
     props = preprocess_egrid(grid)
     write_h5_from_dict(props, grid_dest_loc)
 
-    return None, grid_dest_loc, None
-
 
 def export_init_properties(
     case_loc,
     case_dest_loc,
     input_src,
     source,
     cases_url,
@@ -230,64 +199,39 @@
     init_src_loc = find_ext(case_loc=case_loc, ext="INIT")
 
     grid = EclGrid(str(grid_src_loc))
     init = EclInitFile(grid, str(init_src_loc))
     endpoint_scaling = get_endpoint()
     props = preprocess_init(init, endpoint_scaling)
 
-    dir_path = os.path.dirname(os.path.realpath(__file__))
+    dir_path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(dir_path, "init_keywords.json")) as file:
         init_keywords = json.load(file)
 
     for init_keyword in init_keywords:
         keywords = {k: props.get(k, []) for k in init_keyword.get("keywords")}
         file_dest_loc = os.path.join(case_dest_loc, init_keyword.get("filename"))
         write_h5_from_dict(keywords, file_dest_loc)
 
-    return init_src_loc, case_dest_loc, None
-
-
-def export_well_init_properties(
-    case_loc,
-    case_dest_loc,
-    input_src,
-    source,
-    cases_url,
-    get_endpoint,
-    *args,
-):
-
-    init_src_loc = None
-    grid_src_loc = None
 
-    if isinstance(input_src, dict):
-        grid_src_loc = next(iter(input_src.get("grid") or []), None)
-        init_src_loc = next(iter(input_src.get("init") or []), None)
-
-    if init_src_loc is None:
-        init_src_loc = find_ext(case_loc=case_loc, ext="INIT", required=True, one=True)
-    if grid_src_loc is None:
-        grid_src_loc = find_ext(case_loc=case_loc, ext="EGRID", required=True, one=True)
+def export_well_init_properties(output_source: LocalSource, grid, init, **_):
 
-    grid = EclGrid(str(grid_src_loc))
-    init = EclInitFile(grid, str(init_src_loc))
-    endpoint_scaling = get_endpoint()
-    props = preprocess_init(init, endpoint_scaling)
+    grid = EclGrid(str(grid.full_path))
+    init = EclInitFile(grid, str(init.full_path))
+    props = preprocess_init(init, False)
 
-    dir_path = os.path.dirname(os.path.realpath(__file__))
+    dir_path = os.path.dirname(os.path.abspath(__file__))
     with open(os.path.join(dir_path, "well_init_keywords.json")) as file:
         init_keywords = json.load(file)
 
     for init_keyword in init_keywords:
         keywords = {k: props.get(k, []) for k in init_keyword.get("keywords")}
-        file_dest_loc = os.path.join(case_dest_loc, init_keyword.get("filename"))
+        file_dest_loc = os.path.join(output_source.uri, init_keyword.get("filename"))
         write_h5_from_dict(keywords, file_dest_loc)
 
-    return init_src_loc, case_dest_loc, None
-
 
 def export_litho(
     case_loc,
     case_dest_loc,
     input_src,
     source,
     cases_url,
@@ -321,76 +265,62 @@
             props = preprocess_grdecl(f, mapping)
 
         _write_keywords_to_h5(props, case_dest_loc)
 
     return grdecl_src_loc, case_dest_loc, None
 
 
-def export_dat_properties(
-    case_loc,
-    case_dest_loc,
-    input_src,
-    source,
-    cases_url,
-    get_mapping,
-    *args,
-):
-    dat_src_locs = [str(find_file(case_loc, src.split("/")[-1])) for src in input_src[None]]
-    mapping = get_mapping()
+EXPORT_DAT_PROPERTIES_LOCK = RLock()
 
-    dat_files = {}
-    for keyword in mapping:
-        source = keyword.get("source", keyword["name"])
-        file = next(
-            filter(lambda f: f"{source}.dat" in f, dat_src_locs),
-            None,
-        )
-        if file:
-            dat_files[keyword["name"]] = file
 
-    props = dat.preprocess(dat_files, mapping)
+def export_dat_properties(output_source: LocalSource, input_files: Sequence[PathMeta], **_):
+    dat_src_locs = {f"{f.full_path}": f"{f.download_name}" for f in input_files}
 
-    _write_keywords_to_h5(props, case_dest_loc)
+    # Loading dat files can be heavy and consume a lot of memory. Ensure 2 steps are not loading
+    # dat data in memory at the same time
+    with EXPORT_DAT_PROPERTIES_LOCK:
+        case_dest_loc = []
+        # Dat files can be very big. Write them individually to reduce memory usage
+        for source, col_name, df in dat.preprocess(dat_src_locs):
+            case_dest_loc.append(_write_keywords_to_h5({col_name: source}, output_source.uri)[0])
 
     return dat_src_locs, case_dest_loc, None
 
 
 def _write_keywords_to_h5(props, dest_loc):
+    locations = []
     for k, v in props.items():
         file_dest_loc = os.path.join(dest_loc, f"{k}.h5")
         write_h5_from_dict({k: v}, file_dest_loc)
+        locations.append(file_dest_loc)
 
+    return locations
 
-def export_wellspec(case_loc, case_dest_loc, _, source, *args, allow_missing_files=tuple(), base_dir=None):
-    runspec_dest_loc = os.path.join(case_dest_loc, "well_spec.p")
-    data_src_loc = find_ext(case_loc, "DATA")
-
-    def download_func(source_path, destination_path):
-        from .utils import download_file
-
-        download_file(source_path, destination_path, source)
 
+def export_wellspec(data: PathMeta, download_func, output_source: LocalSource, allow_missing_files=tuple(), **_):
     # Read and download data includes
-    find_section(data_src_loc, "RUNSPEC", download_func, allow_missing_files=allow_missing_files, base_dir=base_dir)
+    find_section(data.full_path, "RUNSPEC", download_func, allow_missing_files=allow_missing_files)
 
-    preprocessor = WellSpecsProcessor(data_src_loc)
-    data = preprocessor.process()
+    wellspec_dest_loc = os.path.join(output_source.uri, "well_spec.p")
 
-    write_pickle_from_dict(data, runspec_dest_loc)
+    preprocessor = WellSpecsProcessor(data.full_path)
+    wellspec_data = preprocessor.process()
 
-    return data_src_loc, runspec_dest_loc, None
+    write_pickle_from_dict(wellspec_data, wellspec_dest_loc)
+
+    return data.full_path, wellspec_dest_loc, None
 
 
 def export_smry(case_loc, case_dest_loc, _, source, *args, allow_missing_files=tuple(), base_dir=None):
     preprocessed_smry_dest_loc = os.path.join(case_dest_loc, "preprocessed_smry.h5")
     raw_smry_dest_loc = os.path.join(case_dest_loc, "raw_smry.h5")
     data_src_loc = find_ext(case_loc, "DATA")
 
     def download_func(source_path, destination_path):
-        from .utils import download_file
+        from cli.utils.files import download_file
 
         download_file(source_path, destination_path, source)
 
     # Read and download data includes
     find_section(data_src_loc, "RUNSPEC", download_func, allow_missing_files=allow_missing_files, base_dir=base_dir)
 
     case_name = extract_casename(case_loc)
@@ -400,47 +330,39 @@
 
     preprocessed_smry.to_hdf(preprocessed_smry_dest_loc, key="df", format="fixed", mode="w")
     raw_smry.to_hdf(raw_smry_dest_loc, key="df", format="fixed", mode="w")
 
     return f"{smry_src_loc}.S????", preprocessed_smry_dest_loc, None
 
 
-def export_smspec(case_loc, case_dest_loc, input_src, source, *args):
-
-    smspec_file_loc = None
-
-    if isinstance(input_src, dict):
-        smspec_file_loc = next(iter(input_src.get("smspec") or []), None)
-
-    if smspec_file_loc is None:
-        smspec_file_loc = find_ext(case_loc=case_loc, ext="SMSPEC", required=True, one=True)
+def export_smspec(output_source: LocalSource, smspec, **_):
 
-    smry = EclSum(str(smspec_file_loc))
+    smry = EclSum(str(smspec.full_path))
 
     wnames = np.array(list(smry.wells()))
 
     for key in SMSPEC_WELL_KEYWORDS:
-        with h5py.File(os.path.join(case_dest_loc, f"{key}.h5"), "w") as h5f:
+        with h5py.File(os.path.join(output_source.uri, f"{key}.h5"), "w") as h5f:
             for i, w in enumerate(wnames):
                 try:
                     data = smry.numpy_vector(f"{key}:{w}", report_only=True)
                     h5f.create_dataset(w, data=data)
                 except KeyError:
                     # Some keywords may be missing, the correct behaviour is to not create a dataset
                     pass
 
     for key in SMSPEC_FIELD_KEYWORDS:
-        with h5py.File(os.path.join(case_dest_loc, f"{key}.h5"), "w") as h5f:
+        with h5py.File(os.path.join(output_source.uri, f"{key}.h5"), "w") as h5f:
             try:
                 data = smry.numpy_vector(key, report_only=True)
                 h5f.create_dataset(key, data=data)
             except KeyError:
                 pass
 
-    return smspec_file_loc, None, None
+    return smspec, None, None
 
 
 """ Steps preprocessing """
 
 
 def export_x_file(case_src_loc, _, input, *args):
     x_src_loc = os.path.join(case_src_loc, input.split("/")[-1])
```

### Comparing `proteus_cli-0.3.8/cli/datasets/preprocessor/utils.py` & `proteus_cli-1.0.0/cli/utils/files.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import datetime
 import os
 import platform
-import time
+import re
 from pathlib import Path
+from threading import RLock
 
-from tqdm import tqdm
-
-from ... import proteus
+from cli import proteus
+from cli.api.hooks import TqdmUpWithReport
+from cli.utils.sync import TaskDependencySemaphore
 
 
 def get_creation_date(path_to_file):
     """
     Calculate the creation date of a file in the system
 
     Args:
@@ -27,118 +28,126 @@
             return datetime.datetime.fromtimestamp(stat.st_birthtime)
         except AttributeError:
             # We're probably on Linux. No easy way to get creation dates here,
             # so we'll settle for when its content was last modified.
             return datetime.datetime.fromtimestamp(stat.st_mtime)
 
 
-def download_file(source_path, destination_path, source, progress=False):
+DOWNLOAD_FILE_LOCK = RLock()
+DOWNLOAD_FILE_SEMAPHORES = {}
+
+
+def download_file(source_path, destination_path, input_source, progress: TqdmUpWithReport = None):
     """
     Download a file from the allowed providers. Ex: local, az, etc.
 
     Args:
         source (string): The url from which we are going to
             download the file
         source_path (string): Path of the file inside the source
         destination_path (string): Path where we are going to
             save the file
 
     Returns: -
     """
-    # Preserve RequiredFilePath with input.__class__
-    source_path = source_path.__class__(source_path.replace("\\", "/"))
+
+    # First, resolve which files have to be downloaded
+    source_path = getattr(source_path, "clone", source_path.__class__)(source_path.replace("\\", "/"))
     destination_path = destination_path.replace("\\", "/")
     if "*" in source_path:
         prefix, suffix = source_path.split("*", 1)
         if "*" in suffix:
             raise RuntimeError("A file path can not include more than one glob symbol ('*')")
-        items_and_paths = list(source.list_contents(starts_with=prefix, ends_with=suffix))
+        items_and_paths = list(input_source.list_contents(starts_with=prefix, ends_with=suffix))
 
         if len(items_and_paths) > 1:
             globbed_paths = ",".join(str(x) for x in items_and_paths)
-            raise RuntimeError(f'"f{source_path}" defines more than one file: {globbed_paths}')
+            raise RuntimeError(f'"{source_path}" defines more than one file: {globbed_paths}')
 
         cannot_resolve_glob = (
             len(items_and_paths) > 1 or len(items_and_paths) == 0 and isinstance(source_path, RequiredFilePath)
         )
         if cannot_resolve_glob:
             raise FileNotFoundError(f'Cannot resolve glob "{source_path}"')
 
         assert len(destination_path.split("*")) in (1, 2)
 
         if items_and_paths:
-            glob_replacement_in_destination_path = suffix.join(
-                items_and_paths[0].path.split(prefix, 1)[1].split(suffix)[:-1]
-            )
+            asterisk_replace_with = items_and_paths[0].path_rel
+            if prefix:
+                asterisk_replace_with = re.sub(rf"^{prefix}", "", asterisk_replace_with)
+            if suffix:
+                asterisk_replace_with = re.sub(rf"{suffix}$", "", asterisk_replace_with)
+
+            transformed_source_path = source_path.replace("*", asterisk_replace_with)
 
             if "*" in destination_path:
-                destination_path_parts = destination_path.split("*")
-                destination_path = (
-                    destination_path_parts[0] + glob_replacement_in_destination_path + destination_path_parts[1]
-                )
-
-            if "*" in source_path:
-                transformed_source_path = prefix + glob_replacement_in_destination_path + suffix
-            else:
-                transformed_source_path = source_path
+                destination_path = destination_path.replace("*", asterisk_replace_with)
 
             proteus.logger.info(
-                f'Glob "{source_path}" resolved to {items_and_paths[0]}. Output path rewritten to f{destination_path}'
+                f'Glob "{source_path}" resolved to {items_and_paths[0].path}. '
+                f"Output path rewritten to {destination_path}"
             )
 
         items_and_paths = iter(items_and_paths)
     else:
-        items_and_paths = source.list_contents(starts_with=source_path)
+        assert "*" not in destination_path, "* can only be used in destionation path if also present in source_path"
+
+        items_and_paths = input_source.list_contents(starts_with=source_path)
         transformed_source_path = source_path
 
-    path_list = destination_path.split("/")[0:-1]
-    Path("/".join(path_list)).mkdir(parents=True, exist_ok=True)
+    destination_path = os.path.abspath(destination_path)
 
-    if os.path.isfile(destination_path):
-        return transformed_source_path, destination_path
-    elif os.path.isfile(f"{destination_path}.tmp"):
-        wait_until_file_is_downloaded(destination_path)
-        return transformed_source_path, destination_path
-    else:
-        try:
-            _, path, reference, size = next(items_and_paths)
+    Path(os.path.dirname(destination_path)).mkdir(parents=True, exist_ok=True)
 
-            destination_file = f"{destination_path}.tmp"
+    # Create a semaphore for each file to be downloaded so that multiple download
+    # processes for the same file cannot start at the same time.
+    with DOWNLOAD_FILE_LOCK:
+        file_semaphore = DOWNLOAD_FILE_SEMAPHORES.get(destination_path)
+        if not file_semaphore:
+            file_semaphore = TaskDependencySemaphore()
+            DOWNLOAD_FILE_SEMAPHORES[destination_path] = file_semaphore
+
+    try:
+        file_semaphore.acquire()
+
+        if os.path.isfile(destination_path):
+            file_semaphore.release()
+            return transformed_source_path, destination_path, True
+
+        _, path, reference, size = next(items_and_paths)
+
+        temp_dst_path = f"{destination_path}.tmp"
+
+        if progress:
+            progress.set_postfix({"downloading": reference.name})
+
+        if not input_source.fastcopy(reference, temp_dst_path):
+            Path(f"{destination_path}.tmp").touch()
+
+            with open(f"{destination_path}.tmp", "wb") as file:
+                for chunk in input_source.chunks(reference):
+                    file.write(chunk)
+
+        try:
+            os.rename(temp_dst_path, destination_path)
+        except FileNotFoundError:
+            if not os.path.exists(destination_path):
+                raise
 
-            if not source.fastcopy(reference, destination_file):
-                Path(f"{destination_path}.tmp").touch()
+        progress.set_postfix({})
 
-                if callable(size):
-                    size = callable(size)
-
-                with open(f"{destination_path}.tmp", "wb") as file:
-                    with tqdm(
-                        total=size,
-                        unit="B",
-                        unit_scale=True,
-                        unit_divisor=1024,
-                        desc=f"Retrieving file {path}",
-                        disable=not progress,
-                    ) as pbar:
-                        read = 0
-                        for chunk in source.chunks(reference):
-                            file.write(chunk)
-                            read += len(chunk)
-                            pbar.update(len(chunk))
-
-                        pbar.set_description("Done")
-
-            os.rename(f"{destination_path}.tmp", destination_path)
-
-            return transformed_source_path, destination_path
-        except StopIteration:
-            if isinstance(source_path, RequiredFilePath):
-                raise FileNotFoundError(f"Required file {source_path} is not found")
-            proteus.logger.error(f"The following file was not found: {source_path}")
-            return None, None
+        return transformed_source_path, destination_path, False
+    except StopIteration:
+        if isinstance(source_path, RequiredFilePath):
+            raise FileNotFoundError(f"Required file {source_path} is not found")
+        proteus.logger.error(f"The following file was not found: {source_path}")
+        return None, None, False
+    finally:
+        file_semaphore.release()
 
 
 @proteus.may_insist_up_to()
 def upload_file(source_path, file_path, url):
     """
     Upload a file to proteus
 
@@ -150,21 +159,14 @@
     Returns: -
     """
     modified = get_creation_date(file_path)
     file_path = Path(file_path)
     proteus.api.post_file(url, source_path, content=file_path, modified=modified, retry=False)
 
 
-""" Destructuring helper function of an object """
-
-
-def pluck(dict, *args):
-    return (dict.get(arg, None) for arg in args)
-
-
 def find_ext(case_loc, ext, required=False, one=False, first=True, last=False):
     """
     Finds if file exists in the directory
     Args:
         case_loc (string): Path of the folder
         ext (string): Extension of the file to find
         required (bool): Fails if no file is found
@@ -204,38 +206,14 @@
         name (string): File name plus extension
 
     Returns: file_path (string): Path of the file if exists
     """
     return next(Path(case_loc).rglob(name))
 
 
-def wait_until_file_is_downloaded(file_path, period=5, timeout=500):
-    """
-    Waits until the file is completely downloaded
-    Args:
-        case_loc (string): Path of the folder
-        ext (string): Extension of the file to find
-
-    Returns: file_path (string): Path of the file if exists
-    """
-    mustend = time.time() + timeout
-    while time.time() < mustend:
-        try:
-            with open(file_path, "rb") as _:
-                return True
-        except FileNotFoundError:
-            time.sleep(period)
-    return False
-
-
-def get_case_info(case_url):
-    r = proteus.api.get(case_url)
-    return r.json().get("case")
-
-
 class PathMeta(str):
     download_name = None
     cloned_from = None
     full_path = None
     replace_with = None
     replaces = None
```

### Comparing `proteus_cli-0.3.8/cli/datasets/sources/az.py` & `proteus_cli-1.0.0/cli/datasets/sources/az.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from azure.core.credentials import AzureSasCredential
 from azure.core.exceptions import HttpResponseError, ClientAuthenticationError
 from azure.identity import DefaultAzureCredential
 from azure.storage.blob import ContainerClient
 
 from cli.config import config
+from proteus.bucket import AZ_COPY_PRESENT, AzCopyError
 from .common import Source, SourcedItem
 from ... import proteus
 
 AZURE_SAS_TOKEN = config.AZURE_SAS_TOKEN
 
 CONTENT_CHUNK_SIZE = 10 * 1024 * 1024
 
@@ -22,43 +23,73 @@
     )
 
     SAS_TOKEN_COMPONENTS = {"sv", "se", "sr", "sp"}
 
     CLIENT_INIT_PARAMS = {"max_single_get_size": 256 * 1024 * 1024, "max_chunk_get_size": 128 * 1024 * 1024}
     MAX_CONCURRENCY = 10
 
-    def __init__(self, uri):
+    def __init__(self, uri, original_uri=None, container_client=None):
+
+        if original_uri:
+            (
+                self.original_container_name,
+                self.original_storage_url,
+                self.original_subpath,
+                _,
+                self.original_uri,
+            ) = self._parse_uri(original_uri)
+        else:
+            self.original_uri = None
+            self.original_storage_url = None
+            self.original_subpath = None
+
+        self.container_name, self.storage_url, self.subpath, self.url_sas_token, uri = self._parse_uri(uri)
+
         super().__init__(uri)
+
+        if container_client is not None:
+            self.container_client = container_client
+        else:
+            self._init_container_client()
+
+    def _parse_uri(self, uri):
         match = self.URI_re.match(uri.rstrip("/"))
-        assert match is not None, f"{uri} must be an s3 URI"
+        assert match is not None, f"{uri} must be a blob storage URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
+        subpath = match.groupdict()["prefix"].split("?")[0].rstrip("/")
 
-        errors = []
+        uri_parts = iter(uri.split("?"))
+
+        uri = next(uri_parts)
+        url_sas_token = next(uri_parts, "")
+
+        return container_name, storage_url, subpath, url_sas_token, uri
+
+    def _init_container_client(self):
+        url_sas_token_components = set(x.split("=")[0] for x in self.url_sas_token.split("&") if x)
 
-        # Check first if the URI include credentials as SAS url
-        url_sas_token = next(iter(uri.split("?")[1:]), "")
-        url_sas_token_components = set(x.split("=")[0] for x in url_sas_token.split("&") if x)
+        errors = []
 
         if self.SAS_TOKEN_COMPONENTS.intersection(url_sas_token_components) == self.SAS_TOKEN_COMPONENTS:
             self.container_client = ContainerClient.from_container_url(
-                f"{storage_url}/{container_name}?" + uri.split("?")[1], **self.CLIENT_INIT_PARAMS
+                f"{self.storage_url}/{self.container_name}?" + self.url_sas_token, **self.CLIENT_INIT_PARAMS
             )
             try:
                 next(self.container_client.list_blobs())
                 return
             except ClientAuthenticationError as e:
                 errors.append(e)
 
         # Try to see if there is a general SAS token
         if AZURE_SAS_TOKEN:
             self.container_client = ContainerClient(
-                storage_url,
+                self.storage_url,
                 credential=AzureSasCredential(AZURE_SAS_TOKEN),
-                container_name=container_name,
+                container_name=self.container_name,
                 **self.CLIENT_INIT_PARAMS,
             )
 
             try:
                 next(self.container_client.list_blobs())
                 return
             except ClientAuthenticationError as e:
@@ -77,17 +108,17 @@
 
         for auth_method in auth_methods:
             try:
                 flags = {auth: True for auth in auth_methods}
                 flags[auth_method] = False
 
                 self.container_client = ContainerClient(
-                    storage_url,
+                    self.storage_url,
                     credential=DefaultAzureCredential(**flags),
-                    container_name=container_name,
+                    container_name=self.container_name,
                     **self.CLIENT_INIT_PARAMS,
                 )
 
                 next(self.container_client.list_blobs())
 
                 return
             except ClientAuthenticationError as e:
@@ -96,40 +127,48 @@
         for error in errors:
             proteus.logger.error(error)
 
         raise RuntimeError("Cannot authenticate into azure")
 
     @proteus.may_insist_up_to(5, 1)
     def list_contents(self, starts_with="", ends_with=None):
-        bucket_uri = self.uri
-        match = self.URI_re.match(bucket_uri.split("?")[0].rstrip("/"))
-        assert match is not None, f"{bucket_uri} must be an s3 URI"
-        prefix = match.groupdict()["prefix"]
+
+        if starts_with:
+            subpath = self.join(self.subpath, starts_with)
+        else:
+            subpath = self.subpath
+
+        original_subpath = self.original_subpath or self.subpath
+        # Do not serve files outside the original URI
+        if not subpath.startswith(original_subpath.lstrip("/")):
+            return
+
         try:
-            for item in self._list_blobs_with_cache(name_starts_with=prefix + starts_with):
+            for item in self._list_blobs_with_cache(self.container_client, name_starts_with=subpath):
                 item_name = f'/{item["name"]}'
-                assert item_name.startswith(f"/{prefix}{starts_with}".replace("//", "/"))
+                assert item_name.startswith(f"/{subpath}".replace("//", "/"))
                 if ends_with is None or item_name.endswith(ends_with):
                     yield SourcedItem(item, item_name, self, item.size)
         except HttpResponseError:
             proteus.logger.error(
                 "Missing Azure credentials to perform this operation, please "
                 "provide a SAS token or provide another authentication method on Azure"
             )
             raise
 
     _blob_cache = {}
 
+    @classmethod
     @lru_cache(maxsize=50000)
-    def _list_blobs_with_cache(self, name_starts_with):
-        items = self._blob_cache.get(name_starts_with)
+    def _list_blobs_with_cache(cls, container_client, name_starts_with):
+        items = cls._blob_cache.setdefault(container_client, {}).get(name_starts_with)
 
         if not items:
-            items = list(self.container_client.list_blobs(name_starts_with=name_starts_with))
-            self._blob_cache[name_starts_with] = items
+            items = list(container_client.list_blobs(name_starts_with=name_starts_with))
+            cls._blob_cache[container_client][name_starts_with] = items
 
         return items
 
     def open(self, reference):
         reference_path = reference.get("name")
         file_size = reference["size"]
         modified = reference["last_modified"]
@@ -157,9 +196,54 @@
     def chunks(self, reference):
         stream = self._download_blob(reference)
 
         for chunk in stream.chunks():
             yield chunk
 
     def fastcopy(self, reference, destination):
+        if AZ_COPY_PRESENT:
+            try:
+                download_url = (
+                    f'{self.storage_url}/{self.container_name}/{reference.name.strip("/")}?{self.url_sas_token}'
+                )
+                proteus.bucket.run_azcopy("copy", download_url, destination)
+            except AzCopyError as e:
+                raise RuntimeError(
+                    f'Could not download {reference.name} to {destination} via azcopy: \n{e.out or ""}\n{e.err}'
+                )
+            return True
+
         # TODO: Maybe fastcopy can use azcopy?
         return False
+
+    def cd(self, subpath):
+        subpath = self.join(self.subpath, subpath)
+        uri = f"{self.storage_url}/{self.container_name}{'/' + subpath if subpath else ''}?" + self.url_sas_token
+
+        return self.__class__(uri, container_client=self.container_client, original_uri=self.original_uri or self.uri)
+
+    def to_relative(self, item: str):
+        container_path = f'/{self.subpath.strip("/")}/'
+        assert item.startswith(container_path)
+        return item.split(container_path, 1)[1].lstrip("/")
+
+    def dirname(self, item: str):
+        return "/".join(item.split("/")[:-1])
+
+    def join(self, item0, *items):
+
+        item0 = item0.rstrip("/")
+
+        for item in items:
+            item = item.rstrip("/")
+            for path_part in item.split("/"):
+                if path_part == "..":
+                    if item0.startswith(".."):
+                        item0 += f"/{path_part}"
+                    elif not item0:
+                        item0 = ".."
+                    else:
+                        item0 = "/".join(item0.split("/")[:-1])
+                else:
+                    item0 += f"/{path_part}"
+
+        return item0
```

### Comparing `proteus_cli-0.3.8/cli/datasets/sources/common.py` & `proteus_cli-1.0.0/cli/datasets/sources/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 import re
 
 
+class SourcedItem:
+    def __init__(self, reference, path, source, size):
+        self.source = source
+        self.path = path
+        self.reference = reference
+        self.size = size
+
+    _path_rel = None
+
+    @property
+    def path_rel(self):
+        if self._path_rel is None:
+            self._path_rel = self.source.to_relative(self.path)
+        return self._path_rel
+
+    def __iter__(self):
+        return iter((self.source, self.path, self.reference, self.size))
+
+    def __str__(self):
+        return f"< {self.path}@{self.source} >"
+
+
 class Source:
 
     URI_re = re.compile(r"^.*$")
 
     def __init__(self, uri):
         self.uri = uri
 
@@ -15,23 +37,21 @@
 
     def list_contents(self, *args):
         raise NotImplementedError()
 
     def open(self, reference):
         raise NotImplementedError()
 
+    def cd(self, subpath):
+        raise NotImplementedError()
+
     def fastcopy(self, reference, destination):
         return False
 
+    def to_relative(self, item: str):
+        raise NotImplementedError()
 
-class SourcedItem:
-    def __init__(self, reference, path, source, size):
-        self.source = source
-        self.path = path
-        self.reference = reference
-        self.size = size
-
-    def __iter__(self):
-        return iter((self.source, self.path, self.reference, self.size))
+    def dirname(self, item: str):
+        raise NotImplementedError()
 
-    def __str__(self):
-        return f"< {self.path}@{self.source} >"
+    def join(self, *items):
+        raise NotImplementedError()
```

### Comparing `proteus_cli-0.3.8/cli/datasets/sources/s3.py` & `proteus_cli-1.0.0/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/debugger/commands.py` & `proteus_cli-1.0.0/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/debugger/init_keyword_check.py` & `proteus_cli-1.0.0/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/jobs/commands.py` & `proteus_cli-1.0.0/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/jobs/list.py` & `proteus_cli-1.0.0/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/simulations/commands.py` & `proteus_cli-1.0.0/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/simulations/create.py` & `proteus_cli-1.0.0/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/simulations/dependencySolver.py` & `proteus_cli-1.0.0/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/cli/simulations/opm.py` & `proteus_cli-1.0.0/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.8/pyproject.toml` & `proteus_cli-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.3.8"
+version = "1.0.0"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
 
@@ -17,16 +17,16 @@
 boto3 = "^1.17.79"
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 azure-storage-blob = "^12.8.1"
 readchar = "^3.0.4"
 azure-identity = "^1.12.0"
 markupsafe = "2.0.1"
-proteus-runtime = "0.2.29"
-proteus-preprocessing = "0.2.15"
+proteus-runtime = "0.3.0"
+proteus-preprocessing = "0.3.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pre-commit = "^2.9.3"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-bdd = "^5.0.0"
```

### Comparing `proteus_cli-0.3.8/PKG-INFO` & `proteus_cli-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.3.8
+Version: 1.0.0
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: cryptography (>=3.3.2,<4.0.0)
 Requires-Dist: jwt (>=1.2.0,<2.0.0)
 Requires-Dist: markupsafe (==2.0.1)
-Requires-Dist: proteus-preprocessing (==0.2.15)
-Requires-Dist: proteus-runtime (==0.2.29)
+Requires-Dist: proteus-preprocessing (==0.3.0)
+Requires-Dist: proteus-runtime (==0.3.0)
 Requires-Dist: pycryptodome (>=3.10.1,<4.0.0)
 Requires-Dist: readchar (>=3.0.4,<4.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: tqdm (>=4.61.0,<5.0.0)
```

