# Comparing `tmp/kedro-graphql-0.3.4.tar.gz` & `tmp/kedro-graphql-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.3.4.tar", last modified: Tue Jun 27 18:53:59 2023, max compression
+gzip compressed data, was "kedro-graphql-0.3.5.tar", last modified: Thu Jul  6 19:17:47 2023, max compression
```

## Comparing `kedro-graphql-0.3.4.tar` & `kedro-graphql-0.3.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.360808 kedro-graphql-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/example/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/json_log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/logs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.364808 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-27 18:53:59.000000 kedro-graphql-0.3.4/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:59.368808 kedro-graphql-0.3.4/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-27 18:53:47.000000 kedro-graphql-0.3.4/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.085961 kedro-graphql-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-06 19:17:47.085961 kedro-graphql-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 19:17:47.085961 kedro-graphql-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.073961 kedro-graphql-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.077961 kedro-graphql-0.3.5/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.077961 kedro-graphql-0.3.5/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/example/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/kedro_graphql/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/logs/json_log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/logs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.077961 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:17:47.000000 kedro-graphql-0.3.5/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.081961 kedro-graphql-0.3.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.085961 kedro-graphql-0.3.5/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:47.085961 kedro-graphql-0.3.5/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-06 19:17:35.000000 kedro-graphql-0.3.5/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.3.4/LICENSE.txt` & `kedro-graphql-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/PKG-INFO` & `kedro-graphql-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.4
+Version: 0.3.5
 Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.3.4/README.md` & `kedro-graphql-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/pyproject.toml` & `kedro-graphql-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/__main__.py` & `kedro-graphql-0.3.5/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/asgi.py` & `kedro-graphql-0.3.5/src/kedro_graphql/asgi.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.3.5/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.3.5/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/commands.py` & `kedro-graphql-0.3.5/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/config.py` & `kedro-graphql-0.3.5/src/kedro_graphql/config.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/decorators.py` & `kedro-graphql-0.3.5/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/events.py` & `kedro-graphql-0.3.5/src/kedro_graphql/events.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import asyncio
 from queue import Queue
 from queue import Empty as QueueEmptyException
 from threading import Thread
 import logging
 from typing import AsyncGenerator
