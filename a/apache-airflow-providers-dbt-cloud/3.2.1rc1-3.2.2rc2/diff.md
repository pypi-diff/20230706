# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:51 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.2rc2.tar", last modified: Thu Jul  6 04:50:38 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1.tar` & `apache-airflow-providers-dbt-cloud-3.2.2rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.021236 apache-airflow-providers-dbt-cloud-3.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:51.022307 apache-airflow-providers-dbt-cloud-3.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10170 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.931297 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.932461 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.933570 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.970994 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.976859 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24235 2023-06-02 11:31:21.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.983054 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13638 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.988790 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.994693 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.018368 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1896 2023-06-20 11:41:51.024226 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.100429 apache-airflow-providers-dbt-cloud-3.2.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-07-06 04:50:38.101014 apache-airflow-providers-dbt-cloud-3.2.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.004457 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.005643 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.006918 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.047748 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.054061 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24242 2023-06-29 05:49:30.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.060405 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13665 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.066375 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-07-05 07:19:39.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.072281 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:50:38.097790 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:50:37.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-07-06 04:50:38.102975 apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-07-06 04:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.1"
+__version__ = "3.2.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-dbt-cloud",
         "name": "dbt Cloud",
         "description": "`dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.2",
             "3.2.1",
             "3.2.0",
             "3.1.1",
             "3.1.0",
             "3.0.0",
             "2.3.1",
             "2.3.0",
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,18 @@
     from requests.models import PreparedRequest, Response
 
     from airflow.models import Connection
 
 
 def fallback_to_default_account(func: Callable) -> Callable:
     """
-    Decorator which provides a fallback value for ``account_id``. If the ``account_id`` is None or not passed
-    to the decorated function, the value will be taken from the configured dbt Cloud Airflow Connection.
+    Decorator which provides a fallback value for ``account_id``.
+
+    If the ``account_id`` is None or not passed to the decorated function,
+    the value will be taken from the configured dbt Cloud Airflow Connection.
     """
     sig = signature(func)
 
     @wraps(func)
     def wrapper(*args, **kwargs) -> Callable:
         bound_args = sig.bind(*args, **kwargs)
 
@@ -130,16 +132,18 @@
 
 
 T = TypeVar("T", bound=Any)
 
 
 def provide_account_id(func: T) -> T:
     """
-    Decorator which provides a fallback value for ``account_id``. If the ``account_id`` is None or not passed
-    to the decorated function, the value will be taken from the configured dbt Cloud Airflow Connection.
+    Decorator which provides a fallback value for ``account_id``.
+
+    If the ``account_id`` is None or not passed to the decorated function,
+    the value will be taken from the configured dbt Cloud Airflow Connection.
     """
     function_signature = signature(func)
 
     @wraps(func)
     async def wrapper(*args: Any, **kwargs: Any) -> Any:
         bound_args = function_signature.bind(*args, **kwargs)
 
@@ -358,16 +362,17 @@
     def list_jobs(
         self,
         account_id: int | None = None,
         order_by: str | None = None,
         project_id: int | None = None,
     ) -> list[Response]:
         """
-        Retrieves metadata for all jobs tied to a specified dbt Cloud account. If a ``project_id`` is
-        supplied, only jobs pertaining to this project will be retrieved.
+        Retrieves metadata for all jobs tied to a specified dbt Cloud account.
+
+        If a ``project_id`` is supplied, only jobs pertaining to this project will be retrieved.
 
         :param account_id: Optional. The ID of a dbt Cloud account.
         :param order_by: Optional. Field to order the result by. Use '-' to indicate reverse order.
             For example, to use reverse order by the run ID use ``order_by=-id``.
         :param project_id: The ID of a dbt Cloud project.
         :return: List of request responses.
         """
@@ -433,16 +438,17 @@
         self,
         account_id: int | None = None,
         include_related: list[str] | None = None,
         job_definition_id: int | None = None,
         order_by: str | None = None,
     ) -> list[Response]:
         """
-        Retrieves metadata for all of the dbt Cloud job runs for an account. If a ``job_definition_id`` is
-        supplied, only metadata for runs of that specific job are pulled.
+        Retrieves metadata for all dbt Cloud job runs for an account.
+
+        If a ``job_definition_id`` is supplied, only metadata for runs of that specific job are pulled.
 
         :param account_id: Optional. The ID of a dbt Cloud account.
         :param include_related: Optional. List of related fields to pull with the run.
             Valid values are "trigger", "job", "repository", and "environment".
         :param job_definition_id: Optional. The dbt Cloud job ID to retrieve run metadata.
         :param order_by: Optional. Field to order the result by. Use '-' to indicate reverse order.
             For example, to use reverse order by the run ID use ``order_by=-id``.
@@ -551,17 +557,18 @@
         self._run_and_get_response(method="POST", endpoint=f"{account_id}/runs/{run_id}/cancel/")
 
     @fallback_to_default_account
     def list_job_run_artifacts(
         self, run_id: int, account_id: int | None = None, step: int | None = None
     ) -> list[Response]:
         """
