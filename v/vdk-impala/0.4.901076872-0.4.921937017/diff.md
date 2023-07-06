# Comparing `tmp/vdk-impala-0.4.901076872.tar.gz` & `tmp/vdk-impala-0.4.921937017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-impala-0.4.901076872.tar", last modified: Thu Jun 15 11:51:17 2023, max compression
+gzip compressed data, was "vdk-impala-0.4.921937017.tar", last modified: Wed Jul  5 17:32:34 2023, max compression
```

## Comparing `vdk-impala-0.4.901076872.tar` & `vdk-impala-0.4.921937017.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.284760 vdk-impala-0.4.901076872/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5637 2023-06-15 11:51:17.280760 vdk-impala-0.4.901076872/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5043 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 11:51:17.284760 vdk-impala-0.4.901076872/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-06-15 11:51:05.000000 vdk-impala-0.4.901076872/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.264760 vdk-impala-0.4.901076872/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.264760 vdk-impala-0.4.901076872/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.264760 vdk-impala-0.4.901076872/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)    20197 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_lineage_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6722 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/data_quality_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)      880 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.268760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3311 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/
--rw-rw-rw-   0 root         (0) root         (0)      815 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.272760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.276760 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/
--rw-rw-rw-   0 root         (0) root         (0)     2076 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     4358 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/template_arguments_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.276760 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5637 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3918 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-15 11:51:17.000000 vdk-impala-0.4.901076872/src/vdk_impala.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.280760 vdk-impala-0.4.901076872/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.264760 vdk-impala-0.4.901076872/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.264760 vdk-impala-0.4.901076872/tests/functional/jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.280760 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job/20_populate_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.280760 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job-non-lineage/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:51:17.280760 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job-syntax-error/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-06-15 11:51:01.000000 vdk-impala-0.4.901076872/tests/test_error_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.171602 vdk-impala-0.4.921937017/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5637 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5043 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 17:32:34.171602 vdk-impala-0.4.921937017/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-07-05 17:32:22.000000 vdk-impala-0.4.921937017/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.155602 vdk-impala-0.4.921937017/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.155602 vdk-impala-0.4.921937017/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.155602 vdk-impala-0.4.921937017/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    20197 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_lineage_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6722 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/data_quality_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.159602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.163602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4358 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/template_arguments_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5637 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-05 17:32:34.000000 vdk-impala-0.4.921937017/src/vdk_impala.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.155602 vdk-impala-0.4.921937017/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.155602 vdk-impala-0.4.921937017/tests/functional/jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job/20_populate_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job-non-lineage/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 17:32:34.167602 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job-syntax-error/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-07-05 17:32:18.000000 vdk-impala-0.4.921937017/tests/test_error_classifier.py
```

### Comparing `vdk-impala-0.4.901076872/PKG-INFO` & `vdk-impala-0.4.921937017/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.901076872
+Version: 0.4.921937017
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.901076872/README.md` & `vdk-impala-0.4.921937017/README.md`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/setup.py` & `vdk-impala-0.4.921937017/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.901076872"
+__version__ = "0.4.921937017"
 
 setuptools.setup(
     name="vdk-impala",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Impala database.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_configuration.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_connection.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_error_classifier.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_error_handler.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_error_handler.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_helper.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_helper.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_lineage_plugin.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_lineage_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/impala_plugin.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/impala_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/data_quality_exception.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/data_quality_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class SlowlyChangingDimensionTypeOverwriteParams(BaseModel):
     target_schema: str
     target_table: str
     source_schema: str
     source_view: str
-    check: Optional[Callable[[str], bool]]
-    staging_schema: Optional[str]
+    check: Optional[Callable[[str], bool]] = None
+    staging_schema: Optional[str] = None
 
 
 class SlowlyChangingDimensionTypeOverwrite(TemplateArgumentsValidator):
     TemplateParams = SlowlyChangingDimensionTypeOverwriteParams
 
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 class FactDailySnapshotParams(BaseModel):
     target_schema: str
     target_table: str
     source_schema: str
     source_view: str
-    check: Optional[Callable[[str], bool]]
-    staging_schema: Optional[str]
+    check: Optional[Callable[[str], bool]] = None
+    staging_schema: Optional[str] = None
 
 
 class FactDailySnapshot(TemplateArgumentsValidator):
     TemplateParams = FactDailySnapshotParams
 
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 class FactDailySnapshotParams(BaseModel):
     target_schema: str
     target_table: str
     source_schema: str
     source_view: str
     last_arrival_ts: str
-    check: Optional[Callable[[str], bool]]
-    staging_schema: Optional[str]
+    check: Optional[Callable[[str], bool]] = None
+    staging_schema: Optional[str] = None
 
 
 class FactDailySnapshot(TemplateArgumentsValidator):
     TemplateParams = FactDailySnapshotParams
 
     def __init__(self) -> None:
         super().__init__()
```

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 
 from pydantic import BaseModel
-from pydantic import validator
+from pydantic import field_validator
+from pydantic import FieldValidationInfo
 from vdk.api.job_input import IJobInput
 from vdk.plugin.impala.templates.template_arguments_validator import (
     TemplateArgumentsValidator,
 )
 
 
 class LoadVersionedParams(BaseModel):
@@ -20,17 +21,19 @@
     tracked_columns: List[str]
     updated_at_column: str = "updated_at"
     sk_column: str = "sk"
     active_from_column: str = "active_from"
     active_to_column: str = "active_to"
     active_to_max_value: str = "9999-12-31"
 
-    @validator("tracked_columns", allow_reuse=True)
-    def passwords_match(cls, tracked_columns, values, **kwargs):
-        value_columns = values.get("value_columns")
+    @field_validator("tracked_columns")
+    def tracked_columns_subset_of_value_columns(
+        cls, tracked_columns: List[str], values: FieldValidationInfo, **kwargs
+    ):
+        value_columns = values.data["value_columns"]
         if type(value_columns) == list and not tracked_columns:
             raise ValueError("The list must contain at least one column")
         if type(value_columns) == list == type(value_columns) and not set(
             tracked_columns
         ) <= set(value_columns):
             raise ValueError(
                 "All elements in the list must be also present in `value_columns`"
```

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/template_arguments_validator.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/template_arguments_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk/plugin/impala/templates/utility.py` & `vdk-impala-0.4.921937017/src/vdk/plugin/impala/templates/utility.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/src/vdk_impala.egg-info/PKG-INFO` & `vdk-impala-0.4.921937017/src/vdk_impala.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.901076872
+Version: 0.4.921937017
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.901076872/src/vdk_impala.egg-info/SOURCES.txt` & `vdk-impala-0.4.921937017/src/vdk_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.901076872/tests/test_error_classifier.py` & `vdk-impala-0.4.921937017/tests/test_error_classifier.py`

 * *Files identical despite different names*