+import time
 from celery.states import READY_STATES, EXCEPTION_STATES
 
 logger = logging.getLogger("kedro-graphql")
 
 class PipelineEventMonitor:
     def __init__(self, app = None, task_id = None, timeout = 1):
         """
@@ -98,8 +100,24 @@
             except QueueEmptyException:
                 if self.app.AsyncResult(self.task_id).status in READY_STATES:
                     break
                 else:
                     continue
 
         event_thread.join(timeout = 0.1)
-          
+          
+    async def start(self, interval = 0.5) -> AsyncGenerator[dict, None]:
+        """
+        A simplified but fully async version of the PipelineEventMonitor().consume() method.
+        
+        The PipelineEventMonitor.consume() method relies on celery's native
+        real time event processing approach which is syncronous and blocking.
+        https://docs.celeryq.dev/en/stable/userguide/monitoring.html#real-time-processing
+        
+        """
+
+        while True:
+            task = self.app.AsyncResult(self.task_id)
+            yield {"task_id": task.id, "status": task.state, "result": task.result, "timestamp": time.time(), "traceback": task.traceback}
+            if self.app.AsyncResult(self.task_id).status in READY_STATES:
+                break
+            await asyncio.sleep(interval)
```

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/example/app.py` & `kedro-graphql-0.3.5/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/logs/json_log_formatter.py` & `kedro-graphql-0.3.5/src/kedro_graphql/logs/json_log_formatter.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/logs/logger.py` & `kedro-graphql-0.3.5/src/kedro_graphql/logs/logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import redis
+import redis.asyncio as redis_asyncio
 import logging
 from logging import LogRecord
 from .json_log_formatter import JSONFormatter ## VerboseJSONFormatter also available
 from celery.signals import task_prerun, task_postrun
 from kedro_graphql.config import config
 from typing import AsyncGenerator
 from celery.result import AsyncResult
@@ -22,20 +23,27 @@
             ## stream will expire in 24 hours (safety mechanism in case task_postrun fails to delete)
             self.connection.expire(self.topic, 86400)
 
     def publish(self, data):
         self.connection.xadd(self.topic, data)
 
 class RedisLogStreamSubscriber(object):
-    def __init__(self, topic, broker_url = config["KEDRO_GRAPHQL_BROKER"]):
-        self.connection = redis.Redis.from_url(broker_url)
-        self.topic = topic   
         
-    def consume(self, count = 1, start_id = 0):
-        r = self.connection.xread(count = count, streams={self.topic:start_id})
+    @classmethod
+    async def create(cls, topic, broker_url = config["KEDRO_GRAPHQL_BROKER"]):
+        """Factory method for async instantiation RedisLogStreamSubscriber objects.
+        """
+        self = RedisLogStreamSubscriber()
+        self.topic = topic
+        self.broker_url = broker_url
+        self.connection = await redis_asyncio.from_url(broker_url)
+        return self
+
+    async def consume(self, count = 1, start_id = 0):
+        r = await self.connection.xread(count = count, streams={self.topic:start_id})
         return r
     
 class KedroGraphQLLogHandler(logging.StreamHandler):
     def __init__(self, topic, broker_url = config["KEDRO_GRAPHQL_BROKER"]):
         logging.StreamHandler.__init__(self)
         self.broker_url = broker_url
         self.topic = topic
@@ -65,26 +73,32 @@
             handler.broker.connection.delete(task_id) ## delete stream
             handler.broker.connection.close()
     logger.handlers = []
 
 
 class PipelineLogStream():
 
-    def __init__(self, task_id = None, broker_url = config["KEDRO_GRAPHQL_BROKER"]):
-        self.broker = RedisLogStreamSubscriber(task_id, broker_url)
+    @classmethod
+    async def create(cls, task_id, broker_url = config["KEDRO_GRAPHQL_BROKER"]):
+        """Factory method for async instantiation PipelineLogStream objects.
+        """
+        self = PipelineLogStream()
         self.task_id = task_id
+        self.broker_url = broker_url
+        self.broker = await RedisLogStreamSubscriber().create(task_id, broker_url)
+        return self
 
     async def consume(self) -> AsyncGenerator[dict, None]:
         start_id = 0
         while True:
-            stream_data = self.broker.consume(count = 1, start_id = start_id)
+            stream_data = await self.broker.consume(count = 1, start_id = start_id)
             if len(stream_data) > 0:
                 for id, value in stream_data[0][1]:
                     yield {"task_id": self.task_id, "message_id": id.decode(), "message": value[b"message"].decode(), "time": value[b"time"].decode()}
                 ## https://redis-py.readthedocs.io/en/stable/examples/redis-stream-example.html#read-more-data-from-the-stream
                 start_id = stream_data[0][1][-1][0]
             else:
                 ## check task status
                 r = AsyncResult(self.task_id)
                 if r.status in READY_STATES:
-                    self.broker.connection.close()
+                    await self.broker.connection.close()
                     break
```

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/models.py` & `kedro-graphql-0.3.5/src/kedro_graphql/models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.3.5/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/schema.py` & `kedro-graphql-0.3.5/src/kedro_graphql/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,33 +55,35 @@
         
         ## PLACE HOLDER for future reolver plugins
         ## testing plugin_resolvers, 
         #RESOLVER_PLUGINS["text_in"].__input__("called text_in resolver")
 
         logger.info(f'Starting {p.name} pipeline with task_id: ' + str(p.task_id))
         p = info.context["request"].app.backend.create(p)
-
         return p
 
 
 @strawberry.type
 class Subscription:
     @strawberry.subscription
-    async def pipeline(self, id: str, info: Info) -> AsyncGenerator[PipelineEvent, None]:
+    async def pipeline(self, id: str, info: Info, interval: float = 0.5) -> AsyncGenerator[PipelineEvent, None]:
+        """Subscribe to pipeline events.
+        """
         p  = info.context["request"].app.backend.load(id=id)
         if p:
-            async for e in PipelineEventMonitor(app = APP_CELERY, task_id = p.task_id).consume():
+            async for e in PipelineEventMonitor(app = APP_CELERY, task_id = p.task_id).start(interval=interval):
                 e["id"] = id
                 yield PipelineEvent(**e)
 
     @strawberry.subscription
     async def pipeline_logs(self, id: str, info: Info) -> AsyncGenerator[PipelineLogMessage, None]:
         p  = info.context["request"].app.backend.load(id=id)
         if p:
-            async for e in PipelineLogStream(task_id = p.task_id ).consume():
+            stream = await PipelineLogStream().create(task_id = p.task_id )
+            async for e in stream.consume():
                 e["id"] = id
                 yield PipelineLogMessage(**e)
 
 
 def build_schema():
     ComboQuery = merge_types("Query", tuple([Query] + TYPE_PLUGINS["query"]))
     ComboMutation = merge_types("Mutation", tuple([Mutation] + TYPE_PLUGINS["mutation"]))
```

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/settings.py` & `kedro-graphql-0.3.5/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql/tasks.py` & `kedro-graphql-0.3.5/src/kedro_graphql/tasks.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.3.5/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.4
+Version: 0.3.5
 Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `kedro-graphql-0.3.4/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.3.5/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/setup.py` & `kedro-graphql-0.3.5/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/conftest.py` & `kedro-graphql-0.3.5/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/test_events.py` & `kedro-graphql-0.3.5/src/tests/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         """
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.before_start")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_success")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_retry")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_failure")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.after_return")
 
