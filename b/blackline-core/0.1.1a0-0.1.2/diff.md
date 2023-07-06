# Comparing `tmp/blackline-core-0.1.1a0.tar.gz` & `tmp/blackline-core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-core-0.1.1a0.tar", last modified: Wed Jun  7 13:00:13 2023, max compression
+gzip compressed data, was "blackline-core-0.1.2.tar", last modified: Thu Jul  6 11:50:10 2023, max compression
```

## Comparing `blackline-core-0.1.1a0.tar` & `blackline-core-0.1.2.tar`

### file list

```diff
@@ -1,99 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sql/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/adapters/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/adapters/sqlite/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/deidentify.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/execution/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/factories/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/models/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/project_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/models/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/models/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.582956 blackline-core-0.1.1a0/blackline/project/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/project/templates/blackline_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/query/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/default_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/doc_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/blackline/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/conftest_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/utils/testing/raw_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/blackline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/blackline_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:13.000000 blackline-core-0.1.1a0/blackline_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-07 13:00:13.590956 blackline-core-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/adapters/test_sqlite_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/conftest_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/execution/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_deifentify.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/execution/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/factories/test_adapter_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/factories/test_query_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/models/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/project/
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/project/test_init_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/query/test_query_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/query/test_template_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:13.586956 blackline-core-0.1.1a0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-07 13:00:03.000000 blackline-core-0.1.1a0/tests/utils/test_doc_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.418367 blackline-core-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 11:50:10.418367 blackline-core-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 11:50:00.000000 blackline-core-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/adapters/sql/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/adapters/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/adapters/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/adapters/sqlite/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/deidentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/execution/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.410367 blackline-core-0.1.2/blackline/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/factories/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/factories/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/datastore_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/project_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/models/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/models/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/project/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/project/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/project/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/project/templates/blackline_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/query/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/query/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/default_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/doc_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/blackline/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/testing/conftest_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/utils/testing/raw_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 11:50:00.000000 blackline-core-0.1.2/blackline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.418367 blackline-core-0.1.2/blackline_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 11:50:10.000000 blackline-core-0.1.2/blackline_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 11:50:10.418367 blackline-core-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:50:00.000000 blackline-core-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/adapters/test_sqlite_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/conftest_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/execution/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/execution/test_deifentify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/execution/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/execution/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/execution/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/factories/test_adapter_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/factories/test_query_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/models/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/models/test_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/models/test_project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/models/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/models/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/project/test_init_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/query/test_template_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:10.414367 blackline-core-0.1.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-06 11:50:00.000000 blackline-core-0.1.2/tests/utils/test_doc_examples.py
```

### Comparing `blackline-core-0.1.1a0/PKG-INFO` & `blackline-core-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-core
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-core-0.1.1a0/blackline/adapters/base.py` & `blackline-core-0.1.2/blackline/adapters/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Optional
 
 from blackline.models.catalogue import Dataset
 from blackline.models.validation import DatasetCollectionValidation
 
-# from blackline.models.adapter import AdapterConfig
-# TODO: Add type hinting for AdapterConfig, it currently causes a circular import.
+# from blackline.models.adapter import DataStoreBase
+# TODO: Add type hinting for DataStoreBase, it currently causes a circular import.
 
 
 class AdapterBase(ABC):
     date_format = "%Y-%m-%d"
 
-    def __init__(self, config) -> None:
-        # def __init__(self, config: AdapterConfig) -> None:
+    def __init__(self, config, condition: Optional[str] = None) -> None:
+        # def __init__(self, config: DataStoreBase) -> None:
         self.config = config
+        self.condition = condition
 
     @abstractmethod
     def connection(self) -> Any:
         """
         Override this method to return a context manager that is
         connection object.
         """
```

### Comparing `blackline-core-0.1.1a0/blackline/adapters/sql/sql.py` & `blackline-core-0.1.2/blackline/adapters/sql/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # from abc import abstractmethod
-from datetime import datetime
+# from datetime import datetime
 from typing import Any, Dict, Optional, Union
 
 from blackline.adapters.base import AdapterBase
 from blackline.constants import (
     CHECK,
     DEFAULT,
     FOREIGN_KEY,
@@ -12,35 +12,35 @@
     UNIQUE,
 )
 from blackline.exceptions import (
     CollectionNotFoundError,
     FieldNotFoundError,
     InvalidFieldConstraintError,
 )
-from blackline.factories.query import QueryFactory
 from blackline.models.catalogue import Dataset, DatasetCollection, DatasetField
 from blackline.models.collection import Column
 from blackline.models.validation import (
     CollectionValidation,
     DatasetCollectionValidation,
     FieldValidation,
 )
-from blackline.query.query import Query
 
 CONSTRINT_MAP: dict[str, dict[str, Union[str, object]]] = {
     NOT_NULL: {"arg": "nullable", "value": False},
     UNIQUE: {"arg": "unique", "value": True},
     PRIMARY_KEY: {"arg": "primary_key", "value": True},
     FOREIGN_KEY: {"arg": "foreign_key", "value": True},
     CHECK: {"arg": "check", "value": not None},
     DEFAULT: {"arg": "default", "value": not None},
 }
 
 
 class SQLAdapter(AdapterBase):
+    dialect: Optional[str] = None
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     # @abstractmethod
     def columns(self, table: str) -> list[Column]:
         pass
 
@@ -64,27 +64,14 @@
 
     def replace_template(self) -> str:
         return "{{ name }} = %({{ value }})s"
 
     def where_template(self) -> str:
         return "WHERE {{ datetime_column }} < %(cutoff)s"
 
-    def deidentify(self, catalogue, start_date: datetime = datetime.now()):
-        for collection in catalogue.collections:
-            queries = QueryFactory(
-                adapter=self,
-                collection=collection,
-                start_date=start_date,
-            ).queries()
-            self.execute_queries(queries=queries)
-
-    def execute_queries(self, queries: list[Query]) -> None:
-        for query in queries:
-            query.execute()
-
     def column_exists(self, table: str, column: str) -> bool:
         """Check if a column exists in a table.
 
         Args:
             table (str): Table name.
             column (str): Column name.
 
@@ -208,10 +195,10 @@
         Returns:
             bool: True if the collection exists.
         """
 
         return DatasetCollectionValidation(
             collections={
                 collection.name: self.validate_collection(collection)
-                for collection in dataset.collections
+                for collection in dataset.collections.values()
             }
         )
```

### Comparing `blackline-core-0.1.1a0/blackline/adapters/sqlite/sqlite.py` & `blackline-core-0.1.2/blackline/adapters/sqlite/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import string
 from sqlite3 import Connection, Cursor, connect
 from typing import Any, Optional, Union
 
 from blackline.adapters.sql.sql import SQLAdapter
 from blackline.models.collection import Column
-from blackline.models.sqlite.sqlite import SQLiteConfig
+from blackline.models.sqlite.sqlite import SQLiteDataStore
 from sqlglot import exp, parse_one
 
 
 class SQLiteAdapter(SQLAdapter):
-    config_model = SQLiteConfig
+    config_model = SQLiteDataStore
+    dialect = "sqlite"
 
-    def __init__(self, config: SQLiteConfig.Config, *args, **kwargs):
+    def __init__(self, config: SQLiteDataStore.Config, *args, **kwargs):
         super().__init__(config=config, *args, **kwargs)
 
     def connection(self) -> Connection:
         return connect(**self.config.connection.dict())
 
     def execute(self, sql: str, values: Optional[dict[str, Any]] = None) -> Any:
         with self.connection() as conn:
```

### Comparing `blackline-core-0.1.1a0/blackline/cli/cli.py` & `blackline-core-0.1.2/blackline/cli/cli.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/constants.py` & `blackline-core-0.1.2/blackline/constants.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/exceptions.py` & `blackline-core-0.1.2/blackline/exceptions.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/execution/debug.py` & `blackline-core-0.1.2/blackline/execution/debug.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/execution/deidentify.py` & `blackline-core-0.1.2/blackline/execution/deidentify.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         for organization in self.catalogue.organizations.values():
             for system in organization.children.values():
                 for resource in system.children.values():
                     for dataset_key, dataset in resource.children.items():
                         store = self.stores.store_by_key(
                             key=dataset_key, profile=self.profile
                         )
-                        store.deidentify(catalogue=dataset, start_date=self.start_date)
+                        store.deidentify(dataset=dataset, start_date=self.start_date)
 
     def validate_catalogue_dataset(self) -> list[DatasetCollectionValidation]:
         dataset_validations = self.validate.validate_catalogue_dataset()
         exceptions = []
         for dataset_validation in dataset_validations.values():
             for collection_validation in dataset_validation.collections.values():
                 if collection_validation.not_found is not None:
```

### Comparing `blackline-core-0.1.1a0/blackline/execution/demo.py` & `blackline-core-0.1.2/blackline/execution/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,16 @@
     """
     return """
     dataset:
       - key: demo_db
         name: Demo Database
         description: Demo database for Blackline
         collections:
-          - name: user
+          user:
+            name: user
             description: User collection
             datetime_field:
               name: created_at
             fields:
               - name: name
                 description: Name of user
                 deidentifier:
@@ -176,15 +177,16 @@
                   value: fake@email.com
                 period: P365D
               - name: ip
                 deidentifier:
                   type: mask
                   value: '#'
                 period: 280 00
-          - name: shipment
+          shipment:
+            name: shipment
             datetime_field:
                 name: order_date
             fields:
               - name: street
                 deidentifier:
                   type: redact
                 period: P185D
```

### Comparing `blackline-core-0.1.1a0/blackline/execution/report.py` & `blackline-core-0.1.2/blackline/execution/report.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/execution/validate.py` & `blackline-core-0.1.2/blackline/execution/validate.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/factories/adapter.py` & `blackline-core-0.1.2/blackline/factories/adapter.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/factories/query.py` & `blackline-core-0.1.2/blackline/factories/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,80 @@
 from datetime import datetime, timedelta
-from typing import Optional
+from typing import Generator, Optional
 
-from blackline.adapters.base import AdapterBase
+import sqlglot
 from blackline.models.catalogue import DatasetCollection, DatasetField
-from blackline.query.query import Query
+from blackline.models.template import TemplateParams
 from blackline.query.template import Template
 
 
 class QueryFactory:
     """Query builder class to build query object."""
 
     def __init__(
         self,
-        adapter: AdapterBase,
         collection: DatasetCollection,
+        template_params: Optional[TemplateParams] = None,
+        dialect: Optional[str] = None,
         start_date: Optional[datetime] = None,
+        date_format: str = "%Y-%m-%d",
+        where_clause: Optional[str] = None,
     ) -> None:
         """
         _summary_
 
         Args:
-            adapter (AdapterBase): _description_
             collection (DatasetCollection): _description_
             start_date (Optional[datetime], optional): _description_. Defaults to None.
+            template_params (Optional[TemplateParams], optional): _description_. Defaults to None.  # noqa: E501
+            date_format (str, optional): _description_. Defaults to "%Y-%m-%d".
+            where_clause (Optional[str], optional): Where clause that will be APPENDED to exisiting WHERE <datetime_field> < :cutoff_date. Defaults to None.
         """
-        self.adapter = adapter
         self.collection = collection
+        self.dialect = dialect
         self.start_date = start_date or datetime.now()
-        self.template = Template(self.adapter, trim_blocks=True, lstrip_blocks=True)
+        self.date_format = date_format
+        self.template = Template(
+            trim_blocks=True,
+            lstrip_blocks=True,
+            params=template_params,
+            where=where_clause,
+        )
 
