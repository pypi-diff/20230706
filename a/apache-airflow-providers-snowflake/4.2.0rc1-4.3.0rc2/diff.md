# Comparing `tmp/apache-airflow-providers-snowflake-4.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.2.0rc1.tar", last modified: Tue Jun 20 11:43:15 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.3.0rc2.tar", last modified: Thu Jul  6 04:51:33 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.2.0rc1.tar` & `apache-airflow-providers-snowflake-4.3.0rc2.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.974181 apache-airflow-providers-snowflake-4.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.975546 apache-airflow-providers-snowflake-4.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18321 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.861078 apache-airflow-providers-snowflake-4.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.862300 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.902943 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4724 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.912718 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    11759 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.918823 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22918 2023-06-17 16:45:00.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.931338 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.942711 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.970806 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1192 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1960 2023-06-20 11:43:15.977871 apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.382175 apache-airflow-providers-snowflake-4.3.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.382708 apache-airflow-providers-snowflake-4.3.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4174 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.267934 apache-airflow-providers-snowflake-4.3.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.269026 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.309311 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-06 04:42:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.319211 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12676 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.325917 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24666 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.338441 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.344467 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.354559 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:33.379560 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5873 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:33.000000 apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-07-06 04:51:33.384605 apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-06 04:51:32.000000 apache-airflow-providers-snowflake-4.3.0rc2/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/LICENSE` & `apache-airflow-providers-snowflake-4.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in` & `apache-airflow-providers-snowflake-4.3.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.5",
             "4.0.4",
             "4.0.3",
             "4.0.2",
             "4.0.1",
@@ -120,8 +121,14 @@
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.snowflake.hooks.snowflake.SnowflakeHook",
                 "connection-type": "snowflake",
             }
         ],
+        "triggers": [
+            {
+                "integration-name": "Snowflake",
+                "python-modules": ["airflow.providers.snowflake.triggers.snowflake_trigger"],
+            }
+        ],
     }
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from __future__ import annotations
 
 import uuid
 from datetime import timedelta
 from pathlib import Path
 from typing import Any
 
+import aiohttp
 import requests
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
 from airflow import AirflowException
 from airflow.providers.snowflake.hooks.snowflake import SnowflakeHook
 from airflow.providers.snowflake.utils.sql_api_generate_jwt import JWTGenerator
@@ -55,15 +56,16 @@
     :param database: name of snowflake database
     :param region: name of snowflake region
     :param role: name of snowflake role
     :param schema: name of snowflake schema
     :param session_parameters: You can set session-level parameters at
         the time you connect to Snowflake
     :param token_life_time: lifetime of the JWT Token in timedelta
