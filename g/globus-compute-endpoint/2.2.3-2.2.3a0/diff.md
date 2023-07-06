# Comparing `tmp/globus-compute-endpoint-2.2.3.tar.gz` & `tmp/globus-compute-endpoint-2.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.2.3.tar", last modified: Thu Jul  6 20:22:05 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.2.3a0.tar", last modified: Wed Jul  5 15:36:21 2023, max compression
```

## Comparing `globus-compute-endpoint-2.2.3.tar` & `globus-compute-endpoint-2.2.3a0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.514362 globus-compute-endpoint-2.2.3/
--rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/LICENSE
--rw-r--r--   0 yadu       (501) staff       (20)       83 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3/MANIFEST.in
--rw-r--r--   0 yadu       (501) staff       (20)     1838 2023-07-06 20:22:05.514461 globus-compute-endpoint-2.2.3/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)      871 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/PyPI.md
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.495167 globus-compute-endpoint-2.2.3/globus_compute_endpoint/
--rw-r--r--   0 yadu       (501) staff       (20)      131 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)    17072 2023-07-06 18:38:51.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.498354 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.500055 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/
--rw-r--r--   0 yadu       (501) staff       (20)       41 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     6533 2023-07-05 19:53:55.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/config.py
--rw-r--r--   0 yadu       (501) staff       (20)      760 2023-07-05 19:53:55.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/default_config.py
--rw-r--r--   0 yadu       (501) staff       (20)      146 2023-07-05 19:53:55.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/default_config.yaml
--rw-r--r--   0 yadu       (501) staff       (20)     3348 2023-07-05 19:53:55.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/model.py
--rw-r--r--   0 yadu       (501) staff       (20)     7326 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/utils.py
--rw-r--r--   0 yadu       (501) staff       (20)    27495 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 yadu       (501) staff       (20)    20355 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 yadu       (501) staff       (20)    23242 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 yadu       (501) staff       (20)     3075 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.501622 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 yadu       (501) staff       (20)      307 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)      689 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 yadu       (501) staff       (20)    11834 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 yadu       (501) staff       (20)     3068 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 yadu       (501) staff       (20)    14076 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 yadu       (501) staff       (20)     5184 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 yadu       (501) staff       (20)     7275 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.502086 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 yadu       (501) staff       (20)     1017 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)      110 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/utils/config.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.503281 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/
--rw-r--r--   0 yadu       (501) staff       (20)      241 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     6257 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/base.py
--rw-r--r--   0 yadu       (501) staff       (20)     3721 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/globus_compute.py
--rw-r--r--   0 yadu       (501) staff       (20)     4608 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/helper.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.506368 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1943 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/container_sched.py
--rw-r--r--   0 yadu       (501) staff       (20)    34568 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/engine.py
--rw-r--r--   0 yadu       (501) staff       (20)    49294 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/interchange.py
--rw-r--r--   0 yadu       (501) staff       (20)     9712 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 yadu       (501) staff       (20)      267 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 yadu       (501) staff       (20)    36121 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/manager.py
--rw-r--r--   0 yadu       (501) staff       (20)     9295 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/messages.py
--rw-r--r--   0 yadu       (501) staff       (20)     7216 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/worker.py
--rw-r--r--   0 yadu       (501) staff       (20)    19094 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/worker_map.py
--rw-r--r--   0 yadu       (501) staff       (20)     5427 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
--rw-r--r--   0 yadu       (501) staff       (20)     3715 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/thread_pool.py
--rw-r--r--   0 yadu       (501) staff       (20)     2020 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 yadu       (501) staff       (20)      220 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.506573 globus-compute-endpoint-2.2.3/globus_compute_endpoint/executors/
--rw-r--r--   0 yadu       (501) staff       (20)      141 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.506975 globus-compute-endpoint-2.2.3/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)      422 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 yadu       (501) staff       (20)     8499 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.507197 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/
--rw-r--r--   0 yadu       (501) staff       (20)      115 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.507834 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)    12926 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 yadu       (501) staff       (20)       50 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.511040 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/
--rw-r--r--   0 yadu       (501) staff       (20)      280 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     7018 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 yadu       (501) staff       (20)     5470 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 yadu       (501) staff       (20)     6145 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 yadu       (501) staff       (20)     1610 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 yadu       (501) staff       (20)      804 2023-07-06 20:21:28.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint/version.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.496245 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/
--rw-r--r--   0 yadu       (501) staff       (20)     1838 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 yadu       (501) staff       (20)     3729 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 yadu       (501) staff       (20)      353 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 yadu       (501) staff       (20)      343 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 yadu       (501) staff       (20)       30 2023-07-06 20:22:05.000000 globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-06 20:22:05.514981 globus-compute-endpoint-2.2.3/setup.cfg
--rw-r--r--   0 yadu       (501) staff       (20)     3678 2023-07-06 20:21:28.000000 globus-compute-endpoint-2.2.3/setup.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.511760 globus-compute-endpoint-2.2.3/tests/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/tests/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     2709 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3/tests/conftest.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.512189 globus-compute-endpoint-2.2.3/tests/integration/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)    11428 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3/tests/integration/conftest.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.512789 globus-compute-endpoint-2.2.3/tests/integration/endpoint/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     1679 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/conftest.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.513251 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/__init__.py
-drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-06 20:22:05.514148 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/
--rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 yadu       (501) staff       (20)     2256 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
--rw-r--r--   0 yadu       (501) staff       (20)     2275 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_manager.py
--rw-r--r--   0 yadu       (501) staff       (20)     1273 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
--rw-r--r--   0 yadu       (501) staff       (20)     1126 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/mock_executors.py
--rw-r--r--   0 yadu       (501) staff       (20)     2925 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3/tests/utils.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.743182 globus-compute-endpoint-2.2.3a0/
+-rw-r--r--   0 yadu       (501) staff       (20)    11330 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/LICENSE
+-rw-r--r--   0 yadu       (501) staff       (20)       83 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3a0/MANIFEST.in
+-rw-r--r--   0 yadu       (501) staff       (20)     1840 2023-07-05 15:36:21.743282 globus-compute-endpoint-2.2.3a0/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)      871 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/PyPI.md
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.723544 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)      131 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    16673 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.726804 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.728630 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/
+-rw-r--r--   0 yadu       (501) staff       (20)       41 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6542 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/config.py
+-rw-r--r--   0 yadu       (501) staff       (20)      766 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.py
+-rw-r--r--   0 yadu       (501) staff       (20)      117 2023-06-16 15:43:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.yaml
+-rw-r--r--   0 yadu       (501) staff       (20)     3522 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/model.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7326 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/utils.py
+-rw-r--r--   0 yadu       (501) staff       (20)    27495 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 yadu       (501) staff       (20)    20355 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)    23242 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3075 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.730265 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 yadu       (501) staff       (20)      307 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      689 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11834 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3068 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 yadu       (501) staff       (20)    14076 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5184 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7275 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.730713 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 yadu       (501) staff       (20)     1017 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      110 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.731965 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/
+-rw-r--r--   0 yadu       (501) staff       (20)      241 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6257 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3721 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 yadu       (501) staff       (20)     4608 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/helper.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.735555 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1943 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/container_sched.py
+-rw-r--r--   0 yadu       (501) staff       (20)    34568 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/engine.py
+-rw-r--r--   0 yadu       (501) staff       (20)    49294 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange.py
+-rw-r--r--   0 yadu       (501) staff       (20)     9712 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 yadu       (501) staff       (20)      267 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 yadu       (501) staff       (20)    36121 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)     9295 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/messages.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7216 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker.py
+-rw-r--r--   0 yadu       (501) staff       (20)    19094 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker_map.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5427 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py
+-rw-r--r--   0 yadu       (501) staff       (20)     3715 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2020 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 yadu       (501) staff       (20)      220 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.735773 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/
+-rw-r--r--   0 yadu       (501) staff       (20)      141 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.736521 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)      422 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 yadu       (501) staff       (20)     8499 2023-06-22 21:30:50.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.737105 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/
+-rw-r--r--   0 yadu       (501) staff       (20)      115 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.738412 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    12926 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 yadu       (501) staff       (20)       50 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.740077 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 yadu       (501) staff       (20)      280 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     7018 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 yadu       (501) staff       (20)     5470 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 yadu       (501) staff       (20)     6145 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1610 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 yadu       (501) staff       (20)      806 2023-07-05 15:23:57.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.724649 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 yadu       (501) staff       (20)     1840 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 yadu       (501) staff       (20)     3729 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 yadu       (501) staff       (20)        1 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      353 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      344 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 yadu       (501) staff       (20)       30 2023-07-05 15:36:21.000000 globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 yadu       (501) staff       (20)      282 2023-07-05 15:36:21.743746 globus-compute-endpoint-2.2.3a0/setup.cfg
+-rw-r--r--   0 yadu       (501) staff       (20)     3679 2023-07-05 15:25:36.000000 globus-compute-endpoint-2.2.3a0/setup.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.740942 globus-compute-endpoint-2.2.3a0/tests/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/tests/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2709 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/tests/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.741427 globus-compute-endpoint-2.2.3a0/tests/integration/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)    11428 2023-04-21 14:48:17.000000 globus-compute-endpoint-2.2.3a0/tests/integration/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.741806 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1679 2023-04-24 17:52:07.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/conftest.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.742133 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/__init__.py
+drwxr-xr-x   0 yadu       (501) staff       (20)        0 2023-07-05 15:36:21.742964 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/
+-rw-r--r--   0 yadu       (501) staff       (20)        0 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2256 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2275 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_manager.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1273 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py
+-rw-r--r--   0 yadu       (501) staff       (20)     1126 2023-06-30 20:13:26.000000 globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/mock_executors.py
+-rw-r--r--   0 yadu       (501) staff       (20)     2925 2023-06-12 16:33:52.000000 globus-compute-endpoint-2.2.3a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.2.3/LICENSE` & `globus-compute-endpoint-2.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/PKG-INFO` & `globus-compute-endpoint-2.2.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.3/PyPI.md` & `globus-compute-endpoint-2.2.3a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import difflib
 import json
 import logging
 import pathlib
