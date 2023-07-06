# Comparing `tmp/apache-airflow-providers-postgres-5.5.1rc1.tar.gz` & `tmp/apache-airflow-providers-postgres-5.5.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-postgres-5.5.1rc1.tar", last modified: Tue Jun 20 11:42:54 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.5.2rc2.tar", last modified: Thu Jul  6 04:51:20 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.5.1rc1.tar` & `apache-airflow-providers-postgres-5.5.2rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.369568 apache-airflow-providers-postgres-5.5.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.371066 apache-airflow-providers-postgres-5.5.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13982 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.296192 apache-airflow-providers-postgres-5.5.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.297518 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.330567 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.336290 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12967 2023-06-05 12:50:36.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.342002 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-02 11:31:21.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.366685 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1914 2023-06-20 11:42:54.373575 apache-airflow-providers-postgres-5.5.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.382146 apache-airflow-providers-postgres-5.5.2rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.2rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.382738 apache-airflow-providers-postgres-5.5.2rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4113 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.304592 apache-airflow-providers-postgres-5.5.2rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.305843 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.340819 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-06 04:42:33.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.347351 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13342 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.353272 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-07-05 07:19:39.000000 apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 04:51:20.379739 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5809 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 04:51:20.000000 apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2012 2023-07-06 04:51:20.384790 apache-airflow-providers-postgres-5.5.2rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-06 04:51:19.000000 apache-airflow-providers-postgres-5.5.2rc2/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/LICENSE` & `apache-airflow-providers-postgres-5.5.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in` & `apache-airflow-providers-postgres-5.5.2rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.5.1"
+__version__ = "5.5.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-postgres",
         "name": "PostgreSQL",
         "description": "`PostgreSQL <https://www.postgresql.org/>`__\n",
         "suspended": False,
         "versions": [
+            "5.5.2",
             "5.5.1",
             "5.5.0",
             "5.4.0",
             "5.3.1",
             "5.3.0",
             "5.2.2",
             "5.2.1",
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/hooks/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,35 +55,39 @@
     For Redshift, also use redshift in the extra connection parameters and
     set it to true. The cluster-identifier is extracted from the beginning of
     the host field, so is optional. It can however be overridden in the extra field.
     extras example: ``{"iam":true, "redshift":true, "cluster-identifier": "my_cluster_id"}``
 
     :param postgres_conn_id: The :ref:`postgres conn id <howto/connection:postgres>`
         reference to a specific postgres database.
+    :param options: Optional. Specifies command-line options to send to the server
+        at connection start. For example, setting this to ``-c search_path=myschema``
+        sets the session's value of the ``search_path`` to ``myschema``.
     """
 
     conn_name_attr = "postgres_conn_id"
     default_conn_name = "postgres_default"
     conn_type = "postgres"
     hook_name = "Postgres"
     supports_autocommit = True
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, options: str | None = None, **kwargs) -> None:
         if "schema" in kwargs:
             warnings.warn(
                 'The "schema" arg has been renamed to "database" as it contained the database name.'
                 'Please use "database" to set the database name.',
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
             kwargs["database"] = kwargs["schema"]
         super().__init__(*args, **kwargs)
         self.connection: Connection | None = kwargs.pop("connection", None)
         self.conn: connection = None
         self.database: str | None = kwargs.pop("database", None)
+        self.options = options
 
     @property
     def schema(self):
         warnings.warn(
             'The "schema" variable has been renamed to "database" as it contained the database name.'
             'Please use "database" to get the database name.',
             AirflowProviderDeprecationWarning,
@@ -127,14 +131,17 @@
             dbname=self.database or conn.schema,
             port=conn.port,
         )
         raw_cursor = conn.extra_dejson.get("cursor", False)
         if raw_cursor:
             conn_args["cursor_factory"] = self._get_cursor(raw_cursor)
 
+        if self.options:
+            conn_args["options"] = self.options
+
         for arg_name, arg_val in conn.extra_dejson.items():
             if arg_name not in [
                 "iam",
                 "redshift",
                 "cursor",
                 "cluster-identifier",
                 "aws_conn_id",
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.5.2rc2/airflow/providers/postgres/operators/postgres.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import warnings
 from typing import Mapping, Sequence
 
-from psycopg2.sql import SQL, Identifier
-
 from airflow.exceptions import AirflowProviderDeprecationWarning
 from airflow.providers.common.sql.operators.sql import SQLExecuteQueryOperator
 
 
 class PostgresOperator(SQLExecuteQueryOperator):
     """
     Executes sql code in a specific Postgres database.
@@ -37,14 +35,15 @@
         reference to a specific postgres database.
     :param autocommit: if True, each command is automatically committed.
         (default value: False)
     :param parameters: (optional) the parameters to render the SQL query with.
     :param database: name of database which overwrite defined one in connection
     :param runtime_parameters: a mapping of runtime params added to the final sql being executed.
         For example, you could set the schema via `{"search_path": "CUSTOM_SCHEMA"}`.
+        Deprecated - use `hook_params={'options': '-c <connection_options>'}` instead.
     """
 
     template_fields: Sequence[str] = ("sql",)
     template_fields_renderers = {"sql": "postgresql"}
     template_ext: Sequence[str] = (".sql",)
     ui_color = "#ededed"
 
@@ -57,34 +56,23 @@
         **kwargs,
     ) -> None:
         if database is not None:
             hook_params = kwargs.pop("hook_params", {})
             kwargs["hook_params"] = {"schema": database, **hook_params}
 
         if runtime_parameters:
-            sql = kwargs.pop("sql")
-            parameters = kwargs.pop("parameters", {})
-
-            final_sql = []
-            sql_param = {}
-            for param in runtime_parameters:
-                set_param_sql = f"SET {{}} TO %({param})s;"
-                dynamic_sql = SQL(set_param_sql).format(Identifier(f"{param}"))
-                final_sql.append(dynamic_sql)
-            for param, val in runtime_parameters.items():
-                sql_param.update({f"{param}": f"{val}"})
-            if parameters:
-                sql_param.update(parameters)
-            if isinstance(sql, str):
-                final_sql.append(SQL(sql))
-            else:
-                final_sql.extend(list(map(SQL, sql)))
-
-            kwargs["sql"] = final_sql
-            kwargs["parameters"] = sql_param
+            warnings.warn(
+                """`runtime_parameters` is deprecated.
+                Please use `hook_params={'options': '-c <connection_options>}`.""",
+                AirflowProviderDeprecationWarning,
+                stacklevel=2,
+            )
+            hook_params = kwargs.pop("hook_params", {})
+            options = " ".join(f"-c {param}={val}" for param, val in runtime_parameters.items())
+            kwargs["hook_params"] = {"options": options, **hook_params}
 
         super().__init__(conn_id=postgres_conn_id, **kwargs)
         warnings.warn(
             """This class is deprecated.
             Please use `airflow.providers.common.sql.operators.sql.SQLExecuteQueryOperator`.
             Also, you can provide `hook_params={'schema': <database>}`.""",
             AirflowProviderDeprecationWarning,
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.5.2rc2/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml` & `apache-airflow-providers-postgres-5.5.2rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/setup.cfg` & `apache-airflow-providers-postgres-5.5.2rc2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -54,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.5.1rc1/setup.py` & `apache-airflow-providers-postgres-5.5.2rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-postgres package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.5.1"
+version = "5.5.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-postgres setup."""
     setup(
         version=version,
         extras_require={
```

