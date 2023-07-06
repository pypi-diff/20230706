# Comparing `tmp/pushcart_deploy-1.6.1.tar.gz` & `tmp/pushcart_deploy-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart_deploy-1.6.1.tar", max compression
+gzip compressed data, was "pushcart_deploy-1.6.5.tar", max compression
```

## Comparing `pushcart_deploy-1.6.1.tar` & `pushcart_deploy-1.6.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/LICENSE
--rw-r--r--   0        0        0       80 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/README.md
--rw-r--r--   0        0        0     2502 2023-06-28 12:43:52.931377 pushcart_deploy-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/__init__.py
--rw-r--r--   0        0        0    16356 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/configuration.py
--rw-r--r--   0        0        0      500 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/__init__.py
--rw-r--r--   0        0        0     3482 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py
--rw-r--r--   0        0        0     4706 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/pipelines_wrapper.py
--rw-r--r--   0        0        0     4496 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/repos_wrapper.py
--rw-r--r--   0        0        0    12091 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/scheduler.py
--rw-r--r--   0        0        0     3173 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py
--rw-r--r--   0        0        0      254 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/__init__.py
--rw-r--r--   0        0        0     4385 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/base_settings.py
--rw-r--r--   0        0        0     4175 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/job_settings.py
--rw-r--r--   0        0        0     6882 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py
--rw-r--r--   0        0        0     9525 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/metadata.py
--rw-r--r--   0        0        0     4201 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/setup.py
--rw-r--r--   0        0        0     3397 2023-06-28 12:42:38.507541 pushcart_deploy-1.6.1/src/pushcart_deploy/validation.py
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pushcart_deploy-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-03 13:39:43.347561 pushcart_deploy-1.6.5/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-05 08:20:56.886928 pushcart_deploy-1.6.5/README.md
+-rw-r--r--   0        0        0     2781 2023-07-06 16:19:13.001269 pushcart_deploy-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-05-23 15:16:36.981069 pushcart_deploy-1.6.5/src/pushcart_deploy/__init__.py
+-rw-r--r--   0        0        0    16895 2023-07-06 16:19:13.001269 pushcart_deploy-1.6.5/src/pushcart_deploy/configuration.py
+-rw-r--r--   0        0        0      500 2023-06-06 13:09:00.738712 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/__init__.py
+-rw-r--r--   0        0        0     3461 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/jobs_wrapper.py
+-rw-r--r--   0        0        0     4762 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/pipelines_wrapper.py
+-rw-r--r--   0        0        0     4485 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/repos_wrapper.py
+-rw-r--r--   0        0        0    11721 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/scheduler.py
+-rw-r--r--   0        0        0     3153 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/secrets_wrapper.py
+-rw-r--r--   0        0        0      254 2023-06-06 13:09:00.738712 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/__init__.py
+-rw-r--r--   0        0        0     4387 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/base_settings.py
+-rw-r--r--   0        0        0     4154 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/job_settings.py
+-rw-r--r--   0        0        0     6861 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py
+-rw-r--r--   0        0        0     9505 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/metadata.py
+-rw-r--r--   0        0        0     4190 2023-07-06 16:19:13.004602 pushcart_deploy-1.6.5/src/pushcart_deploy/setup.py
+-rw-r--r--   0        0        0     3397 2023-06-06 13:09:00.738712 pushcart_deploy-1.6.5/src/pushcart_deploy/validation.py
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 pushcart_deploy-1.6.5/PKG-INFO
```

### Comparing `pushcart_deploy-1.6.1/LICENSE` & `pushcart_deploy-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.6.1/pyproject.toml` & `pushcart_deploy-1.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart-deploy"
-version = "1.6.1"
+version = "1.6.5"
 description = "Deployment helper for pipeline configurations using Pushcart"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
@@ -94,23 +94,24 @@
 
 [tool.poetry.dependencies]
 aiofiles = "^23.1.0"
 click = "^8.1.3"
 databricks-cli = "^0.17.4"
 databricks-connect = "^13.0.0"
 methodtools = "^0.4.7"
-pydantic = "^1.10.7"
+pydantic = "^2.0.0"
 python = "^3.10"
 python-dotenv = "^1.0.0"
 pyyaml = "^6.0"
 tomli = "^2.0.1"
 urllib3 = "^1"
 
 [tool.poetry.group.dev.dependencies]
 black = { version = "*", allow-prereleases = true }
+bumpver = "^2023.1124"
 coverage = "^7.2.7"
 hypothesis = "^6.70.1"
 ipykernel = "^6.22.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
@@ -118,7 +119,18 @@
 
 [tool.poetry.scripts]
 pushcart-deploy = "pushcart_deploy.setup:deploy"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.bumpver]