-    :param token_renewal_delta: Renewal time of the JWT Token in  timedelta
+    :param token_renewal_delta: Renewal time of the JWT Token in timedelta
+    :param deferrable: Run operator in the deferrable mode.
     """
 
     LIFETIME = timedelta(minutes=59)  # The tokens will have a 59 minute lifetime
     RENEWAL_DELTA = timedelta(minutes=54)  # Tokens will be renewed after 54 minutes
 
     def __init__(
         self,
@@ -221,25 +223,15 @@
                 response.raise_for_status()
                 self.log.info(response.json())
             except requests.exceptions.HTTPError as e:
                 raise AirflowException(
                     f"Response: {e.response.content}, Status Code: {e.response.status_code}"
                 )
 
-    def get_sql_api_query_status(self, query_id: str) -> dict[str, str | list[str]]:
-        """
-        Based on the query id async HTTP request is made to snowflake SQL API and return response.
-
-        :param query_id: statement handle id for the individual statements.
-        """
-        self.log.info("Retrieving status for query id %s", {query_id})
-        header, params, url = self.get_request_url_header_params(query_id)
-        response = requests.get(url, params=params, headers=header)
-        status_code = response.status_code
-        resp = response.json()
+    def _process_response(self, status_code, resp):
         self.log.info("Snowflake SQL GET statements status API response: %s", resp)
         if status_code == 202:
             return {"status": "running", "message": "Query statements are still running"}
         elif status_code == 422:
             return {"status": "error", "message": resp["message"]}
         elif status_code == 200:
             statement_handles = []
@@ -250,7 +242,34 @@
             return {
                 "status": "success",
                 "message": resp["message"],
                 "statement_handles": statement_handles,
             }
         else:
             return {"status": "error", "message": resp["message"]}
+
+    def get_sql_api_query_status(self, query_id: str) -> dict[str, str | list[str]]:
+        """
+        Based on the query id async HTTP request is made to snowflake SQL API and return response.
+
+        :param query_id: statement handle id for the individual statements.
+        """
+        self.log.info("Retrieving status for query id %s", query_id)
+        header, params, url = self.get_request_url_header_params(query_id)
+        response = requests.get(url, params=params, headers=header)
+        status_code = response.status_code
+        resp = response.json()
+        return self._process_response(status_code, resp)
+
+    async def get_sql_api_query_status_async(self, query_id: str) -> dict[str, str | list[str]]:
+        """
+        Based on the query id async HTTP request is made to snowflake SQL API and return response.
+
+        :param query_id: statement handle id for the individual statements.
+        """
+        self.log.info("Retrieving status for query id %s", query_id)
+        header, params, url = self.get_request_url_header_params(query_id)
+        async with aiohttp.ClientSession(headers=header) as session:
+            async with session.get(url, params=params) as response:
+                status_code = response.status
+                resp = await response.json()
+                return self._process_response(status_code, resp)
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import time
 import warnings
 from datetime import timedelta
-from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence, SupportsAbs
+from typing import TYPE_CHECKING, Any, Iterable, List, Mapping, Sequence, SupportsAbs, cast
 
 from airflow import AirflowException
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import (
     SQLCheckOperator,
     SQLExecuteQueryOperator,
     SQLIntervalCheckOperator,
     SQLValueCheckOperator,
 )
 from airflow.providers.snowflake.hooks.snowflake_sql_api import (
     SnowflakeSqlApiHook,
 )
+from airflow.providers.snowflake.triggers.snowflake_trigger import SnowflakeSqlApiTrigger
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class SnowflakeOperator(SQLExecuteQueryOperator):
     """
@@ -426,14 +427,15 @@
     :param poll_interval: the interval in seconds to poll the query
     :param statement_count: Number of SQL statement to be executed
     :param token_life_time: lifetime of the JWT Token
     :param token_renewal_delta: Renewal time of the JWT Token
     :param bindings: (Optional) Values of bind variables in the SQL statement.
             When executing the statement, Snowflake replaces placeholders (? and :name) in
             the statement with these specified values.
+    :param deferrable: Run operator in the deferrable mode.
     """  # noqa
 
     LIFETIME = timedelta(minutes=59)  # The tokens will have a 59 minutes lifetime
     RENEWAL_DELTA = timedelta(minutes=54)  # Tokens will be renewed after 54 minutes
 
     def __init__(
         self,
@@ -446,23 +448,25 @@
         authenticator: str | None = None,
         session_parameters: dict[str, Any] | None = None,
         poll_interval: int = 5,
         statement_count: int = 0,
         token_life_time: timedelta = LIFETIME,
         token_renewal_delta: timedelta = RENEWAL_DELTA,
         bindings: dict[str, Any] | None = None,
+        deferrable: bool = False,
         **kwargs: Any,
     ) -> None:
         self.snowflake_conn_id = snowflake_conn_id
         self.poll_interval = poll_interval
         self.statement_count = statement_count
         self.token_life_time = token_life_time
         self.token_renewal_delta = token_renewal_delta
         self.bindings = bindings
         self.execute_async = False
+        self.deferrable = deferrable
         if any([warehouse, database, role, schema, authenticator, session_parameters]):  # pragma: no cover
             hook_params = kwargs.pop("hook_params", {})  # pragma: no cover
             kwargs["hook_params"] = {
                 "warehouse": warehouse,
                 "database": database,
                 "role": role,
                 "schema": schema,
@@ -478,27 +482,41 @@
         By deferring the SnowflakeSqlApiTrigger class passed along with query ids.
         """
         self.log.info("Executing: %s", self.sql)
         self._hook = SnowflakeSqlApiHook(
             snowflake_conn_id=self.snowflake_conn_id,
             token_life_time=self.token_life_time,
             token_renewal_delta=self.token_renewal_delta,
+            deferrable=self.deferrable,
         )
         self.query_ids = self._hook.execute_query(
             self.sql, statement_count=self.statement_count, bindings=self.bindings  # type: ignore[arg-type]
         )
         self.log.info("List of query ids %s", self.query_ids)
 
         if self.do_xcom_push:
             context["ti"].xcom_push(key="query_ids", value=self.query_ids)
 