-import re
 import shutil
 import sys
 import uuid
 
 import click
 from click import ClickException
 from globus_compute_endpoint.endpoint.config.utils import get_config, load_config_yaml
@@ -303,15 +302,14 @@
             error_msg = "No cached tokens were found, already logged out?"
             log.info(error_msg)
     return tokens_revoked, error_msg
 
 
 FUNCX_COMPUTE_IMPORT_UPDATES = {
     "from funcx_endpoint.endpoint.utils.config": "from globus_compute_endpoint.endpoint.config",  # noqa E501
-    "from funcx_endpoint.engines": "from globus_compute_endpoint.engines",  # noqa E501
     "from funcx_endpoint.executors": "from globus_compute_endpoint.executors",  # noqa E501
 }
 
 
 def _upgrade_funcx_imports_in_config(name: str, force=False) -> str:
     """
     This only modifies unindented import lines, as are in the original
@@ -327,16 +325,16 @@
     config_path = ep_dir / "config.py"
     config_backup = ep_dir / "config.py.bak"
 
     try:
         config_text = config_path.read_text()
         upd_config_text = config_text
 
-        for pattern, repl in FUNCX_COMPUTE_IMPORT_UPDATES.items():
-            upd_config_text = re.sub(f"^{pattern}", repl, upd_config_text, flags=re.M)
+        for original, repl in FUNCX_COMPUTE_IMPORT_UPDATES.items():
+            upd_config_text = upd_config_text.replace(original, repl)
 
         if upd_config_text == config_text:
             return f"No funcX import statements found in config.py for {name}"
 
         change_diff = "".join(
             difflib.unified_diff(
                 config_text.splitlines(keepends=True),
@@ -359,23 +357,15 @@
             raise ClickException(msg)
 
         # Write to temporary file in case of issues
         tmp_output_path = ep_dir / ("config.py." + uuid.uuid4().hex)
         tmp_output_path.write_text(upd_config_text)
 
         # Rename files last, as it's the least likely to err
-        if sys.version_info < (3, 8):
-            try:
-                # Dropping support for Python 3.7 "real soon", so this branch will
-                # soon go away
-                config_backup.unlink()
-            except FileNotFoundError:
-                pass
-        else:
-            config_backup.unlink(missing_ok=True)
+        config_backup.unlink(missing_ok=True)
         shutil.move(config_path, config_backup)  # Preserve file timestamp
         shutil.move(tmp_output_path, config_path)
 
         return (
             f"Applied following diff for endpoint {name}:\n{change_diff}\n\n"
             f"  The previous config has been renamed to {config_backup}"
         )
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import inspect
 import warnings
 
-from globus_compute_endpoint.engines import HighThroughputEngine
+from globus_compute_endpoint.executors import HighThroughputExecutor
 from parsl.utils import RepresentationMixin
 
-_DEFAULT_EXECUTORS = [HighThroughputEngine()]
+_DEFAULT_EXECUTORS = [HighThroughputExecutor()]
 
 
 class Config(RepresentationMixin):
     """Specification of Globus Compute configuration options.
 
     Parameters
     ----------
 
     executors : list of Executors
         A list of executors which serve as the backend for function execution.
         As of 0.2.2, this list should contain only one executor.
