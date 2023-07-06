# Comparing `tmp/rondsspark-0.0.4.4.tar.gz` & `tmp/rondsspark-0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rondsspark-0.0.4.4.tar", last modified: Thu Jul  6 06:40:08 2023, max compression
+gzip compressed data, was "dist\rondsspark-0.0.4.5.tar", last modified: Thu Jul  6 07:25:34 2023, max compression
```

## Comparing `rondsspark-0.0.4.4.tar` & `rondsspark-0.0.4.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/
--rw-rw-rw-   0        0        0      220 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/rondsspark.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/rondsspark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/rondsspark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       84 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/rondsspark.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1502 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/rondsspark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/rondsspark.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/dataframe/
--rw-rw-rw-   0        0        0     4377 2023-06-26 08:10:36.000000 rondsspark-0.0.4.4/ronds_sdk/dataframe/pvalue.py
--rw-rw-rw-   0        0        0        0 2023-06-08 01:43:15.000000 rondsspark-0.0.4.4/ronds_sdk/dataframe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/datasources/
--rw-rw-rw-   0        0        0     3335 2023-07-06 03:29:31.000000 rondsspark-0.0.4.4/ronds_sdk/datasources/cassandra_manager.py
--rw-rw-rw-   0        0        0        0 2023-06-27 13:38:08.000000 rondsspark-0.0.4.4/ronds_sdk/datasources/__init__.py
--rw-rw-rw-   0        0        0      792 2023-06-08 13:00:10.000000 rondsspark-0.0.4.4/ronds_sdk/error.py
--rw-rw-rw-   0        0        0      267 2023-07-05 12:51:09.000000 rondsspark-0.0.4.4/ronds_sdk/logger_config.py
--rw-rw-rw-   0        0        0      531 2023-06-07 03:32:55.000000 rondsspark-0.0.4.4/ronds_sdk/logging_config.yml
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/ml/
--rw-rw-rw-   0        0        0        0 2023-06-07 06:10:31.000000 rondsspark-0.0.4.4/ronds_sdk/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/options/
--rw-rw-rw-   0        0        0     7497 2023-07-05 03:15:47.000000 rondsspark-0.0.4.4/ronds_sdk/options/pipeline_options.py
--rw-rw-rw-   0        0        0     6424 2023-06-09 11:16:10.000000 rondsspark-0.0.4.4/ronds_sdk/options/value_provider.py
--rw-rw-rw-   0        0        0        0 2023-06-08 03:30:12.000000 rondsspark-0.0.4.4/ronds_sdk/options/__init__.py
--rw-rw-rw-   0        0        0    13648 2023-07-03 10:06:11.000000 rondsspark-0.0.4.4/ronds_sdk/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/runners/
--rw-rw-rw-   0        0        0        0 2023-06-08 09:17:22.000000 rondsspark-0.0.4.4/ronds_sdk/runners/pipeline_context.py
--rw-rw-rw-   0        0        0      538 2023-07-04 02:31:48.000000 rondsspark-0.0.4.4/ronds_sdk/runners/python_runner.py
--rw-rw-rw-   0        0        0     2953 2023-06-29 09:56:08.000000 rondsspark-0.0.4.4/ronds_sdk/runners/runner.py
--rw-rw-rw-   0        0        0     2624 2023-06-30 02:32:09.000000 rondsspark-0.0.4.4/ronds_sdk/runners/spark_runner.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:07.000000 rondsspark-0.0.4.4/ronds_sdk/runners/visitors/
--rw-rw-rw-   0        0        0     3856 2023-07-06 02:15:52.000000 rondsspark-0.0.4.4/ronds_sdk/runners/visitors/spark_runner_visitor.py
--rw-rw-rw-   0        0        0        0 2023-06-29 09:25:38.000000 rondsspark-0.0.4.4/ronds_sdk/runners/visitors/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:10:46.000000 rondsspark-0.0.4.4/ronds_sdk/runners/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/ronds_sdk/tools/
--rw-rw-rw-   0        0        0     1416 2023-07-06 02:14:39.000000 rondsspark-0.0.4.4/ronds_sdk/tools/utils.py
--rw-rw-rw-   0        0        0        0 2023-06-07 06:11:02.000000 rondsspark-0.0.4.4/ronds_sdk/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/
--rw-rw-rw-   0        0        0       73 2023-06-08 13:20:13.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/core.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/
--rw-rw-rw-   0        0        0     6022 2023-07-06 06:27:37.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/cassandra_rule.py
--rw-rw-rw-   0        0        0     4868 2023-06-30 11:12:05.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/rule_merge_data.py
--rw-rw-rw-   0        0        0     5990 2023-07-06 06:33:09.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/transforms.py
--rw-rw-rw-   0        0        0        0 2023-06-30 02:11:50.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/__init__.py
--rw-rw-rw-   0        0        0     7460 2023-07-03 06:11:22.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/ptransform.py
--rw-rw-rw-   0        0        0      530 2023-06-29 12:12:57.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/remote_debug.py
--rw-rw-rw-   0        0        0     5363 2023-07-06 06:14:37.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/ronds.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/spark/
--rw-rw-rw-   0        0        0     4331 2023-06-30 02:29:55.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/spark/transforms.py
--rw-rw-rw-   0        0        0        0 2023-06-30 02:11:59.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/spark/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-08 01:41:33.000000 rondsspark-0.0.4.4/ronds_sdk/transforms/__init__.py
--rw-rw-rw-   0        0        0      855 2023-07-04 10:53:54.000000 rondsspark-0.0.4.4/ronds_sdk/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      534 2023-07-06 06:40:04.000000 rondsspark-0.0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/test/
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/test/sdk/
--rw-rw-rw-   0        0        0     3598 2023-07-04 07:02:09.000000 rondsspark-0.0.4.4/test/sdk/sdk_test.py
--rw-rw-rw-   0        0        0     3130 2023-07-04 06:44:02.000000 rondsspark-0.0.4.4/test/sdk/sdk_unitest.py
--rw-rw-rw-   0        0        0        0 2023-06-13 06:59:02.000000 rondsspark-0.0.4.4/test/sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/test/simple/
--rw-rw-rw-   0        0        0      949 2023-06-09 13:10:50.000000 rondsspark-0.0.4.4/test/simple/overloading_test.py
--rw-rw-rw-   0        0        0        0 2023-06-09 13:04:55.000000 rondsspark-0.0.4.4/test/simple/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 06:40:08.000000 rondsspark-0.0.4.4/test/spark/
--rw-rw-rw-   0        0        0      522 2023-06-07 07:41:05.000000 rondsspark-0.0.4.4/test/spark/SimpleTest.py
--rw-rw-rw-   0        0        0     2830 2023-06-19 11:56:18.000000 rondsspark-0.0.4.4/test/spark/SparkTest.py
--rw-rw-rw-   0        0        0        0 2023-06-07 03:03:37.000000 rondsspark-0.0.4.4/test/spark/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-07 03:06:08.000000 rondsspark-0.0.4.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/
+-rw-rw-rw-   0        0        0      220 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1502 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/rondsspark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/dataframe/
+-rw-rw-rw-   0        0        0     4377 2023-06-26 08:10:36.000000 rondsspark-0.0.4.5/ronds_sdk/dataframe/pvalue.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 01:43:15.000000 rondsspark-0.0.4.5/ronds_sdk/dataframe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/datasources/
+-rw-rw-rw-   0        0        0     3296 2023-07-06 07:06:36.000000 rondsspark-0.0.4.5/ronds_sdk/datasources/cassandra_manager.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 13:38:08.000000 rondsspark-0.0.4.5/ronds_sdk/datasources/__init__.py
+-rw-rw-rw-   0        0        0      792 2023-06-08 13:00:10.000000 rondsspark-0.0.4.5/ronds_sdk/error.py
+-rw-rw-rw-   0        0        0      267 2023-07-05 12:51:09.000000 rondsspark-0.0.4.5/ronds_sdk/logger_config.py
+-rw-rw-rw-   0        0        0      531 2023-06-07 03:32:55.000000 rondsspark-0.0.4.5/ronds_sdk/logging_config.yml
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/ml/
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:10:31.000000 rondsspark-0.0.4.5/ronds_sdk/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/options/
+-rw-rw-rw-   0        0        0     7491 2023-07-06 07:21:09.000000 rondsspark-0.0.4.5/ronds_sdk/options/pipeline_options.py
+-rw-rw-rw-   0        0        0     6424 2023-06-09 11:16:10.000000 rondsspark-0.0.4.5/ronds_sdk/options/value_provider.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:30:12.000000 rondsspark-0.0.4.5/ronds_sdk/options/__init__.py
+-rw-rw-rw-   0        0        0    13648 2023-07-03 10:06:11.000000 rondsspark-0.0.4.5/ronds_sdk/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/runners/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:17:22.000000 rondsspark-0.0.4.5/ronds_sdk/runners/pipeline_context.py
+-rw-rw-rw-   0        0        0      538 2023-07-04 02:31:48.000000 rondsspark-0.0.4.5/ronds_sdk/runners/python_runner.py
+-rw-rw-rw-   0        0        0     2953 2023-06-29 09:56:08.000000 rondsspark-0.0.4.5/ronds_sdk/runners/runner.py
+-rw-rw-rw-   0        0        0     2750 2023-07-06 07:24:51.000000 rondsspark-0.0.4.5/ronds_sdk/runners/spark_runner.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/runners/visitors/
+-rw-rw-rw-   0        0        0     3856 2023-07-06 02:15:52.000000 rondsspark-0.0.4.5/ronds_sdk/runners/visitors/spark_runner_visitor.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 09:25:38.000000 rondsspark-0.0.4.5/ronds_sdk/runners/visitors/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:10:46.000000 rondsspark-0.0.4.5/ronds_sdk/runners/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/tools/
+-rw-rw-rw-   0        0        0     1416 2023-07-06 02:14:39.000000 rondsspark-0.0.4.5/ronds_sdk/tools/utils.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:11:02.000000 rondsspark-0.0.4.5/ronds_sdk/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/
+-rw-rw-rw-   0        0        0       73 2023-06-08 13:20:13.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/core.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/
+-rw-rw-rw-   0        0        0     6022 2023-07-06 06:27:37.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/cassandra_rule.py
+-rw-rw-rw-   0        0        0     4868 2023-06-30 11:12:05.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/rule_merge_data.py
+-rw-rw-rw-   0        0        0     6126 2023-07-06 07:24:05.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/transforms.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 02:11:50.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/__init__.py
+-rw-rw-rw-   0        0        0     7460 2023-07-03 06:11:22.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/ptransform.py
+-rw-rw-rw-   0        0        0      530 2023-06-29 12:12:57.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/remote_debug.py
+-rw-rw-rw-   0        0        0     5253 2023-07-06 07:02:37.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/ronds.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/spark/
+-rw-rw-rw-   0        0        0     4755 2023-07-06 07:03:56.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/spark/transforms.py
+-rw-rw-rw-   0        0        0        0 2023-06-30 02:11:59.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/spark/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 01:41:33.000000 rondsspark-0.0.4.5/ronds_sdk/transforms/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-07-04 10:53:54.000000 rondsspark-0.0.4.5/ronds_sdk/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-07-06 07:25:08.000000 rondsspark-0.0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/test/
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/test/sdk/
+-rw-rw-rw-   0        0        0     3598 2023-07-04 07:02:09.000000 rondsspark-0.0.4.5/test/sdk/sdk_test.py
+-rw-rw-rw-   0        0        0     3130 2023-07-04 06:44:02.000000 rondsspark-0.0.4.5/test/sdk/sdk_unitest.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:59:02.000000 rondsspark-0.0.4.5/test/sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/test/simple/
+-rw-rw-rw-   0        0        0      949 2023-06-09 13:10:50.000000 rondsspark-0.0.4.5/test/simple/overloading_test.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 13:04:55.000000 rondsspark-0.0.4.5/test/simple/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:25:34.000000 rondsspark-0.0.4.5/test/spark/
+-rw-rw-rw-   0        0        0      522 2023-06-07 07:41:05.000000 rondsspark-0.0.4.5/test/spark/SimpleTest.py
+-rw-rw-rw-   0        0        0     2830 2023-06-19 11:56:18.000000 rondsspark-0.0.4.5/test/spark/SparkTest.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 03:03:37.000000 rondsspark-0.0.4.5/test/spark/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 03:06:08.000000 rondsspark-0.0.4.5/test/__init__.py
```

### Comparing `rondsspark-0.0.4.4/rondsspark.egg-info/SOURCES.txt` & `rondsspark-0.0.4.5/rondsspark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/dataframe/pvalue.py` & `rondsspark-0.0.4.5/ronds_sdk/dataframe/pvalue.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/datasources/cassandra_manager.py` & `rondsspark-0.0.4.5/ronds_sdk/datasources/cassandra_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import logging
 import uuid
 from typing import Sequence, List
 