-        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id).consume():
+        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id).start():
             print(e)
             assert e["status"] in ALL_STATES
 
     @pytest.mark.asyncio
     async def test_consume_short_timeout(self, mocker, celery_session_app, mock_pipeline):
         """
         Requires Redis to run.
@@ -46,15 +46,15 @@
         """
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.before_start")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_success")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_retry")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_failure")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.after_return")
 
-        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id, timeout = 0.01).consume():
+        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id, timeout = 0.01).start():
             print(e)
             assert e["status"] in ALL_STATES
         
     @pytest.mark.asyncio
     async def test_consume_exception(self, mocker, celery_session_app, mock_pipeline):
         """
         Requires Redis to run.
@@ -64,10 +64,10 @@
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.before_start")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_success")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_retry")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.on_failure")
         mocker.patch("kedro_graphql.tasks.KedroGraphqlTask.after_return")
 
         result = AsyncResult(mock_pipeline.task_id).wait()
-        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id).consume():
+        async for e in PipelineEventMonitor(app = celery_session_app, task_id = mock_pipeline.task_id).start():
             print(e)
             assert e["status"] in ALL_STATES
```

### Comparing `kedro-graphql-0.3.4/src/tests/test_logs.py` & `kedro-graphql-0.3.5/src/tests/test_logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 @pytest.mark.usefixtures('celery_session_worker')
 class TestPipelineLogStream:
     @pytest.mark.asyncio
     async def test_consume(self, mock_pipeline):
         """Requires Redis to run.
         """
         task_id = mock_pipeline.task_id
-        subscriber = PipelineLogStream(task_id = task_id)
+        subscriber = await PipelineLogStream().create(task_id=task_id)
         async for e in subscriber.consume():
             assert set(e.keys()) == set(["task_id", "message_id", "message", "time"])
```

### Comparing `kedro-graphql-0.3.4/src/tests/test_models.py` & `kedro-graphql-0.3.5/src/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/test_run.py` & `kedro-graphql-0.3.5/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/test_schema_mutation.py` & `kedro-graphql-0.3.5/src/tests/test_schema_mutation.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/test_schema_query.py` & `kedro-graphql-0.3.5/src/tests/test_schema_query.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.4/src/tests/test_schema_subscription.py` & `kedro-graphql-0.3.5/src/tests/test_schema_subscription.py`

 * *Files identical despite different names*

