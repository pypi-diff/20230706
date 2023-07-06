# Comparing `tmp/devcycle-python-server-sdk-2.0.1.tar.gz` & `tmp/devcycle-python-server-sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-2.0.1.tar", last modified: Tue Jun 20 18:48:38 2023, max compression
+gzip compressed data, was "devcycle-python-server-sdk-3.0.0.tar", last modified: Thu Jul  6 16:41:57 2023, max compression
```

## Comparing `devcycle-python-server-sdk-2.0.1.tar` & `devcycle-python-server-sdk-3.0.0.tar`

### file list

```diff
@@ -1,56 +1,76 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.098317 devcycle-python-server-sdk-2.0.1/
--rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-20 18:48:38.098387 devcycle-python-server-sdk-2.0.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2013 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.093218 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/
--rw-r--r--   0 chris      (501) staff       (20)        5 2023-06-20 18:46:37.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.093779 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     5186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)      115 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/local_bucketing.py
--rw-r--r--   0 chris      (501) staff       (20)     5637 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)     5357 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_local_client.py
--rw-r--r--   0 chris      (501) staff       (20)     2028 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/dvc_options.py
--rw-r--r--   0 chris      (501) staff       (20)      522 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/exceptions.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.094282 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      720 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/config_manager.py
--rw-r--r--   0 chris      (501) staff       (20)      495 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/managers/event_queue_manager.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.095247 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 chris      (501) staff       (20)      551 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/event.py
--rw-r--r--   0 chris      (501) staff       (20)      480 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 chris      (501) staff       (20)     1002 2023-06-20 18:40:44.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/user.py
--rw-r--r--   0 chris      (501) staff       (20)     1380 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 17:48:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/py.typed
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.095514 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/util/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096095 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1452 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       52 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       33 2023-06-20 18:48:38.000000 devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096290 devcycle-python-server-sdk-2.0.1/example/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/example/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2289 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/example/example.py
--rw-r--r--   0 chris      (501) staff       (20)       79 2023-06-20 18:48:38.098597 devcycle-python-server-sdk-2.0.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      890 2023-06-20 17:48:34.000000 devcycle-python-server-sdk-2.0.1/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.096656 devcycle-python-server-sdk-2.0.1/test/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.1/test/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.097155 devcycle-python-server-sdk-2.0.1/test/api/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7285 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/test_bucketing_client.py
--rw-r--r--   0 chris      (501) staff       (20)      348 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/api/test_local_bucketing.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.097780 devcycle-python-server-sdk-2.0.1/test/managers/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/managers/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      396 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/test/managers/test_config_manager.py
--rw-r--r--   0 chris      (501) staff       (20)      372 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/managers/test_event_queue_manager.py
--rw-r--r--   0 chris      (501) staff       (20)    11559 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.1/test/test_dvc_cloud_client.py
--rw-r--r--   0 chris      (501) staff       (20)     4806 2023-06-16 18:06:24.000000 devcycle-python-server-sdk-2.0.1/test/test_dvc_local_client.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-20 18:48:38.098078 devcycle-python-server-sdk-2.0.1/test/util/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-2.0.1/test/util/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      368 2023-06-20 18:46:37.000000 devcycle-python-server-sdk-2.0.1/test/util/test_version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.147117 devcycle-python-server-sdk-3.0.0/
+-rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-07-06 16:41:57.147189 devcycle-python-server-sdk-3.0.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     3139 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.138433 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/
+-rw-r--r--   0 chris      (501) staff       (20)        5 2023-07-06 16:38:43.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/VERSION.txt
+-rw-r--r--   0 chris      (501) staff       (20)      265 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.139628 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      303 2023-06-26 21:35:27.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/backoff.py
+-rw-r--r--   0 chris      (501) staff       (20)     5074 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     4226 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/config_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     3319 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/event_client.py
+-rw-r--r--   0 chris      (501) staff       (20)    16322 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/local_bucketing.py
+-rw-r--r--   0 chris      (501) staff       (20)     6675 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     1053 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/exceptions.py
+-rw-r--r--   0 chris      (501) staff       (20)     8605 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/local_client.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.140173 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/managers/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/managers/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3122 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/managers/config_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)     7909 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/managers/event_queue_manager.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.142095 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     3814 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/bucketed_config.py
+-rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 chris      (501) staff       (20)     3713 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 chris      (501) staff       (20)      852 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 chris      (501) staff       (20)      783 2023-06-29 23:05:15.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/platform_data.py
+-rw-r--r--   0 chris      (501) staff       (20)     2616 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 chris      (501) staff       (20)     1711 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/variable.py
+-rw-r--r--   0 chris      (501) staff       (20)     4525 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/options.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.142574 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/protobuf/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 21:51:55.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/protobuf/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     4684 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/protobuf/utils.py
+-rw-r--r--   0 chris      (501) staff       (20)     4244 2023-06-28 18:13:43.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-20 20:00:51.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/py.typed
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.143041 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/util/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-23 22:50:02.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.143707 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-07-06 16:41:57.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2036 2023-07-06 16:41:57.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-07-06 16:41:57.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       85 2023-07-06 16:41:57.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       33 2023-07-06 16:41:57.000000 devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.144037 devcycle-python-server-sdk-3.0.0/example/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.0/example/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2463 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/example/cloud_client_example.py
+-rw-r--r--   0 chris      (501) staff       (20)     2676 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/example/local_bucketing_client_example.py
+-rw-r--r--   0 chris      (501) staff       (20)       87 2023-07-05 21:12:29.000000 devcycle-python-server-sdk-3.0.0/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)       79 2023-07-06 16:41:57.147412 devcycle-python-server-sdk-3.0.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      890 2023-06-20 20:00:51.000000 devcycle-python-server-sdk-3.0.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.144378 devcycle-python-server-sdk-3.0.0/test/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-3.0.0/test/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.145129 devcycle-python-server-sdk-3.0.0/test/api/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.0/test/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7565 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/api/test_bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     4275 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/api/test_config_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     3211 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/api/test_event_client.py
+-rw-r--r--   0 chris      (501) staff       (20)    15156 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/api/test_local_bucketing.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.145353 devcycle-python-server-sdk-3.0.0/test/fixture/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-21 22:58:59.000000 devcycle-python-server-sdk-3.0.0/test/fixture/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     1372 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/test/fixture/data.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.145980 devcycle-python-server-sdk-3.0.0/test/managers/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.0/test/managers/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     5366 2023-07-04 17:13:35.000000 devcycle-python-server-sdk-3.0.0/test/managers/test_config_manager.py
+-rw-r--r--   0 chris      (501) staff       (20)    11053 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/managers/test_event_queue_manager.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.146240 devcycle-python-server-sdk-3.0.0/test/models/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/test/models/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      858 2023-06-28 20:55:41.000000 devcycle-python-server-sdk-3.0.0/test/models/test_bucketed_config.py
+-rw-r--r--   0 chris      (501) staff       (20)    11442 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/test/test_cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)    12671 2023-07-05 21:43:31.000000 devcycle-python-server-sdk-3.0.0/test/test_local_client.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-07-06 16:41:57.146886 devcycle-python-server-sdk-3.0.0/test/util/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-15 17:15:50.000000 devcycle-python-server-sdk-3.0.0/test/util/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     6671 2023-07-05 20:31:32.000000 devcycle-python-server-sdk-3.0.0/test/util/test_utils.py
+-rw-r--r--   0 chris      (501) staff       (20)      368 2023-07-06 16:38:43.000000 devcycle-python-server-sdk-3.0.0/test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-2.0.1/LICENSE` & `devcycle-python-server-sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/api/bucketing_client.py` & `devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/api/bucketing_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import logging
-import math
-from os.path import join
-import random
 import time
