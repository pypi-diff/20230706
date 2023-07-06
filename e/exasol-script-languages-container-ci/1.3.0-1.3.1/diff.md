# Comparing `tmp/exasol_script_languages_container_ci-1.3.0.tar.gz` & `tmp/exasol_script_languages_container_ci-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_ci-1.3.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci-1.3.1.tar", max compression
```

## Comparing `exasol_script_languages_container_ci-1.3.0.tar` & `exasol_script_languages_container_ci-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/LICENSE
--rw-r--r--   0        0        0       95 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/cli.py
--rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/__init__.py
--rw-r--r--   0        0        0     1926 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_ci.py
--rw-r--r--   0        0        0     2703 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_release.py
--rw-r--r--   0        0        0        0 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/__init__.py
--rw-r--r--   0        0        0     1304 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/asset_uploader.py
--rw-r--r--   0        0        0     1677 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/branch_config.py
--rw-r--r--   0        0        0     4940 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci.py
--rw-r--r--   0        0        0     2674 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_build.py
--rw-r--r--   0        0        0      944 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_export.py
--rw-r--r--   0        0        0     1157 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_push.py
--rw-r--r--   0        0        0     1071 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_security_scan.py
--rw-r--r--   0        0        0     1309 2023-07-04 07:16:55.767849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
--rw-r--r--   0        0        0     4816 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_test.py
--rw-r--r--   0        0        0      334 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/common.py
--rw-r--r--   0        0        0        0 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/__init__.py
--rw-r--r--   0        0        0      584 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/config_data_model.py
--rw-r--r--   0        0        0     2153 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/data_model_generator.py
--rw-r--r--   0        0        0     1501 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/git_access.py
--rw-r--r--   0        0        0     1223 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
--rw-r--r--   0        0        0     2890 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release.py
--rw-r--r--   0        0        0     2443 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release_uploader.py
--rw-r--r--   0        0        0      321 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/render_template.py
--rwxr-xr-x   0        0        0      125 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/main.py
--rw-r--r--   0        0        0      950 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/templates/config_schema.json
--rw-r--r--   0        0        0      822 2023-07-04 07:16:55.771849 exasol_script_languages_container_ci-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-06 11:42:03.331398 exasol_script_languages_container_ci-1.3.1/LICENSE
+-rw-r--r--   0        0        0       95 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/__init__.py
+-rw-r--r--   0        0        0       50 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1926 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/commands/run_ci.py
+-rw-r--r--   0        0        0     2703 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/commands/run_release.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/__init__.py
+-rw-r--r--   0        0        0     1304 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/asset_uploader.py
+-rw-r--r--   0        0        0     1677 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/branch_config.py
+-rw-r--r--   0        0        0     4705 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci.py
+-rw-r--r--   0        0        0     2674 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_build.py
+-rw-r--r--   0        0        0      944 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_export.py
+-rw-r--r--   0        0        0      486 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_prepare.py
+-rw-r--r--   0        0        0     1157 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_push.py
+-rw-r--r--   0        0        0     1071 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_security_scan.py
+-rw-r--r--   0        0        0     1309 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_step_output_printer.py
+-rw-r--r--   0        0        0     4816 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_test.py
+-rw-r--r--   0        0        0      334 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/common.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/config/__init__.py
+-rw-r--r--   0        0        0      584 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/config/config_data_model.py
+-rw-r--r--   0        0        0     2153 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/config/data_model_generator.py
+-rw-r--r--   0        0        0     1501 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/git_access.py
+-rw-r--r--   0        0        0     1223 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py
+-rw-r--r--   0        0        0     2906 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/release.py
+-rw-r--r--   0        0        0     2443 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/release_uploader.py
+-rw-r--r--   0        0        0      321 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/render_template.py
+-rwxr-xr-x   0        0        0      125 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/main.py
+-rw-r--r--   0        0        0      950 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/templates/config_schema.json
+-rw-r--r--   0        0        0      822 2023-07-06 11:42:03.335398 exasol_script_languages_container_ci-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci-1.3.1/PKG-INFO
```

### Comparing `exasol_script_languages_container_ci-1.3.0/LICENSE` & `exasol_script_languages_container_ci-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_ci.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/commands/run_ci.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/cli/commands/run_release.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/cli/commands/run_release.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/asset_uploader.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/branch_config.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/branch_config.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import logging
-import os
-from pathlib import Path
-from typing import Set
-
-from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
-from exasol_integration_test_docker_environment.lib.base import luigi_log_config
+from typing import Set, Callable
 
 from exasol_script_languages_container_ci.lib.branch_config import BranchConfig
 from exasol_script_languages_container_ci.lib.ci_build import CIBuild
+from exasol_script_languages_container_ci.lib.ci_prepare import CIPrepare
 from exasol_script_languages_container_ci.lib.ci_push import CIPush
 from exasol_script_languages_container_ci.lib.ci_security_scan import CISecurityScan
 from exasol_script_languages_container_ci.lib.ci_test import CIExecuteTest
 from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.git_access import GitAccess
 
 