+current_version = "1.6.1"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['^version = "{version}"$']
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/configuration.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 import tomli
 import yaml
 from pydantic import (
     Field,
     conint,
     constr,
     dataclasses,
-    root_validator,
-    validate_arguments,
-    validator,
+    field_validator,
+    model_validator,
+    validate_call,
 )
+from pydantic_core._pydantic_core import ArgsKwargs
 
 
 async def get_transformations_from_csv(csv_path: Path | str) -> AsyncIterator[dict]:
     """Return transformations from the metadata .csv line-by-line.
 
     Parameters
     ----------
@@ -137,15 +138,15 @@
     if len(existing_paths) > 1:
         msg = f"Expecting only one {settings_path}.[json|toml|yml|yaml] file. Found:\n{os.linesep.join(existing_paths)}"
         raise FileExistsError(msg)
 
     return existing_paths[0]
 
 
-@validate_arguments
+@validate_call
 async def get_config_from_file(settings_path: Path | str) -> dict | None:
     """Load a configuration file into a dictionary. Supported formats are JSON, YAML, and TOML.
 
     Parameters
     ----------
     settings_path : Path | str
         Path to the configuration file.
@@ -209,15 +210,19 @@
     Has two main fields: validation_rule and validation_action. The validation_rule
     field is a Spark SQL string that defines the rule that the input data must follow,
     while the validation_action field is a string that defines the action to take if
     the input data fails to meet the validation rule.
     """
 
     validation_rule: constr(min_length=1, strict=True)
-    validation_action: constr(to_upper=True, strict=True, regex=r"\A(LOG|DROP|FAIL)\Z")
+    validation_action: constr(
+        to_upper=True,
+        strict=True,
+        pattern=r"^(LOG|DROP|FAIL)$",
+    )
 
     def __getitem__(self, item: str) -> any:
         """Avoid Pydantic throwing ValidationError: object not subscriptable.
 
         Parameters
         ----------
         item : str
@@ -257,15 +262,15 @@
 
     origin: constr(min_length=1, strict=True)
     datatype: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
     params: str | None = None
     validations: list[Validation] | None = Field(default_factory=list)
 
-    @validator("validations")
+    @field_validator("validations")
     @classmethod
     def check_multiple_validations_with_same_rule(cls, value: dict) -> dict:
         """Check that there are no multiple validation actions for the same rule."""
         if value and (fails := _get_multiple_validations_with_same_rule(value)):
             msg = f"Different actions for the same validation:\n{fails}"
             raise ValueError(msg)
         return value
@@ -301,45 +306,45 @@
 
     origin: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
     column_order: conint(ge=1) | None = 1
     source_column_name: constr(strict=True) | None = None
     source_column_type: constr(
         strict=True,
-        regex="\\A(string|int|double|date|timestamp|boolean|struct|array|map)\\Z",
+        pattern="^(string|int|double|date|timestamp|boolean|struct|array|map)$",
     ) | None = None
     dest_column_name: constr(strict=True) | None = None
     dest_column_type: constr(
         strict=True,
-        regex="\\A(string|int|double|date|timestamp|boolean|struct|array|map)\\Z",
+        pattern="^(string|int|double|date|timestamp|boolean|struct|array|map)$",
     ) | None = None
     transform_function: constr(strict=True) | None = None
     sql_query: constr(min_length=1, strict=True) | None = None
     default_value: constr(strict=True) | None = None
     validations: list[Validation] | None = Field(default_factory=list)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
     def check_only_one_of_config_or_sql_query_defined(cls, values: dict) -> dict:
         """Check that one and only one of the config or sql_query fields is defined."""
+        data = values.kwargs if isinstance(values, ArgsKwargs) else values
         if not any(
-            values.get(v) is not None
+            data.get(v) is not None
             for v in ["source_column_name", "dest_column_name", "sql_query"]
         ):
-            msg = f"No transformation defined. Please provide either a config or a sql_query.\nGot: {values}"
+            msg = f"No transformation defined. Please provide either a config or a sql_query.\nGot: {data}"
             raise ValueError(msg)
         if all(
-            values.get(t)
-            for t in ["source_column_name", "dest_column_name", "sql_query"]
+            data.get(t) for t in ["source_column_name", "dest_column_name", "sql_query"]
         ):
-            msg = f"Only one of config or sql_query allowed.\nGot: {values}"
+            msg = f"Only one of config or sql_query allowed.\nGot: {data}"
             raise ValueError(msg)
         return values
 
-    @validator("validations")
+    @field_validator("validations")
     @classmethod
     def check_multiple_validations_with_same_rule(cls, value: dict) -> dict:
         """Validate that there are no multiple validations with the same rule."""
         if value and (fails := _get_multiple_validations_with_same_rule(value)):
             msg = f"Different actions for the same validation:\n{fails}"
             raise ValueError(msg)
         return value