-    def queries(self) -> list[Query]:
-        """Get queries."""
-        return [
-            self.query_by_period(period=period, fields=fields)
+    def queries(
+        self,
+    ) -> Generator[tuple[str, dict[str, Optional[str]]], None, None]:
+        return (
+            (
+                self.render_sql(fields=fields),
+                self.values_from_fields(fields=fields, period=period),
+            )
             for period, fields in self.fields_by_period().items()
-        ]
-
-    def query_by_period(self, period: timedelta, fields: list[DatasetField]) -> Query:
-        return Query(
-            adapter=self.adapter,
-            sql=self.render_sql(fields=fields),
-            fields=fields,
-            cutoff_date=self.cutoff_date(period=period),
         )
 
     def render_sql(self, fields: list[DatasetField]) -> str:
-        return self.template.template.render(
+        sql = self.template.template.render(
             table=self.collection.name,
             columns=fields,
             datetime_column=self.collection.datetime_field.name,
         )
+        if self.dialect is not None:
+            sqlglot.transpile(sql=sql, read=self.dialect)
+        return sql
+
+    def values_from_fields(
+        self, fields: list[DatasetField], period: timedelta
+    ) -> dict[str, Optional[str]]:
+        values: dict[str, Optional[str]] = {
+            f"{field.name}_value": field.deidentifier.value
+            for field in fields
+            if field.deidentifier is not None
+        }
+        values["cutoff"] = self.cutoff_date(period=period).strftime(self.date_format)
+        return values
 
     def cutoff_date(self, period: timedelta) -> datetime:
         """Get cutoff date."""
         return self.start_date - period
 
     def fields_by_period(self) -> dict[timedelta, list[DatasetField]]:
         """Get columns by retention period."""
```

### Comparing `blackline-core-0.1.1a0/blackline/models/catalogue.py` & `blackline-core-0.1.2/blackline/models/catalogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # from blackline.constants import CHECK, NOT_NULL
 from blackline.models.validation import (
     Key,
     check_valid_country_code,
     no_self_reference,
     sort_list_objects_by_name,
 )
-from pydantic import AnyUrl, BaseModel, Field, HttpUrl, validator
+from pydantic import AnyUrl, BaseModel, Field, HttpUrl, root_validator, validator
 
 country_code_validator = validator("third_country_transfers", allow_reuse=True)(
     check_valid_country_code
 )
 
 
 name_field = Field(description="Human-Readable name for this resource.")
@@ -139,25 +139,20 @@
 class BlacklineModel(BaseModel):
     """The base model for all Resources."""
 
     key: Key = Field(description="A unique key used to identify this resource.")
     tags: Optional[list[str]] = Field(description="A list of tags for this resource.")
     name: Optional[str] = name_field
     description: Optional[str] = description_field
-
     children: Optional[dict[str, Type[BlacklineModel]]] = Field(
         None, description="The children resources."
     )
     stem: ClassVar[str] = Field(description="The stem of the resource.")
-    children_stem: ClassVar[Optional[str]] = Field(
-        description="The stem of the children resources."
-    )
-    children_cls: ClassVar[Optional[type[BlacklineModel]]] = Field(
-        description="The children class."
-    )
+    children_stem: ClassVar[Optional[str]] = None
+    children_cls: ClassVar[Optional[type[BlacklineModel]]] = None
 
     class Config:
         "Config for the BlacklineModel"
         extra = "forbid"
         orm_mode = True
 
     def __getitem__(self, key: str) -> Type[BlacklineModel]:
@@ -185,14 +180,39 @@
         """
         key = ".".join([key_prefix, path.name]) if key_prefix is not None else path.name
         children = cls.parse_children(path=path, key_prefix=key)
         filepath = cls.find_definition_file(path=path)
         return cls.parse_yaml(path=filepath, key=key, children=children)
 
     @classmethod
+    def parse_children(
+        cls, path: Path, key_prefix: Optional[str] = None
+    ) -> dict[str, Type[BlacklineModel]]:
+        """
+        Parse a directory of YAML files into a dictionary of Dataset objects.
+
+        Args:
+            path: The path to the directory of YAML files.
+            path: Path
+
+        Returns:
+            A dictionary of Dataset objects.
+        """
+        children: dict[str, Type[BlacklineModel]] = {}
+        if cls.children_cls is None:
+            return children
+        for child_path in path.iterdir():
+            if child_path.is_dir():
+                child = cls.children_cls.parse_dir(
+                    path=child_path, key_prefix=key_prefix
+                )
+                children[child.key] = child
+        return children
+
+    @classmethod
     def find_definition_file(cls, path: Path) -> Path:
         file = list(path.glob(f"{cls.stem}.yml")) + list(path.glob(f"{cls.stem}.yaml"))
         file_len = len(list(file))
         if file_len == 0:
             raise FileNotFoundError(
                 f"No {cls.stem} file found in directory: {path.absolute()}"
             )
@@ -218,43 +238,19 @@
 
         Returns:
             Dataset object.
         """
         with open(path, "r") as f:
             info = yaml.safe_load(f)[cls.stem][0]
             info["key"] = key
-            if cls.children_stem is not None:
-                info[cls.children_stem] = children
+            if cls.stem == "dataset":
+                return cls.parse_obj(info)
+            info[cls.children_stem] = children
             return cls.parse_obj(info)
 
-    @classmethod
-    def parse_children(
-        cls, path: Path, key_prefix: Optional[str] = None
-    ) -> dict[str, Type[BlacklineModel]]:
-        """
-        Parse a directory of YAML files into a dictionary of Dataset objects.
-
-        Args:
-            path: The path to the directory of YAML files.
-            path: Path
-
-        Returns:
-            A dictionary of Dataset objects.
-        """
-        children: dict[str, Type[BlacklineModel]] = {}
-        if cls.children_cls is None:
-            return children
-        for child_path in path.iterdir():
-            if child_path.is_dir():
-                child = cls.children_cls.parse_dir(
-                    path=child_path, key_prefix=key_prefix
-                )
-                children[child.key] = child
-        return children
-
 
 class ContactDetails(BaseModel):
     """
     The contact details information model.
 
     Used to capture contact information for controllers, used
     as part of exporting a data map / ROPA.
@@ -387,42 +383,50 @@
     )
 
 
 class DatetimeField(BaseModel):
     name: str = Field(description="The name of the field to use datetime information.")
 
 
-class DatasetCollection(BaseModel):
+class DatasetCollection(BlacklineModel):
     """
     The DatasetCollection resource model.
 
     This resource is nested witin a Dataset.
     """
 
-    name: str = name_field
-    description: Optional[str] = description_field
+    name: str = Field(..., description="The name of the collection.")
+
+    datetime_field: DatetimeField = Field(
+        description="The datetime field to use for the retention limit calculations."
+    )
+    where: Optional[str] = Field(
+        None,
+        description="An addional where clause to append to the exeisting: 'WHERE {{ datetime_column }} < %(cutoff)s'.",  # noqa: E501
+    )
+    fields: list[DatasetField] = Field(
+        description="An array of objects that describe the collection's fields.",
+    )
+
     data_categories: Optional[list[Key]] = Field(
         description="Array of Data Category resources identified by `key`, that apply to all fields in the collection.",
     )
     data_qualifier: Key = Field(
         default=Key(
             "aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified"
         ),
         description="Array of Data Qualifier resources identified by `key`, that apply to all fields in the collection.",
     )
-    fields: list[DatasetField] = Field(
-        description="An array of objects that describe the collection's fields.",
-    )
-    datetime_field: DatetimeField = Field(
-        description="The datetime field to use for the retention limit calculations."
-    )
 
     _sort_fields: classmethod = validator("fields", allow_reuse=True)(
         sort_list_objects_by_name
     )
+    dependencies: Optional[list[str]] = Field(
+        None, description="The collection dependencies."
+    )
 
 
 class DeidentifierBase(BaseModel):
     description: Optional[str] = None
     valid_constraints: ClassVar[list] = []
     invalid_constraints: ClassVar[list] = []
 
@@ -485,25 +489,30 @@
     )
     joint_controller: Optional[ContactDetails] = Field(
         description=ContactDetails.__doc__,
     )
     third_country_transfers: Optional[list[str]] = Field(
         description="An optional array to identify any third countries where data is transited to. For consistency purposes, these fields are required to follow the Alpha-3 code set in [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3).",
     )
-    collections: list[DatasetCollection] = Field(
-        description="An array of objects that describe the Dataset's collections.",
-    )
-    _sort_collections: classmethod = validator("collections", allow_reuse=True)(
-        sort_list_objects_by_name
-    )
     _check_valid_country_code: classmethod = country_code_validator
-
+    _alias = "collections"
+    children: dict[str, DatasetCollection] = Field(description=f"Collection dict. Alaised to {_alias}", alias=_alias)  # type: ignore[assignment]
     stem = "dataset"
-    children_stem = None
-    children_cls = None
+    children_stem = "collections"
+    children_cls = DatasetCollection
+
+    @root_validator(pre=True)
+    def add_key_to_collection(cls, values):
+        for key, collection in values["collections"].items():
+            collection["key"] = values["key"] + "." + key
+        return values
+
+    @property
+    def collections(self) -> dict[str, DatasetCollection]:
+        return self.children
 
 
 class Resource(BlacklineModel):
     """
     The System resource model.
 
     Describes an application and includes a list of PrivacyDeclaration resources.
```

### Comparing `blackline-core-0.1.1a0/blackline/models/collection.py` & `blackline-core-0.1.2/blackline/models/collection.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/models/datastores.py` & `blackline-core-0.1.2/blackline/models/datastores.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import re
 from importlib import import_module
 from pathlib import Path
 from typing import Annotated, Any, Optional, Type, Union
 
 import yaml
-from blackline.models.adapter import AdapterConfig
-from blackline.models.sqlite.sqlite import SQLiteConfig
+from blackline.models.datastore_base import DataStoreBase
+from blackline.models.sqlite.sqlite import SQLiteDataStore
 from pydantic import BaseModel, BaseSettings, Field, create_model, root_validator
 
 
 def load_adapter_configs_from_submodules(name: str) -> set:
     mod = import_module(name)
     model_modules = inspect.getmembers(
         mod,
@@ -19,59 +19,77 @@
     )
 
     configs = {
         member[1]
         for member in inspect.getmembers(
             mod,
             lambda member: inspect.isclass(member)
-            and issubclass(member, AdapterConfig)
-            and member != AdapterConfig,
+            and issubclass(member, DataStoreBase)
+            and member != DataStoreBase,
         )
     }
 
     for module in model_modules:
         configs.update(load_adapter_configs_from_submodules(module[1].__name__))
 
     return configs
 
 
 def assign_store(
     adapter_configs: set,
-) -> Union[Type[AdapterConfig], Type[object]]:
+) -> Union[Type[DataStoreBase], Type[object]]:
     if len(adapter_configs) == 1:
-        return SQLiteConfig
+        return SQLiteDataStore
     return Annotated[
         Union[tuple(adapter_configs)],  # type: ignore
         Field(discriminator="type"),
     ]
 
 
 adapter_configs = load_adapter_configs_from_submodules(name="blackline.models")
-Adapter: Any = assign_store(adapter_configs=adapter_configs)
+Store: Any = assign_store(adapter_configs=adapter_configs)
 
 
 def config_files(folderpath: Path) -> list[Path]:
     return list(folderpath.glob("**/*.yml")) + list(folderpath.glob("**/*.yaml"))
 
 
 class DataStore(BaseSettings):
     """
     A data model representing a data store, with profiles for connecting to different adapters. # noqa: E501
     """
 
-    profiles: dict[str, Adapter]
+    profiles: dict[str, Store]
     name: str
     key: str
     env_prefix: str = ""
 
     class Config:
         extra = "allow"
         env_prefix = ""
         env_nested_delimiter = "__"
 
+    def __getitem__(self, key: str) -> DataStoreBase:
+        """
+        Retrieves an adapter profile by name.
+
+        Args:
+            key (str): The name of the adapter profile to retrieve.
+
+        Raises:
+            ValueError: If the specified adapter profile is not found.
+
+        Returns:
+            (DataStoreBase): The adapter profile matching the specified key.
+        """
+        try:
+            return self.profiles[key]
+        except KeyError:
+            raise ValueError(f"Profile {key} not found")
+
     @root_validator(pre=True)
     def validate_store(cls, values):
         values["key"] = cls.build_key(values)
         return values
 
     def build_key(values):
         organization_name = values.get("organization_name", "")
@@ -84,14 +102,33 @@
 class DataStores(BaseModel):
     """
     A data model representing a collection of data stores.
     """
 
     stores: list[DataStore] = Field(..., description="A list of DataStore objects.")
 
+    def __getitem__(self, key: str) -> DataStore:
+        """
+        Retrieves a data store by key.
+
+        Args:
+            key (str): The key or name of the data store to retrieve.
+
+        Raises:
+            ValueError: If the specified data store is not found.
+
+        Returns:
+            (DataStore): The data store matching the specified key.
+        """
+
+        for store in self.stores:
+            if store.name == key or store.key == key:
+                return store
+        raise ValueError(f"Store {key} not found")
+
     def store(self, name: str, profile: Optional[str] = None):
         """
         Retrieves a data store by name and returns its adapter profiles or a specific profile. # noqa: E501
 
         Args:
             name (str): The name of the data store to retrieve.
             profile (Optional[str], optional): The name of the adapter profile to retrieve. If None, returns all profiles. Defaults to None.  # noqa: E501
@@ -105,27 +142,27 @@
         for store in self.stores:
             if store.name == name:
                 if profile:
                     return store.profiles[profile]
                 return store.profiles
         raise ValueError(f"Store {name} not found")
 
-    def store_by_key(self, key: str, profile: str) -> AdapterConfig:
+    def store_by_key(self, key: str, profile: str) -> DataStoreBase:
         """
         Retrieves a data store by key and returns the specified adapter profile.
 
         Args:
             key (str): The unique key of the data store to retrieve.
             profile (str): The name of the adapter profile to retrieve.
 
         Raises:
             ValueError: If the specified data store is not found.
 
         Returns:
-            AdapterConfig: The adapter configuration for the specified data store and profile. # noqa: E501
+            DataStoreBase: The adapter configuration for the specified data store and profile. # noqa: E501
         """
         for store in self.stores:
             if store.key == key:
                 return store.profiles[profile]
         raise ValueError(f"Store {key} not found")
 
     @classmethod
```

### Comparing `blackline-core-0.1.1a0/blackline/models/project_config.py` & `blackline-core-0.1.2/blackline/models/project_config.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/models/sqlite/sqlite.py` & `blackline-core-0.1.2/blackline/models/sqlite/sqlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from sqlite3 import Connection
 from typing import Any, Literal
 
-from blackline.models.adapter import AdapterConfig, ConnectionConfig
 from blackline.models.collection import Column as SQLColumn
+from blackline.models.datastore_base import ConnectionConfig, DataStoreBase
 from pydantic import BaseModel, Field
 
 
 class SQLiteConnectionConfig(ConnectionConfig):
     """
     A data model representing a connection configuration for a SQLite database.
     """
@@ -42,30 +42,30 @@
         default=False, description="Whether to use a URI-style connection string."
     )
 
     class Config:
         env_prefix = ""
 
 
-class SQLiteConfig(AdapterConfig):
+class SQLiteDataStore(DataStoreBase):
     """
     A data model representing the configuration for the SQLite adapter.
 
     Args:
         Config (BaseModel): A nested BaseModel class representing the SQLite connection configuration.  # noqa: E501
 
     Returns:
-        SQLiteConfig: An instance of the SQLiteConfig class.
+        SQLiteDataStore: An instance of the SQLiteDataStore class.
 
     """
 
-    class _Config(BaseModel):
+    class Config(BaseModel):
         connection: SQLiteConnectionConfig = Field(
             ..., description="The connection configuration for the adapter."
         )
 
     type: Literal["sqlite"] = Field(..., description="The type of adapter.")
-    config: _Config = Field(..., description="The configuration for the adapter.")
+    config: Config = Field(..., description="The configuration for the adapter.")
 
 
 class Column(SQLColumn):
     ...
```

### Comparing `blackline-core-0.1.1a0/blackline/models/validation.py` & `blackline-core-0.1.2/blackline/models/validation.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/project/init.py` & `blackline-core-0.1.2/blackline/project/init.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/query/template.py` & `blackline-core-0.1.2/blackline/query/template.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import logging
+from typing import Optional
 
-from blackline.adapters.base import AdapterBase
+from blackline.models.template import TemplateParams
 from blackline.query.templates import deidentifier_marco_base, layout, query
 from jinja2 import Environment
 from jinja2 import Template as JinjaTemplate
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
 class Template(object):
     def __init__(
         self,
-        adapter: AdapterBase,
+        params: TemplateParams,
         trim_blocks=True,
         lstrip_blocks=True,
+        where: Optional[str] = None,
         *args,
         **kwrgs,
     ) -> None:
-        self.adapter = adapter
+        if where is not None:
+            params.where_template += " " + where
+        self.params = params
+        self.where = where
         self.env = Environment(
             *args, trim_blocks=trim_blocks, lstrip_blocks=lstrip_blocks, **kwrgs
         )
         self.layout = self.env.from_string(layout)
         self.deidentifier_marco_base = self.env.from_string(deidentifier_marco_base)
         self._load_marcos()
 
@@ -37,15 +42,15 @@
                 "replace": self.replace_macro(),
                 "mask": self.mask_macro(),
             }
         )
 
     def _deidentifer_macro(self, name, method) -> str:
         sql_str = self.deidentifier_marco_base.module.deidentifier_marco_base(
-            macro_name=name, assignment=getattr(self.adapter, method)()
+            macro_name=name, assignment=getattr(self.params, method)
         )
         logger.debug(f"{name} macro: \n{sql_str}")
 
         return getattr(self.env.from_string(sql_str).module, name.lower())
 
     def redact_macro(self) -> str:
         return self._deidentifer_macro(name="Redact", method="redact_template")
@@ -53,19 +58,20 @@
     def replace_macro(self) -> str:
         return self._deidentifer_macro(name="Replace", method="replace_template")
 
     def mask_macro(self) -> str:
         return self._deidentifer_macro(name="Mask", method="mask_template")
 
     def template_str(self) -> str:
-        template = self.env.from_string(query).render(
+        # if self.where is not None:
+        #     self.params.where_template += " " + self.where
+
+        return self.env.from_string(query).render(
             layout=self.layout,
-            update_statement=self.adapter.update_template(),
-            set_statement=self.adapter.set_template(),
-            where_statement=self.adapter.where_template(),
+            update_statement=self.params.update_template,
+            set_statement=self.params.set_template,
+            where_statement=self.params.where_template,
         )
-        logger.debug(f"render_template:\n{template}")
-        return template
 
     def render_template(self, *args, **kwargs) -> str:
         template = self.template()
         return self.env.from_string(template).render(*args, **kwargs)
```

### Comparing `blackline-core-0.1.1a0/blackline/query/templates.py` & `blackline-core-0.1.2/blackline/query/templates.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/utils/default_fixtures.py` & `blackline-core-0.1.2/blackline/utils/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/blackline/utils/doc_examples.py` & `blackline-core-0.1.2/blackline/utils/doc_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
   description: <system description> [optional]
 
 """
 
 
 RESOURCE = """
 resource:
-  key: foo_key
+  key: resource_key
   tags:
   - foo
   - bar
   name: <resource name>
   description: <resource description>
   resource_type: Service
   data_responsibility_title: Processor
@@ -69,15 +69,15 @@
     is_required: true
     status: Complete
     link: https://example.org/analytics_system_data_protection_impact_assessment
 """
 
 DATASET = """
 dataset:
-  key: foo_key
+  key: dataset_key
   tags:
   - foo
   - bar
   name: user
   description: <resource description>
   meta:
     last_updated: '2021-01-01'
@@ -90,39 +90,40 @@
     address: Museumplein 10, 1071 DJ Amsterdam, Netherlands
     email: dave@organization.com
     phone: 020 573 2911
   third_country_transfers:
   - USA
   - CAN
   collections:
-  - name: user
-    description: user data
-    data_categories:
-    - user.contact
-    data_qualifier: identified
-    fields:
-    - name: email
-      description: user email
-      data_categories:
-      - user.contact.email
-      data_qualifier: identified
-      deidentifier:
-        type: replace
-        value: fake@email.com
-      period: P365D
-    - name: name
-      description: user name
+    user:
+      name: user
+      description: user data
       data_categories:
-      - user.name
+      - user.contact
       data_qualifier: identified
-      deidentifier:
-        type: redact
-      period: P365D
-    datetime_field:
-      name: created_at
+      fields:
+      - name: email
+        description: user email
+        data_categories:
+        - user.contact.email
+        data_qualifier: identified
+        deidentifier:
+          type: replace
+          value: fake@email.com
+        period: P365D
+      - name: name
+        description: user name
+        data_categories:
+        - user.name
+        data_qualifier: identified
+        deidentifier:
+          type: redact
+        period: P365D
+      datetime_field:
+        name: created_at
 """
 
 SQLITE = """
 profiles:
   dev:
     type: sqlite
     config:
```

### Comparing `blackline-core-0.1.1a0/blackline/utils/testing/conftest_shared.py` & `blackline-core-0.1.2/blackline/utils/testing/conftest_shared.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import datetime
 from pathlib import Path
 from typing import Callable
 
 import pytest
-from blackline.adapters.base import AdapterBase
 from blackline.constants import PROJECT_CONFIG_FILE
 from blackline.factories.query import QueryFactory
 from blackline.models.catalogue import Catalogue
 from blackline.models.project_config import ProjectConfig
+from blackline.models.template import TemplateParams
 from blackline.utils.testing.raw_yaml import (
     dataset_yaml,
     organization_yaml,
     project_yaml,
     resource_yaml,
     sqlite_adapter_yaml,
     system_yaml,
@@ -28,15 +28,15 @@
 @pytest.fixture
 def fake_project_name() -> str:
     return "fake-project"
 
 
 @pytest.fixture
 def test_table() -> str:
-    return "test_table"
+    return "user"
 
 
 @pytest.fixture
 def profile() -> str:
     return "dev"
 
 
@@ -52,87 +52,52 @@
 
 @pytest.fixture
 def start_date() -> datetime:
     return datetime(2023, 1, 1)
 
 
 @pytest.fixture
-def mock_data() -> list:
+def mock_user_data() -> list:
+    # fmt: off
     return [
-        (
-            datetime(2021, 1, 1),
-            "Dave",
-            "dave@example.com",
-            "12345",
-            True,
-            "127.0.0.1",
-        ),
-        (
-            datetime(2021, 6, 1),
-            "Alison",
-            "alison@example.com",
-            "23456",
-            True,
-            "127.0.0.2",
-        ),
-        (
-            datetime(2022, 3, 1),
-            "Chris",
-            "chris@example.com",
-            "34567",
-            False,
-            "127.0.0.3",
-        ),
-        (
-            datetime(2022, 4, 1),
-            "Megan",
-            "megan@example.com",
-            "45678",
-            True,
-            "127.0.0.4",
-        ),
+        (datetime(2021, 1, 1), "Dave", "dave@example.com", "12345", True, "127.0.0.1", None),  # noqa: E501
+        (datetime(2021, 6, 1), "Alison", "alison@example.com", "23456", True, "127.0.0.2", None),  # noqa: E501
+        (datetime(2022, 3, 1), "Chris", "chris@example.com", "34567", False, "127.0.0.3", None),  # noqa: E501
+        (datetime(2022, 4, 1), "Megan", "megan@example.com", "45678", True, "127.0.0.4", None),  # noqa: E501
+        (datetime(2022, 12, 31), "Roy", "Roy@example.com", "45638", True, "127.0.0.5", datetime(2023, 1, 1)),  # noqa: E501
     ]
+    # fmt: on
 
 
 @pytest.fixture
-def deidentified_mock_data() -> list:
+def deidentified_mock_user_data() -> list:
+    # fmt: off
     return [
-        (
-            datetime(2022, 4, 1, 0, 0),
-            "Megan",
-            "megan@example.com",
-            "45678",
-            True,
-            "127.0.0.4",
-        ),
-        (
-            datetime(2022, 3, 1, 0, 0),
-            "Chris",
-            "chris@example.com",
-            "34567",
-            False,
-            "###.#.#.#",
-        ),
-        (
-            datetime(2021, 1, 1, 0, 0),
-            None,
-            "fake@email.com",
-            "12345",
-            True,
-            "###.#.#.#",
-        ),
-        (
-            datetime(2021, 6, 1, 0, 0),
-            None,
-            "fake@email.com",
-            "23456",
-            True,
-            "###.#.#.#",
-        ),
+        (datetime(2022, 4, 1, 0, 0), "Megan", "megan@example.com", "45678", 1, "127.0.0.4", None),  # noqa: E501
+        (datetime(2022, 3, 1, 0, 0), "Chris", "chris@example.com", "34567", 0, "###.#.#.#", None),  # noqa: E501
+        (datetime(2021, 1, 1, 0, 0), None, "fake@email.com", "12345", 1, "###.#.#.#", None),  # noqa: E501
+        (datetime(2021, 6, 1, 0, 0), None, "fake@email.com", "23456", 1, "###.#.#.#", None),  # noqa: E501
+        (datetime(2022, 12, 31, 0, 0), None, "fake@email.com", "45638", 1, "###.#.#.#", datetime(2023, 1, 1)),  # noqa: E501
     ]
+    # fmt: on
+
+
+@pytest.fixture
+def mock_session_data() -> list:
+    # fmt: off
+    return [
+        (datetime(2021, 1, 2), datetime(2021, 1, 3), "dave@example.com", "127.0.0.11", "344DE1ED-B9FB-4B17-960C-F096EA1C05C4"),  # noqa: E501
+        (datetime(2021, 1, 3), datetime(2021, 1, 4), "dave@example.com", "127.0.0.11", "BA0F580D-7EE8-4AAA-B105-394A9AFF85FC"),  # noqa: E501
+        (datetime(2021, 1, 4), datetime(2021, 1, 5), "dave@example.com", "127.0.0.11", "1F3FDE90-5132-4DCE-A6C3-C630395673B4"),  # noqa: E501
+        (datetime(2021, 6, 2), datetime(2021, 6, 3), "alison@example.com", "127.0.0.22", "1DC4FB44-F563-43C3-901F-C968D3896162"),  # noqa: E501
+        (datetime(2022, 3, 2), datetime(2022, 3, 3), "chris@example.com", "127.0.0.33", "2EE29388-A9F0-49E3-AE67-798ABB3584CB"),  # noqa: E501
+        (datetime(2022, 4, 2), datetime(2022, 4, 3), "megan@example.com", "127.0.0.44", "4C747E07-CE33-46FC-940B-7B8AFB4EFCFA"),  # noqa: E501
+        (datetime(2022, 4, 5), datetime(2022, 4, 6), "megan@example.com", "127.0.0.44", "1D268CF9-53B7-4D5E-9333-3DD97341AA28"),  # noqa: E501
+    ]
+    # fmt: on
 
 
 @pytest.fixture()
 def sample_project(
     test_table: str,
     project_config_file: Path,
     create_project_config: None,
@@ -160,26 +125,30 @@
 @pytest.fixture
 def query_factory_factory(
     catalogue: Catalogue,
     test_table: str,
     start_date: datetime,
     store_name: str,
 ) -> Callable:
-    def _query_factory_factory(adapter: AdapterBase) -> QueryFactory:
+    def _query_factory_factory(template_params: TemplateParams) -> QueryFactory:
         store_catalogue = catalogue[
             "organization_foo.system_foo.resource_foo.dataset_foo"
         ]
 
         collection = [
             collection
-            for collection in store_catalogue.collections
+            for collection in store_catalogue.collections.values()
             if collection.name == test_table
         ][0]
+
         return QueryFactory(
-            adapter=adapter, collection=collection, start_date=start_date
+            template_params=template_params,
+            collection=collection,
+            start_date=start_date,
+            where_clause=collection.where,
         )
 
     return _query_factory_factory
 
 
 @pytest.fixture
 def catalogue_dir(tmp_path: Path) -> Path:
```

### Comparing `blackline-core-0.1.1a0/blackline/utils/testing/raw_yaml.py` & `blackline-core-0.1.2/blackline/utils/testing/raw_yaml.py`

 * *Files 21% similar despite different names*

```diff
@@ -93,34 +93,35 @@
               - yet_another_demo_system
       """
 
 
 def dataset_yaml(table: str) -> str:
     return f"""
     dataset:
-      - key: demo_users_dataset
-        name: Demo Users Dataset
+      - name: Demo Users Dataset
         description: Data collected about users for our analytics system.
         third_country_transfers:
-        - USA
-        - CAN
+          - USA
+          - CAN
         joint_controller:
           name: Dave L. Epper
           address: 1 Acme Pl. New York, NY
           email: controller@acmeinc.com
           phone: +1 555 555 5555
           retention: 1 year post account deletion
         collections:
-          - name: {table}
+          {table}:
+            name: {table}
             description: User information
             data_categories:
               - user
-            retention: 30 days post account deletion
             datetime_field:
                 name: created_at
+            where:
+              OR deactivation_date IS NOT NULL
             fields:
               - name: name
                 description: User's first name
                 data_categories:
                   - user.name
                 deidentifier:
                   type: redact
@@ -137,8 +138,33 @@
                 description: User's IP address
                 data_categories:
                   - user.device.ip_address
                 deidentifier:
                   type: mask
                   value: "#"
                 period: "280 00" # [-][DD ][HH:MM]SS[.ffffff]
+          session:
+            name: session
+            description: User sessions
+            data_categories:
+              - user.device.ip_address
+            datetime_field:
+              name: session_started_at
+            dependencies:
+              - {table}
+            fields:
+              - name: ip
+                description: User's IP address
+                data_categories:
+                  - user.device.ip_address
+                deidentifier:
+                  type: mask
+                  value: "#"
+                period: "183 00"
+              - name: cookie_id
+                description: User's cookie ID
+                data_categories:
+                  - user.device.cookie_id
+                deidentifier:
+                  type: redact
+                period: "183 00"
     """
```

### Comparing `blackline-core-0.1.1a0/blackline_core.egg-info/PKG-INFO` & `blackline-core-0.1.2/blackline_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-core
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-core-0.1.1a0/blackline_core.egg-info/SOURCES.txt` & `blackline-core-0.1.2/blackline_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,34 @@
 ./blackline/execution/deidentify.py
 ./blackline/execution/demo.py
 ./blackline/execution/report.py
 ./blackline/execution/validate.py
 ./blackline/factories/__init__.py
 ./blackline/factories/adapter.py
 ./blackline/factories/query.py
-./blackline/models/adapter.py
 ./blackline/models/catalogue.py
 ./blackline/models/collection.py
+./blackline/models/datastore_base.py
 ./blackline/models/datastores.py
 ./blackline/models/project_config.py
+./blackline/models/template.py
 ./blackline/models/validation.py
 ./blackline/models/sqlite/__init__.py
 ./blackline/models/sqlite/sqlite.py
 ./blackline/project/__init__.py
 ./blackline/project/init.py
 ./blackline/project/templates/__init__.py
 ./blackline/project/templates/blackline_project.yml
 ./blackline/query/__init__.py
-./blackline/query/query.py
 ./blackline/query/template.py
 ./blackline/query/templates.py
 ./blackline/utils/__init__.py
 ./blackline/utils/default_fixtures.py
 ./blackline/utils/doc_examples.py
 ./blackline/utils/testing/__init__.py
-./blackline/utils/testing/catalogue.py
 ./blackline/utils/testing/conftest_shared.py
 ./blackline/utils/testing/raw_yaml.py
 ./tests/conftest.py
 ./tests/conftest_sqlite.py
 ./tests/adapters/test_sqlite_adapter.py
 ./tests/cli/test_cli.py
 ./tests/execution/test_debug.py
@@ -58,15 +57,14 @@
 ./tests/factories/test_query_factory.py
 ./tests/models/test_catalogue.py
 ./tests/models/test_datastores.py
 ./tests/models/test_project_config.py
 ./tests/models/test_sqlite.py
 ./tests/models/test_validation.py
 ./tests/project/test_init_project.py
-./tests/query/test_query_query.py
 ./tests/query/test_template_query.py
 ./tests/utils/test_doc_examples.py
 blackline_core.egg-info/PKG-INFO
 blackline_core.egg-info/SOURCES.txt
 blackline_core.egg-info/dependency_links.txt
 blackline_core.egg-info/entry_points.txt
 blackline_core.egg-info/requires.txt
```

### Comparing `blackline-core-0.1.1a0/setup.cfg` & `blackline-core-0.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blackline-core
-version = 0.1.1a0
+version = 0.1.2
 url = https://github.com/blacklinedata/blackline-core
 description = Manage personal data in your data stores.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
```

### Comparing `blackline-core-0.1.1a0/tests/adapters/test_sqlite_adapter.py` & `blackline-core-0.1.2/tests/adapters/test_sqlite_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,34 +35,36 @@
 
 
 def test_test_connection(sqlite_adapter: SQLiteAdapter) -> None:
     # Run & Assert
     assert sqlite_adapter.test_connection()
 
 
-def test_execute(sqlite_adapter: SQLiteAdapter, mock_data: List) -> None:
+def test_execute(
+    sqlite_adapter: SQLiteAdapter, mock_user_data: List, test_table: str
+) -> None:
     # Run
-    res = sqlite_adapter.execute(sql="SELECT * FROM test_table")
+    res = sqlite_adapter.execute(sql=f"SELECT * FROM {test_table}")
     data = res.fetchall()
 
     # Assert
-    assert len(data) == len(mock_data)
+    assert len(data) == len(mock_user_data)
 
 
-def test_table_exists(sqlite_adapter: SQLiteAdapter) -> None:
+def test_table_exists(sqlite_adapter: SQLiteAdapter, test_table: str) -> None:
     # Run
-    res = sqlite_adapter.table_exists(table="test_table")
+    res = sqlite_adapter.table_exists(table=test_table)
 
     # Assert
     assert res
 
 
-def test_columns_exist(sqlite_adapter: SQLiteAdapter) -> None:
+def test_columns_exist(sqlite_adapter: SQLiteAdapter, test_table: str) -> None:
     # Run
-    res = sqlite_adapter.columns_exist(table="test_table", columns=["id", "name"])
+    res = sqlite_adapter.columns_exist(table=test_table, columns=["id", "name"])
 
     # Assert
     assert not res["id"]  # id is not in the test_table
     assert res["name"]
 
 
 def test_invalid_column_constraints_with_valid_constraints(
@@ -162,14 +164,15 @@
             name="name",
             deidentifier=Mask(type="mask", value="#"),
             period=timedelta(days=30),
         ),
     ]
 
     collection = DatasetCollection(
+        key=table,
         name=table,
         fields=fields,
         datetime_field=DatetimeField(name="created_at"),
     )
 
     # Run
     result = sqlite_adapter.validate_collection(collection=collection)