-        statement_status = self.poll_on_queries()
-        if statement_status["error"]:
-            raise AirflowException(statement_status["error"])
-        self._hook.check_query_output(self.query_ids)
+        if self.deferrable:
+            self.defer(
+                timeout=self.execution_timeout,
+                trigger=SnowflakeSqlApiTrigger(
+                    poll_interval=self.poll_interval,
+                    query_ids=self.query_ids,
+                    snowflake_conn_id=self.snowflake_conn_id,
+                    token_life_time=self.token_life_time,
+                    token_renewal_delta=self.token_renewal_delta,
+                ),
+                method_name="execute_complete",
+            )
+        else:
+            statement_status = self.poll_on_queries()
+            if statement_status["error"]:
+                raise AirflowException(statement_status["error"])
+            self._hook.check_query_output(self.query_ids)
 
     def poll_on_queries(self):
         """Poll on requested queries."""
         queries_in_progress = set(self.query_ids)
         statement_success_status = {}
         statement_error_status = {}
         for query_id in self.query_ids:
@@ -513,7 +531,25 @@
                 queries_in_progress.remove(query_id)
                 statement_error_status[query_id] = statement_status
             if statement_status.get("status") == "success":
                 statement_success_status[query_id] = statement_status
                 queries_in_progress.remove(query_id)
             time.sleep(self.poll_interval)
         return {"success": statement_success_status, "error": statement_error_status}
+
+    def execute_complete(self, context: Context, event: dict[str, str | list[str]] | None = None) -> None:
+        """
+        Callback for when the trigger fires - returns immediately.
+        Relies on trigger to throw an exception, otherwise it assumes execution was
+        successful.
+        """
+        if event:
+            if "status" in event and event["status"] == "error":
+                msg = f"{event['status']}: {event['message']}"
+                raise AirflowException(msg)
+            elif "status" in event and event["status"] == "success":
+                hook = SnowflakeSqlApiHook(snowflake_conn_id=self.snowflake_conn_id)
+                query_ids = cast(List[str], event["statement_query_ids"])
+                hook.check_query_output(query_ids)
+                self.log.info("%s completed successfully.", self.task_id)
+        else:
+            self.log.info("%s completed successfully.", self.task_id)
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.3.0rc2/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.3.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 airflow/providers/snowflake/hooks/snowflake_sql_api.py
 airflow/providers/snowflake/operators/__init__.py
 airflow/providers/snowflake/operators/snowflake.py
 airflow/providers/snowflake/transfers/__init__.py
 airflow/providers/snowflake/transfers/copy_into_snowflake.py
 airflow/providers/snowflake/transfers/s3_to_snowflake.py
 airflow/providers/snowflake/transfers/snowflake_to_slack.py
+airflow/providers/snowflake/triggers/__init__.py
+airflow/providers/snowflake/triggers/snowflake_trigger.py
 airflow/providers/snowflake/utils/__init__.py
 airflow/providers/snowflake/utils/common.py
 airflow/providers/snowflake/utils/sql_api_generate_jwt.py
 apache_airflow_providers_snowflake.egg-info/PKG-INFO
 apache_airflow_providers_snowflake.egg-info/SOURCES.txt
 apache_airflow_providers_snowflake.egg-info/dependency_links.txt
 apache_airflow_providers_snowflake.egg-info/entry_points.txt
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml` & `apache-airflow-providers-snowflake-4.3.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg` & `apache-airflow-providers-snowflake-4.3.0rc2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.3.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -55,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.2.0rc1/setup.py` & `apache-airflow-providers-snowflake-4.3.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-snowflake package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.2.0"
+version = "4.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-snowflake setup."""
     setup(
         version=version,
         extras_require={
```