@@ -372,45 +377,47 @@
 
     target_catalog_name: constr(strip_whitespace=True, min_length=1, strict=True)
     target_schema_name: constr(strip_whitespace=True, min_length=1, strict=True)
     pipeline_name: constr(strip_whitespace=True, min_length=1, strict=True)
 
     origin: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
-    mode: constr(min_length=1, strict=True, regex=r"^(append|upsert)$")
+    mode: constr(min_length=1, strict=True, pattern=r"^(append|upsert)$")
     path: Path | None = None
     keys: list[constr(min_length=1, strict=True)] | None = Field(
         default_factory=list,
     )
     sequence_by: constr(min_length=1, strict=True) | None = None
     validations: list[Validation] | None = Field(default_factory=list)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
     def check_keys_and_sequence_for_upsert(cls, values: dict) -> dict:
         """Check that the keys and sequence_by fields are defined for upsert mode."""
-        if values.get("mode") == "upsert" and not all(
-            values[v] for v in ["keys", "sequence_by"]
+        data = values.kwargs if isinstance(values, ArgsKwargs) else values
+
+        if data.get("mode") == "upsert" and not all(
+            data[v] for v in ["keys", "sequence_by"]
         ):
             msg = "Mode upsert requires that keys and sequence_by are defined"
             raise ValueError(
                 msg,
             )
         return values
 
-    @validator("validations")
+    @field_validator("validations")
     @classmethod
     def check_multiple_validations_with_same_rule(cls, value: dict) -> dict:
         """Check that there are no multiple validations with the same rule."""
         if value and (fails := _get_multiple_validations_with_same_rule(value)):
             msg = f"Different actions for the same validation:\n{fails}"
             raise ValueError(msg)
         return value
 
-    @validator("path", pre=False, always=True)
+    @field_validator("path", mode="after")
     @classmethod
     def convert_to_absolute_string(cls, value: Path | None) -> str | None:
         """Convert the Path object to its absolute POSIX representation."""
         if value:
             return value.absolute().as_posix()
 
         return None
@@ -436,37 +443,49 @@
         unique.
     """
 
     sources: list[Source] | None = Field(default_factory=list)
     transformations: list[Transformation] | None = Field(default_factory=list)
     destinations: list[Destination] | None = Field(default_factory=list)
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
-    def check_at_least_one_stage_defined(cls, values: dict) -> dict:
+    def check_at_least_one_stage_defined(cls, values: dict[str, list[any]]) -> dict:
         """Check that at least one of the sources, transformations, or destinations fields is defined in the configuration file."""
-        if not any(v in ["sources", "transformations", "destinations"] for v in values):
-            msg = "No stage definition found. Please define at least one of: sources, transformations, destinations"
+        msg = "No stage definition found. Please define at least one of: sources, transformations, destinations"
+
+        data = values.kwargs if isinstance(values, ArgsKwargs) else values
+
+        if not data:
             raise ValueError(msg)
+
+        if not any(v in ["sources", "transformations", "destinations"] for v in data):
+            raise ValueError(msg)
+
         return values
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     @classmethod
-    def check_all_dlt_target_objects_are_unique(cls, values: dict) -> dict:
+    def check_all_dlt_target_objects_are_unique(
+        cls,
+        values: dict[str, list[any]],
+    ) -> dict:
         """Check that no values of the "target" fields of "sources", "transformations" and "destinations", taken together, overlap."""
-        sources = values.get("sources", [])
-        transformations = values.get("transformations", [])
-        destinations = values.get("destinations", [])
+        data = values.kwargs if isinstance(values, ArgsKwargs) else values
+
+        sources = (data or {}).get("sources", [])
+        transformations = (data or {}).get("transformations", [])
+        destinations = (data or {}).get("destinations", [])
 
         target_values = (
             [source.get("target") for source in sources if source]
             + [
                 transformation.get("target")
                 for transformation in transformations
-                if transformation.get("sql_query")
+                if transformation and transformation.get("sql_query")
             ]
             + [destination.get("target") for destination in destinations if destination]
         )
 
         duplicates = [
             value for value in set(target_values) if target_values.count(value) > 1
         ]
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/jobs_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 
 import logging
 
 from databricks_cli.jobs.api import JobsApi
 from databricks_cli.runs.api import RunsApi
 from databricks_cli.sdk.api_client import ApiClient
-from pydantic import dataclasses, validate_arguments
+from pydantic import dataclasses, validate_call
 
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class JobsWrapper:
     """Manages Databricks jobs.
@@ -37,15 +37,15 @@
     running jobs and retrieving their status. Uses the JobSettings class to load
     job settings from a JSON file or string, or to retrieve default job settings
     for checkpoint, pipeline, and release jobs.
     """
 
     api_client: ApiClient
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize the logger instance and creates instances of JobsApi and RunsApi."""
         self.log = logging.getLogger(__name__)
 
         self.jobs_api = JobsApi(self.api_client)
         self.runs_api = RunsApi(self.api_client)
 
     def get_jobs_list(self) -> list:
@@ -85,15 +85,15 @@
     def update_job(self, job_id: str, job_settings: dict) -> str:
         """Update a job using the provided job settings."""
         self.jobs_api.reset_job({"job_id": job_id, "new_settings": job_settings})
         self.log.info(f"Updated job {job_settings['name']} with ID: {job_id}")
 
         return job_id
 
-    @validate_arguments
+    @validate_call
     def delete_job(self, job_id: str) -> None:
         """Delete a job by ID.
 
         Parameters
         ----------
         job_id : str
             ID of Databricks Workflows job to be deleted
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/pipelines_wrapper.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/pipelines_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,53 +16,55 @@
 -----
 Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
 environment.
 
 """
 import logging
 
+from databricks.sdk import WorkspaceClient
 from databricks.sdk.dbutils import RemoteDbUtils
 from databricks_cli.pipelines.api import PipelinesApi
 from databricks_cli.sdk.api_client import ApiClient
-from pydantic import DirectoryPath, dataclasses, validate_arguments
+from pydantic import DirectoryPath, dataclasses, validate_call
 
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class PipelinesWrapper:
     """Manages Databricks DLT Pipelines.
 
     Provides methods for creating, updating and deleting DLT pipelines.
     """
 
     api_client: ApiClient
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize the logger instance and create an instance of PipelinesApi."""
         self.log = logging.getLogger(__name__)
 
+        self.workspace = WorkspaceClient()
         self.pipelines_api = PipelinesApi(self.api_client)
         self.dbutils = RemoteDbUtils()
 
     def get_pipelines_list(self) -> list:
         """Get a list of all the pipelines currently defined in Databricks Workflows.
 
         Returns
         -------
         list
             a list of dict containing pipeline ids and names, e.g. [ { pipeline_name: pipeline_id }, ... ]
         """
-        pipelines = self.pipelines_api.list()
+        pipelines = self.workspace.pipelines.list_pipelines()
 
         return [
             {
-                "pipeline_name": p["name"],
-                "pipeline_id": p["pipeline_id"],
+                "name": p.name,
+                "pipeline_id": p.pipeline_id,
             }
             for p in pipelines
         ]
 
     def get_pipeline_id(self, pipeline_name: str) -> str:
         """Retrieve a pipeline ID by name.
 
@@ -78,15 +80,15 @@
         """
         pipelines_filtered = {
             p["name"]: p["pipeline_id"] for p in self.get_pipelines_list()
         }
 
         return pipelines_filtered.get(pipeline_name)
 
-    @validate_arguments
+    @validate_call
     def create_pipeline(self, pipeline_settings: dict, repo_path: str) -> str:
         """Create a DLT pipeline using the provided settings.
 
         Parameters
         ----------
         pipeline_settings : dict
             Settings dictionary for DLT pipelines as described in the Databricks Delta
@@ -106,15 +108,15 @@
         )
 
         self.log.info(
             f"Created pipeline {pipeline_settings['name']} with ID: {pipeline['pipeline_id']}",
         )
         return pipeline["pipeline_id"]
 
