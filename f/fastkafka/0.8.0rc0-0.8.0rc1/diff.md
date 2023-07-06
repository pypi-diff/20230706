# Comparing `tmp/fastkafka-0.8.0rc0.tar.gz` & `tmp/fastkafka-0.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.8.0rc0.tar", last modified: Thu Jun 29 13:54:24 2023, max compression
+gzip compressed data, was "fastkafka-0.8.0rc1.tar", last modified: Thu Jul  6 10:02:43 2023, max compression
```

## Comparing `fastkafka-0.8.0rc0.tar` & `fastkafka-0.8.0rc1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.333007 fastkafka-0.8.0rc0/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12572 2023-06-29 13:51:03.000000 fastkafka-0.8.0rc0/CONTRIBUTING.md
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-06-01 05:47:44.000000 fastkafka-0.8.0rc0/LICENSE
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-06-01 05:47:44.000000 fastkafka-0.8.0rc0/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24665 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    23237 2023-06-01 07:29:35.000000 fastkafka-0.8.0rc0/README.md
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      398 2023-06-29 13:51:30.000000 fastkafka-0.8.0rc0/fastkafka/_aiokafka_imports.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    40035 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13420 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5764 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4981 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13656 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7414 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    10312 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    25289 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51560 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    87522 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7313 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28096 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28660 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    14098 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5428 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/executors.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-06-29 13:51:30.000000 fastkafka-0.8.0rc0/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24665 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1441 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-06-01 08:53:21.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-06-29 12:08:23.000000 fastkafka-0.8.0rc0/settings.ini
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-06-29 13:54:24.333007 fastkafka-0.8.0rc0/setup.cfg
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-06-29 13:51:03.000000 fastkafka-0.8.0rc0/setup.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    12572 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 tvrtko    (1004) tvrtko    (1005)    11357 2023-01-26 06:58:43.000000 fastkafka-0.8.0rc1/LICENSE
+-rw-r--r--   0 tvrtko    (1004) tvrtko    (1005)      111 2023-01-26 06:58:43.000000 fastkafka-0.8.0rc1/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    24706 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    23278 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/README.md
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      525 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/__init__.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      398 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_aiokafka_imports.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    40048 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13467 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     2108 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     5764 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      996 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4981 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13623 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    19082 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     2905 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     6991 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    15024 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1612 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4136 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     4730 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13150 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     8102 2023-07-06 09:59:25.000000 fastkafka-0.8.0rc1/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    11893 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    10312 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    32769 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    51560 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    87787 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     7313 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 09:59:27.000000 fastkafka-0.8.0rc1/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    27911 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    28557 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    13966 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     5428 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      598 2023-07-06 09:59:26.000000 fastkafka-0.8.0rc1/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      454 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      858 2023-07-06 09:59:24.000000 fastkafka-0.8.0rc1/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1004) tvrtko    (1005)        0 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)    24706 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1441 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        1 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      146 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)        1 2023-01-26 07:01:03.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)      693 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)       10 2023-07-06 10:02:43.000000 fastkafka-0.8.0rc1/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     1231 2023-07-06 09:59:12.000000 fastkafka-0.8.0rc1/settings.ini
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)       38 2023-07-06 10:02:43.386407 fastkafka-0.8.0rc1/setup.cfg
+-rw-rw-r--   0 tvrtko    (1004) tvrtko    (1005)     3780 2023-07-06 07:52:26.000000 fastkafka-0.8.0rc1/setup.py
```

### Comparing `fastkafka-0.8.0rc0/CONTRIBUTING.md` & `fastkafka-0.8.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/LICENSE` & `fastkafka-0.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/PKG-INFO` & `fastkafka-0.8.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.8.0rc0
+Version: 0.8.0rc1
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -81,34 +81,34 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
-You can install base version of `fastkafka` with `pip` as usual:
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating
+systems. You can install base version of FastKafka with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
-To install fastkafka with testing features please use:
+To install FastKafka with testing features please use:
 
 ``` sh
 pip install fastkafka[test]
 ```
 
-To install fastkafka with asyncapi docs please use:
+To install FastKafka with asyncapi docs please use:
 
 ``` sh
 pip install fastkafka[docs]
 ```
 
-To install fastkafka with all the features please use:
+To install FastKafka with all the features please use:
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
@@ -162,15 +162,15 @@
 contains two entries: `"localhost"` and `"production"`, specifying local
 development and production Kafka brokers. Each entry specifies the URL,
 port, and other details of a Kafka broker. This dictionary is used for
 both generating the documentation and later to run the actual server
 against one of the given kafka broker.
 
 Next, an object of the