-from cassandra import ProtocolVersion
 from cassandra.cluster import Cluster, Session, ResultSet
 from ronds_sdk.options.pipeline_options import CassandraOptions
 
 
 class Singleton(object):
     def __init__(self, cls):
         self._cls = cls
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/error.py` & `rondsspark-0.0.4.5/ronds_sdk/error.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/logging_config.yml` & `rondsspark-0.0.4.5/ronds_sdk/logging_config.yml`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/options/pipeline_options.py` & `rondsspark-0.0.4.5/ronds_sdk/options/pipeline_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
 
 class SparkRunnerOptions(PipelineOptions):
     @classmethod
     def _add_argparse_args(cls, parser):  # type: (_RondsArgumentParser) -> None
         parser.add_argument(
             '--spark_master_url',
-            default='local[2]',
+            default=None,
         )
         parser.add_argument(
             '--spark_job_server_jar',
         )
         parser.add_argument(
             '--spark_version',
             default='3'
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/options/value_provider.py` & `rondsspark-0.0.4.5/ronds_sdk/options/value_provider.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/pipeline.py` & `rondsspark-0.0.4.5/ronds_sdk/pipeline.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/runners/python_runner.py` & `rondsspark-0.0.4.5/ronds_sdk/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/runners/runner.py` & `rondsspark-0.0.4.5/ronds_sdk/runners/runner.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/runners/spark_runner.py` & `rondsspark-0.0.4.5/ronds_sdk/runners/spark_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,19 @@
         import findspark
         findspark.init()
         self.spark_options = self.options.view_as(SparkRunnerOptions)
         self.spark = self.new_spark(self.spark_options)
 
     @staticmethod
     def new_spark(options):
-        return SparkSession\
-            .builder\
-            .master(options.spark_master_url)\
-            .getOrCreate()
+        builder = SparkSession.builder
+        logging.info("spark master url: %s" % options.spark_master_url)
+        if options.spark_master_url is not None:
+            builder.master(options.spark_master_url)
+        return builder.getOrCreate()
 
     def transform_package(self):
         return self.spark_options.spark_transform_package
 
     def run_pipeline(self, pipeline, options):
         visitor = SparkRunnerVisitor(self.options, self.spark)
         pipeline.visit(visitor)
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/runners/visitors/spark_runner_visitor.py` & `rondsspark-0.0.4.5/ronds_sdk/runners/visitors/spark_runner_visitor.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/tools/utils.py` & `rondsspark-0.0.4.5/ronds_sdk/tools/utils.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/cassandra_rule.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/cassandra_rule.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/rule_merge_data.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/rule_merge_data.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/pandas/transforms.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/pandas/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import importlib
 import json
+import logging
 import sys
+import time
 from os.path import dirname, abspath
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 import pandas as pd
 from pyspark.sql import DataFrame, SparkSession
 
@@ -23,15 +25,18 @@
     def __init__(self,
                  _sleep  # type: ronds.Sleep
                  ):
         super(Sleep, self).__init__()
         self._sleep = _sleep
 
     def expand(self, input_inputs, action_func=None):
-        return self._sleep.expand(input_inputs, action_func)
+        logging.info("start sleep~")
+        time.sleep(self._sleep.seconds)
+        logging.info("end sleep~")
+        return input_inputs
 
 
 class RulesCassandraScan(ForeachBatchTransform):
 
     def __init__(self,
                  rule_load,  # type: ronds.RulesCassandraScan
                  options,  # type: PipelineOptions
@@ -74,14 +79,15 @@
         super(Console, self).__init__()
         self._mode = console.mode
 
     def expand(self, input_inputs, action_func=None):
         assert isinstance(input_inputs, pvalue.PCollection)
         df = input_inputs.element_value
         assert isinstance(df, pd.DataFrame)
+        print('*' * 20)
         print(df.head(10))
         return pvalue.PDone(input_inputs.pipeline,
                             element_type=pd.DataFrame,
                             is_bounded=True)
 
 
 class Algorithm(PTransform):
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/ptransform.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/ptransform.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/remote_debug.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/remote_debug.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/ronds.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/ronds.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,20 +19,17 @@
 
 class Sleep(PTransform):
 
     def __init__(self,
                  seconds=60,  # type: int
                  ):
         super(Sleep, self).__init__()
-        self._seconds = seconds
+        self.seconds = seconds
 
     def expand(self, input_inputs, action_func=None):
-        logging.info("start sleep~")
-        time.sleep(self._seconds)
-        logging.info("end sleep~")
         return input_inputs
 
 
 class RulesCassandraScan(PTransform):
     """
     根据规则配置, 按照制定时间窗口周期, 进行 Cassandra 定期读表加载数据
     """
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/transforms/spark/transforms.py` & `rondsspark-0.0.4.5/ronds_sdk/transforms/spark/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+import logging
+import time
+
 from ronds_sdk import error
 from ronds_sdk.transforms.ptransform import PTransform, ForeachBatchTransform
 from ronds_sdk.dataframe import pvalue
 from ronds_sdk.runners.spark_runner import SparkRunner
 from pyspark.sql import DataFrame
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ronds_sdk.transforms import ronds
 
 
+class Sleep(PTransform):
+
+    def __init__(self,
+                 _sleep  # type: ronds.Sleep
+                 ):
+        super(Sleep, self).__init__()
+        self._sleep = _sleep
+
+    def expand(self, input_inputs, action_func=None):
+        logging.info("start sleep~")
+        time.sleep(self._sleep.seconds)
+        logging.info("end sleep~")
+        return input_inputs
+
+
 class Create(PTransform):
     def __init__(self,
                  create,  # type: ronds.Create
                  ):
         super(Create, self).__init__()
         self.values = create.values
```