-    @validate_arguments
+    @validate_call
     def update_pipeline(self, pipeline_settings: dict, repo_path: str) -> str:
         """Update an existing pipeline with new settings.
 
         Parameters
         ----------
         pipeline_settings : dict
             Dictionary holding pipeline settings as per Databricks Delta Live Tables
@@ -133,15 +135,15 @@
             allow_duplicate_names=False,
         )
         self.log.info(
             f"Updated pipeline {pipeline_settings['name']} with ID: {pipeline_settings['id']}",
         )
         return pipeline_settings["id"]
 
-    @validate_arguments
+    @validate_call
     def delete_pipeline(self, pipeline_id: str) -> None:
         """Delete a pipeline from DLT workflows.
 
         Parameters
         ----------
         pipeline_id : str
             Pipeline ID as found in Databricks Workflows Delta Live Tables
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/repos_wrapper.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/repos_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     branch, and detect the Git provider from a given URL. Also handles Git
     credentials.
     """
 
     api_client: ApiClient
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger and object configuration."""
         self.log = logging.getLogger(__name__)
 
         self.workspace_api = WorkspaceApi(self.api_client)
         self.repos_api = ReposApi(self.api_client)
         self.git_creds = GitCredentialsAPI(SdkApiClient())
         self.repo_id = None
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/scheduler.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Helper module handling pipeline and job sets."""
 
 import logging
 
 from databricks_cli.repos.api import ReposApi
 from databricks_cli.sdk.api_client import ApiClient
-from pydantic import DirectoryPath, dataclasses, validate_arguments
+from pydantic import DirectoryPath, dataclasses, validate_call
 
 from pushcart_deploy.databricks_api import JobsWrapper, PipelinesWrapper
 from pushcart_deploy.databricks_api.settings import JobSettings, PipelineSettings
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
@@ -18,22 +18,22 @@
     Defines logic for determining which pipelines and associated jobs are new, obsolete
     or in need of updating during a release process.
     """
 
     api_client: ApiClient
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize the logger and create instances of needed classes."""
         self.log = logging.getLogger(__name__)
         self.jobs_wrapper = JobsWrapper(self.api_client)
         self.pipelines_wrapper = PipelinesWrapper(self.api_client, self.config_dir)
         self.repos_api = ReposApi(self.api_client)
 
-    @validate_arguments
+    @validate_call
     def get_obsolete_pipelines_list(
         self,
         metadata_pipelines: list,
         workflows_pipelines: list,
     ) -> list:
         """Get a list of obsolete pipelines.
 