@@ -197,15 +200,18 @@
             name="nonexistent_field",
             deidentifier=Mask(type="mask", value="#"),
             period=timedelta(days=30),
         ),
     ]
 
     collection = DatasetCollection(
-        name=table, fields=fields, datetime_field=DatetimeField(name="created_at")
+        key=table,
+        name=table,
+        fields=fields,
+        datetime_field=DatetimeField(name="created_at"),
     )
 
     # Run
     result = sqlite_adapter.validate_collection(collection=collection)
 
     # Assert
     assert isinstance(result.fields["nonexistent_field"].not_found, FieldNotFoundError)
@@ -228,15 +234,18 @@
             name="name",
             deidentifier=Mask(type="mask", value="#"),
             period=timedelta(days=30),
         ),
     ]
 
     collection = DatasetCollection(
-        name=table, fields=fields, datetime_field=DatetimeField(name="created_at")
+        key=table,
+        name=table,
+        fields=fields,
+        datetime_field=DatetimeField(name="created_at"),
     )
 
     # Run
     result = sqlite_adapter.validate_collection(collection=collection)
 
     # Assert
     assert isinstance(
```

### Comparing `blackline-core-0.1.1a0/tests/cli/test_cli.py` & `blackline-core-0.1.2/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/conftest.py` & `blackline-core-0.1.2/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
 @pytest.fixture
 def store(
     stores: DataStores,
     profile: str,
     store_name: str,
 ) -> DataStore:
-    return stores.store(name=store_name, profile=profile)
+    return stores[store_name][profile]
 
 
 @pytest.fixture
 def query_factory(
     query_factory_factory: Callable,
     store: DataStore,
     mock_sqlite_store: Connection,
 ) -> QueryFactory:
-    return query_factory_factory(adapter=store.adapter)
+    return query_factory_factory(template_params=store.template_params)
 
 
 @pytest.fixture
 def deidentify(
     project_root: Path, sample_project: Callable, profile: str, start_date: datetime
 ) -> None:
     return Deidentify(path=project_root, profile=profile, start_date=start_date)
```

### Comparing `blackline-core-0.1.1a0/tests/conftest_sqlite.py` & `blackline-core-0.1.2/tests/conftest_sqlite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,99 @@
 import sqlite3
 from sqlite3 import Connection
-from typing import List
 
 import pytest
 from blackline.adapters.sqlite.sqlite import SQLiteAdapter
 from blackline.models.datastores import DataStore
 
 
 @pytest.fixture
 def sqlite_store_name() -> str:
     return "test_sqlite"
 
 
 @pytest.fixture
-def deidentified_mock_data_sqlite() -> List:
+def deidentified_mock_data_sqlite(deidentified_mock_user_data: list) -> list:
     return [
-        ("2021-01-01 00:00:00", None, "fake@email.com", "12345", 1, "###.#.#.#"),
-        ("2021-06-01 00:00:00", None, "fake@email.com", "23456", 1, "###.#.#.#"),
-        ("2022-03-01 00:00:00", "Chris", "chris@example.com", "34567", 0, "###.#.#.#"),
         (
-            "2022-04-01 00:00:00",
-            "Megan",
-            "megan@example.com",
-            "45678",
-            1,
-            "127.0.0.4",
-        ),
+            user[0].strftime("%Y-%m-%d %H:%M:%S"),
+            user[1],
+            user[2],
+            user[3],
+            int(user[4]),
+            user[5],
+            user[6].strftime("%Y-%m-%d %H:%M:%S") if user[6] is not None else None,
+        )
+        for user in deidentified_mock_user_data
     ]
 
 
 @pytest.fixture