-        Retrieves a list of the available artifact files generated for a completed run of a dbt Cloud job. By
-        default, this returns artifacts from the last step in the run. To list artifacts from other steps in
-        the run, use the ``step`` parameter.
+        Retrieves a list of the available artifact files generated for a completed run of a dbt Cloud job.
+
+        By default, this returns artifacts from the last step in the run. To
+        list artifacts from other steps in the run, use the ``step`` parameter.
 
         :param run_id: The ID of a dbt Cloud job run.
         :param account_id: Optional. The ID of a dbt Cloud account.
         :param step: Optional. The index of the Step in the Run to query for artifacts. The first step in the
             run has the index 1. If the step parameter is omitted, artifacts for the last step in the run will
             be returned.
         :return: List of request responses.
@@ -571,17 +578,18 @@
         )
 
     @fallback_to_default_account
     def get_job_run_artifact(
         self, run_id: int, path: str, account_id: int | None = None, step: int | None = None
     ) -> Response:
         """
-        Retrieves a list of the available artifact files generated for a completed run of a dbt Cloud job. By
-        default, this returns artifacts from the last step in the run. To list artifacts from other steps in
-        the run, use the ``step`` parameter.
+        Retrieves a list of the available artifact files generated for a completed run of a dbt Cloud job.
+
+        By default, this returns artifacts from the last step in the run. To
+        list artifacts from other steps in the run, use the ``step`` parameter.
 
         :param run_id: The ID of a dbt Cloud job run.
         :param path: The file path related to the artifact file. Paths are rooted at the target/ directory.
             Use "manifest.json", "catalog.json", or "run_results.json" to download dbt-generated artifacts
             for the run.
         :param account_id: Optional. The ID of a dbt Cloud account.
         :param step: Optional. The index of the Step in the Run to query for artifacts. The first step in the
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import json
 import time
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException
 from airflow.models import BaseOperator, BaseOperatorLink, XCom
 from airflow.providers.dbt.cloud.hooks.dbt import (
     DbtCloudHook,
     DbtCloudJobRunException,
     DbtCloudJobRunStatus,
     JobRunInfo,
@@ -33,18 +34,15 @@
 from airflow.providers.dbt.cloud.triggers.dbt import DbtCloudRunJobTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DbtCloudRunJobOperatorLink(BaseOperatorLink):
-    """
-    Operator link for DbtCloudRunJobOperator. This link allows users to monitor the triggered job run
-    directly in dbt Cloud.
-    """
+    """Allows users to monitor the triggered job run directly in dbt Cloud."""
 
     name = "Monitor Job Run"
 
     def get_link(self, operator: BaseOperator, *, ti_key=None):
         return XCom.get_value(key="job_run_url", ti_key=ti_key)
 
 
@@ -98,15 +96,15 @@
         trigger_reason: str | None = None,
         steps_override: list[str] | None = None,
         schema_override: str | None = None,
         wait_for_termination: bool = True,
         timeout: int = 60 * 60 * 24 * 7,
         check_interval: int = 60,
         additional_run_config: dict[str, Any] | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.dbt_cloud_conn_id = dbt_cloud_conn_id
         self.account_id = account_id
         self.job_id = job_id
         self.trigger_reason = trigger_reason
@@ -188,16 +186,16 @@
                     "`deferrable` parameter doesn't have any effect",
                 )
             return self.run_id
 
     def execute_complete(self, context: Context, event: dict[str, Any]) -> int:
         """
         Callback for when the trigger fires - returns immediately.
-        Relies on trigger to throw an exception, otherwise it assumes execution was
-        successful.
+
+        Relies on trigger to throw an exception, otherwise it assumes execution was successful.
         """
         if event["status"] == "error":
             raise AirflowException(event["message"])
         self.log.info(event["message"])
         return int(event["run_id"])
 
     def on_kill(self) -> None:
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # under the License.
 from __future__ import annotations
 
 import time
 import warnings
 from typing import TYPE_CHECKING, Any
 
+from airflow.configuration import conf
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.dbt.cloud.hooks.dbt import DbtCloudHook, DbtCloudJobRunException, DbtCloudJobRunStatus
 from airflow.providers.dbt.cloud.triggers.dbt import DbtCloudRunJobTrigger
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -46,15 +47,15 @@
 
     def __init__(
         self,
         *,
         dbt_cloud_conn_id: str = DbtCloudHook.default_conn_name,
         run_id: int,
         account_id: int | None = None,
-        deferrable: bool = False,
+        deferrable: bool = conf.getboolean("operators", "default_deferrable", fallback=False),
         **kwargs,
     ) -> None:
         if deferrable:
             if "poke_interval" not in kwargs:
                 # TODO: Remove once deprecated
                 if "polling_interval" in kwargs:
                     kwargs["poke_interval"] = kwargs["polling_interval"]
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -55,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.2rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-dbt-cloud package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.1"
+version = "3.2.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-dbt-cloud setup."""
     setup(
         version=version,
         extras_require={"http": ["apache-airflow-providers-http"]},
```