@@ -52,29 +52,27 @@
             List of dictionaries representing the pipelines in Databricks Workflows.
 
         Returns
         -------
         list
             List of dictionaries representing obsolete pipelines.
             [{
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": pipeline_id
             }, ...]
         """
-        metadata_pipelines_set = {
-            pipeline["pipeline_name"] for pipeline in metadata_pipelines
-        }
+        metadata_pipelines_set = {pipeline["name"] for pipeline in metadata_pipelines}
 
         return [
             pipeline
             for pipeline in workflows_pipelines
-            if pipeline["pipeline_name"] not in metadata_pipelines_set
+            if pipeline["name"] not in metadata_pipelines_set
         ]
 
-    @validate_arguments
+    @validate_call
     def get_new_pipelines_list(
         self,
         metadata_pipelines: list,
         workflows_pipelines: list,
     ) -> list:
         """Get a list of new pipelines.
 
@@ -94,29 +92,27 @@
 
         Returns
         -------
         list
             List of dictionaries representing the new pipelines.
             [{
                 "target_schema_name": target_schema_name,
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": None,
             }, ...]
         """
-        workflows_pipelines_set = {
-            pipeline["pipeline_name"] for pipeline in workflows_pipelines
-        }
+        workflows_pipelines_set = {pipeline["name"] for pipeline in workflows_pipelines}
 
         return [
             pipeline
             for pipeline in metadata_pipelines
-            if pipeline["pipeline_name"] not in workflows_pipelines_set
+            if pipeline["name"] not in workflows_pipelines_set
         ]
 
-    @validate_arguments
+    @validate_call
     def get_matching_pipelines_list(
         self,
         metadata_pipelines: list,
         workflows_pipelines: list,
     ) -> list:
         """Get a list of matching pipelines.
 
@@ -137,116 +133,114 @@
         Returns
         -------
         list
             List of dictionaries representing the matching pipelines, in the format
             [{
                 "target_catalog_name": target_catalog_name,
                 "target_schema_name": target_schema_name,
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": pipeline_id,
             }, ...]
         """
-        scheduled_dict = {
-            d["pipeline_name"]: d["pipeline_id"] for d in workflows_pipelines
-        }
+        scheduled_dict = {d["name"]: d["pipeline_id"] for d in workflows_pipelines}
 
         matching_pipelines = []
 
         for pipeline in metadata_pipelines:
-            pipeline_name = pipeline["pipeline_name"]
+            pipeline_name = pipeline["name"]
             if pipeline_name in scheduled_dict:
                 matching_pipeline = {
                     "target_catalog_name": pipeline["target_catalog_name"],
                     "target_schema_name": pipeline["target_schema_name"],
-                    "pipeline_name": pipeline_name,
+                    "name": pipeline_name,
                     "pipeline_id": scheduled_dict[pipeline_name],
                 }
                 matching_pipelines.append(matching_pipeline)
 
         return matching_pipelines
 
-    @validate_arguments
+    @validate_call
     def delete_obsolete_pipelines(self, obsolete_pipelines: list) -> None:
         """Remove all obsolete DLT pipelines from Workflows.
 
         Parameters
         ----------
         obsolete_pipelines : list
             List of pipeline IDs not found anymore in the metadata tables
         """
         self.log.info("Removing obsolete pipelines")
         for p in obsolete_pipelines:
             self.pipelines_wrapper.delete_pipeline(pipeline_id=p["pipeline_id"])
 
-    @validate_arguments
+    @validate_call
     def create_or_update_pipelines(
         self,
-        repo_id: str,
+        repo_id: str | int,
         metadata_pipelines: list,
     ) -> list:
         """Update or create new DLT pipelines from a list of pipelines available in the metadata.
 
         Parameters
         ----------