-def mock_sqlite_store(mock_data: List, test_table: str) -> Connection:
+def mock_sqlite_store(
+    mock_user_data: list, test_table: str, mock_session_data: list
+) -> Connection:
     con = sqlite3.connect(
         "file::memory:?cache=shared",
         detect_types=sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES,
         uri=True,
     )
-    cur = con.cursor()
-    cur.execute(f"DROP TABLE IF EXISTS {test_table}")
-    cur.execute(
-        f"""CREATE TABLE {test_table}(
+
+    with con:
+        cur = con.cursor()
+        cur.execute(f"DROP TABLE IF EXISTS {test_table}")
+        cur.execute(
+            f"""CREATE TABLE {test_table}(
+                created_at TEXT,
+                name TEXT,
+                email TEXT,
+                postal_code TEXT,
+                active BOOLEAN,
+                ip TEXT,
+                deactivation_date TEXT
+                )"""
+        )
+
+        cur.executemany(
+            f"INSERT INTO {test_table} VALUES (?, ?, ?, ?, ?, ?, ?)", mock_user_data
+        )
+
+    with con:
+        cur = con.cursor()
+        cur.execute("DROP TABLE IF EXISTS session")
+        cur.execute(
+            """CREATE TABLE session(
             created_at TEXT,
-            name TEXT,
+            session_started_at TEXT,
             email TEXT,
-            postal_code TEXT,
-            active BOOLEAN,
-            ip TEXT
+            ip TEXT,
+            cookie_id TEXT
             )"""
-    )
-
-    cur.executemany(f"INSERT INTO {test_table} VALUES (?, ?, ?, ?, ?, ?)", mock_data)
-    con.commit()
+        )
+        cur.executemany("INSERT INTO session VALUES (?, ?, ?, ?, ?)", mock_session_data)
 
     yield con
 
-    con.cursor().execute(f"DROP TABLE {test_table}")
+    with con:
+        con.cursor().execute("DROP TABLE session")
+
+    with con:
+        con.cursor().execute(f"DROP TABLE {test_table}")
+
     con.close()
 
 
 @pytest.fixture
 def sqlite_adapter(
     store: DataStore, mock_sqlite_store: Connection, store_name: str
 ) -> SQLiteAdapter:
     return store.adapter
 
 
 @pytest.fixture
-def sqlite_store_yml() -> str:
+def sqlite_store_profiles_yaml() -> str:
     return """
     profiles:
       dev:
         type: sqlite
         config:
           connection:
             database: "file::memory:"
```

### Comparing `blackline-core-0.1.1a0/tests/execution/test_debug.py` & `blackline-core-0.1.2/tests/execution/test_debug.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/execution/test_deifentify.py` & `blackline-core-0.1.2/tests/execution/test_deifentify.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     profile: str,
 ) -> None:
     # Run
     deidentify.deidentify()
 
     # Assert
     assert deidentify.catalogue is not None