+from os.path import join
 from typing import Dict, List, Optional
 
 import requests
 
+from devcycle_python_sdk.api.backoff import exponential_backoff
+from devcycle_python_sdk.options import DevCycleCloudOptions
 from devcycle_python_sdk.exceptions import (
     CloudClientError,
     NotFoundError,
     CloudClientUnauthorizedError,
 )
-from devcycle_python_sdk.dvc_options import DevCycleCloudOptions
-from devcycle_python_sdk.models.user import User
-from devcycle_python_sdk.models.event import Event
-from devcycle_python_sdk.models.variable import Variable
+from devcycle_python_sdk.models.event import DevCycleEvent
 from devcycle_python_sdk.models.feature import Feature
+from devcycle_python_sdk.models.user import DevCycleUser
+from devcycle_python_sdk.models.variable import Variable
 
 logger = logging.getLogger(__name__)
 
 
 class BucketingAPIClient:
     def __init__(self, sdk_key: str, options: DevCycleCloudOptions):
         self.sdk_key = sdk_key
@@ -30,15 +29,15 @@
             "Authorization": sdk_key,
             "Content-Type": "application/json",
             "Accept": "application/json",
         }
         self.session.max_redirects = 0
 
     def _url(self, *path_args: str) -> str:
-        return join(self.options.bucketing_API_URI, "v1", *path_args)
+        return join(self.options.bucketing_api_uri, "v1", *path_args)
 
     def request(self, method: str, url: str, **kwargs) -> dict:
         retries_remaining = self.options.request_retries + 1
         timeout = self.options.request_timeout
 
         query_params = {}
         if self.options.enable_edge_db:
@@ -68,15 +67,15 @@
                     )
             except requests.exceptions.RequestException as e:
                 request_error = e
 
             if not request_error:
                 break
 
-            logger.error(
+            logger.debug(
                 f"DevCycle cloud bucketing request failed (attempt {attempts}): {request_error}"
             )
             retries_remaining -= 1
             if retries_remaining:
                 retry_delay = exponential_backoff(
                     attempts, self.options.retry_delay / 1000.0
                 )
@@ -85,40 +84,40 @@
                 continue
 
             raise CloudClientError(message="Retries exceeded", cause=request_error)
 
         data: dict = res.json()
         return data
 
-    def variable(self, key: str, user: User) -> Variable:
+    def variable(self, key: str, user: DevCycleUser) -> Variable:
         data = self.request("POST", self._url("variables", key), json=user.to_json())
 
         return Variable(
             _id=data.get("_id"),
-            key=data.get("key"),
-            type=data.get("type"),
+            key=data.get("key", ""),
+            type=data.get("type", ""),
             value=data.get("value"),
         )
 
-    def variables(self, user: User) -> Dict[str, Variable]:
+    def variables(self, user: DevCycleUser) -> Dict[str, Variable]:
         data = self.request("POST", self._url("variables"), json=user.to_json())
 
         result: Dict[str, Variable] = {}
         for key, value in data.items():
             result[key] = Variable(
                 _id=str(value.get("_id")),
                 key=str(value.get("key")),
                 type=str(value.get("type")),
                 value=value.get("value"),
                 isDefaulted=None,
             )
 
         return result
 
-    def features(self, user: User) -> Dict[str, Feature]:
+    def features(self, user: DevCycleUser) -> Dict[str, Feature]:
         data = self.request("POST", self._url("features"), json=user.to_json())
 
         result: Dict[str, Feature] = {}
         for key, value in data.items():
             result[key] = Feature(
                 _id=value.get("_id"),
                 key=value.get("key"),
@@ -127,27 +126,20 @@
                 variationKey=value.get("variationKey"),
                 variationName=value.get("variationName"),
                 evalReason=value.get("evalReason"),
             )
 
         return result
 
-    def track(self, user: User, events: List[Event]) -> str:
+    def track(self, user: DevCycleUser, events: List[DevCycleEvent]) -> str:
         data = self.request(
             "POST",
             self._url("track"),
             json={
                 "user": user.to_json(),
-                "events": [event.to_json() for event in events],
+                "events": [
+                    event.to_json(use_bucketing_api_format=True) for event in events
+                ],
             },
         )
         message = data.get("message", "")
         return message
-
-
-def exponential_backoff(attempt: int, base_delay: float) -> float:
-    """
-    Exponential backoff starting with 200ms +- 0...40ms jitter
-    """
-    delay = math.pow(2, attempt) * base_delay / 2.0
-    random_sum = delay * 0.1 * random.random()
-    return delay + random_sum
```

### Comparing `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/exceptions.py` & `devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 from typing import Optional
 
 
-class CloudClientError(Exception):
+class APIClientError(Exception):
     def __init__(self, message: str, cause: Optional[Exception] = None):
         self.message = message
         self.__cause__ = cause
 
     def __str__(self):
-        return f"CloudClientException: {self.message}"
+        return f"APIClientError: {self.message}"
 
 
-class CloudClientUnauthorizedError(Exception):
+class APIClientUnauthorizedError(Exception):
     def __init__(self, message: str):
         self.message = message
         super().__init__(message)
 
 
+class CloudClientError(APIClientError):
+    def __init__(self, message: str, cause: Optional[Exception] = None):
+        super().__init__(message, cause)
+
+    def __str__(self):
+        return f"CloudClientException: {self.message}"
+
+
+class CloudClientUnauthorizedError(APIClientUnauthorizedError):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
 class NotFoundError(Exception):
     def __init__(self, key: str):
         self.key = key
+
+
+class VariableTypeMismatchError(Exception):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
+class MalformedConfigError(Exception):
+    pass
```

### Comparing `devcycle-python-server-sdk-2.0.1/devcycle_python_sdk/models/variable.py` & `devcycle-python-server-sdk-3.0.0/devcycle_python_sdk/models/variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,28 +22,40 @@
     else:
         raise TypeError(f"Unsupported type: {type(value)}")
 
 
 @dataclass(order=False)
 class Variable:
     _id: Optional[str]
-    key: Optional[str]
-    type: Optional[str]
-    value: Optional[Any] = None
+    key: str
+    type: str
+    value: Any = None
     isDefaulted: Optional[bool] = False
-    defaultValue: Optional[Any] = None
-    # evalReason: Optional[str] = None
+    defaultValue: Any = None
+    evalReason: Optional[str] = None
 
     def to_json(self):
         return {
             key: getattr(self, key)
             for key in self.__dataclass_fields__
             if getattr(self, key) is not None
         }
 
+    @classmethod
+    def from_json(cls, data: dict) -> "Variable":
+        return cls(
+            _id=data["_id"],
+            key=data["key"],
+            type=data["type"],
+            value=data["value"],
+            isDefaulted=data.get("isDefaulted", None),
+            defaultValue=data.get("defaultValue"),
+            evalReason=data.get("evalReason"),
+        )
+
     @staticmethod
     def create_default_variable(key: str, default_value: Any) -> "Variable":
         var_type = determine_variable_type(default_value)
         return Variable(
             _id=None,
             key=key,
             type=var_type,
```

### Comparing `devcycle-python-server-sdk-2.0.1/devcycle_python_server_sdk.egg-info/SOURCES.txt` & `devcycle-python-server-sdk-3.0.0/devcycle_python_server_sdk.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,60 @@
 LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 devcycle_python_sdk/VERSION.txt
 devcycle_python_sdk/__init__.py
-devcycle_python_sdk/dvc_cloud_client.py
-devcycle_python_sdk/dvc_local_client.py
-devcycle_python_sdk/dvc_options.py
+devcycle_python_sdk/cloud_client.py
 devcycle_python_sdk/exceptions.py
+devcycle_python_sdk/local_client.py
+devcycle_python_sdk/options.py
 devcycle_python_sdk/py.typed
 devcycle_python_sdk/api/__init__.py
+devcycle_python_sdk/api/backoff.py
 devcycle_python_sdk/api/bucketing_client.py
+devcycle_python_sdk/api/config_client.py
+devcycle_python_sdk/api/event_client.py
 devcycle_python_sdk/api/local_bucketing.py
 devcycle_python_sdk/managers/__init__.py
 devcycle_python_sdk/managers/config_manager.py
 devcycle_python_sdk/managers/event_queue_manager.py
 devcycle_python_sdk/models/__init__.py
+devcycle_python_sdk/models/bucketed_config.py
 devcycle_python_sdk/models/error_response.py
 devcycle_python_sdk/models/event.py
 devcycle_python_sdk/models/feature.py
+devcycle_python_sdk/models/platform_data.py
 devcycle_python_sdk/models/user.py
 devcycle_python_sdk/models/variable.py
+devcycle_python_sdk/protobuf/__init__.py
+devcycle_python_sdk/protobuf/utils.py
+devcycle_python_sdk/protobuf/variableForUserParams_pb2.py
 devcycle_python_sdk/util/__init__.py
 devcycle_python_sdk/util/version.py
 devcycle_python_server_sdk.egg-info/PKG-INFO
 devcycle_python_server_sdk.egg-info/SOURCES.txt
 devcycle_python_server_sdk.egg-info/dependency_links.txt
 devcycle_python_server_sdk.egg-info/requires.txt
 devcycle_python_server_sdk.egg-info/top_level.txt
 example/__init__.py
-example/example.py
+example/cloud_client_example.py
+example/local_bucketing_client_example.py
 test/__init__.py
-test/test_dvc_cloud_client.py
-test/test_dvc_local_client.py
+test/test_cloud_client.py
+test/test_local_client.py
 test/api/__init__.py
 test/api/test_bucketing_client.py
+test/api/test_config_client.py
+test/api/test_event_client.py
 test/api/test_local_bucketing.py
+test/fixture/__init__.py
+test/fixture/data.py
 test/managers/__init__.py
 test/managers/test_config_manager.py
 test/managers/test_event_queue_manager.py
+test/models/__init__.py
+test/models/test_bucketed_config.py
 test/util/__init__.py
+test/util/test_utils.py
 test/util/test_version.py
```

### Comparing `devcycle-python-server-sdk-2.0.1/example/example.py` & `devcycle-python-server-sdk-3.0.0/example/local_bucketing_client_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,74 @@
 import logging
+import datetime
 import os
+import time
 
-from devcycle_python_sdk import DevCycleCloudClient, DevCycleCloudOptions
-from devcycle_python_sdk.models.user import User
-from devcycle_python_sdk.models.event import Event
+from devcycle_python_sdk import DevCycleLocalClient, DevCycleLocalOptions
+from devcycle_python_sdk.models.user import DevCycleUser
+from devcycle_python_sdk.models.event import DevCycleEvent, EventType
 
 VARIABLE_KEY = "test-boolean-variable"
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     """
-    Sample generic usage of the Python SDK.
+    Sample usage of the Python Server SDK using Local Bucketing.
     For a Django specific sample app, please see https://github.com/DevCycleHQ/python-django-example-app/
-
     """
     logging.basicConfig(level="INFO", format="%(levelname)s: %(message)s")
 
-    options = DevCycleCloudOptions(enable_edge_db=True)
-
-    # create an instance of the API class
-    server_sdk_key = os.environ["DVC_SERVER_SDK_KEY"]
-    dvc = DevCycleCloudClient(server_sdk_key, options)
+    # create an instance of the DevCycle Client object
+    server_sdk_key = os.environ["DEVCYCLE_SERVER_SDK_KEY"]
+    options = DevCycleLocalOptions()
+    client = DevCycleLocalClient(server_sdk_key, options)
+
+    # Wait for DevCycle to initialize and load the configuration
+    while not client.is_initialized():
+        logger.info("Waiting for DevCycle to initialize...")
+        time.sleep(1)
 
-    user = User(user_id="test", email="yo@yo.ca", country="CA")
-    event = Event(type="customEvent", target="somevariable.key")
+    user = DevCycleUser(user_id="test-1234", email="test-user@domain.com", country="US")
 
     # Use variable_value to access the value of a variable directly
-    if dvc.variable_value(user, VARIABLE_KEY, False):
+    if client.variable_value(user, VARIABLE_KEY, False):
         logger.info(f"Variable {VARIABLE_KEY} is enabled")
     else:
         logger.info(f"Variable {VARIABLE_KEY} is not enabled")
 
     # DevCycle handles missing or wrongly typed variables by returning the default value
     # You can check this explicitly by using the variable method
-    variable = dvc.variable(user, VARIABLE_KEY + "-does-not-exist", False)
+    variable = client.variable(user, VARIABLE_KEY + "-does-not-exist", False)
     if variable.isDefaulted:
         logger.info(f"Variable {variable.key} is defaulted to {variable.value}")
 
     try:
         # Get all variables by key for user data
-        all_variables_response = dvc.all_variables(user)
-        logger.info("All variables:\n%s", all_variables_response)
+        all_variables_response = client.all_variables(user)
+        logger.info(f"All variables:\n{all_variables_response}")
 
         if VARIABLE_KEY not in all_variables_response:
             logger.warning(
                 f"Variable {VARIABLE_KEY} does not exist - create it in the dashboard for this example"
             )
 
         # Get all features by key for user data
-        all_features_response = dvc.all_features(user)
-        logger.info("All features:\n%s", all_features_response)
+        all_features_response = client.all_features(user)
+        logger.info(f"All features:\n{all_features_response}")
 
-        # Post events to DevCycle for user
-        track_response = dvc.track(user, event)
-        logger.info(track_response)
+        # Post a custom event to DevCycle for user
+        event = DevCycleEvent(
+            type=EventType.CustomEvent,
+            target="some.variable.key",
+            date=datetime.datetime.now(),
+        )
+        client.track(user, event)
     except Exception as e:
-        logger.exception("Exception when calling Devcycle API: %s\n" % e)
+        logger.exception(f"Exception when calling DevCycle API: {e}")
+    finally:
+        client.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `devcycle-python-server-sdk-2.0.1/setup.py` & `devcycle-python-server-sdk-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `devcycle-python-server-sdk-2.0.1/test/api/test_bucketing_client.py` & `devcycle-python-server-sdk-3.0.0/test/api/test_bucketing_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+import json
 import logging
 import requests
 import responses
 from responses.registries import OrderedRegistry
 import unittest
 import uuid
 
 from devcycle_python_sdk.api.bucketing_client import BucketingAPIClient
 from devcycle_python_sdk.exceptions import (
     CloudClientError,
     CloudClientUnauthorizedError,
     NotFoundError,
 )
-from devcycle_python_sdk.dvc_options import DevCycleCloudOptions
-from devcycle_python_sdk.models.event import Event
+from devcycle_python_sdk.options import DevCycleCloudOptions
+from devcycle_python_sdk.models.event import DevCycleEvent
 from devcycle_python_sdk.models.feature import Feature
-from devcycle_python_sdk.models.user import User
+from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.variable import Variable
 
 logger = logging.getLogger(__name__)
 
 
 class BucketingClientTest(unittest.TestCase):
     def setUp(self) -> None:
         sdk_key = "dvc_server_" + str(uuid.uuid4())
         options = DevCycleCloudOptions(retry_delay=0)
         self.test_client = BucketingAPIClient(sdk_key, options)
-        self.test_user = User(user_id="test_user_id")
+        self.test_user = DevCycleUser(user_id="test_user_id")
 
     @responses.activate
     def test_variable(self):
         responses.add(
             responses.POST,
             "https://bucketing-api.devcycle.com/v1/variables/variable-key",
             json={
@@ -212,17 +213,21 @@
             json={
                 "message": "success",
             },
         )
         result = self.test_client.track(
             self.test_user,
             events=[
-                Event(
+                DevCycleEvent(
                     type="sample-event",
                 )
             ],
         )
         self.assertEqual(result, "success")
+        data = json.loads(responses.calls[0].request.body)
+        self.assertTrue(type(data["events"][0]["date"]) == int)
+        self.assertEqual(len(data["events"]), 1)
+        self.assertEqual(data["events"][0]["type"], "sample-event")
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `devcycle-python-server-sdk-2.0.1/test/test_dvc_cloud_client.py` & `devcycle-python-server-sdk-3.0.0/test/test_cloud_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import unittest
 import uuid
 
 from time import time
 from unittest.mock import patch
 
 from devcycle_python_sdk import DevCycleCloudClient, DevCycleCloudOptions
-from devcycle_python_sdk.models.user import User
+from devcycle_python_sdk.models.user import DevCycleUser
 from devcycle_python_sdk.models.variable import Variable, TypeEnum
-from devcycle_python_sdk.models.event import Event
+from devcycle_python_sdk.models.event import DevCycleEvent
 from devcycle_python_sdk.exceptions import (
     CloudClientUnauthorizedError,
     NotFoundError,
 )
 
 logger = logging.getLogger(__name__)
 
 
-class DVCCloudClientTest(unittest.TestCase):
+class DevCycleCloudClientTest(unittest.TestCase):
     def setUp(self) -> None:
         sdk_key = "dvc_server_" + str(uuid.uuid4())
         options = DevCycleCloudOptions()
         self.test_client = DevCycleCloudClient(sdk_key, options)
-        self.test_user = User(user_id="test_user_id")
-        self.test_user_no_id = User(user_id=None)
-        self.test_user_empty_id = User(user_id="")
+        self.test_user = DevCycleUser(user_id="test_user_id")
+        self.test_user_no_id = DevCycleUser(user_id=None)  # type: ignore
+        self.test_user_empty_id = DevCycleUser(user_id="")
 
     def tearDown(self) -> None:
         pass
 
     def test_create_client_invalid_sdk_key(self):
         with self.assertRaises(ValueError):
             DevCycleCloudClient(None, None)
@@ -51,16 +51,14 @@
         empty_options = DevCycleCloudOptions()
         client = DevCycleCloudClient(sdk_key, empty_options)
         self.assertIsNotNone(client)
 
         option_with_data = DevCycleCloudOptions(
             enable_edge_db=False,
             bucketing_api_uri="https://localhost:8080",
-            config_cdn_uri="https://localhost:8080",
-            events_api_uri="https://localhost:8080",
         )
         client = DevCycleCloudClient(sdk_key, option_with_data)
         self.assertIsNotNone(client)
 
     def test_variable_bad_user(self):
         with self.assertRaises(ValueError):
             self.test_client.variable(None, "strKey", "default_value")
@@ -206,15 +204,15 @@
         mock_features_call.reset_mock()
         mock_features_call.side_effect = Exception("Some error")
         result = self.test_client.all_features(self.test_user)
         self.assertDictEqual(result, {})
 
     @patch("devcycle_python_sdk.api.bucketing_client.BucketingAPIClient.track")
     def test_track_event_bad_user(self, mock_track_call):
-        event = Event(
+        event = DevCycleEvent(
             type="user",
             target="test_target",
             date=time(),
             value=42,
             metaData={"key": "value"},
         )
 
@@ -232,60 +230,56 @@
 
     @patch("devcycle_python_sdk.api.bucketing_client.BucketingAPIClient.track")
     def test_track_bad_event(self, mock_track_call):
         with self.assertRaises(ValueError):
             self.test_client.track(self.test_user, None)
         mock_track_call.assert_not_called()
 
-        event = Event(
+        event = DevCycleEvent(
             type=None,
             target="test_target",
-            date=time(),
             value=42,
             metaData={"key": "value"},
         )
         with self.assertRaises(ValueError):
             self.test_client.track(self.test_user, event)
         mock_track_call.assert_not_called()
 
-        event = Event(
+        event = DevCycleEvent(
             type="",
             target="test_target",
-            date=time(),
             value=42,
             metaData={"key": "value"},
         )
         with self.assertRaises(ValueError):
             self.test_client.track(self.test_user, event)
         mock_track_call.assert_not_called()
 
     @patch("devcycle_python_sdk.api.bucketing_client.BucketingAPIClient.track")
     def test_track_exceptions(self, mock_track_call):
         # unauthorized - return error
         mock_track_call.side_effect = CloudClientUnauthorizedError("No auth")
         with self.assertRaises(CloudClientUnauthorizedError):
             self.test_client.track(
                 self.test_user,
-                Event(
+                DevCycleEvent(
                     type="user",
                     target="test_target",
-                    date=time(),
                     value=42,
                     metaData={"key": "value"},
                 ),
             )
 
         # other error - shouldn't propagate
         mock_track_call.side_effect = Exception("Some error")
         self.test_client.track(
             self.test_user,
-            Event(
+            DevCycleEvent(
                 type="user",
                 target="test_target",
-                date=time(),
                 value=42,
                 metaData={"key": "value"},
             ),
         )
 
 
 if __name__ == "__main__":
```