-        repo_id : str
+        repo_id : str | int
             ID of Databricks Repos used to point to the appropriate Pipeline notebook
         metadata_pipelines : list
             List of pipelines available in metadata, in the form of
             [{
                 "target_catalog_name": target_catalog_name,
                 "target_schema_name": target_schema_name,
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": pipeline_id | None,
             }, ...]
 
         Returns
         -------
         list
             List of created DLT pipelines, in the form of
             [{
                 "target_catalog_name": target_catalog_name,
                 "target_schema_name": target_schema_name,
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": pipeline_id,
             }, ...]
         """
         pipelines = []
-        repo_path = self.repos_api.get(repo_id)["path"]
+        repo_path = self.repos_api.get(str(repo_id))["path"]
 
         self.log.info("Creating new DLT pipelines")
         for pipeline in metadata_pipelines:
             libraries = [
                 {
                     "notebook": {"path": f"{repo_path}/runner/pipeline"},
                 },
             ]
             configuration = {
-                "pushcart.pipeline_name": pipeline["pipeline_name"],
+                "pushcart.pipeline_name": pipeline["name"],
             }
 
             if not (pipeline_id := pipeline["pipeline_id"]):
                 pipeline_id = self.pipelines_wrapper.get_pipeline_id(
-                    pipeline["pipeline_name"],
+                    pipeline["name"],
                 )
 
             pipeline_settings = PipelineSettings(
                 self.api_client,
                 self.config_dir,
             ).load_pipeline_settings(
                 target_catalog_name=pipeline["target_catalog_name"],
                 target_schema_name=pipeline["target_schema_name"],
-                pipeline_name=pipeline["pipeline_name"],
+                pipeline_name=pipeline["name"],
                 libraries=libraries,
                 configuration=configuration,
                 pipeline_id=pipeline_id,
             )
 
             if not pipeline_id:
                 self.log.warning(
-                    f"Pipeline not found: {pipeline['pipeline_name']}. Creating a new one",
+                    f"Pipeline not found: {pipeline['name']}. Creating a new one",
                 )
                 pipeline_id = self.pipelines_wrapper.create_pipeline(
                     pipeline_settings,
                     repo_path,
                 )
             else:
                 pipeline_id = self.pipelines_wrapper.update_pipeline(
@@ -254,32 +248,32 @@
                     repo_path,
                 )
 
             pipelines.append(
                 {
                     "target_catalog_name": pipeline["target_catalog_name"],
                     "target_schema_name": pipeline["target_schema_name"],
-                    "pipeline_name": pipeline["pipeline_name"],
+                    "name": pipeline["name"],
                     "pipeline_id": pipeline_id,
                 },
             )
 
         return pipelines
 
-    @validate_arguments
+    @validate_call
     def create_or_update_jobs(self, pipelines: list) -> list:
         """Create or update jobs for a list of DLT pipelines.
 
         Parameters
         ----------
         pipelines : list
             List of DLT pipelines, in the form of [{
                 "target_schema_name": target_schema_name,
                 "target_catalog_name": target_catalog_name,
-                "pipeline_name": pipeline_name,
+                "name": pipeline_name,
                 "pipeline_id": pipeline_id,
             }, ...]
 
         Returns
         -------
         list
             Job IDs for updated or newly created Databricks Workflows jobs
@@ -288,23 +282,23 @@
 
         self.log.info("(Re)scheduling pipelines")
 
         for p in pipelines:
             job_settings = JobSettings(self.config_dir).load_job_settings(
                 target_catalog_name=p["target_catalog_name"],
                 target_schema_name=p["target_schema_name"],
-                pipeline_name=p["pipeline_name"],
+                pipeline_name=p["name"],
                 pipeline_id=p["pipeline_id"],
             )
 
-            job_id = self.jobs_wrapper.get_job_id(p["pipeline_name"])
+            job_id = self.jobs_wrapper.get_job_id(p["name"])
 
             if not job_id:
                 self.log.warning(
-                    f"Job not found: {p['pipeline_name']}. Creating a new one",
+                    f"Job not found: {p['name']}. Creating a new one",
                 )
                 jobs.append(self.jobs_wrapper.create_job(job_settings))
             else:
                 jobs.append(self.jobs_wrapper.update_job(job_id, job_settings))
 
         return jobs
 