@@ -52,32 +48,31 @@
        docker_release_repository: str,
        commit_sha: str,
        build_config: Config,
        git_access: GitAccess,
        ci_build: CIBuild = CIBuild(),
        ci_execute_tests: CIExecuteTest = CIExecuteTest(),
        ci_push: CIPush = CIPush(),
-       ci_security_scan: CISecurityScan = CISecurityScan()):
+       ci_security_scan: CISecurityScan = CISecurityScan(),
+       ci_prepare: CIPrepare = CIPrepare()):
     """
     Run CI build:
     1. Build image
     2. Run db tests
     3. Run security scan
     4. Push to docker repositories
     """
     logging.info(f"Running CI build for parameters: {locals()}")
 
     flavor_path = (f"flavors/{flavor}",)
     test_container_folder = "test_container"
     rebuild = BranchConfig.rebuild(branch_name)
     needs_to_build = check_if_need_to_build(branch_name, build_config, flavor, git_access)
     if needs_to_build:
-        log_path = Path(DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
-        os.environ[luigi_log_config.LOG_ENV_VARIABLE_NAME] = f"{log_path.absolute()}"
-
+        ci_prepare.prepare()
         ci_build.build(flavor_path=flavor_path,
                        rebuild=rebuild,
                        build_docker_repository=docker_build_repository,
                        commit_sha=commit_sha,
                        docker_user=docker_user,
                        docker_password=docker_password,
                        test_container_folder=test_container_folder)
```

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_build.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_export.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_export.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_push.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_security_scan.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_step_output_printer.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_step_output_printer.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/ci_test.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/ci_test.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/config_data_model.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/config/config_data_model.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/config/data_model_generator.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/config/data_model_generator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/git_access.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/git_access.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/github_release_asset_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 import os
 from pathlib import Path
+from typing import Callable
 
 from exasol_integration_test_docker_environment.cli.options.system_options import DEFAULT_OUTPUT_DIRECTORY
 from exasol_integration_test_docker_environment.lib.base import luigi_log_config
 
 from exasol_script_languages_container_ci.lib.ci_build import CIBuild
+from exasol_script_languages_container_ci.lib.ci_prepare import CIPrepare
 from exasol_script_languages_container_ci.lib.ci_push import CIPush
 from exasol_script_languages_container_ci.lib.ci_security_scan import CISecurityScan
 from exasol_script_languages_container_ci.lib.ci_test import CIExecuteTest
 from exasol_script_languages_container_ci.lib.config.config_data_model import Config
 from exasol_script_languages_container_ci.lib.release_uploader import ReleaseUploader
 
 
@@ -21,29 +23,28 @@
             source_repo_url: str,
             release_id: int,
             is_dry_run: bool,
             release_uploader: ReleaseUploader,
             ci_build: CIBuild = CIBuild(),
             ci_execute_tests: CIExecuteTest = CIExecuteTest(),
             ci_push: CIPush = CIPush(),
-            ci_security_scan: CISecurityScan = CISecurityScan()):
+            ci_security_scan: CISecurityScan = CISecurityScan(),
+            ci_prepare: CIPrepare = CIPrepare()):
     """
     Run Release build:
     1. Build image
     2. Run basic tests
     3. Push to docker release repository
     4. Upload to GH release url
     """
     logging.info(f"Running Release build for parameters: {locals()}")
 
     flavor_path = (f"flavors/{flavor}",)
     test_container_folder = "test_container"
-    log_path = Path(DEFAULT_OUTPUT_DIRECTORY) / "jobs" / "logs" / "main.log"
-    os.environ[luigi_log_config.LOG_ENV_VARIABLE_NAME] = f"{log_path.absolute()}"
-
+    ci_prepare.prepare()
     ci_build.build(flavor_path=flavor_path, rebuild=True,
                    build_docker_repository=None,
                    commit_sha="",
                    docker_user=None,
                    docker_password=None,
                    test_container_folder=test_container_folder)
     ci_execute_tests.execute_tests(flavor_path=flavor_path,
```

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/lib/release_uploader.py` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/lib/release_uploader.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/exasol_script_languages_container_ci/templates/config_schema.json` & `exasol_script_languages_container_ci-1.3.1/exasol_script_languages_container_ci/templates/config_schema.json`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci-1.3.0/pyproject.toml` & `exasol_script_languages_container_ci-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci"
-version = "1.3.0"
+version = "1.3.1"
 description = "Implements CI builds for script-language-container."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
```

### Comparing `exasol_script_languages_container_ci-1.3.0/PKG-INFO` & `exasol_script_languages_container_ci-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-ci
-Version: 1.3.0
+Version: 1.3.1
 Summary: Implements CI builds for script-language-container.
 License: MIT
 Author: Thomas Uebensee
 Author-email: ext.thomas.uebensee@exasol.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