-    adapter = deidentify.stores.store(name="dataset_foo", profile=profile).adapter
+    adapter = deidentify.stores["dataset_foo"][profile].adapter
 
     with adapter.connection() as conn:
         deidentified_data = conn.execute(f"SELECT * FROM {test_table}").fetchall()
-    assert deidentified_data == deidentified_mock_data_sqlite
+    assert set(deidentified_data) == set(deidentified_mock_data_sqlite)
 
 
 def test_deidentify_validate_catalogue_dataset_no_exceptions(
     deidentify: Deidentify,
     mock_sqlite_store: Connection,
     deidentified_mock_data_sqlite: list[tuple],
     test_table: str,
@@ -79,19 +79,20 @@
     # Run
     excs = deidentify_func(
         path=deidentify.path, profile=profile, start_date=deidentify.start_date
     )
 
     # Assert
     assert excs is None
-    adapter = deidentify.stores.store(name="dataset_foo", profile=profile).adapter
+    adapter = deidentify.stores["dataset_foo"][profile].adapter
 
     with adapter.connection() as conn:
         deidentified_data = conn.execute(f"SELECT * FROM {test_table}").fetchall()
-    assert deidentified_data == deidentified_mock_data_sqlite
+
+    assert set(deidentified_data) == set(deidentified_mock_data_sqlite)
 
 
 def test_deidentify_with_exceptions(
     profile: str,
     project_root: Path,
     sample_project: Callable,
     start_date: datetime,
```

### Comparing `blackline-core-0.1.1a0/tests/execution/test_demo.py` & `blackline-core-0.1.2/tests/execution/test_demo.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/execution/test_report.py` & `blackline-core-0.1.2/tests/execution/test_report.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/execution/test_validate.py` & `blackline-core-0.1.2/tests/execution/test_validate.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/factories/test_adapter_factory.py` & `blackline-core-0.1.2/tests/factories/test_adapter_factory.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/models/test_catalogue.py` & `blackline-core-0.1.2/tests/models/test_catalogue.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 
     # Run
     dataset = Dataset.parse_dir(path=dataset_dir)
 
     # Assert
     assert isinstance(dataset, Dataset)
     assert dataset.key == key
+    # breakpoint()
 
 
 def test_resource_parse_dir(project_config: ProjectConfig, resource_dirs: list[Path]):
     # Setup
     resource_dir = resource_dirs[0]
     key = "resource_foo"
 
     # Run
     resource = Resource.parse_dir(path=resource_dir)
 
     assert isinstance(resource, Resource)
     assert resource.key == key
     assert isinstance(resource["dataset_foo"], Dataset)
+    for child in resource.children.values():
+        assert isinstance(child, Dataset)
 
 
 def test_system_parse_dir(project_config: ProjectConfig, system_dirs: list[Path]):
     # Setup
     system_dir = system_dirs[0]
     key = "system_foo"
 
@@ -45,14 +48,18 @@
     system = System.parse_dir(path=system_dir)
 
     # Assert
     assert isinstance(system, System)
     assert system.key == key
     assert isinstance(system["resource_foo"], Resource)
     assert isinstance(system["resource_foo.dataset_foo"], Dataset)
+    for system_child in system.children.values():
+        for resource_child in system_child.children.values():
+            assert isinstance(resource_child, Dataset)
+        assert isinstance(system_child, Resource)
 
 
 def test_organization_parse_dir(
     project_config: ProjectConfig, organization_dirs: list[Path]
 ):
     # Setup
     organization_dir = organization_dirs[0]
@@ -61,14 +68,21 @@
     organization = Organization.parse_dir(path=organization_dir)
 
     assert isinstance(organization, Organization)
     assert organization.key == "organization_foo"
     assert isinstance(organization["system_foo"], System)
     assert isinstance(organization["system_foo.resource_foo"], Resource)
 
+    for organization_child in organization.children.values():
+        for system_child in organization_child.children.values():
+            for resource_child in system_child.children.values():
+                assert isinstance(resource_child, Dataset)
+            assert isinstance(system_child, Resource)
+        assert isinstance(organization_child, System)
+
 
 def test_catalogue_parse_dir(project_config: ProjectConfig, catalogue_dir: list[Path]):
     # Run
     catalogue = Catalogue.parse_dir(path=catalogue_dir)
 
     assert isinstance(catalogue, Catalogue)
     assert isinstance(catalogue["organization_foo"], Organization)
```

### Comparing `blackline-core-0.1.1a0/tests/models/test_datastores.py` & `blackline-core-0.1.2/tests/models/test_datastores.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,100 @@
 from pathlib import Path
 
 import pytest
 from blackline.adapters.sqlite.sqlite import SQLiteAdapter
-from blackline.models.adapter import AdapterConfig
+from blackline.models.datastore_base import DataStoreBase
 from blackline.models.datastores import DataStore, DataStores
 from blackline.models.project_config import ProjectConfig
-from blackline.models.sqlite.sqlite import SQLiteConfig
+from blackline.models.sqlite.sqlite import SQLiteDataStore
 from yaml import safe_load
 
 
-def test_DataStore(profile: str, sqlite_store_yml: str) -> None:
-    info = safe_load(sqlite_store_yml)
+def test_DataStore(profile: str, sqlite_store_profiles_yaml: str) -> None:
+    # Setup
+    info = safe_load(sqlite_store_profiles_yaml)
     info["name"] = "foo"
+
+    # Run
     config = DataStore.parse_obj(info)
+
+    # Assert
     assert config.name == "foo"
-    assert isinstance(config.profiles[profile], SQLiteConfig)
+    assert isinstance(config.profiles[profile], SQLiteDataStore)
 
 
-def test_DataStores(profile: str, sqlite_store_yml: str) -> None:
-    info = safe_load(sqlite_store_yml)
+def test_DataStores(profile: str, sqlite_store_profiles_yaml: str) -> None:
+    # Setup
+    info = safe_load(sqlite_store_profiles_yaml)
     info["name"] = "foo"
     config = DataStore.parse_obj(info)
+
+    # Run
     stores = DataStores(stores=[config])
+
+    # Assert
     for store in stores.stores:
         assert isinstance(store, DataStore)
 
 
-def test_DataStores_store_with_profile(profile: str, sqlite_store_yml: str) -> None:
-    info = safe_load(sqlite_store_yml)
+def test_DataStores_store_with_profile(
+    profile: str, sqlite_store_profiles_yaml: str
+) -> None:
+    # Setup
+    info = safe_load(sqlite_store_profiles_yaml)
     info["name"] = "foo"
     config = DataStore.parse_obj(info)
     stores = DataStores(stores=[config])
-    store = stores.store(name="foo", profile=profile)
-    assert isinstance(store, SQLiteConfig)
 
+    # Run
+    store = stores["foo"][profile]
 
-def test_DataStores_store_no_profile(profile: str, sqlite_store_yml: str) -> None:
-    info = safe_load(sqlite_store_yml)
+    # Assert
+    assert isinstance(store, SQLiteDataStore)
+
+
+def test_DataStores_store_no_profile(
+    profile: str, sqlite_store_profiles_yaml: str
+) -> None:
+    # Setup
+    info = safe_load(sqlite_store_profiles_yaml)
     info["name"] = "foo"
     config = DataStore.parse_obj(info)
     stores = DataStores(stores=[config])
-    store = stores.store(name="foo")
-    assert isinstance(store, dict)
 
+    # Run
+    store = stores["foo"]
+
+    # Assert
+    assert isinstance(store, DataStore)
 
-def test_DataStores_store_not_found(profile: str, sqlite_store_yml: str) -> None:
-    info = safe_load(sqlite_store_yml)
+
+def test_DataStores_store_not_found(
+    profile: str, sqlite_store_profiles_yaml: str
+) -> None:
+    # Setup
+    info = safe_load(sqlite_store_profiles_yaml)
     info["name"] = "foo"
     config = DataStore.parse_obj(info)
     stores = DataStores(stores=[config])
+
+    # Run
     with pytest.raises(ValueError) as excinfo:
-        stores.store(name="bar")
+        stores["bar"]
+
+        # Assert
         assert "Store bar not found" in str(excinfo.value)
 
 
 def test_DataStores_parse_folder(
     project_config: ProjectConfig, profile: str, store_name: str
 ):
     path = Path(project_config.project_root, project_config.adapters_path)
 
     # Run
     stores = DataStores.parse_folder(path=path)
-    store = stores.store(name=store_name, profile=profile)
+    store = stores[store_name][profile]
 
     # Assert
-    assert isinstance(store, AdapterConfig)
+    assert isinstance(store, DataStoreBase)
     assert isinstance(store.adapter, SQLiteAdapter)
     assert store.config.connection.database == "file::memory:?cache=shared"
```

### Comparing `blackline-core-0.1.1a0/tests/models/test_project_config.py` & `blackline-core-0.1.2/tests/models/test_project_config.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/models/test_validation.py` & `blackline-core-0.1.2/tests/models/test_validation.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/project/test_init_project.py` & `blackline-core-0.1.2/tests/project/test_init_project.py`

 * *Files identical despite different names*

### Comparing `blackline-core-0.1.1a0/tests/utils/test_doc_examples.py` & `blackline-core-0.1.2/tests/utils/test_doc_examples.py`

 * *Files identical despite different names*