### Comparing `rondsspark-0.0.4.4/ronds_sdk/__init__.py` & `rondsspark-0.0.4.5/ronds_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/setup.py` & `rondsspark-0.0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 # noinspection SpellCheckingInspection
 setup(
     name='rondsspark',
-    version='0.0.4.4',
+    version='0.0.4.5',
     description='ronds spark sdk',
     author='dongyunlong',
     author_email='yunlong.dong@ronds.com.cn',
-    install_requires=['pyspark', 'cassandra-driver', 'pandas', 'pyYAML',
+    install_requires=['cassandra-driver', 'pandas', 'pyYAML',
                       'schedule', 'wheel', 'findspark', 'importlib_resources'],
     package_data={
         '': ['logging_config.yml'],
     },
     packages=find_packages(),
     license='apache 3.0',
 )
```

### Comparing `rondsspark-0.0.4.4/test/sdk/sdk_test.py` & `rondsspark-0.0.4.5/test/sdk/sdk_test.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/test/sdk/sdk_unitest.py` & `rondsspark-0.0.4.5/test/sdk/sdk_unitest.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/test/simple/overloading_test.py` & `rondsspark-0.0.4.5/test/simple/overloading_test.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/test/spark/SimpleTest.py` & `rondsspark-0.0.4.5/test/spark/SimpleTest.py`

 * *Files identical despite different names*

### Comparing `rondsspark-0.0.4.4/test/spark/SparkTest.py` & `rondsspark-0.0.4.5/test/spark/SparkTest.py`

 * *Files identical despite different names*