-        Default: [HighThroughputEngine()]
+        Default: [HighThroughtputExecutor()]
 
     environment: str
         Environment the endpoint should connect to. Sets funcx_service_address and
         results_ws_uri unless they are also specified. If not specified, the endpoint
         connects to production.
         Default: None
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/default_config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/default_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from globus_compute_endpoint.endpoint.config import Config
-from globus_compute_endpoint.engines import HighThroughputEngine
+from globus_compute_endpoint.executors import HighThroughputExecutor
 from parsl.providers import LocalProvider
 
 config = Config(
     display_name=None,  # If None, defaults to the endpoint name
     executors=[
-        HighThroughputEngine(
+        HighThroughputExecutor(
             provider=LocalProvider(
                 init_blocks=1,
                 min_blocks=0,
                 max_blocks=1,
             ),
         )
     ],
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/model.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import typing as t
 from types import ModuleType
 
-from globus_compute_endpoint import engines, strategies
+from globus_compute_endpoint import strategies
+from globus_compute_endpoint.executors import HighThroughputExecutor
 from parsl import addresses as parsl_addresses
 from parsl import channels as parsl_channels
 from parsl import launchers as parsl_launchers
 from parsl import providers as parsl_providers
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
 
 def _validate_import(field: str, package: ModuleType):
     def inner(cls, module: str):
         cls = getattr(package, module, None)
         if cls is None:
             raise ValueError(f"{module} could not be found")
@@ -32,69 +33,78 @@
             return cls(**fields)
         except Exception as err:
             raise ValueError(str(err)) from err
 
     return validator(field, allow_reuse=True)(inner)
 
 
-class BaseConfigModel(BaseModel):
-    class Config:
-        extra = "allow"
-
-
-class AddressModel(BaseConfigModel):
+class AddressModel(BaseModel):
     type: str
 
     _validate_type = _validate_import("type", parsl_addresses)
 
+    class Config:
+        extra = "allow"
+
 
-class StrategyModel(BaseConfigModel):
+class StrategyModel(BaseModel):
     type: str
 
     _validate_type = _validate_import("type", strategies)
 
+    class Config:
+        extra = "allow"
+
 
-class LauncherModel(BaseConfigModel):
+class LauncherModel(BaseModel):
     type: str
 
     _validate_type = _validate_import("type", parsl_launchers)
 
+    class Config:
+        extra = "allow"
 
-class ChannelModel(BaseConfigModel):
+
+class ChannelModel(BaseModel):
     type: str
 
     _validate_type = _validate_import("type", parsl_channels)
 
+    class Config:
+        extra = "allow"
+
 
-class ProviderModel(BaseConfigModel):
+class ProviderModel(BaseModel):
     type: str
     channel: t.Optional[ChannelModel]
     launcher: t.Optional[LauncherModel]
 
     _validate_type = _validate_import("type", parsl_providers)
     _validate_channel = _validate_params("channel")
     _validate_launcher = _validate_params("launcher")
 
+    class Config:
+        extra = "allow"
 
-class EngineModel(BaseConfigModel):
-    type: str = "HighThroughputEngine"
+
+class EngineModel(BaseModel):
+    type: type = Field(default=HighThroughputExecutor, const=True)
     provider: ProviderModel
     strategy: t.Optional[StrategyModel]
     address: t.Optional[t.Union[str, AddressModel]]
 
-    _validate_type = _validate_import("type", engines)
     _validate_provider = _validate_params("provider")
     _validate_strategy = _validate_params("strategy")
     _validate_address = _validate_params("address")
 
     class Config:
-        validate_all = True
+        extra = "allow"
 
 
-class ConfigModel(BaseConfigModel):
+class ConfigModel(BaseModel):
     engine: EngineModel
     display_name: t.Optional[str]
     environment: t.Optional[str]
     funcx_service_address: t.Optional[str]
     multi_tenant: t.Optional[bool]
     allowed_functions: t.Optional[t.List[str]]
     heartbeat_period: t.Optional[int]
@@ -113,7 +123,10 @@
     def dict(self, *args, **kwargs):
         # Slight modification is needed here since we still
         # store the engine/executor in a list named executors
         ret = super().dict(*args, **kwargs)
         executor = ret.pop("engine")
         ret["executors"] = [executor]
         return ret
+
+    class Config:
+        extra = "allow"
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/config/utils.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/config/utils.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/globus_compute.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/globus_compute.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/helper.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/helper.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/container_sched.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/engine.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/engine.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/interchange.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/manager.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/messages.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/worker.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/worker_map.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/engines/thread_pool.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/engines/thread_pool.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.3"
+__version__ = "2.2.3a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.2.3
+Version: 2.2.3a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.2.3/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.2.3a0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/setup.py` & `globus-compute-endpoint-2.2.3a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk==2.2.3",
+    "globus-compute-sdk==2.2.3a0",
     "globus-compute-common==0.2.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
     # TODO: re-evaluate bound after we have an answer of some kind from psutil
     # see:
     #   https://github.com/giampaolo/psutil/issues/2002
     "psutil<6",
     # provides easy daemonization of the endpoint
     "python-daemon>=2,<3",
     # CLI parsing
-    "click<=8.1.3",
+    "click>=8,<9",
     # disallow use of 22.3.0; the whl package on some platforms causes ZMQ issues
     #
     # NOTE: 22.3.0 introduced a patched version of libzmq.so to the wheel packaging
     # which may be the source of the problems , the problem can be fixed by
     # building from source, which may mean there's an issue in the packaged library
     # further investigation may be needed if the issue persists in the next pyzmq
     # release
```

### Comparing `globus-compute-endpoint-2.2.3/tests/conftest.py` & `globus-compute-endpoint-2.2.3a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/conftest.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/endpoint/conftest.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_htex_regression.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_manager.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/high_throughput/test_worker_map.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/high_throughput/test_worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/integration/endpoint/executors/mock_executors.py` & `globus-compute-endpoint-2.2.3a0/tests/integration/endpoint/executors/mock_executors.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.2.3/tests/utils.py` & `globus-compute-endpoint-2.2.3a0/tests/utils.py`

 * *Files identical despite different names*