-[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka#fastkafka.FastKafka)
+[`FastKafka`](https://airtai.github.io/fastkafka/docs/api/fastkafka#fastkafka.FastKafka)
 class is initialized with the minimum set of arguments:
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
@@ -250,15 +250,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
+[`Tester`](https://airtai.github.io/fastkafka/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -311,15 +311,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
-We have created a simple fastkafka application. The app will consume the
+We have created a simple FastKafka application. The app will consume the
 `Data` from the `input_data` topic, log it and produce the incremented
 data to `output_data` topic.
 
 To test the app we have:
 
 1.  Created the app
```

### Comparing `fastkafka-0.8.0rc0/README.md` & `fastkafka-0.8.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,34 +51,34 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
-You can install base version of `fastkafka` with `pip` as usual:
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating
+systems. You can install base version of FastKafka with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
-To install fastkafka with testing features please use:
+To install FastKafka with testing features please use:
 
 ``` sh
 pip install fastkafka[test]
 ```
 
-To install fastkafka with asyncapi docs please use:
+To install FastKafka with asyncapi docs please use:
 
 ``` sh
 pip install fastkafka[docs]
 ```
 
-To install fastkafka with all the features please use:
+To install FastKafka with all the features please use:
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
@@ -132,15 +132,15 @@
 contains two entries: `"localhost"` and `"production"`, specifying local
 development and production Kafka brokers. Each entry specifies the URL,
 port, and other details of a Kafka broker. This dictionary is used for
 both generating the documentation and later to run the actual server
 against one of the given kafka broker.
 
 Next, an object of the
-[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka#fastkafka.FastKafka)
+[`FastKafka`](https://airtai.github.io/fastkafka/docs/api/fastkafka#fastkafka.FastKafka)
 class is initialized with the minimum set of arguments:
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
@@ -220,15 +220,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
+[`Tester`](https://airtai.github.io/fastkafka/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -281,15 +281,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
-We have created a simple fastkafka application. The app will consume the
+We have created a simple FastKafka application. The app will consume the
 `Data` from the `input_data` topic, log it and produce the incremented
 data to `output_data` topic.
 
 To test the app we have:
 
 1.  Created the app
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/__init__.py` & `fastkafka-0.8.0rc1/fastkafka/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0rc0"
+__version__ = "0.8.0rc1"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_application/app.py` & `fastkafka-0.8.0rc1/fastkafka/_application/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from inspect import signature
 from pathlib import Path
 from typing import *
 from unittest.mock import AsyncMock, MagicMock
 
 import anyio
 from pydantic import BaseModel
-from pydantic.main import ModelMetaclass
 
 from fastkafka._components.aiokafka_consumer_loop import (
     aiokafka_consumer_loop,
     sanitize_kafka_config,
 )
 from fastkafka._components.asyncapi import (
     ConsumeCallable,
@@ -107,24 +106,26 @@
         if isinstance(kafka_brokers, KafkaBrokers):
             return kafka_brokers
 
         retval = KafkaBrokers(
             brokers={
                 k: (
                     [
-                        KafkaBroker.parse_raw(
-                            unwrapped_v.json()
-                            if hasattr(unwrapped_v, "json")
+                        KafkaBroker.model_validate_json(
+                            unwrapped_v.model_dump_json()
+                            if hasattr(unwrapped_v, "model_dump_json")
                             else json.dumps(unwrapped_v)
                         )
                         for unwrapped_v in v
                     ]
                     if isinstance(v, list)
-                    else KafkaBroker.parse_raw(
-                        v.json() if hasattr(v, "json") else json.dumps(v)
+                    else KafkaBroker.model_validate_json(
+                        v.model_dump_json()
+                        if hasattr(v, "model_dump_json")
+                        else json.dumps(v)
                     )
                 )
                 for k, v in kafka_brokers.items()
             }
         )
 
     return retval
@@ -255,15 +256,15 @@
         self._kafka_config = _get_kafka_config(**kwargs)
 
         #
         self._consumers_store: Dict[
             str,
             Tuple[
                 ConsumeCallable,
-                Callable[[bytes, ModelMetaclass], Any],
+                Callable[[bytes, Type[BaseModel]], Any],
                 Union[str, StreamExecutor, None],
                 Optional[KafkaBrokers],
                 Dict[str, Any],
             ],
         ] = {}
 
         self._producers_store: Dict[  # type: ignore
@@ -322,17 +323,14 @@
         Sets the Kafka broker to start FastKafka with
 
         Args:
             kafka_broker_name: The name of the Kafka broker to start FastKafka
 
         Raises:
             ValueError: If the provided kafka_broker_name is not found in dictionary of kafka_brokers
-
-        Returns:
-            None
         """
 
         if kafka_broker_name not in self._kafka_brokers.brokers:
             raise ValueError(
                 f"Given kafka_broker_name '{kafka_broker_name}' is not found in kafka_brokers, available options are {self._kafka_brokers.brokers.keys()}"
             )
 
@@ -425,15 +423,15 @@
     async def _shutdown_producers(self) -> None:
         raise NotImplementedError
 
     async def _shutdown_bg_tasks(self) -> None:
         raise NotImplementedError
 
 # %% ../../nbs/015_FastKafka.ipynb 27
-def _get_decoder_fn(decoder: str) -> Callable[[bytes, ModelMetaclass], Any]:
+def _get_decoder_fn(decoder: str) -> Callable[[bytes, Type[BaseModel]], Any]:
     """
     Imports and returns decoder function based on input
     """
     if decoder == "json":
         from fastkafka._components.encoder.json import json_decoder
 
         return json_decoder
@@ -472,15 +470,15 @@
 
 # %% ../../nbs/015_FastKafka.ipynb 31
 @patch
 @delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
-    decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
+    decoder: Union[str, Callable[[bytes, Type[BaseModel]], Any]] = "json",
     *,
     executor: Union[str, StreamExecutor, None] = None,
     brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None,
     prefix: str = "on_",
     description: Optional[str] = None,
     **kwargs: Dict[str, Any],
 ) -> Callable[[ConsumeCallable], ConsumeCallable]:
@@ -521,15 +519,15 @@
         ValueError
 
     """
 
     def _decorator(
         on_topic: ConsumeCallable,
         topic: Optional[str] = topic,
-        decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = decoder,
+        decoder: Union[str, Callable[[bytes, Type[BaseModel]], Any]] = decoder,
         executor: Union[str, StreamExecutor, None] = executor,
         brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = brokers,
         description: Optional[str] = description,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ConsumeCallable:
         topic_resolved: str = (
             _get_topic_name(topic_callable=on_topic, prefix=prefix)
@@ -944,17 +942,14 @@
     This function exports the asyncapi specification based on the configured consumers
     and producers in the FastKafka instance. It generates the asyncapi documentation by
     extracting the topics and callbacks from the consumers and producers.
 
     Note:
         The asyncapi documentation is saved to the location specified by the `_asyncapi_path`
         attribute of the FastKafka instance.
-
-    Returns:
-        None
     """
     (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
     (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
     export_async_spec(
         consumers={
             remove_suffix(topic) if topic.endswith("_0") else topic: callback
             for topic, (callback, _, _, _, _) in self._consumers_store.items()
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_application/tester.py` & `fastkafka-0.8.0rc1/fastkafka/_application/tester.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,38 +49,36 @@
     __test__ = False
 
     def __init__(
         self,
         app: Union[FastKafka, List[FastKafka]],
         *,
         use_in_memory_broker: bool = True,
-        patch_module: Optional[ModuleType] = None,
     ):
         """Mirror-like object for testing a FastKafka application
 
         Can be used as context manager
 
         Args:
             app: The FastKafka application to be tested.
-            broker: An optional broker to start and to use for testing.
+            use_in_memory_broker: Whether to use an in-memory broker for testing or not.
         """
         self.apps = app if isinstance(app, list) else [app]
 
         for app in self.apps:
             app.create_mocks()
 
         super().__init__()
         self.mirrors: Dict[Any, Any] = {}
         self._kafka_brokers = self.apps[0]._kafka_brokers
         self._kafka_config["bootstrap_servers_id"] = self.apps[0]._kafka_config[
             "bootstrap_servers_id"
         ]
         self._create_mirrors()
         self.use_in_memory_broker = use_in_memory_broker
-        self.patch_module = patch_module
 
     async def _start_tester(self) -> None:
         """Starts the Tester"""
         for app in self.apps:
             await app.__aenter__()
         self.create_mocks()
         self._arrange_mirrors()
@@ -98,15 +96,15 @@
 
     def _arrange_mirrors(self) -> None:
         pass
 
     @asynccontextmanager
     async def _create_ctx(self) -> AsyncGenerator["Tester", None]:
         if self.use_in_memory_broker == True:
-            with InMemoryBroker(patch_module=self.patch_module):  # type: ignore
+            with InMemoryBroker():  # type: ignore
                 await self._start_tester()
                 try:
                     yield self
                 finally:
                     await self._stop_tester()
         else:
             await self._start_tester()
@@ -220,28 +218,32 @@
         None
     """
     for app in self.apps:
         for topic, (consumer_f, _, _, brokers, _) in app._consumers_store.items():
             mirror_f = mirror_consumer(
                 topic,
                 consumer_f,
-                brokers.json() if brokers is not None else app._kafka_brokers.json(),
+                brokers.model_dump_json()
+                if brokers is not None
+                else app._kafka_brokers.model_dump_json(),
                 app,
             )
             mirror_f = self.produces(  # type: ignore
                 topic=remove_suffix(topic),
                 brokers=brokers,
             )(mirror_f)
             self.mirrors[consumer_f] = mirror_f
             setattr(self, mirror_f.__name__, mirror_f)
         for topic, (producer_f, _, brokers, _) in app._producers_store.items():
             mirror_f = mirror_producer(
                 topic,
                 producer_f,
-                brokers.json() if brokers is not None else app._kafka_brokers.json(),
+                brokers.model_dump_json()
+                if brokers is not None
+                else app._kafka_brokers.model_dump_json(),
                 app,
             )
             mirror_f = self.consumes(
                 topic=remove_suffix(topic),
                 brokers=brokers,
             )(
                 mirror_f  # type: ignore
@@ -334,17 +336,17 @@
             mirror_f = self.mirrors[consumer_f]
             self.mirrors[getattr(app, consumer_f.__name__)] = mirror_f
             set_sugar(
                 tester=self,
                 prefix="to_",
                 topic_brokers=topic_brokers,
                 topic=remove_suffix(topic),
-                brokers=brokers.json()
+                brokers=brokers.model_dump_json()
                 if brokers is not None
-                else app._kafka_brokers.json(),
+                else app._kafka_brokers.model_dump_json(),
                 origin_function_name=consumer_f.__name__,
                 function=mirror_f,
             )
 
             mocks[f"to_{remove_suffix(topic)}"] = getattr(self.mocks, mirror_f.__name__)
             awaited_mocks[f"to_{remove_suffix(topic)}"] = getattr(
                 self.awaited_mocks, mirror_f.__name__
@@ -356,17 +358,17 @@
                 self.awaited_mocks, mirror_f.__name__
             )
             set_sugar(
                 tester=self,
                 prefix="on_",
                 topic_brokers=topic_brokers,
                 topic=remove_suffix(topic),
-                brokers=brokers.json()
+                brokers=brokers.model_dump_json()
                 if brokers is not None
-                else app._kafka_brokers.json(),
+                else app._kafka_brokers.model_dump_json(),
                 origin_function_name=producer_f.__name__,
                 function=getattr(self.awaited_mocks, mirror_f.__name__),
             )
             mocks[f"on_{remove_suffix(topic)}"] = getattr(self.mocks, mirror_f.__name__)
             awaited_mocks[f"on_{remove_suffix(topic)}"] = getattr(
                 self.awaited_mocks, mirror_f.__name__
             )
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_cli.py` & `fastkafka-0.8.0rc1/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_cli_docs.py` & `fastkafka-0.8.0rc1/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_cli_testing.py` & `fastkafka-0.8.0rc1/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/_subprocess.py` & `fastkafka-0.8.0rc1/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.8.0rc1/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from asyncio import iscoroutinefunction, Task  # do not use the version from inspect
 from typing import *
 from dataclasses import dataclass
 
 import asyncer
 from aiokafka.structs import ConsumerRecord
 from pydantic import BaseModel
-from pydantic.main import ModelMetaclass
 
 import fastkafka._aiokafka_imports
 from .logger import get_logger
 from .meta import delegates, export
 from .task_streaming import get_executor, StreamExecutor
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 5
@@ -139,23 +138,23 @@
     return _callback_parameters_wrapper(async_callback)
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 24
 def _get_single_msg_handlers(  # type: ignore
     *,
     consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     callback: AsyncConsumeMeta,
-    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    decoder_fn: Callable[[bytes, Type[BaseModel]], Any],
     msg_type: Type[BaseModel],
     **kwargs: Any,
 ) -> Tuple[
     Callable[
         [
             ConsumerRecord,
             AsyncConsumeMeta,
-            Callable[[bytes, ModelMetaclass], Any],
+            Callable[[bytes, Type[BaseModel]], Any],
             Type[BaseModel],
         ],
         Awaitable[None],
     ],
     Callable[
         [fastkafka._aiokafka_imports.AIOKafkaConsumer, Any],
         Awaitable[List[ConsumerRecord]],
@@ -174,15 +173,15 @@
     Returns:
         The handle_msg function and poll_consumer function.
     """
 
     async def handle_msg(  # type: ignore
         record: ConsumerRecord,
         callback: AsyncConsumeMeta = callback,
-        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
+        decoder_fn: Callable[[bytes, Type[BaseModel]], Any] = decoder_fn,
         msg_type: Type[BaseModel] = msg_type,
     ) -> None:
         await callback(
             decoder_fn(record.value, msg_type),
             EventMetadata.create_event_metadata(record),
         )
 
@@ -196,23 +195,23 @@
     return handle_msg, poll_consumer
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 26
 def _get_batch_msg_handlers(  # type: ignore
     *,
     consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     callback: AsyncConsumeMeta,
-    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    decoder_fn: Callable[[bytes, Type[BaseModel]], Any],
     msg_type: Type[BaseModel],
     **kwargs: Any,
 ) -> Tuple[
     Callable[
         [
             List[ConsumerRecord],
             AsyncConsumeMeta,
-            Callable[[bytes, ModelMetaclass], Any],
+            Callable[[bytes, Type[BaseModel]], Any],
             Type[BaseModel],
         ],
         Awaitable[None],
     ],
     Callable[
         [fastkafka._aiokafka_imports.AIOKafkaConsumer, Any],
         Awaitable[List[List[ConsumerRecord]]],
@@ -231,15 +230,15 @@
     Returns:
         The handle_msg function and poll_consumer function.
     """
 
     async def handle_msg(  # type: ignore
         records: List[ConsumerRecord],
         callback: AsyncConsumeMeta = callback,
-        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
+        decoder_fn: Callable[[bytes, Type[BaseModel]], Any] = decoder_fn,
         msg_type: Type[BaseModel] = msg_type,
     ) -> None:
         await callback(
             [decoder_fn(record.value, msg_type) for record in records],
             [EventMetadata.create_event_metadata(record) for record in records],
         )
 
@@ -254,15 +253,15 @@
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 28
 @delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer.getmany)
 async def _aiokafka_consumer_loop(  # type: ignore
     consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     *,
     topic: str,
-    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    decoder_fn: Callable[[bytes, Type[BaseModel]], Any],
     callback: ConsumeCallable,
     max_buffer_size: int = 100_000,
     msg_type: Union[Type[List[BaseModel]], Type[BaseModel]],
     is_shutting_down_f: Callable[[], bool],
     executor: Union[str, StreamExecutor, None] = None,
     **kwargs: Any,
 ) -> None:
@@ -311,15 +310,15 @@
     return {k: "*" * len(v) if "pass" in k.lower() else v for k, v in kwargs.items()}
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 37
 @delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer)
 @delegates(_aiokafka_consumer_loop, keep=True)
 async def aiokafka_consumer_loop(
     topic: str,
-    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
+    decoder_fn: Callable[[bytes, Type[BaseModel]], Any],
     *,
     timeout_ms: int = 100,
     max_buffer_size: int = 100_000,
     callback: ConsumeCallable,
     msg_type: Union[Type[List[BaseModel]], Type[BaseModel]],
     is_shutting_down_f: Callable[[], bool],
     executor: Union[str, StreamExecutor, None] = None,
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/asyncapi.py` & `fastkafka-0.8.0rc1/fastkafka/_components/asyncapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 import subprocess  # nosec: B404: Consider possible security implications associated with the subprocess module.
 import tempfile
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import *
 
-from pydantic import BaseModel, Field, HttpUrl
-from pydantic.json import timedelta_isoformat
-from pydantic.schema import schema
+from pydantic import ConfigDict, BaseModel, Field, HttpUrl, model_serializer
+from pydantic.type_adapter import TypeAdapter
 
 from .aiokafka_consumer_loop import ConsumeCallable
 from .docs_dependencies import _check_npm_with_local
 from .helpers import unwrap_list_type
 from .logger import get_logger
 from fastkafka._components.producer_decorator import (
     ProduceCallable,
@@ -29,20 +28,16 @@
 )
 
 # %% ../../nbs/014_AsyncAPI.ipynb 3
 logger = get_logger(__name__)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 5
 class KafkaMessage(BaseModel):
-    class Config:
-        """This class is used for specific JSON encoders, in our case to properly format timedelta in ISO format."""
-
-        json_encoders = {
-            timedelta: timedelta_isoformat,
-        }
+    # This following config is used to properly format timedelta in ISO 8601 format
+    model_config = ConfigDict(ser_json_timedelta="iso8601")
 
 # %% ../../nbs/014_AsyncAPI.ipynb 7
 class SecurityType(str, Enum):
     plain = "plain"
     userPassword = "userPassword"
     apiKey = "apiKey"
     X509 = "X509"
@@ -80,53 +75,55 @@
 
     def __init__(self, **kwargs: Any):
         for k, v in sec_scheme_name_mapping.items():
             if v in kwargs:
                 kwargs[k] = kwargs.pop(v)
         super().__init__(**kwargs)
 
-    def dict(self, *args: Any, **kwarg: Any) -> Dict[str, Any]:
+    def model_dump(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Renames internal names of members ('security_type' -> 'type', 'api_key_loc' -> 'in')"""
-        d = super().dict(*args, **kwarg)
+        d = super().model_dump(*args, **kwargs)
 
         for k, v in sec_scheme_name_mapping.items():
             d[v] = d.pop(k)
 
         # removes None values
         d = {k: v for k, v in d.items() if v is not None}
 
         return d
 
-    def json(self, *args: Any, **kwargs: Any) -> str:
-        """Serialize into JSON using dict()"""
-        return json.dumps(self.dict(), *args, **kwargs)
+    def model_dump_json(self, *args: Any, **kwargs: Any) -> str:
+        """Serialize into JSON using model_dump()"""
+        return json.dumps(self.model_dump(), *args, **kwargs)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 9
 class KafkaBroker(BaseModel):
     """Kafka broker"""
 
     url: str = Field(..., example="localhost")
     description: str = Field("Kafka broker")
-    port: str = Field("9092")
+    port: Union[str, int] = Field("9092")
     protocol: str = Field("kafka")
     security: Optional[SecuritySchema] = None
 
-    def dict(self, *args: Any, **kwarg: Any) -> Dict[str, Any]:
+    def model_dump(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Makes port a variable and remove it from the dictionary"""
-        d = super().dict(*args, **kwarg)
-        d["variables"] = {"port": {"default": self.port}}
+        d = super().model_dump(*args, **kwargs)
+        if self.security:
+            d["security"] = self.security.model_dump(*args, **kwargs)
+        d["variables"] = {"port": {"default": str(self.port)}}
         d.pop("port")
 
         d = {k: v for k, v in d.items() if v is not None}
 
         return d
 
-    def json(self, *args: Any, **kwargs: Any) -> str:
+    def model_dump_json(self, *args: Any, **kwargs: Any) -> str:
         """Serialize into JSON using dict()"""
-        return json.dumps(self.dict(), *args, **kwargs)
+        return json.dumps(self.model_dump(), *args, **kwargs)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 12
 class ContactInfo(BaseModel):
     name: str = Field(..., example="My company")
     url: HttpUrl = Field(..., example="https://www.github.com/mycompany")
     email: str = Field(..., example="noreply@mycompany.com")
 
@@ -139,34 +136,37 @@
         ...,
     )
 
 # %% ../../nbs/014_AsyncAPI.ipynb 14
 class KafkaBrokers(BaseModel):
     brokers: Dict[str, Union[List[KafkaBroker], KafkaBroker]]
 
-    def dict(self, *args: Any, **kwarg: Any) -> Dict[str, Any]:
+    def model_dump(self, *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Transcribe brokers into bootstrap server groups"""
-        d = super().dict(*args, **kwarg)
+        d = super().model_dump(*args, **kwargs)
 
         brokers = {}
         for k, v in self.brokers.items():
             if isinstance(v, list):
                 brokers.update(
-                    {f"{k}-bootstrap-server-{i}": u_v.dict() for i, u_v in enumerate(v)}
+                    {
+                        f"{k}-bootstrap-server-{i}": u_v.model_dump()
+                        for i, u_v in enumerate(v)
+                    }
                 )
             else:
-                brokers.update({f"{k}": v.dict()})
+                brokers.update({f"{k}": v.model_dump()})
         d["brokers"] = brokers
         d = {k: v for k, v in d.items() if v is not None}
 
         return d
 
-    def json(self, *args: Any, **kwargs: Any) -> str:
+    def model_dump_json(self, *args: Any, **kwargs: Any) -> str:
         """Serialize into JSON using dict()"""
-        return json.dumps(self.dict(), *args, **kwargs)
+        return json.dumps(self.model_dump(), *args, **kwargs)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 17
 # T = TypeVar("T")
 
 
 def _get_msg_cls_for_producer(f: ProduceCallable) -> Type[Any]:
     types = get_type_hints(f)
@@ -257,57 +257,58 @@
     return set(fc + fp)
 
 
 def _get_kafka_msg_definitions(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Any]]:
-    return schema(_get_kafka_msg_classes(consumers, producers))  # type: ignore
+    msg_classes = _get_kafka_msg_classes(consumers, producers)
+    _, msg_definitions = TypeAdapter.json_schemas(
+        [(msg_cls, "validation", TypeAdapter(msg_cls)) for msg_cls in msg_classes]
+    )
+    return msg_definitions
 
 # %% ../../nbs/014_AsyncAPI.ipynb 35
 def _get_example(cls: Type[BaseModel]) -> BaseModel:
     kwargs: Dict[str, Any] = {}
-    for k, v in cls.__fields__.items():
+    for k, v in cls.model_fields.items():
         #         try:
-        if (
-            hasattr(v, "field_info")
-            and hasattr(v.field_info, "extra")
-            and "example" in v.field_info.extra
-        ):
-            example = v.field_info.extra["example"]
+        if hasattr(v, "json_schema_extra") and "example" in v.json_schema_extra:  # type: ignore
+            example = v.json_schema_extra["example"]  # type: ignore
             kwargs[k] = example
     #         except:
     #             pass
-
-    return json.loads(cls(**kwargs).json())  # type: ignore
+    return json.loads(cls(**kwargs).model_dump_json())  # type: ignore
 
 # %% ../../nbs/014_AsyncAPI.ipynb 37
 def _add_example_to_msg_definitions(
     msg_cls: Type[BaseModel], msg_schema: Dict[str, Dict[str, Any]]
 ) -> None:
     try:
         example = _get_example(msg_cls)
     except Exception as e:
         example = None
     if example is not None:
-        msg_schema["definitions"][msg_cls.__name__]["example"] = example
+        msg_schema["$defs"][msg_cls.__name__]["example"] = example
 
 
 def _get_msg_definitions_with_examples(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Any]]:
     msg_classes = _get_kafka_msg_classes(consumers, producers)
-    msg_schema: Dict[str : Dict[str, Any]] = schema(msg_classes)  # type: ignore
+    msg_schema: Dict[str, Dict[str, Any]]
+    _, msg_schema = TypeAdapter.json_schemas(
+        [(msg_cls, "validation", TypeAdapter(msg_cls)) for msg_cls in msg_classes]
+    )
     for msg_cls in msg_classes:
         _add_example_to_msg_definitions(msg_cls, msg_schema)
-
     msg_schema = (
-        {k: {"payload": v} for k, v in msg_schema["definitions"].items()}
-        if "definitions" in msg_schema
+        {k: {"payload": v} for k, v in msg_schema["$defs"].items()}
+        if "$defs" in msg_schema
         else {}
     )
 
     return msg_schema
 
 # %% ../../nbs/014_AsyncAPI.ipynb 39
 def _get_security_schemes(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
@@ -316,15 +317,15 @@
         if isinstance(broker, list):
             kafka_broker = broker[0]
         else:
             kafka_broker = broker
 
         if kafka_broker.security is not None:
             security_schemes[f"{key}_default_security"] = json.loads(
-                kafka_broker.security.json()
+                kafka_broker.security.model_dump_json()
             )
     return security_schemes
 
 # %% ../../nbs/014_AsyncAPI.ipynb 41
 def _get_components_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
@@ -334,15 +335,15 @@
     msg_classes = [cls.__name__ for cls in _get_kafka_msg_classes(consumers, producers)]
     components = {
         "messages": {k: v for k, v in definitions.items() if k in msg_classes},
         "schemas": {k: v for k, v in definitions.items() if k not in msg_classes},
         "securitySchemes": _get_security_schemes(kafka_brokers),
     }
     substitutions = {
-        f"#/definitions/{k}": f"#/components/messages/{k}"
+        f"#/$defs/{k}": f"#/components/messages/{k}"
         if k in msg_classes
         else f"#/components/schemas/{k}"
         for k in definitions.keys()
     }
 
     def _sub_values(d: Any, substitutions: Dict[str, str] = substitutions) -> Any:
         if isinstance(d, dict):
@@ -355,30 +356,30 @@
                     d = v
         return d
 
     return _sub_values(components)  # type: ignore
 
 # %% ../../nbs/014_AsyncAPI.ipynb 43
 def _get_servers_schema(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
-    servers = json.loads(kafka_brokers.json(sort_keys=False))["brokers"]
+    servers = json.loads(kafka_brokers.model_dump_json(sort_keys=False))["brokers"]
 
     for key, kafka_broker in servers.items():
         if "security" in kafka_broker:
             servers[key]["security"] = [{f"{key}_default_security": []}]
     return servers  # type: ignore
 
 # %% ../../nbs/014_AsyncAPI.ipynb 45
 def _get_asyncapi_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
 ) -> Dict[str, Any]:
     #     # we don't use dict because we need custom JSON encoders
-    info = json.loads(kafka_service_info.json(sort_keys=False))
+    info = json.loads(kafka_service_info.model_dump_json())
     servers = _get_servers_schema(kafka_brokers)
     #     # should be in the proper format already
     channels = _get_channels_schema(consumers, producers)
     components = _get_components_schema(consumers, producers, kafka_brokers)
     return {
         "asyncapi": "2.5.0",
         "info": info,
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/benchmarking.py` & `fastkafka-0.8.0rc1/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.8.0rc1/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.8.0rc1/fastkafka/_components/encoder/avro.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,67 +6,93 @@
 # %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 1
 import io
 import json
 from typing import *
 
 import fastavro
 from pydantic import BaseModel, create_model
-from pydantic.main import ModelMetaclass
 
 from ..logger import get_logger
 from ..meta import export
 
 # %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 7
 @export("fastkafka.encoder")
 class AvroBase(BaseModel):
     """This is base pydantic class that will add some methods"""
 
     @classmethod
-    def avro_schema_for_pydantic(
+    def avro_schema_for_pydantic_object(
         cls,
-        pydantic_model: Union[BaseModel, ModelMetaclass],
+        pydantic_model: BaseModel,
         by_alias: bool = True,
         namespace: Optional[str] = None,
     ) -> Dict[str, Any]:
         """
-        Return the avro schema for the pydantic class
+        Returns the Avro schema for the given Pydantic object.
 
-        :param by_alias: generate the schemas using the aliases defined, if any
-        :param namespace: Provide an optional namespace string to use in schema generation
-        :return: dict with the Avro Schema for the model
+        Args:
+            pydantic_model (BaseModel): The Pydantic object.
+            by_alias (bool, optional): Generate schemas using aliases defined. Defaults to True.
+            namespace (Optional[str], optional): Optional namespace string for schema generation.
+
+        Returns:
+            Dict[str, Any]: The Avro schema for the model.
         """
 
-        if isinstance(pydantic_model, BaseModel):
-            schema = pydantic_model.__class__.schema(by_alias=by_alias)
-        elif isinstance(pydantic_model, ModelMetaclass):
-            schema = pydantic_model.schema(by_alias=by_alias)
-        else:
-            raise ValueError(
-                f"Unknown type {type(pydantic_model)} given for pydantic_model parameter"
-            )
+        schema = pydantic_model.__class__.model_json_schema(by_alias=by_alias)
+
+        if namespace is None:
+            # default namespace will be based on title
+            namespace = schema["title"]
+
+        return cls._avro_schema(schema, namespace)
+
+    @classmethod
+    def avro_schema_for_pydantic_class(
+        cls,
+        pydantic_model: Type[BaseModel],
+        by_alias: bool = True,
+        namespace: Optional[str] = None,
+    ) -> Dict[str, Any]:
+        """
+        Returns the Avro schema for the given Pydantic class.
+
+        Args:
+            pydantic_model (Type[BaseModel]): The Pydantic class.
+            by_alias (bool, optional): Generate schemas using aliases defined. Defaults to True.
+            namespace (Optional[str], optional): Optional namespace string for schema generation.
+
+        Returns:
+            Dict[str, Any]: The Avro schema for the model.
+        """
+
+        schema = pydantic_model.model_json_schema(by_alias=by_alias)
 
         if namespace is None:
             # default namespace will be based on title
             namespace = schema["title"]
 
         return cls._avro_schema(schema, namespace)
 
     @classmethod
     def avro_schema(
         cls, by_alias: bool = True, namespace: Optional[str] = None
     ) -> Dict[str, Any]:
         """
-        Return the avro schema for the pydantic class
+        Returns the Avro schema for the Pydantic class.
+
+        Args:
+            by_alias (bool, optional): Generate schemas using aliases defined. Defaults to True.
+            namespace (Optional[str], optional): Optional namespace string for schema generation.
 
-        :param by_alias: generate the schemas using the aliases defined, if any
-        :param namespace: Provide an optional namespace string to use in schema generation
-        :return: dict with the Avro Schema for the model
+        Returns:
+            Dict[str, Any]: The Avro schema for the model.
         """
         schema = cls.schema(by_alias=by_alias)
 
         if namespace is None:
             # default namespace will be based on title
             namespace = schema["title"]
 
@@ -180,14 +206,18 @@
 
         def get_fields(s: Dict[str, Any]) -> List[Dict[str, Any]]:
             """Return a list of fields of a struct"""
             fields = []
 
             required = s.get("required", [])
             for key, value in s.get("properties", {}).items():
+                if "type" not in value and "anyOf" in value:
+                    any_of_types = value.pop("anyOf")
+                    types = [x["type"] for x in any_of_types if x["type"] != "null"]
+                    value["type"] = types[0]
                 avro_type_dict = get_type(value)
                 avro_type_dict["name"] = key
 
                 if key not in required:
                     if avro_type_dict.get("default") is None:
                         avro_type_dict["type"] = ["null", avro_type_dict["type"]]
                         avro_type_dict["default"] = None
@@ -212,43 +242,49 @@
 
     Args:
         msg: An instance of pydantic basemodel
 
     Returns:
         A bytes message which is encoded from pydantic basemodel
     """
-    schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic(msg))
+    schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic_object(msg))
     bytes_writer = io.BytesIO()
-    fastavro.schemaless_writer(bytes_writer, schema, msg.dict())
+
+    d = msg.model_dump()
+    for k, v in d.items():
+        if "pydantic_core" in str(type(v)):
+            d[k] = str(v)
+
+    fastavro.schemaless_writer(bytes_writer, schema, d)
     raw_bytes = bytes_writer.getvalue()
     return raw_bytes
 
 # %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 13
 @export("fastkafka.encoder")
-def avro_decoder(raw_msg: bytes, cls: ModelMetaclass) -> Any:
+def avro_decoder(raw_msg: bytes, cls: Type[BaseModel]) -> Any:
     """
     Decoder to decode avro encoded messages to pydantic model instance
 
     Args:
         raw_msg: Avro encoded bytes message received from Kafka topic
         cls: Pydantic class; This pydantic class will be used to construct instance of same class
 
     Returns:
         An instance of given pydantic class
     """
-    schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic(cls))
+    schema = fastavro.schema.parse_schema(AvroBase.avro_schema_for_pydantic_class(cls))
 
     bytes_reader = io.BytesIO(raw_msg)
     msg_dict = fastavro.schemaless_reader(bytes_reader, schema)
 
     return cls(**msg_dict)
 
 # %% ../../../nbs/018_Avro_Encode_Decoder.ipynb 16
 @export("fastkafka.encoder")
-def avsc_to_pydantic(schema: Dict[str, Any]) -> ModelMetaclass:
+def avsc_to_pydantic(schema: Dict[str, Any]) -> Type[BaseModel]:
     """
     Generate pydantic model from given Avro Schema
 
     Args:
         schema: Avro schema in dictionary format
 
     Returns:
@@ -328,15 +364,15 @@
                 f"please report this at https://github.com/godatadriven/pydantic-avro/issues"
             )
         if optional:
             return f"Optional[{py_type}]"
         else:
             return py_type
 
-    def record_type_to_pydantic(schema: Dict[str, Any]) -> ModelMetaclass:
+    def record_type_to_pydantic(schema: Dict[str, Any]) -> Type[BaseModel]:
         """Convert a single avro record type to a pydantic class"""
         name = (
             schema["name"]
             if "." not in schema["name"]
             else schema["name"].split(".")[-1]
         )
         current = f"class {schema['name']}(BaseModel):\n"
@@ -357,11 +393,11 @@
                 kwargs[n] = (t, default)
                 current += f"    {n}: {t} = {default}\n"
             else:
                 kwargs[n] = (t, default)
                 current += f"    {n}: {t} = {json.dumps(default)}\n"
 
         classes[name] = current
-        pydantic_model = create_model(name, **kwargs)  # type: ignore
+        pydantic_model = create_model(name, __module__=__name__, **kwargs)  # type: ignore
         return pydantic_model  # type: ignore
 
     return record_type_to_pydantic(schema)
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/encoder/json.py` & `fastkafka-0.8.0rc1/fastkafka/_components/encoder/json.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 __all__ = ['logger', 'json_encoder', 'json_decoder']
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 1
 import json
 from typing import *
 
 from pydantic import BaseModel
-from pydantic.main import ModelMetaclass
 
 from ..logger import get_logger
 from ..meta import export
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 6
 def _to_json_utf8(o: Any) -> bytes:
     """Converts to JSON and then encodes with UTF-8"""
-    if hasattr(o, "json"):
-        return o.json().encode("utf-8")  # type: ignore
+    if hasattr(o, "model_dump_json"):
+        return o.model_dump_json().encode("utf-8")  # type: ignore
     else:
         return json.dumps(o).encode("utf-8")
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 9
 @export("fastkafka.encoder")
 def json_encoder(msg: BaseModel) -> bytes:
     """
@@ -36,15 +35,15 @@
     Returns:
         Json string in bytes which is encoded from pydantic basemodel
     """
     return _to_json_utf8(msg)
 
 # %% ../../../nbs/019_Json_Encode_Decoder.ipynb 11
 @export("fastkafka.encoder")
-def json_decoder(raw_msg: bytes, cls: ModelMetaclass) -> Any:
+def json_decoder(raw_msg: bytes, cls: Type[BaseModel]) -> Any:
     """
     Decoder to decode json string in bytes to pydantic model instance
 
     Args:
         raw_msg: Bytes message received from Kafka topic
         cls: Pydantic class; This pydantic class will be used to construct instance of same class
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/helpers.py` & `fastkafka-0.8.0rc1/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/logger.py` & `fastkafka-0.8.0rc1/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/meta.py` & `fastkafka-0.8.0rc1/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/producer_decorator.py` & `fastkafka-0.8.0rc1/fastkafka/_components/producer_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/013_ProducerDecorator.ipynb.
 
 # %% auto 0
-__all__ = ['BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'unwrap_from_kafka_event', 'release_callback',
-           'produce_single', 'send_batch', 'produce_batch', 'producer_decorator']
+__all__ = ['logger', 'BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'unwrap_from_kafka_event',
+           'release_callback', 'produce_single', 'send_batch', 'produce_batch', 'producer_decorator']
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 1
 import asyncio
 import functools
 import random
 import time
 from asyncio import iscoroutinefunction  # do not use the version from inspect
 from dataclasses import dataclass
 from inspect import Parameter
 from typing import *
 
+from aiokafka import AIOKafkaProducer
+from aiokafka.errors import KafkaTimeoutError
 from aiokafka.producer.message_accumulator import BatchBuilder
 from pydantic import BaseModel
 
-from .._aiokafka_imports import AIOKafkaProducer
+from .logger import get_logger
 from .meta import export
 from .helpers import remove_suffix
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 3
+logger = get_logger(__name__)
+
+# %% ../../nbs/013_ProducerDecorator.ipynb 5
 BaseSubmodel = TypeVar("BaseSubmodel", bound=Union[List[BaseModel], BaseModel])
 BaseSubmodel
 
 
 @dataclass
 @export("fastkafka")
 class KafkaEvent(Generic[BaseSubmodel]):
@@ -36,15 +41,15 @@
         message (BaseSubmodel): The message contained in the Kafka event, can be of type pydantic.BaseModel.
         key (bytes, optional): The optional key used to identify the Kafka event.
     """
 
     message: BaseSubmodel
     key: Optional[bytes] = None
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 5
+# %% ../../nbs/013_ProducerDecorator.ipynb 7
 def unwrap_from_kafka_event(var_type: Union[Type, Parameter]) -> Union[Type, Parameter]:
     """
     Unwraps the type from a KafkaEvent.
 
     Args:
         var_type: Type to unwrap.
 
@@ -58,58 +63,63 @@
           Output: int
     """
     if hasattr(var_type, "__origin__") and var_type.__origin__ == KafkaEvent:
         return var_type.__args__[0]  # type: ignore
     else:
         return var_type
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 7
+# %% ../../nbs/013_ProducerDecorator.ipynb 9
 ProduceReturnTypes = Union[
     BaseModel, KafkaEvent[BaseModel], List[BaseModel], KafkaEvent[List[BaseModel]]
 ]
 
 ProduceCallable = Union[
     Callable[..., ProduceReturnTypes], Callable[..., Awaitable[ProduceReturnTypes]]
 ]
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 10
+# %% ../../nbs/013_ProducerDecorator.ipynb 12
 def _wrap_in_event(
     message: Union[BaseModel, List[BaseModel], KafkaEvent]
 ) -> KafkaEvent:
     return message if type(message) == KafkaEvent else KafkaEvent(message)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 13
+# %% ../../nbs/013_ProducerDecorator.ipynb 15
 def release_callback(fut: asyncio.Future) -> None:
     pass
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 14
+# %% ../../nbs/013_ProducerDecorator.ipynb 16
 async def produce_single(  # type: ignore
     producer: AIOKafkaProducer,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
     wrapped_val: KafkaEvent[BaseModel],
-) -> ProduceReturnTypes:
+) -> None:
     """
     Sends a single message to the Kafka producer.
 
     Args:
         producer (AIOKafkaProducer): The Kafka producer object.
         topic (str): The topic to which the message will be sent.
         encoder_fn (Callable[[BaseModel], bytes]): The encoding function to encode the message.
         wrapped_val (KafkaEvent[BaseModel]): The wrapped Kafka event containing the message.
-
-    Returns:
-        ProduceReturnTypes: The return value from the decorated function.
     """
-    fut = await producer.send(
-        topic, encoder_fn(wrapped_val.message), key=wrapped_val.key
-    )
-    fut.add_done_callback(release_callback)
+    while True:
+        try:
+            fut = await producer.send(
+                topic, encoder_fn(wrapped_val.message), key=wrapped_val.key
+            )
+            fut.add_done_callback(release_callback)
+            break
+        except KafkaTimeoutError as e:
+            logger.warning(
+                f"produce_single(): Exception {e} raised when producing {wrapped_val.message} to {topic=}, sleeping for 1 second and retrying.."
+            )
+            await asyncio.sleep(1)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 16
+# %% ../../nbs/013_ProducerDecorator.ipynb 20
 async def send_batch(  # type: ignore
     producer: AIOKafkaProducer, topic: str, batch: BatchBuilder, key: Optional[bytes]
 ) -> None:
     """
     Sends a batch of messages to the Kafka producer.
 
     Args:
@@ -122,15 +132,23 @@
         None
     """
     partitions = await producer.partitions_for(topic)
     if key == None:
         partition = random.choice(tuple(partitions))  # nosec
     else:
         partition = producer._partition(topic, None, None, None, key, None)
-    await producer.send_batch(batch, topic, partition=partition)
+    while True:
+        try:
+            await producer.send_batch(batch, topic, partition=partition)
+            break
+        except KafkaTimeoutError as e:
+            logger.warning(
+                f"send_batch(): Exception {e} raised when producing {batch} to {topic=}, sleeping for 1 second and retrying.."
+            )
+            await asyncio.sleep(1)
 
 
 async def produce_batch(  # type: ignore
     producer: AIOKafkaProducer,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
     wrapped_val: KafkaEvent[List[BaseModel]],
@@ -162,15 +180,15 @@
             batch = producer.create_batch()
             batch.append(
                 key=None, value=encoder_fn(message), timestamp=int(time.time() * 1000)
             )
 
     await send_batch(producer, topic, batch, wrapped_val.key)
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 18
+# %% ../../nbs/013_ProducerDecorator.ipynb 23
 def producer_decorator(
     producer_store: Dict[str, Any],
     func: ProduceCallable,
     topic_key: str,
     encoder_fn: Callable[[BaseModel], bytes],
 ) -> ProduceCallable:
     """
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/task_streaming.py` & `fastkafka-0.8.0rc1/fastkafka/_components/task_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,14 @@
         """
         Abstract method for running the stream executor.
 
         Args:
             is_shutting_down_f: Function to check if the executor is shutting down.
             generator: Generator function for retrieving consumer records.
             processor: Processor function for processing consumer records.
-
-        Returns:
-            None
         """
         pass
 
 # %% ../../nbs/006_TaskStreaming.ipynb 20
 def _process_items_task(  # type: ignore
     processor: Callable[[ConsumerRecord], Awaitable[None]], task_pool: TaskPool
 ) -> Callable[
@@ -249,17 +246,14 @@
         """
         Runs the dynamic task executor.
 
         Args:
             is_shutting_down_f: Function to check if the executor is shutting down.
             generator: Generator function for retrieving consumer records.
             processor: Processor function for processing consumer records.
-
-        Returns:
-            None
         """
         send_stream, receive_stream = anyio.create_memory_object_stream(
             max_buffer_size=self.max_buffer_size
         )
 
         async with self.exception_monitor, self.task_pool:
             async with anyio.create_task_group() as tg:
@@ -341,17 +335,14 @@
         """
         Runs the sequential executor.
 
         Args:
             is_shutting_down_f: Function to check if the executor is shutting down.
             generator: Generator function for retrieving consumer records.
             processor: Processor function for processing consumer records.
-
-        Returns:
-            None
         """
 
         send_stream, receive_stream = anyio.create_memory_object_stream(
             max_buffer_size=self.max_buffer_size
         )
 
         async with anyio.create_task_group() as tg:
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.8.0rc1/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.8.0rc1/fastkafka/_docusaurus_helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,264 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/096_Docusaurus_Helper.ipynb.
 
 # %% auto 0
 __all__ = ['CustomNbdevLookup', 'fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar',
-           'delete_unused_markdown_files_from_sidebar']
+           'delete_unused_markdown_files_from_sidebar', 'update_readme']
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 2
 import itertools
 import re
 import ast
 import types
 from inspect import (
     Signature,
     getmembers,
     isclass,
     isfunction,
     signature,
     ismethod,
     getsource,
+    Parameter,
 )
 from pathlib import Path
 from typing import *
 from urllib.parse import urljoin
 from functools import lru_cache
 
 import typer
 from docstring_parser import parse
-from docstring_parser.common import DocstringParam, DocstringRaises, DocstringReturns
+from docstring_parser.common import (
+    DocstringParam,
+    DocstringRaises,
+    DocstringReturns,
+    Docstring,
+)
 from nbdev.config import get_config
+from nbdev.quarto import nbdev_readme
 from nbdev.doclinks import NbdevLookup, patch_name, L, _find_mod
 from nbdev_mkdocs.mkdocs import (
     _add_all_submodules,
     _import_all_members,
     _import_functions_and_classes,
     _import_submodules,
 )
+from nbdev_mkdocs._helpers.doc_links_utils import (
+    fix_sym_links as update_default_symbol_links,
+)
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 4
-def _format_docstring_sections(
-    items: Union[List[DocstringParam], List[DocstringReturns], List[DocstringRaises]],
-    keyword: str,
+def _get_return_annotation(s: Signature) -> str:
+    """Get the return annotation from the function signature.
+
+    Args:
+        s: The signature of the function from which the annotations must be extracted.
+
+    Returns:
+        The return annotation, or an empty string if not available.
+
+    """
+    if s.return_annotation == None or "inspect._empty" in str(s.return_annotation):
+        return ""
+    if isinstance(s.return_annotation, str):
+        return s.return_annotation
+    ret_val: str = (
+        str(s.return_annotation).replace("typing.", "").replace("NoneType", "None")
+        if "typing." in str(s.return_annotation)
+        else str(s.return_annotation.__name__)
+    )
+    return ret_val
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 19
+def _get_param_annotation(param: Parameter) -> str:
+    """Get the annotation of a function parameter.
+
+    Args:
+        param: The parameter object.
+
+    Returns:
+        The parameter annotation, or an empty string if not available.
+
+    """
+
+    if "typing." in str(param.annotation):
+        return f'`{str(param.annotation).replace("typing.", "")}`'
+    elif isinstance(param.annotation, str):
+        return param.annotation
+    else:
+        return (
+            ""
+            if param.annotation.__name__ == "_empty"
+            else f"`{param.annotation.__name__}`"
+        )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 21
+def _get_default_value(param: Parameter) -> str:
+    """Get the default value of the function parameter.
+
+    Args:
+        param: The parameter object.
+
+    Returns:
+        The default value of the function parameter.
+
+    """
+    if param.default is param.empty:
+        return "*required*"
+
+    return (
+        f"`'{param.default}'`"
+        if isinstance(param.default, str)
+        else f"`{param.default}`"
+    )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 23
+def _get_params_annotation(s: Signature) -> Dict[str, Dict[str, str]]:
+    """Get the annotations along with its default values for the parameters of the symbol.
+
+    Args:
+        s: The signature of the function from which the annotations must be extracted.
+
+    Returns:
+        The parameter annotations along with its default value.
+    """
+    return {
+        f"{param.name}": {
+            "type": _get_param_annotation(param),
+            "default": _get_default_value(param),
+        }
+        for param in s.parameters.values()
+    }
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 25
+def _generate_parameters_table(
+    symbol_annotations: Dict[str, Union[Dict[str, str], str]],
+    section_items: Union[List[DocstringParam]],
+    section_name: str,
+) -> str:
+    """Generate parameter table in markdown format
+
+    Args:
+        symbol_annotations: Symbol annotations along with its default value
+        section_items: The parameter section of a parsed docstring
+        section_name: The name of the section
+
+    Returns:
+        The parameters of a symbol in markdown-formatted string
+    """
+    nl = "\n"
+    _section_template = (
+        "|  Name | Type | Description | Default |\n|---|---|---|---|\n{section_body}\n"
+    )
+    section_body = "".join(
+        [
+            f'| `{section.arg_name}` | {symbol_annotations["parameters"][section.arg_name]["type"]} | {section.description.replace(nl, "")} | {symbol_annotations["parameters"][section.arg_name]["default"]} |\n'  # type: ignore
+            if section.arg_name in symbol_annotations["parameters"]
+            else ""
+            for section in section_items
+        ]
+    )
+    return f"**{section_name}**:\n\n" + _section_template.format(
+        section_body=section_body,
+    )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 27
+def _generate_return_and_raises_table(
+    symbol_annotations: Dict[str, Union[Dict[str, str], str]],
+    section_items: Union[List[DocstringReturns], List[DocstringRaises]],
+    section_name: str,
 ) -> str:
-    """Format a list of docstring sections
+    """Generate return and raises table in markdown format
 
     Args:
-        items: A list of DocstringParam objects
-        keyword: The type of section to format (e.g. 'Parameters', 'Returns', 'Exceptions')
+        symbol_annotations: Symbol annotations along with its default value
+        section_items: The parameter section of a parsed docstring
+        section_name: The name of the section
 
     Returns:
-        The formatted docstring.
+        The return and raises section of a symbol in markdown-formatted string
     """
+    nl = "\n"
+    _section_template = "|  Type | Description |\n|---|---|\n{section_body}\n"
+    section_body = "".join(
+        [
+            f'| `{symbol_annotations["return"] if section_name == "Returns" else section.type_name}` | {section.description.replace(nl, "")} |\n'  # type: ignore
+            for section in section_items
+        ]
+    )
+    return f"**{section_name}**:\n\n" + _section_template.format(
+        section_body=section_body,
+    )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 30
+def _format_docstring_section_items(
+    symbol_annotations: Dict[str, Union[Dict[str, str], str]],
+    section_items: Union[
+        List[DocstringParam], List[DocstringReturns], List[DocstringRaises]
+    ],
+    section_name: str,
+) -> str:
+    """Format the docstring sections in a table format
+
+    Args:
+        symbol_annotations: Symbol annotations along with its default value
+        section_items: The parameter section of a parsed docstring
+        section_name: The name of the section
+
+    Returns:
+        The docstring sections of the symbol in markdown-formatted string
+    """
+    if section_name == "Parameters":
+        return _generate_parameters_table(symbol_annotations, section_items, section_name)  # type: ignore
+    else:
+        return _generate_return_and_raises_table(symbol_annotations, section_items, section_name)  # type: ignore
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 35
+def _get_annotation(symbol: Type) -> Dict[str, Union[Dict[str, Dict[str, str]], str]]:
+    """Get annotations along with its default value for a symbol
+
+    Args:
+        symbol: The symbol for which the annotations needs to be extracted
+
+    Returns:
+        The annotations dict along with its default value
+    """
+    symbol = symbol.fget if isinstance(symbol, property) else symbol
+    symbol_signature = signature(symbol)
+    params_dict = _get_params_annotation(symbol_signature)
+    return_annotation = _get_return_annotation(symbol_signature)
+    return {"parameters": params_dict, "return": return_annotation}
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 38
+def _format_docstring_sections(symbol: Type, parsed_docstring: Docstring) -> str:
+    """Format the parsed docstring sections into markdown-formatted table
+
+    Args:
+        symbol: The symbol for which to parse the docstring.
+        parsed_docstring: A Docstring object
+
+    Returns:
+        The markdown-formatted docstring.
+    """
+    symbol_annotations = _get_annotation(symbol)
     formatted_docstring = ""
-    if len(items) > 0:
-        formatted_docstring += f"**{keyword}**:\n"
-        for item in items:
-            if keyword == "Parameters":
-                formatted_docstring += f"- **{item.arg_name}**: {item.description}\n"  # type: ignore
-            elif keyword == "Exceptions":
-                formatted_docstring += f"- **{item.type_name}**: {item.description}\n"
-            else:
-                formatted_docstring += f"- {item.description}\n"
-        formatted_docstring = f"{formatted_docstring}\n"
+    sections = [
+        ("Parameters", parsed_docstring.params),
+        ("Returns", parsed_docstring.many_returns),
+        ("Exceptions", parsed_docstring.raises),
+    ]
+
+    for section_name, section_items in sections:
+        if len(section_items) > 0:  # type: ignore
+            formatted_docstring += _format_docstring_section_items(
+                symbol_annotations, section_items, section_name  # type: ignore
+            )
+
     return formatted_docstring
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 8
+# %% ../nbs/096_Docusaurus_Helper.ipynb 40
 def _format_free_links(s: str) -> str:
     """Format free links in a given string by adding proper spacing around them.
 
     Args:
         s: The input string containing free links.
 
     Returns:
@@ -74,46 +266,37 @@
     """
     pattern = r"([\"'])(https?:\/\/[^\s]+)([\"'])"
     ret_val = re.sub(
         pattern, lambda match: f"{match.group(1)} {match.group(2)} {match.group(3)}", s
     )
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 10
-def _docstring_to_markdown(docstring: str) -> str:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 42
+def _docstring_to_markdown(symbol: Type) -> str:
     """Converts a docstring to a markdown-formatted string.
 
     Args:
-        docstring: The docstring to convert.
+        symbol: The symbol for which the documentation needs to be generated in markdown format.
 
     Returns:
         The markdown-formatted docstring.
     """
-    parsed_docstring = parse(docstring)
+    parsed_docstring = parse(symbol.__doc__)  # type: ignore
     formatted_docstring = f"{parsed_docstring.short_description}\n\n"
     formatted_docstring += (
         f"{parsed_docstring.long_description}\n\n"
         if parsed_docstring.long_description
         else ""
     )
-    formatted_docstring += _format_docstring_sections(
-        parsed_docstring.params, "Parameters"
-    )
-    formatted_docstring += _format_docstring_sections(
-        parsed_docstring.many_returns, "Returns"
-    )
-    formatted_docstring += _format_docstring_sections(
-        parsed_docstring.raises, "Exceptions"
-    )
-
+    formatted_docstring += _format_docstring_sections(symbol, parsed_docstring)
     ret_val = _format_free_links(formatted_docstring)
 
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 14
+# %% ../nbs/096_Docusaurus_Helper.ipynb 46
 def _get_submodules(module_name: str) -> List[str]:
     """Get a list of all submodules contained within the module.
 
     Args:
         module_name: The name of the module to retrieve submodules from
 
     Returns:
@@ -122,39 +305,39 @@
     members = _import_all_members(module_name)
     members_with_submodules = _add_all_submodules(members)
     members_with_submodules_str: List[str] = [
         x[:-1] if x.endswith(".") else x for x in members_with_submodules
     ]
     return members_with_submodules_str
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 16
+# %% ../nbs/096_Docusaurus_Helper.ipynb 48
 def _load_submodules(
     module_name: str, members_with_submodules: List[str]
-) -> List[Union[types.FunctionType, Type[Any]]]:
+) -> List[Type]:
     """Load the given submodules from the module.
 
     Args:
         module_name: The name of the module whose submodules to load
         members_with_submodules: A list of submodule names to load
 
     Returns:
         A list of imported submodule objects.
     """
     submodules = _import_submodules(module_name)
-    members: List[Tuple[str, Union[types.FunctionType, Type[Any]]]] = list(
+    members: List[Tuple[str, Type]] = list(
         itertools.chain(*[_import_functions_and_classes(m) for m in submodules])
     )
     names = [
         y
         for x, y in members
         if f"{y.__module__}.{y.__name__}" in members_with_submodules
     ]
     return names
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 18
+# %% ../nbs/096_Docusaurus_Helper.ipynb 50
 def _get_parameters(_signature: Signature) -> List[str]:
     """Convert a function's signature into a string representation of its parameter list.
 
     Args:
         _signature: The signature object representing the function's signature.
 
     Returns:
@@ -167,36 +350,35 @@
         else f"{param.name}='{param.default}'"
         if isinstance(param.default, str)
         else f"{param.name}={param.default}"
         for param in params
     ]
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 22
-def _format_symbol_definition(
-    symbol: Union[types.FunctionType, Type[Any]], params_list: List[str]
-) -> str:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 54
+def _format_symbol_definition(symbol: Type, params_list: List[str]) -> str:
     """Format the given symbol parameters by adding a new line and indentation.
 
     Args:
+        symbol: The symbol for which the symbol definition needs to be formatted.
         params_list: A string representation of the parameter list.
 
     Returns:
         A formatted string representation of the parameters with new lines and indentation.
     """
     parameters = ", ".join(params_list)
     if parameters == "":
         return f"{symbol.__name__}()\n"
     elif len(f"{symbol.__name__}({parameters})") <= 79:
         return f"{symbol.__name__}(\n    {parameters}\n)\n"
     else:
         formatted_parameters = "".join([f"\n    {param}," for param in params_list])
         return f"{symbol.__name__}({formatted_parameters}\n)\n"
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 29
+# %% ../nbs/096_Docusaurus_Helper.ipynb 61
 def _get_exps(mod: str) -> Dict[str, str]:
     mf = _find_mod(mod)
     if not mf:
         return {}
     txt = mf.read_text()
     _def_types = ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef
     d = {}
@@ -210,15 +392,15 @@
                     tree.name + "." + t2.name: f"{t2.lineno}-L{t2.end_lineno}"
                     for t2 in tree.body
                     if isinstance(t2, _def_types)
                 }
             )
     return d
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 31
+# %% ../nbs/096_Docusaurus_Helper.ipynb 63
 def _lineno(sym: str, fname: str) -> Optional[str]:
     return _get_exps(fname).get(sym, None) if fname else None
 
 
 @lru_cache(None)
 class CustomNbdevLookup(NbdevLookup.__wrapped__):  # type: ignore
     def __init__(
@@ -234,59 +416,55 @@
         res = self[sym]
         if not isinstance(res, tuple):
             return None
         _, py, gh = res
         line = _lineno(sym, py)
         return f"{gh}#L{line}"
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 34
-def _get_symbol_source_link(
-    symbol: Union[types.FunctionType, Type[Any]], lib_version: str
-) -> str:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 66
+def _get_symbol_source_link(symbol: Type, lib_version: str) -> str:
     """Returns the source code link for a given symbol.
 
     Args:
         symbol: The symbol to get the source code link for.
         lib_version: The current version of the library.
 
     Returns:
         The source code link for the symbol.
     """
-    symbol = symbol.fget if isinstance(symbol, property) else symbol  # type: ignore
+    symbol = symbol.fget if isinstance(symbol, property) else symbol
     source_link = CustomNbdevLookup().code(f"{symbol.__qualname__}")
 
     if source_link is None:
         return ""
 
     href = (
         source_link.replace("/blob/main/", f"/blob/{lib_version}/")
         if lib_version.replace(".", "").isdigit()
         else source_link
     )
     return f'<a href="{href}" class="link-to-source" target="_blank">View source</a>'
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 38
-def _get_method_type(symbol: Union[types.FunctionType, Type[Any]]) -> str:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 70
+def _get_method_type(symbol: Type) -> str:
     try:
         source = getsource(symbol).strip()
     except TypeError as e:
         return ""
 
     first_line = source.split("\n")[0]
     return (
         f"{first_line}\n"
         if first_line
         in ["@abstractmethod", "@staticmethod", "@classmethod", "@property"]
         else ""
     )
 
 
-def _get_symbol_definition(
-    symbol: Union[types.FunctionType, Type[Any]], header_level: int, lib_version: str
-) -> str:
+def _get_symbol_definition(symbol: Type, header_level: int, lib_version: str) -> str:
     """Return the definition of a given symbol.
 
     Args:
         symbol: A function or method object to get the definition for.
         header_level: The level of the markdown header to append.
         lib_version: The current version of the library.
 
@@ -307,49 +485,44 @@
     link_to_source = f"{_get_symbol_source_link(symbol, lib_version)}\n\n"
 
     _signature = signature(symbol)
     parameters = _get_parameters(_signature)
     symbol_definition = f"```py\n{_get_method_type(symbol)}{_format_symbol_definition(symbol, parameters)}```\n"
     return symbol_anchor + link_to_source + symbol_definition
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 44
-def _is_method(symbol: Union[types.FunctionType, Type[Any]]) -> bool:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 76
+def _is_method(symbol: Type) -> bool:
     """Check if the given symbol is a method.
 
     Args:
         symbol: A function or method object to check.
 
     Returns:
         A boolean indicating whether the symbol is a method.
     """
     return ismethod(symbol) or isfunction(symbol) or isinstance(symbol, property)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 46
+# %% ../nbs/096_Docusaurus_Helper.ipynb 78
 def _get_formatted_docstring_for_symbol(
-    symbol: Union[types.FunctionType, Type[Any]],
-    lib_version: str,
-    header_level: int = 2,
+    symbol: Type, lib_version: str, header_level: int = 2
 ) -> str:
     """Recursively parses and get formatted docstring of a symbol.
 
     Args:
         symbol: A Python class or function object to parse the docstring for.
         lib_version: The current version of the library.
         header_level: The level of the markdown header to append.
 
     Returns:
         A formatted docstring of the symbol and its members.
 
     """
 
     def traverse(
-        symbol: Union[types.FunctionType, Type[Any]],
-        contents: str,
-        header_level: int,
-        lib_version: str,
+        symbol: Type, contents: str, header_level: int, lib_version: str
     ) -> str:
         """Recursively traverse the members of a symbol and append their docstrings to the provided contents string.
 
         Args:
             symbol: A Python class or function object to parse the docstring for.
             contents: The current formatted docstrings.
             header_level: The level of the markdown header to append.
@@ -358,30 +531,30 @@
         Returns:
             The updated formatted docstrings.
 
         """
         for x, y in getmembers(symbol):
             if not x.startswith("_") or x == "__init__":
                 if _is_method(y) and y.__doc__ is not None:
-                    contents += f"{_get_symbol_definition(y, header_level, lib_version)}\n{_docstring_to_markdown(y.__doc__)}"
+                    contents += f"{_get_symbol_definition(y, header_level, lib_version)}\n{_docstring_to_markdown(y)}"
                 elif isclass(y) and y.__doc__ is not None and not x.startswith("_"):
-                    contents += f"{_get_symbol_definition(y, header_level+1, lib_version)}\n{_docstring_to_markdown(y.__doc__)}"
+                    contents += f"{_get_symbol_definition(y, header_level+1, lib_version)}\n{_docstring_to_markdown(y)}"
                     contents = traverse(y, contents, header_level + 1, lib_version)
         return contents
 
     contents = (
-        f"{_get_symbol_definition(symbol, header_level+1, lib_version)}\n{_docstring_to_markdown(symbol.__doc__)}"
+        f"{_get_symbol_definition(symbol, header_level+1, lib_version)}\n{_docstring_to_markdown(symbol)}"
         if symbol.__doc__ is not None
         else ""
     )
     if isclass(symbol):
         contents = traverse(symbol, contents, header_level + 1, lib_version)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 49
+# %% ../nbs/096_Docusaurus_Helper.ipynb 81
 def _convert_html_style_attribute_to_jsx(contents: str) -> str:
     """Converts the inline style attributes in an HTML string to JSX compatible format.
 
     Args:
         contents: A string containing an HTML document or fragment.
 
     Returns:
@@ -405,72 +578,99 @@
         for key, value in style_dict.items():
             replacement += f"{key}: '{value}', "
         replacement = replacement[:-2] + "}}"
         contents = contents.replace(f'style="{style_match}"', replacement)
 
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 51
+# %% ../nbs/096_Docusaurus_Helper.ipynb 83
 def _get_all_markdown_files_path(docs_path: Path) -> List[Path]:
     """Get all Markdown files in a directory and its subdirectories.
 
     Args:
         directory: The path to the directory to search in.
 
     Returns:
         A list of paths to all Markdown files found in the directory and its subdirectories.
     """
     markdown_files = [file_path for file_path in docs_path.glob("**/*.md")]
     return markdown_files
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 53
+# %% ../nbs/096_Docusaurus_Helper.ipynb 85
 def _fix_special_symbols_in_html(contents: str) -> str:
     contents = contents.replace("”", '"')
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 55
+# %% ../nbs/096_Docusaurus_Helper.ipynb 87
 def _add_file_extension_to_link(url: str) -> str:
     """Add file extension to the last segment of a URL
 
     Args:
         url: A URL string.
 
     Returns:
         A string of the updated URL with a file extension added to the last segment of the URL.
     """
     segments = url.split("/#")[0].split("/")[-2:]
     return url.replace(f"/{segments[1]}", f"/{segments[1]}.md").replace(".md/#", ".md#")
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 59
+# %% ../nbs/096_Docusaurus_Helper.ipynb 91
+def _generate_production_url(url: str) -> str:
+    """Generate a Docusaurus compatible production URL for the given symbol URL.
+
+    Args:
+        url: The symbol URL to be converted.
+
+    Returns:
+        The production URL of the symbol.
+    """
+    url_segment, hash_segment = url.split(".md")
+    url_split = url_segment.split("/")
+    if url_split[-1].lower() == url_split[-2].lower():
+        return "/".join(url_split[:-1]) + hash_segment
+    return url.replace(".md", "")
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 93
 def _fix_symbol_links(
-    contents: str, dir_prefix: str, doc_host: str, doc_baseurl: str
+    contents: str,
+    dir_prefix: str,
+    doc_host: str,
+    doc_baseurl: str,
+    use_relative_doc_links: bool = True,
 ) -> str:
     """Fix symbol links in Markdown content.
 
     Args:
         contents: The Markdown content to search for symbol links.
         dir_prefix: Directory prefix to append in the relative URL.
         doc_host: The host URL for the documentation site.
         doc_baseurl: The base URL for the documentation site.
+        use_relative_doc_links: If set to True, then the relative link to symbols will be added else,
+            production link will be added.
 
     Returns:
         str: The Markdown content with updated symbol links.
     """
     prefix = re.escape(urljoin(doc_host + "/", doc_baseurl))
     pattern = re.compile(rf"\[(.*?)\]\(({prefix}[^)]+)\)")
     matches = pattern.findall(contents)
     for match in matches:
         old_url = match[1]
         new_url = _add_file_extension_to_link(old_url).replace("/api/", "/docs/api/")
-        dir_prefix = "./" if dir_prefix == "" else dir_prefix
-        relative_url = dir_prefix + new_url.split("/docs/")[1]
-        contents = contents.replace(old_url, relative_url)
+        if use_relative_doc_links:
+            dir_prefix = "./" if dir_prefix == "" else dir_prefix
+            updated_url = dir_prefix + new_url.split("/docs/")[1]
+        else:
+            updated_url = _generate_production_url(
+                doc_host + doc_baseurl + "/docs/" + new_url.split("/docs/")[1]
+            )
+        contents = contents.replace(old_url, updated_url)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 66
+# %% ../nbs/096_Docusaurus_Helper.ipynb 101
 def _get_relative_url_prefix(docs_path: Path, sub_path: Path) -> str:
     """Returns a relative url prefix from a sub path to a docs path.
 
     Args:
         docs_path (Path): The docs directory path.
         sub_path (Path): The sub directory path.
 
@@ -485,15 +685,15 @@
     except ValueError:
         raise ValueError(f"{sub_path} is not a descendant of {docs_path}")
 
     return (
         "../" * (len(relative_path.parts) - 1) if len(relative_path.parts) > 1 else ""
     )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 68
+# %% ../nbs/096_Docusaurus_Helper.ipynb 103
 def fix_invalid_syntax_in_markdown(docs_path: str) -> None:
     """Fix invalid HTML syntax in markdown files and converts inline style attributes to JSX-compatible format.
 
     Args:
         docs_path: The path to the root directory to search for markdown files.
     """
     cfg = get_config()
@@ -508,15 +708,15 @@
         contents = _convert_html_style_attribute_to_jsx(contents)
         contents = _fix_special_symbols_in_html(contents)
         contents = _fix_symbol_links(
             contents, relative_url_prefix, doc_host, doc_baseurl
         )
         file.write_text(contents)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 70
+# %% ../nbs/096_Docusaurus_Helper.ipynb 105
 def generate_markdown_docs(module_name: str, docs_path: str) -> None:
     """Generates Markdown documentation files for the symbols in the given module and save them to the given directory.
 
     Args:
         module_name: The name of the module to generate documentation for.
         docs_path: The path to the directory where the documentation files will be saved.
     """
@@ -528,15 +728,15 @@
         content = _get_formatted_docstring_for_symbol(symbol, lib_version)
         target_file_path = (
             "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
         )
         with open((Path(docs_path) / "api" / target_file_path), "w") as f:
             f.write(content)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 73
+# %% ../nbs/096_Docusaurus_Helper.ipynb 108
 def _parse_lines(lines: List[str]) -> Tuple[List[str], int]:
     """Parse a list of lines and return a tuple containing a list of filenames and an index indicating how many lines to skip.
 
     Args:
         lines: A list of strings representing lines of input text.
 
     Returns:
@@ -545,15 +745,15 @@
     """
     index = next(
         (i for i, line in enumerate(lines) if not line.strip().startswith("- [")),
         len(lines),
     )
     return [line.split("(")[1][:-4] for line in lines[:index]], index
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 76
+# %% ../nbs/096_Docusaurus_Helper.ipynb 111
 def _parse_section(text: str, ignore_first_line: bool = False) -> List[Any]:
     """Parse the given section contents and return a list of file names in the expected format.
 
     Args:
         text: A string representing the contents of a file.
         ignore_first_line: Flag indicating whether to ignore the first line extracting the section contents.
 
@@ -574,15 +774,15 @@
             value, skip_lines = _parse_lines(lines[index + 1 :])
             ret_val.append({line.replace("-", "").strip(): value})
             index += skip_lines + 1
         else:
             index += 1
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 79
+# %% ../nbs/096_Docusaurus_Helper.ipynb 114
 def _get_section_from_markdown(
     markdown_text: str, section_header: str
 ) -> Optional[str]:
     """Get the contents of the section header from the given markdown text
 
     Args:
         markdown_text: A string containing the markdown text to extract the section from.
@@ -592,15 +792,15 @@
         A string representing the contents of the section header if the section header
         is present in the markdown text, else None
     """
     pattern = re.compile(rf"^- {section_header}\n((?:\s+- .*\n)+)", re.M)
     match = pattern.search(markdown_text)
     return match.group(1) if match else None
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 84
+# %% ../nbs/096_Docusaurus_Helper.ipynb 119
 def generate_sidebar(
     summary_file: str = "./docusaurus/docs/SUMMARY.md",
     summary: str = "",
     target: str = "./docusaurus/sidebars.js",
 ) -> None:
     """
     Generate a sidebar js file for a Docusaurus documentation site based on a SUMMARY.md file.
@@ -648,15 +848,15 @@
     "LICENSE",
     "CONTRIBUTING",
     "CHANGELOG",
 ],
 };"""
         )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 86
+# %% ../nbs/096_Docusaurus_Helper.ipynb 121
 def _get_markdown_filenames_from_sidebar(sidebar_file_path: str) -> List[str]:
     """Get a list of Markdown filenames included in the sidebar.
 
     Args:
         sidebar_file_path: The path to the sidebar file.
 
     Returns:
@@ -669,15 +869,15 @@
         match = re.search(pattern, file_content, re.DOTALL)
         all_sidebar_files = ast.literal_eval(match.group(1)) if match else []
         markdown_filenames = [
             f"{v}.md" for v in all_sidebar_files if isinstance(v, str)
         ]
         return markdown_filenames
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 88
+# %% ../nbs/096_Docusaurus_Helper.ipynb 123
 def _delete_files(files: List[Path]) -> None:
     """Deletes a list of files.
 
     Args:
         files: A list of Path objects representing the files to be deleted.
 
     Raises:
@@ -688,15 +888,15 @@
         try:
             file.unlink()
         except OSError as e:
             typer.echo(
                 f"Error deleting files from docusaurus/docs directory. Could not delete file: {file} - {e}"
             )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 91
+# %% ../nbs/096_Docusaurus_Helper.ipynb 126
 def delete_unused_markdown_files_from_sidebar(
     docs_path: str, sidebar_file_path: str
 ) -> None:
     """Delete the markdown files from the docs directory that are not present in the sidebar.
 
     Args:
         docs_path: Path to the directory containing the markdown files.
@@ -710,7 +910,25 @@
             file_path for file_path in Path(docs_path).glob("*.md")
         ]
         md_files_in_sidebar = [Path(docs_path) / f for f in md_filenames_in_sidebar]
         md_files_to_delete = list(
             set(all_md_files_in_docs_dir) - set(md_files_in_sidebar)
         )
         _delete_files(md_files_to_delete)
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 128
+def update_readme() -> None:
+    """Update the readme file and fix the symbol links"""
+    cfg = get_config()
+    readme_path = cfg.config_path / "README.md"
+    nbdev_readme.__wrapped__()
+
+    with open(readme_path, "r", encoding="utf-8") as f:
+        contents = f.read()
+
+    contents = update_default_symbol_links(
+        contents, NbdevLookup(incl_libs=cfg.lib_path.name), "", "", False
+    )
+    contents = _fix_symbol_links(contents, "./", cfg.doc_host, cfg.doc_baseurl, False)
+
+    with open(readme_path, "w", encoding="utf-8") as f:
+        f.write(contents)
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_helpers.py` & `fastkafka-0.8.0rc1/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_modidx.py` & `fastkafka-0.8.0rc1/fastkafka/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,38 +129,36 @@
                                                                                                                                       'fastkafka/_components/aiokafka_consumer_loop.py')},
             'fastkafka._components.asyncapi': { 'fastkafka._components.asyncapi.APIKeyLocation': ( 'asyncapi.html#apikeylocation',
                                                                                                    'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.ContactInfo': ( 'asyncapi.html#contactinfo',
                                                                                                 'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBroker': ( 'asyncapi.html#kafkabroker',
                                                                                                 'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.KafkaBroker.dict': ( 'asyncapi.html#kafkabroker.dict',
-                                                                                                     'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.KafkaBroker.json': ( 'asyncapi.html#kafkabroker.json',
-                                                                                                     'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBroker.model_dump': ( 'asyncapi.html#kafkabroker.model_dump',
+                                                                                                           'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBroker.model_dump_json': ( 'asyncapi.html#kafkabroker.model_dump_json',
+                                                                                                                'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBrokers': ( 'asyncapi.html#kafkabrokers',
                                                                                                  'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.KafkaBrokers.dict': ( 'asyncapi.html#kafkabrokers.dict',
-                                                                                                      'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.KafkaBrokers.json': ( 'asyncapi.html#kafkabrokers.json',
-                                                                                                      'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBrokers.model_dump': ( 'asyncapi.html#kafkabrokers.model_dump',
+                                                                                                            'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBrokers.model_dump_json': ( 'asyncapi.html#kafkabrokers.model_dump_json',
+                                                                                                                 'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaMessage': ( 'asyncapi.html#kafkamessage',
                                                                                                  'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.KafkaMessage.Config': ( 'asyncapi.html#kafkamessage.config',
-                                                                                                        'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaServiceInfo': ( 'asyncapi.html#kafkaserviceinfo',
                                                                                                      'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.SecuritySchema': ( 'asyncapi.html#securityschema',
                                                                                                    'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.SecuritySchema.__init__': ( 'asyncapi.html#securityschema.__init__',
                                                                                                             'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.SecuritySchema.dict': ( 'asyncapi.html#securityschema.dict',
-                                                                                                        'fastkafka/_components/asyncapi.py'),
-                                                'fastkafka._components.asyncapi.SecuritySchema.json': ( 'asyncapi.html#securityschema.json',
-                                                                                                        'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.SecuritySchema.model_dump': ( 'asyncapi.html#securityschema.model_dump',
+                                                                                                              'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.SecuritySchema.model_dump_json': ( 'asyncapi.html#securityschema.model_dump_json',
+                                                                                                                   'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.SecurityType': ( 'asyncapi.html#securitytype',
                                                                                                  'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi._add_example_to_msg_definitions': ( 'asyncapi.html#_add_example_to_msg_definitions',
                                                                                                                     'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi._generate_async_docs': ( 'asyncapi.html#_generate_async_docs',
                                                                                                          'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi._generate_async_spec': ( 'asyncapi.html#_generate_async_spec',
@@ -205,16 +203,18 @@
                                                                                                                     'fastkafka/_components/docs_dependencies.py')},
             'fastkafka._components.encoder.avro': { 'fastkafka._components.encoder.avro.AvroBase': ( 'avro_encode_decoder.html#avrobase',
                                                                                                      'fastkafka/_components/encoder/avro.py'),
                                                     'fastkafka._components.encoder.avro.AvroBase._avro_schema': ( 'avro_encode_decoder.html#avrobase._avro_schema',
                                                                                                                   'fastkafka/_components/encoder/avro.py'),
                                                     'fastkafka._components.encoder.avro.AvroBase.avro_schema': ( 'avro_encode_decoder.html#avrobase.avro_schema',
                                                                                                                  'fastkafka/_components/encoder/avro.py'),
-                                                    'fastkafka._components.encoder.avro.AvroBase.avro_schema_for_pydantic': ( 'avro_encode_decoder.html#avrobase.avro_schema_for_pydantic',
-                                                                                                                              'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.AvroBase.avro_schema_for_pydantic_class': ( 'avro_encode_decoder.html#avrobase.avro_schema_for_pydantic_class',
+                                                                                                                                    'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.AvroBase.avro_schema_for_pydantic_object': ( 'avro_encode_decoder.html#avrobase.avro_schema_for_pydantic_object',
+                                                                                                                                     'fastkafka/_components/encoder/avro.py'),
                                                     'fastkafka._components.encoder.avro.avro_decoder': ( 'avro_encode_decoder.html#avro_decoder',
                                                                                                          'fastkafka/_components/encoder/avro.py'),
                                                     'fastkafka._components.encoder.avro.avro_encoder': ( 'avro_encode_decoder.html#avro_encoder',
                                                                                                          'fastkafka/_components/encoder/avro.py'),
                                                     'fastkafka._components.encoder.avro.avsc_to_pydantic': ( 'avro_encode_decoder.html#avsc_to_pydantic',
                                                                                                              'fastkafka/_components/encoder/avro.py')},
             'fastkafka._components.encoder.json': { 'fastkafka._components.encoder.json._to_json_utf8': ( 'json_encode_decoder.html#_to_json_utf8',
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_server.py` & `fastkafka-0.8.0rc1/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.8.0rc1/fastkafka/_testing/apache_kafka_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,34 +164,32 @@
     return kafka_config
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 12
 @export("fastkafka.testing")
 class ApacheKafkaBroker:
     """ApacheKafkaBroker class, used for running unique kafka brokers in tests to prevent topic clashing."""
 
-    @delegates(get_kafka_config_string)
-    @delegates(get_zookeeper_config_string, keep=True)
+    @delegates(get_kafka_config_string, but=["data_dir"])
+    @delegates(get_zookeeper_config_string, keep=True, but=["data_dir"])
     def __init__(
         self,
         topics: Iterable[str] = [],
         *,
         retries: int = 3,
         apply_nest_asyncio: bool = False,
         **kwargs: Dict[str, Any],
     ):
         """Initialises the ApacheKafkaBroker object
 
         Args:
-            data_dir: Path to the directory where the zookeepeer instance will save data
-            zookeeper_port: Port for clients (Kafka brokes) to connect
-            listener_port: Port on which the clients (producers and consumers) can connect
             topics: List of topics to create after sucessfull Kafka broker startup
             retries: Number of retries to create kafka and zookeeper services using random
             apply_nest_asyncio: set to True if running in notebook
-            port allocation if the requested port was taken
+            zookeeper_port: Port for clients (Kafka brokes) to connect
+            listener_port: Port on which the clients (producers and consumers) can connect
         """
         self.zookeeper_kwargs = filter_using_signature(
             get_zookeeper_config_string, **kwargs
         )
         self.kafka_kwargs = filter_using_signature(get_kafka_config_string, **kwargs)
 
         if "zookeeper_port" not in self.zookeeper_kwargs:
@@ -242,18 +240,15 @@
         """Starts a local kafka broker and zookeeper instance synchronously
         Returns:
            Kafka broker bootstrap server address in string format: add:port
         """
         raise NotImplementedError
 
     def stop(self) -> None:
-        """Stops a local kafka broker and zookeeper instance synchronously
-        Returns:
-           None
-        """
+        """Stops a local kafka broker and zookeeper instance synchronously"""
         raise NotImplementedError
 
     async def _stop(self) -> None:
         """Stops a local kafka broker and zookeeper instance synchronously
         Returns:
            None
         """
@@ -667,18 +662,15 @@
         return retval
     finally:
         logger.info(f"{self.__class__.__name__}.start(): exited.")
 
 
 @patch
 def stop(self: ApacheKafkaBroker) -> None:
-    """Stops a local kafka broker and zookeeper instance synchronously
-    Returns:
-       None
-    """
+    """Stops a local kafka broker and zookeeper instance synchronously"""
     logger.info(f"{self.__class__.__name__}.stop(): entering...")
     try:
         if not self._is_started:
             raise RuntimeError(
                 "ApacheKafkaBroker not started yet, please call ApacheKafkaBroker.start() before!"
             )
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.8.0rc1/fastkafka/_testing/in_memory_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,22 +318,19 @@
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 22
 @classcontextmanager()
 class InMemoryBroker:
     def __init__(
         self,
         num_partitions: int = 1,
-        *,
-        patch_module: Optional[ModuleType] = None,
     ):
         self.num_partitions = num_partitions
         self.topics: Dict[Tuple[str, str], KafkaTopic] = {}
         self.topic_groups: Dict[Tuple[str, str, str], GroupMetadata] = {}
         self.is_started: bool = False
-        self.patch_module = patch_module
 
     def connect(self) -> uuid.UUID:
         return uuid.uuid4()
 
     def dissconnect(self, consumer_id: uuid.UUID) -> None:
         """
         Disconnect a consumer from the broker.
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.8.0rc1/fastkafka/_testing/local_redpanda_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,24 +92,23 @@
         retries: int = 3,
         apply_nest_asyncio: bool = False,
         **kwargs: Dict[str, Any],
     ):
         """Initialises the LocalRedpandaBroker object
 
         Args:
+            topics: List of topics to create after sucessfull redpanda broker startup
+            retries: Number of retries to create redpanda service
+            apply_nest_asyncio: set to True if running in notebook
             listener_port: Port on which the clients (producers and consumers) can connect
             tag: Tag of Redpanda image to use to start container
             seastar_core: Core(s) to use byt Seastar (the framework Redpanda uses under the hood)
             memory: The amount of memory to make available to Redpanda
             mode: Mode to use to load configuration properties in container
             default_log_level: Log levels to use for Redpanda
-            topics: List of topics to create after sucessfull redpanda broker startup
-            retries: Number of retries to create redpanda service
-            apply_nest_asyncio: set to True if running in notebook
-            port allocation if the requested port was taken
         """
         self.redpanda_kwargs = kwargs
 
         if "listener_port" not in self.redpanda_kwargs:
             self.redpanda_kwargs["listener_port"] = 9092  # type: ignore
 
         self.retries = retries
@@ -152,18 +151,15 @@
         """Starts a local redpanda broker instance synchronously
         Returns:
            Redpanda broker bootstrap server address in string format: add:port
         """
         raise NotImplementedError
 
     def stop(self) -> None:
-        """Stops a local redpanda broker instance synchronously
-        Returns:
-           None
-        """
+        """Stops a local redpanda broker instance synchronously"""
         raise NotImplementedError
 
     async def _stop(self) -> None:
         """Stops a local redpanda broker instance synchronously
         Returns:
            None
         """
@@ -374,18 +370,15 @@
         return retval
     finally:
         logger.info(f"{self.__class__.__name__}.start(): exited.")
 
 
 @patch
 def stop(self: LocalRedpandaBroker) -> None:
-    """Stops a local redpanda broker instance synchronously
-    Returns:
-       None
-    """
+    """Stops a local redpanda broker instance synchronously"""
     logger.info(f"{self.__class__.__name__}.stop(): entering...")
     try:
         if not self._is_started:
             raise RuntimeError(
                 "LocalRedpandaBroker not started yet, please call LocalRedpandaBroker.start() before!"
             )
```

### Comparing `fastkafka-0.8.0rc0/fastkafka/_testing/test_utils.py` & `fastkafka-0.8.0rc1/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/encoder.py` & `fastkafka-0.8.0rc1/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka/testing.py` & `fastkafka-0.8.0rc1/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.8.0rc1/fastkafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.8.0rc0
+Version: 0.8.0rc1
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -81,34 +81,34 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
-You can install base version of `fastkafka` with `pip` as usual:
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating
+systems. You can install base version of FastKafka with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
-To install fastkafka with testing features please use:
+To install FastKafka with testing features please use:
 
 ``` sh
 pip install fastkafka[test]
 ```
 
-To install fastkafka with asyncapi docs please use:
+To install FastKafka with asyncapi docs please use:
 
 ``` sh
 pip install fastkafka[docs]
 ```
 
-To install fastkafka with all the features please use:
+To install FastKafka with all the features please use:
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
@@ -162,15 +162,15 @@
 contains two entries: `"localhost"` and `"production"`, specifying local
 development and production Kafka brokers. Each entry specifies the URL,
 port, and other details of a Kafka broker. This dictionary is used for
 both generating the documentation and later to run the actual server
 against one of the given kafka broker.
 
 Next, an object of the
-[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka#fastkafka.FastKafka)
+[`FastKafka`](https://airtai.github.io/fastkafka/docs/api/fastkafka#fastkafka.FastKafka)
 class is initialized with the minimum set of arguments:
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
@@ -250,15 +250,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
+[`Tester`](https://airtai.github.io/fastkafka/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -311,15 +311,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
-We have created a simple fastkafka application. The app will consume the
+We have created a simple FastKafka application. The app will consume the
 `Data` from the `input_data` topic, log it and produce the incremented
 data to `output_data` topic.
 
 To test the app we have:
 
 1.  Created the app
```

### Comparing `fastkafka-0.8.0rc0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.8.0rc1/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.8.0rc0/fastkafka.egg-info/requires.txt` & `fastkafka-0.8.0rc1/fastkafka.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 aiokafka>=0.8.0
 anyio>=3.0
 asyncer>=0.0.2
 docstring-parser>=0.15
 nest-asyncio>=1.5.6
-pydantic>=1.9
+pydantic>=2.0
 tqdm>=4.62
 typer>=0.7.0
 
 [:platform_system == "Windows"]
 psutil>=5.9.5
 
 [avro]
 fastavro>=1.7.3
 
 [dev]
 PyYAML>=5.3.1
 aiohttp>=3.8.4
 bandit==1.7.5
 black==23.3.0
-email-validator==1.3.1
-fastapi>=0.95.1
+email-validator>=2.0.0
+fastapi>=0.100.0b2
 fastavro>=1.7.3
 install-jdk==0.3.0
 ipython<8.13
 ipywidgets<=8.0.4,>=8.0
 isort==5.12.0
 mypy==1.3.0
 nbconvert>=7.2.9
```

### Comparing `fastkafka-0.8.0rc0/settings.ini` & `fastkafka-0.8.0rc1/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.8.0rc0
+version = 0.8.0rc1
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.8.0rc0/setup.py` & `fastkafka-0.8.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
 
 requirements = [
-    "pydantic>=1.9",
+    "pydantic>=2.0",
     "anyio>=3.0",
     "aiokafka>=0.8.0",
     "asyncer>=0.0.2",
     "tqdm>=4.62",
     "docstring-parser>=0.15",
     "typer>=0.7.0",
     "nest-asyncio>=1.5.6",
@@ -61,18 +61,18 @@
     "black==23.3.0",
     "isort==5.12.0",
     "bandit==1.7.5",
     "semgrep==1.21.0",
     "pytest==7.3.1",
     "numpy>=1.21.0",
     "pandas>=1.2.0",
-    "email-validator==1.3.1",
+    "email-validator>=2.0.0",
     "scikit-learn==1.2.1",
     "ipython<8.13",
-    "fastapi>=0.95.1",
+    "fastapi>=0.100.0b2",
     "uvicorn==0.22.0",
 ]
 
 project_urls = {
    'Bug Tracker': cfg['git_url'] + '/issues',
    'CI': cfg['git_url'] + '/actions',
    'Documentation': 'https://fastkafka.airt.ai/',
```