@@ -315,24 +309,21 @@
     ) -> None:
         """Remove jobs that schedule obsolete pipelines.
 
         Parameters
         ----------
         obsolete_pipelines : list
             List of dictionaries representing obsolete pipelines in the format
-            [{ "pipeline_name": pipeline_name,
+            [{ "name": pipeline_name,
                "pipeline_id": pipeline_id
             }, ...]
         workflows_jobs : list
             List of jobs scheduled in Databricks Workflows, having the format
             [{ "job_name": job_name,
                "job_id": job_id,
                "pipeline_id": pipeline_id | None
             }, ...]
         """
         for p in obsolete_pipelines:
             for j in workflows_jobs:
-                if (
-                    j["name"] == p["pipline_name"]
-                    or j["pipeline_id"] == p["pipeline_id"]
-                ):
+                if j["name"] == p["name"] or j["pipeline_id"] == p["pipeline_id"]:
                     self.jobs_wrapper.delete_job(j["job_id"])
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/secrets_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,74 +16,74 @@
 
 """
 
 import logging
 
 from databricks_cli.sdk.api_client import ApiClient
 from databricks_cli.secrets.api import SecretApi
-from pydantic import Field, constr, dataclasses, validate_arguments
+from pydantic import Field, constr, dataclasses, validate_call
 
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class SecretsWrapper:
     """Wrapper around the Databricks Secrets API.
 
     Manage secrets in a Databricks workspace. It allows creating a secret scope if it
     does not exist and pushing secrets to the scope.
     """
 
     client: ApiClient
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger."""
         self.log = logging.getLogger(__name__)
 
         self.secrets_api = SecretApi(self.client)
 
-    @validate_arguments
+    @validate_call
     def create_scope_if_not_exists(
         self,
         secret_scope_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
-            regex=r"^[A-Za-z0-9\-_.]{1,128}$",
+            pattern=r"^[A-Za-z0-9\-_.]{1,128}$",
         ) = "pushcart",  # noqa: S107
     ) -> None:
         """Create a secret scope if it does not exist in the workspace."""
         scopes = self.secrets_api.list_scopes()["scopes"]
         if secret_scope_name not in [scope["name"] for scope in scopes]:
             self.secrets_api.create_scope(
                 initial_manage_principal="users",
                 scope=secret_scope_name,
                 scope_backend_type="DATABRICKS",
                 backend_azure_keyvault=None,
             )
             self.log.info(f"Created secret scope {secret_scope_name}")
 
-    @validate_arguments
+    @validate_call
     def push_secrets(
         self,
         secret_scope_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
-            regex=r"^[A-Za-z0-9\-_.]{1,128}$",
+            pattern=r"^[A-Za-z0-9\-_.]{1,128}$",
         ) = "pushcart",  # noqa: S107
         secrets_dict: dict[
             constr(
                 strip_whitespace=True,
                 to_lower=True,
                 strict=True,
                 min_length=1,
-                regex=r"^[A-Za-z0-9\-_.]{1,128}$",
+                pattern=r"^[A-Za-z0-9\-_.]{1,128}$",
             ),
             str,
         ] = Field(  # noqa: B008
             default_factory=dict,
         ),
     ) -> None:
         """Pushes secrets to a secret scope in the workspace."""
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/base_settings.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/base_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 Loads a configuration from file. Settings may come in JSON, TOML or YAML formats.
 """
 
 import asyncio
 import logging
 from pathlib import Path
 
-from pydantic import DirectoryPath, constr, dataclasses, validate_arguments
+from pydantic import DirectoryPath, constr, dataclasses, validate_call
 
 from pushcart_deploy.configuration import expect_at_most_one_file, get_config_from_file
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class BaseSettings:
     """Base Databricks API settings class.
 
     Retrieves pipeline/job settings file, if one exists.
     """
 
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger."""
         self.log = logging.getLogger(__name__)
 
+    @validate_call
     def get_settings_path_for_pipeline(
         self,
         target_catalog_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
@@ -47,15 +48,15 @@
             min_length=1,
         ),
         settings_file_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
-            regex=r"^(_job_settings|_pipeline_settings)$",
+            pattern=r"^(_job_settings|_pipeline_settings)$",
         ),
     ) -> Path:
         """Look for a settings file in the pipeline directory.
 
         Parameters
         ----------
         target_catalog_name : str
@@ -79,15 +80,15 @@
             / target_schema_name
             / pipeline_name
             / settings_file_name
         )
 
         return expect_at_most_one_file(base_path)
 
-    @validate_arguments
+    @validate_call
     def load_settings(
         self,
         target_catalog_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
@@ -105,15 +106,15 @@
             min_length=1,
         ),
         settings_file_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
-            regex=r"^(_job_settings|_pipeline_settings)$",
+            pattern=r"^(_job_settings|_pipeline_settings)$",
         ),
     ) -> dict:
         """Load pipeline/job settings from file, if one exists.
 
         Parameters
         ----------
         target_catalog_name : str
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/job_settings.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/job_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
 environment.
 
 """
 
 import logging
 
-from pydantic import DirectoryPath, dataclasses, validate_arguments
+from pydantic import DirectoryPath, dataclasses, validate_call
 
 from pushcart_deploy.databricks_api.settings import BaseSettings
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class JobSettings:
@@ -29,15 +29,15 @@
 
     Provides methods for loading job settings from a JSON file or string, as well as
     for retrieving default job settings for checkpoint and pipeline jobs.
     """
 
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger and BaseSettings."""
         self.log = logging.getLogger(__name__)
         self.base_settings = BaseSettings(self.config_dir)
 
     def _update_job_settings(
         self,
         job_settings: dict,
@@ -55,15 +55,15 @@
         pipeline_id : str
             ID of an existing pipeline.
         """
         job_settings["name"] = pipeline_name
         job_settings["tasks"][0]["task_key"] = pipeline_name
         job_settings["tasks"][0]["pipeline_task"]["pipeline_id"] = pipeline_id
 
-    @validate_arguments
+    @validate_call
     def load_job_settings(
         self,
         target_catalog_name: str,
         target_schema_name: str,
         pipeline_name: str,
         pipeline_id: str,
     ) -> dict:
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import logging
 import operator
 
 from databricks_cli.clusters.api import ClusterApi
 from databricks_cli.sdk.api_client import ApiClient
 from methodtools import lru_cache
-from pydantic import DirectoryPath, dataclasses, validate_arguments
+from pydantic import DirectoryPath, dataclasses, validate_call
 
 from pushcart_deploy.databricks_api.settings import BaseSettings
 from pushcart_deploy.validation import PydanticArbitraryTypesConfig
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class PipelineSettings:
@@ -22,15 +22,15 @@
     Provides methods for loading pipeline settings from a JSON file or string, as well
     as for retrieving default settings for DLT pipelines.
     """
 
     api_client: ApiClient
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger and dependent API classes."""
         self.log = logging.getLogger(__name__)
         self.cluster_api = ClusterApi(self.api_client)
         self.base_settings = BaseSettings(self.config_dir)
 
     @lru_cache(maxsize=1)
     def _get_smallest_cluster_node_type(self) -> str:
@@ -103,15 +103,15 @@
         pipeline_settings["target"] = target_schema_name
         pipeline_settings["libraries"] = libraries
         pipeline_settings["configuration"] = configuration
 
         if pipeline_id:
             pipeline_settings["id"] = pipeline_id
 
-    @validate_arguments
+    @validate_call
     def load_pipeline_settings(  # noqa: PLR0913
         self,
         target_catalog_name: str,
         target_schema_name: str,
         pipeline_name: str,
         libraries: list[dict],
         configuration: dict[str, str],
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/metadata.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         - pushcart.sources
         - pushcart.transformations
         - pushcart.destinations
     """
 
     config_dir: DirectoryPath
 
-    def __post_init_post_parse__(self) -> None:
+    def __post_init__(self) -> None:
         """Initialize logger."""
         self.log = logging.getLogger(__name__)
 
     @staticmethod
     async def _load_pipeline_with_metadata(file_path: str) -> dict:
         config = await get_config_from_file(file_path)
         if config is None:
@@ -261,12 +261,12 @@
                 ),
             )
 
         return [
             {
                 "target_catalog_name": row["target_catalog_name"],
                 "target_schema_name": row["target_schema_name"],
-                "pipeline_name": row["pipeline_name"],
+                "name": row["pipeline_name"],
                 "pipeline_id": None,
             }
             for row in pipelines_df.distinct().collect()
         ]
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/setup.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 class Setup:
     """Runs a Pushcart deployment."""
 
     config_dir: DirectoryPath
     non_destructive: bool
 
     @provide_api_client
-    def __post_init_post_parse__(self, api_client: ApiClient) -> None:
+    def __post_init__(self, api_client: ApiClient) -> None:
         """Initialize logger.
 
         Parameters
         ----------
         api_client : ApiClient
             Used to log target Databricks environment URL
         """
```

### Comparing `pushcart_deploy-1.6.1/src/pushcart_deploy/validation.py` & `pushcart_deploy-1.6.5/src/pushcart_deploy/validation.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.6.1/PKG-INFO` & `pushcart_deploy-1.6.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushcart-deploy
-Version: 1.6.1
+Version: 1.6.5
 Summary: Deployment helper for pipeline configurations using Pushcart
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
 Requires-Dist: databricks-connect (>=13.0.0,<14.0.0)
 Requires-Dist: methodtools (>=0.4.7,<0.5.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: urllib3 (>=1,<2)
 Description-Content-Type: text/markdown
 
 # pushcart-deploy
```

