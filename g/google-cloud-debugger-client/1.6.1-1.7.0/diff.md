# Comparing `tmp/google-cloud-debugger-client-1.6.1.tar.gz` & `tmp/google-cloud-debugger-client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-debugger-client-1.6.1.tar", last modified: Mon Jan 23 16:18:58 2023, max compression
+gzip compressed data, was "google-cloud-debugger-client-1.7.0.tar", last modified: Thu Jul  6 16:16:34 2023, max compression
```

## Comparing `google-cloud-debugger-client-1.6.1.tar` & `google-cloud-debugger-client-1.7.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.222741 google-cloud-debugger-client-1.6.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4818 2023-01-23 16:18:58.222741 google-cloud-debugger-client-1.6.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3878 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.210741 google-cloud-debugger-client-1.6.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.210741 google-cloud-debugger-client-1.6.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger/
--rw-rw-r--   0 root         (0)     1003     2531 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/
--rw-rw-r--   0 root         (0)     1003     2241 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     2877 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/
--rw-rw-r--   0 root         (0)     1003      757 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/__init__.py
--rw-rw-r--   0 root         (0)     1003    25446 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/async_client.py
--rw-rw-r--   0 root         (0)     1003    33603 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8013 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17193 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17448 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.214741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/
--rw-rw-r--   0 root         (0)     1003      749 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/__init__.py
--rw-rw-r--   0 root         (0)     1003    35158 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/async_client.py
--rw-rw-r--   0 root         (0)     1003    42898 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/
--rw-rw-r--   0 root         (0)     1003     1148 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9587 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/base.py
--rw-rw-r--   0 root         (0)     1003    16931 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17275 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/
--rw-rw-r--   0 root         (0)     1003     1859 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     5468 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/controller.py
--rw-rw-r--   0 root         (0)     1003    23962 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/data.py
--rw-rw-r--   0 root         (0)     1003     9547 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/debugger.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/
--rw-r--r--   0 root         (0)     1003     4818 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1987 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      360 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:18:58.000000 google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:18:58.222741 google-cloud-debugger-client-1.6.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3054 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:58.218741 google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003    74282 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/test_controller2.py
--rw-rw-r--   0 root         (0)     1003    91474 2023-01-23 16:15:37.000000 google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/test_debugger2.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4818 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3878 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.341865 google-cloud-debugger-client-1.7.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.341865 google-cloud-debugger-client-1.7.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.345866 google-cloud-debugger-client-1.7.0/google/cloud/debugger/
+-rw-rw-r--   0 root         (0)     1003     2531 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.345866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/
+-rw-rw-r--   0 root         (0)     1003     2244 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4119 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.345866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.345866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/
+-rw-rw-r--   0 root         (0)     1003      757 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25474 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/async_client.py
+-rw-rw-r--   0 root         (0)     1003    33716 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.349866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8013 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17193 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17448 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    24332 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.349866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/
+-rw-rw-r--   0 root         (0)     1003      749 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35184 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43007 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.349866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/
+-rw-rw-r--   0 root         (0)     1003     1330 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9587 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    16931 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17275 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    31936 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.349866 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1859 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5504 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/controller.py
+-rw-rw-r--   0 root         (0)     1003    23998 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/data.py
+-rw-rw-r--   0 root         (0)     1003     9583 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/debugger.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/
+-rw-r--r--   0 root         (0)     1003     4818 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2115 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      360 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-07-06 16:16:34.000000 google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3054 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-07-06 16:16:34.353867 google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   106826 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/test_controller2.py
+-rw-rw-r--   0 root         (0)     1003   149820 2023-07-06 16:13:32.000000 google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/test_debugger2.py
```

### Comparing `google-cloud-debugger-client-1.6.1/LICENSE` & `google-cloud-debugger-client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/MANIFEST.in` & `google-cloud-debugger-client-1.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/PKG-INFO` & `google-cloud-debugger-client-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-debugger-client
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Debugger Client API client library
 Home-page: https://github.com/googleapis/python-debugger-client
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-debugger-client-1.6.1/README.rst` & `google-cloud-debugger-client-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger/gapic_version.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from google.cloud.debugger import gapic_version as package_version
+from google.cloud.debugger_v2 import gapic_version as package_version
 
 __version__ = package_version.__version__
 
 
 from .services.controller2 import Controller2AsyncClient, Controller2Client
 from .services.debugger2 import Debugger2AsyncClient, Debugger2Client
 from .types.controller import (
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/gapic_metadata.json` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/gapic_metadata.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555555%*

 * *Differences: {"'services'": "{'Controller2': {'clients': {'rest': OrderedDict([('libraryClient', "*

 * *               "'Controller2Client'), ('rpcs', OrderedDict([('ListActiveBreakpoints', "*

 * *               "OrderedDict([('methods', ['list_active_breakpoints'])])), ('RegisterDebuggee', "*

 * *               "OrderedDict([('methods', ['register_debuggee'])])), ('UpdateActiveBreakpoint', "*

 * *               "OrderedDict([('methods', ['update_active_breakpoint'])]))]))])}}, 'Debugger2': "*

 * *               "{'clients': {'rest': OrderedDic […]*

```diff
@@ -42,14 +42,34 @@
                         },
                         "UpdateActiveBreakpoint": {
                             "methods": [
                                 "update_active_breakpoint"
                             ]
                         }
                     }
+                },
+                "rest": {
+                    "libraryClient": "Controller2Client",
+                    "rpcs": {
+                        "ListActiveBreakpoints": {
+                            "methods": [
+                                "list_active_breakpoints"
+                            ]
+                        },
+                        "RegisterDebuggee": {
+                            "methods": [
+                                "register_debuggee"
+                            ]
+                        },
+                        "UpdateActiveBreakpoint": {
+                            "methods": [
+                                "update_active_breakpoint"
+                            ]
+                        }
+                    }
                 }
             }
         },
         "Debugger2": {
             "clients": {
                 "grpc": {
                     "libraryClient": "Debugger2Client",
@@ -86,14 +106,44 @@
                     "rpcs": {
                         "DeleteBreakpoint": {
                             "methods": [
                                 "delete_breakpoint"
                             ]
                         },
                         "GetBreakpoint": {
+                            "methods": [
+                                "get_breakpoint"
+                            ]
+                        },
+                        "ListBreakpoints": {
+                            "methods": [
+                                "list_breakpoints"
+                            ]
+                        },
+                        "ListDebuggees": {
+                            "methods": [
+                                "list_debuggees"
+                            ]
+                        },
+                        "SetBreakpoint": {
+                            "methods": [
+                                "set_breakpoint"
+                            ]
+                        }
+                    }
+                },
+                "rest": {
+                    "libraryClient": "Debugger2Client",
+                    "rpcs": {
+                        "DeleteBreakpoint": {
+                            "methods": [
+                                "delete_breakpoint"
+                            ]
+                        },
+                        "GetBreakpoint": {
                             "methods": [
                                 "get_breakpoint"
                             ]
                         },
                         "ListBreakpoints": {
                             "methods": [
                                 "list_breakpoints"
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/gapic_version.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/gapic_version.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.6.1"  # {x-release-please-version}
+__version__ = "1.7.0"  # {x-release-please-version}
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/async_client.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,15 +590,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "Controller2AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/client.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,27 +47,29 @@
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.debugger_v2.types import controller, data
 
 from .transports.base import DEFAULT_CLIENT_INFO, Controller2Transport
 from .transports.grpc import Controller2GrpcTransport
 from .transports.grpc_asyncio import Controller2GrpcAsyncIOTransport
+from .transports.rest import Controller2RestTransport
 
 
 class Controller2ClientMeta(type):
     """Metaclass for the Controller2 client.
 
     This provides class-level methods for building and retrieving
     support objects (e.g. transport) without polluting the client instance
     objects.
     """
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[Controller2Transport]]
     _transport_registry["grpc"] = Controller2GrpcTransport
     _transport_registry["grpc_asyncio"] = Controller2GrpcAsyncIOTransport
+    _transport_registry["rest"] = Controller2RestTransport
 
     def get_transport_class(
         cls,
         label: Optional[str] = None,
     ) -> Type[Controller2Transport]:
         """Returns an appropriate transport class.
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from collections import OrderedDict
 from typing import Dict, Type
 
-from .base import Controller2Transport
-from .grpc import Controller2GrpcTransport
-from .grpc_asyncio import Controller2GrpcAsyncIOTransport
+from .base import Debugger2Transport
+from .grpc import Debugger2GrpcTransport
+from .grpc_asyncio import Debugger2GrpcAsyncIOTransport
+from .rest import Debugger2RestInterceptor, Debugger2RestTransport
 
 # Compile a registry of transports.
-_transport_registry = OrderedDict()  # type: Dict[str, Type[Controller2Transport]]
-_transport_registry["grpc"] = Controller2GrpcTransport
-_transport_registry["grpc_asyncio"] = Controller2GrpcAsyncIOTransport
+_transport_registry = OrderedDict()  # type: Dict[str, Type[Debugger2Transport]]
+_transport_registry["grpc"] = Debugger2GrpcTransport
+_transport_registry["grpc_asyncio"] = Debugger2GrpcAsyncIOTransport
+_transport_registry["rest"] = Debugger2RestTransport
 
 __all__ = (
-    "Controller2Transport",
-    "Controller2GrpcTransport",
-    "Controller2GrpcAsyncIOTransport",
+    "Debugger2Transport",
+    "Debugger2GrpcTransport",
+    "Debugger2GrpcAsyncIOTransport",
+    "Debugger2RestTransport",
+    "Debugger2RestInterceptor",
 )
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/base.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/grpc.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/controller2/transports/grpc_asyncio.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/controller2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/async_client.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,15 +842,15 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
-    async def __aenter__(self):
+    async def __aenter__(self) -> "Debugger2AsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
 
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/client.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,27 +47,29 @@
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.cloud.debugger_v2.types import data, debugger
 
 from .transports.base import DEFAULT_CLIENT_INFO, Debugger2Transport
 from .transports.grpc import Debugger2GrpcTransport
 from .transports.grpc_asyncio import Debugger2GrpcAsyncIOTransport
+from .transports.rest import Debugger2RestTransport
 
 
 class Debugger2ClientMeta(type):
     """Metaclass for the Debugger2 client.
 
     This provides class-level methods for building and retrieving
     support objects (e.g. transport) without polluting the client instance
     objects.
     """
 
     _transport_registry = OrderedDict()  # type: Dict[str, Type[Debugger2Transport]]
     _transport_registry["grpc"] = Debugger2GrpcTransport
     _transport_registry["grpc_asyncio"] = Debugger2GrpcAsyncIOTransport
+    _transport_registry["rest"] = Debugger2RestTransport
 
     def get_transport_class(
         cls,
         label: Optional[str] = None,
     ) -> Type[Debugger2Transport]:
         """Returns an appropriate transport class.
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/base.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/grpc.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/services/debugger2/transports/grpc_asyncio.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/services/debugger2/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/__init__.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/controller.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.cloud.debugger_v2.types import data
 
 __protobuf__ = proto.module(
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/data.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 from google.cloud.source_context_v1.types import (
     source_context as source_context_pb2,
 )  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
```

### Comparing `google-cloud-debugger-client-1.6.1/google/cloud/debugger_v2/types/debugger.py` & `google-cloud-debugger-client-1.7.0/google/cloud/debugger_v2/types/debugger.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from __future__ import annotations
+
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 from google.cloud.debugger_v2.types import data
 
 __protobuf__ = proto.module(
```

### Comparing `google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/PKG-INFO` & `google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-debugger-client
-Version: 1.6.1
+Version: 1.7.0
 Summary: Google Cloud Debugger Client API client library
 Home-page: https://github.com/googleapis/python-debugger-client
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-debugger-client-1.6.1/google_cloud_debugger_client.egg-info/SOURCES.txt` & `google-cloud-debugger-client-1.7.0/google_cloud_debugger_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,23 @@
 google/cloud/debugger_v2/services/controller2/__init__.py
 google/cloud/debugger_v2/services/controller2/async_client.py
 google/cloud/debugger_v2/services/controller2/client.py
 google/cloud/debugger_v2/services/controller2/transports/__init__.py
 google/cloud/debugger_v2/services/controller2/transports/base.py
 google/cloud/debugger_v2/services/controller2/transports/grpc.py
 google/cloud/debugger_v2/services/controller2/transports/grpc_asyncio.py
+google/cloud/debugger_v2/services/controller2/transports/rest.py
 google/cloud/debugger_v2/services/debugger2/__init__.py
 google/cloud/debugger_v2/services/debugger2/async_client.py
 google/cloud/debugger_v2/services/debugger2/client.py
 google/cloud/debugger_v2/services/debugger2/transports/__init__.py
 google/cloud/debugger_v2/services/debugger2/transports/base.py
 google/cloud/debugger_v2/services/debugger2/transports/grpc.py
 google/cloud/debugger_v2/services/debugger2/transports/grpc_asyncio.py
+google/cloud/debugger_v2/services/debugger2/transports/rest.py
 google/cloud/debugger_v2/types/__init__.py
 google/cloud/debugger_v2/types/controller.py
 google/cloud/debugger_v2/types/data.py
 google/cloud/debugger_v2/types/debugger.py
 google_cloud_debugger_client.egg-info/PKG-INFO
 google_cloud_debugger_client.egg-info/SOURCES.txt
 google_cloud_debugger_client.egg-info/dependency_links.txt
```

### Comparing `google-cloud-debugger-client-1.6.1/setup.py` & `google-cloud-debugger-client-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/tests/__init__.py` & `google-cloud-debugger-client-1.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/tests/unit/__init__.py` & `google-cloud-debugger-client-1.7.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/tests/unit/gapic/__init__.py` & `google-cloud-debugger-client-1.7.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/__init__.py` & `google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-debugger-client-1.6.1/tests/unit/gapic/debugger_v2/test_controller2.py` & `google-cloud-debugger-client-1.7.0/tests/unit/gapic/debugger_v2/test_controller2.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,33 +18,38 @@
 # try/except added for compatibility with python < 3.8
 try:
     from unittest import mock
     from unittest.mock import AsyncMock  # pragma: NO COVER
 except ImportError:  # pragma: NO COVER
     import mock
 
+from collections.abc import Iterable
+import json
 import math
 
 from google.api_core import gapic_v1, grpc_helpers, grpc_helpers_async, path_template
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
 from google.cloud.source_context_v1.types import (
     source_context as source_context_pb2,
 )  # type: ignore
 from google.oauth2 import service_account
+from google.protobuf import json_format
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.protobuf import wrappers_pb2  # type: ignore
 import grpc
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
+from requests import PreparedRequest, Request, Response
+from requests.sessions import Session
 
 from google.cloud.debugger_v2.services.controller2 import (
     Controller2AsyncClient,
     Controller2Client,
     transports,
 )
 from google.cloud.debugger_v2.types import controller, data
@@ -92,35 +97,41 @@
 
 
 @pytest.mark.parametrize(
     "client_class,transport_name",
     [
         (Controller2Client, "grpc"),
         (Controller2AsyncClient, "grpc_asyncio"),
+        (Controller2Client, "rest"),
     ],
 )
 def test_controller2_client_from_service_account_info(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_info"
     ) as factory:
         factory.return_value = creds
         info = {"valid": True}
         client = client_class.from_service_account_info(info, transport=transport_name)
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == ("clouddebugger.googleapis.com:443")
+        assert client.transport._host == (
+            "clouddebugger.googleapis.com:443"
+            if transport_name in ["grpc", "grpc_asyncio"]
+            else "https://clouddebugger.googleapis.com"
+        )
 
 
 @pytest.mark.parametrize(
     "transport_class,transport_name",
     [
         (transports.Controller2GrpcTransport, "grpc"),
         (transports.Controller2GrpcAsyncIOTransport, "grpc_asyncio"),
+        (transports.Controller2RestTransport, "rest"),
     ],
 )
 def test_controller2_client_service_account_always_use_jwt(
     transport_class, transport_name
 ):
     with mock.patch.object(
         service_account.Credentials, "with_always_use_jwt_access", create=True
@@ -138,14 +149,15 @@
 
 
 @pytest.mark.parametrize(
     "client_class,transport_name",
     [
         (Controller2Client, "grpc"),
         (Controller2AsyncClient, "grpc_asyncio"),
+        (Controller2Client, "rest"),
     ],
 )
 def test_controller2_client_from_service_account_file(client_class, transport_name):
     creds = ga_credentials.AnonymousCredentials()
     with mock.patch.object(
         service_account.Credentials, "from_service_account_file"
     ) as factory:
@@ -158,21 +170,26 @@
 
         client = client_class.from_service_account_json(
             "dummy/file/path.json", transport=transport_name
         )
         assert client.transport._credentials == creds
         assert isinstance(client, client_class)
 
-        assert client.transport._host == ("clouddebugger.googleapis.com:443")
+        assert client.transport._host == (
+            "clouddebugger.googleapis.com:443"
+            if transport_name in ["grpc", "grpc_asyncio"]
+            else "https://clouddebugger.googleapis.com"
+        )
 
 
 def test_controller2_client_get_transport_class():
     transport = Controller2Client.get_transport_class()
     available_transports = [
         transports.Controller2GrpcTransport,
+        transports.Controller2RestTransport,
     ]
     assert transport in available_transports
 
     transport = Controller2Client.get_transport_class("grpc")
     assert transport == transports.Controller2GrpcTransport
 
 
@@ -181,14 +198,15 @@
     [
         (Controller2Client, transports.Controller2GrpcTransport, "grpc"),
         (
             Controller2AsyncClient,
             transports.Controller2GrpcAsyncIOTransport,
             "grpc_asyncio",
         ),
+        (Controller2Client, transports.Controller2RestTransport, "rest"),
     ],
 )
 @mock.patch.object(
     Controller2Client, "DEFAULT_ENDPOINT", modify_default_endpoint(Controller2Client)
 )
 @mock.patch.object(
     Controller2AsyncClient,
@@ -324,14 +342,16 @@
         (Controller2Client, transports.Controller2GrpcTransport, "grpc", "false"),
         (
             Controller2AsyncClient,
             transports.Controller2GrpcAsyncIOTransport,
             "grpc_asyncio",
             "false",
         ),
+        (Controller2Client, transports.Controller2RestTransport, "rest", "true"),
+        (Controller2Client, transports.Controller2RestTransport, "rest", "false"),
     ],
 )
 @mock.patch.object(
     Controller2Client, "DEFAULT_ENDPOINT", modify_default_endpoint(Controller2Client)
 )
 @mock.patch.object(
     Controller2AsyncClient,
@@ -517,14 +537,15 @@
     [
         (Controller2Client, transports.Controller2GrpcTransport, "grpc"),
         (
             Controller2AsyncClient,
             transports.Controller2GrpcAsyncIOTransport,
             "grpc_asyncio",
         ),
+        (Controller2Client, transports.Controller2RestTransport, "rest"),
     ],
 )
 def test_controller2_client_client_options_scopes(
     client_class, transport_class, transport_name
 ):
     # Check the case scopes are provided.
     options = client_options.ClientOptions(
@@ -552,14 +573,15 @@
         (Controller2Client, transports.Controller2GrpcTransport, "grpc", grpc_helpers),
         (
             Controller2AsyncClient,
             transports.Controller2GrpcAsyncIOTransport,
             "grpc_asyncio",
             grpc_helpers_async,
         ),
+        (Controller2Client, transports.Controller2RestTransport, "rest", None),
     ],
 )
 def test_controller2_client_client_options_credentials_file(
     client_class, transport_class, transport_name, grpc_helpers
 ):
     # Check the case credentials file is provided.
     options = client_options.ClientOptions(credentials_file="credentials.json")
@@ -1339,14 +1361,834 @@
         await client.update_active_breakpoint(
             controller.UpdateActiveBreakpointRequest(),
             debuggee_id="debuggee_id_value",
             breakpoint_=data.Breakpoint(id="id_value"),
         )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        controller.RegisterDebuggeeRequest,
+        dict,
+    ],
+)
+def test_register_debuggee_rest(request_type):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.RegisterDebuggeeResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.RegisterDebuggeeResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.register_debuggee(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, controller.RegisterDebuggeeResponse)
+
+
+def test_register_debuggee_rest_required_fields(
+    request_type=controller.RegisterDebuggeeRequest,
+):
+    transport_class = transports.Controller2RestTransport
+
+    request_init = {}
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).register_debuggee._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).register_debuggee._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = controller.RegisterDebuggeeResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "post",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = controller.RegisterDebuggeeResponse.pb(return_value)
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.register_debuggee(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_register_debuggee_rest_unset_required_fields():
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.register_debuggee._get_unset_required_fields({})
+    assert set(unset_fields) == (set(()) & set(("debuggee",)))
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_register_debuggee_rest_interceptors(null_interceptor):
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.Controller2RestInterceptor(),
+    )
+    client = Controller2Client(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.Controller2RestInterceptor, "post_register_debuggee"
+    ) as post, mock.patch.object(
+        transports.Controller2RestInterceptor, "pre_register_debuggee"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = controller.RegisterDebuggeeRequest.pb(
+            controller.RegisterDebuggeeRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = controller.RegisterDebuggeeResponse.to_json(
+            controller.RegisterDebuggeeResponse()
+        )
+
+        request = controller.RegisterDebuggeeRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = controller.RegisterDebuggeeResponse()
+
+        client.register_debuggee(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_register_debuggee_rest_bad_request(
+    transport: str = "rest", request_type=controller.RegisterDebuggeeRequest
+):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.register_debuggee(request)
+
+
+def test_register_debuggee_rest_flattened():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.RegisterDebuggeeResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            debuggee=data.Debuggee(id="id_value"),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.RegisterDebuggeeResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.register_debuggee(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v2/controller/debuggees/register" % client.transport._host, args[1]
+        )
+
+
+def test_register_debuggee_rest_flattened_error(transport: str = "rest"):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.register_debuggee(
+            controller.RegisterDebuggeeRequest(),
+            debuggee=data.Debuggee(id="id_value"),
+        )
+
+
+def test_register_debuggee_rest_error():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        controller.ListActiveBreakpointsRequest,
+        dict,
+    ],
+)
+def test_list_active_breakpoints_rest(request_type):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"debuggee_id": "sample1"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.ListActiveBreakpointsResponse(
+            next_wait_token="next_wait_token_value",
+            wait_expired=True,
+        )
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.ListActiveBreakpointsResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.list_active_breakpoints(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, controller.ListActiveBreakpointsResponse)
+    assert response.next_wait_token == "next_wait_token_value"
+    assert response.wait_expired is True
+
+
+def test_list_active_breakpoints_rest_required_fields(
+    request_type=controller.ListActiveBreakpointsRequest,
+):
+    transport_class = transports.Controller2RestTransport
+
+    request_init = {}
+    request_init["debuggee_id"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_active_breakpoints._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["debuggeeId"] = "debuggee_id_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).list_active_breakpoints._get_unset_required_fields(jsonified_request)
+    # Check that path parameters and body parameters are not mixing in.
+    assert not set(unset_fields) - set(
+        (
+            "success_on_timeout",
+            "wait_token",
+        )
+    )
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "debuggeeId" in jsonified_request
+    assert jsonified_request["debuggeeId"] == "debuggee_id_value"
+
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = controller.ListActiveBreakpointsResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "get",
+                "query_params": pb_request,
+            }
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = controller.ListActiveBreakpointsResponse.pb(return_value)
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.list_active_breakpoints(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_list_active_breakpoints_rest_unset_required_fields():
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.list_active_breakpoints._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(
+            (
+                "successOnTimeout",
+                "waitToken",
+            )
+        )
+        & set(("debuggeeId",))
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_list_active_breakpoints_rest_interceptors(null_interceptor):
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.Controller2RestInterceptor(),
+    )
+    client = Controller2Client(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.Controller2RestInterceptor, "post_list_active_breakpoints"
+    ) as post, mock.patch.object(
+        transports.Controller2RestInterceptor, "pre_list_active_breakpoints"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = controller.ListActiveBreakpointsRequest.pb(
+            controller.ListActiveBreakpointsRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = controller.ListActiveBreakpointsResponse.to_json(
+            controller.ListActiveBreakpointsResponse()
+        )
+
+        request = controller.ListActiveBreakpointsRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = controller.ListActiveBreakpointsResponse()
+
+        client.list_active_breakpoints(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_list_active_breakpoints_rest_bad_request(
+    transport: str = "rest", request_type=controller.ListActiveBreakpointsRequest
+):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"debuggee_id": "sample1"}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_active_breakpoints(request)
+
+
+def test_list_active_breakpoints_rest_flattened():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.ListActiveBreakpointsResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"debuggee_id": "sample1"}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            debuggee_id="debuggee_id_value",
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.ListActiveBreakpointsResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.list_active_breakpoints(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v2/controller/debuggees/{debuggee_id}/breakpoints"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_list_active_breakpoints_rest_flattened_error(transport: str = "rest"):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_active_breakpoints(
+            controller.ListActiveBreakpointsRequest(),
+            debuggee_id="debuggee_id_value",
+        )
+
+
+def test_list_active_breakpoints_rest_error():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        controller.UpdateActiveBreakpointRequest,
+        dict,
+    ],
+)
+def test_update_active_breakpoint_rest(request_type):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"debuggee_id": "sample1", "breakpoint_": {"id": "sample2"}}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.UpdateActiveBreakpointResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.UpdateActiveBreakpointResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+        response = client.update_active_breakpoint(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, controller.UpdateActiveBreakpointResponse)
+
+
+def test_update_active_breakpoint_rest_required_fields(
+    request_type=controller.UpdateActiveBreakpointRequest,
+):
+    transport_class = transports.Controller2RestTransport
+
+    request_init = {}
+    request_init["debuggee_id"] = ""
+    request = request_type(**request_init)
+    pb_request = request_type.pb(request)
+    jsonified_request = json.loads(
+        json_format.MessageToJson(
+            pb_request,
+            including_default_value_fields=False,
+            use_integers_for_enums=False,
+        )
+    )
+
+    # verify fields with default values are dropped
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_active_breakpoint._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with default values are now present
+
+    jsonified_request["debuggeeId"] = "debuggee_id_value"
+
+    unset_fields = transport_class(
+        credentials=ga_credentials.AnonymousCredentials()
+    ).update_active_breakpoint._get_unset_required_fields(jsonified_request)
+    jsonified_request.update(unset_fields)
+
+    # verify required fields with non-default values are left alone
+    assert "debuggeeId" in jsonified_request
+    assert jsonified_request["debuggeeId"] == "debuggee_id_value"
+
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request = request_type(**request_init)
+
+    # Designate an appropriate value for the returned response.
+    return_value = controller.UpdateActiveBreakpointResponse()
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(Session, "request") as req:
+        # We need to mock transcode() because providing default values
+        # for required fields will fail the real version if the http_options
+        # expect actual values for those fields.
+        with mock.patch.object(path_template, "transcode") as transcode:
+            # A uri without fields and an empty body will force all the
+            # request fields to show up in the query_params.
+            pb_request = request_type.pb(request)
+            transcode_result = {
+                "uri": "v1/sample_method",
+                "method": "put",
+                "query_params": pb_request,
+            }
+            transcode_result["body"] = pb_request
+            transcode.return_value = transcode_result
+
+            response_value = Response()
+            response_value.status_code = 200
+
+            pb_return_value = controller.UpdateActiveBreakpointResponse.pb(return_value)
+            json_return_value = json_format.MessageToJson(pb_return_value)
+
+            response_value._content = json_return_value.encode("UTF-8")
+            req.return_value = response_value
+
+            response = client.update_active_breakpoint(request)
+
+            expected_params = [("$alt", "json;enum-encoding=int")]
+            actual_params = req.call_args.kwargs["params"]
+            assert expected_params == actual_params
+
+
+def test_update_active_breakpoint_rest_unset_required_fields():
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials
+    )
+
+    unset_fields = transport.update_active_breakpoint._get_unset_required_fields({})
+    assert set(unset_fields) == (
+        set(())
+        & set(
+            (
+                "debuggeeId",
+                "breakpoint",
+            )
+        )
+    )
+
+
+@pytest.mark.parametrize("null_interceptor", [True, False])
+def test_update_active_breakpoint_rest_interceptors(null_interceptor):
+    transport = transports.Controller2RestTransport(
+        credentials=ga_credentials.AnonymousCredentials(),
+        interceptor=None
+        if null_interceptor
+        else transports.Controller2RestInterceptor(),
+    )
+    client = Controller2Client(transport=transport)
+    with mock.patch.object(
+        type(client.transport._session), "request"
+    ) as req, mock.patch.object(
+        path_template, "transcode"
+    ) as transcode, mock.patch.object(
+        transports.Controller2RestInterceptor, "post_update_active_breakpoint"
+    ) as post, mock.patch.object(
+        transports.Controller2RestInterceptor, "pre_update_active_breakpoint"
+    ) as pre:
+        pre.assert_not_called()
+        post.assert_not_called()
+        pb_message = controller.UpdateActiveBreakpointRequest.pb(
+            controller.UpdateActiveBreakpointRequest()
+        )
+        transcode.return_value = {
+            "method": "post",
+            "uri": "my_uri",
+            "body": pb_message,
+            "query_params": pb_message,
+        }
+
+        req.return_value = Response()
+        req.return_value.status_code = 200
+        req.return_value.request = PreparedRequest()
+        req.return_value._content = controller.UpdateActiveBreakpointResponse.to_json(
+            controller.UpdateActiveBreakpointResponse()
+        )
+
+        request = controller.UpdateActiveBreakpointRequest()
+        metadata = [
+            ("key", "val"),
+            ("cephalopod", "squid"),
+        ]
+        pre.return_value = request, metadata
+        post.return_value = controller.UpdateActiveBreakpointResponse()
+
+        client.update_active_breakpoint(
+            request,
+            metadata=[
+                ("key", "val"),
+                ("cephalopod", "squid"),
+            ],
+        )
+
+        pre.assert_called_once()
+        post.assert_called_once()
+
+
+def test_update_active_breakpoint_rest_bad_request(
+    transport: str = "rest", request_type=controller.UpdateActiveBreakpointRequest
+):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # send a request that will satisfy transcoding
+    request_init = {"debuggee_id": "sample1", "breakpoint_": {"id": "sample2"}}
+    request = request_type(**request_init)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.update_active_breakpoint(request)
+
+
+def test_update_active_breakpoint_rest_flattened():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = controller.UpdateActiveBreakpointResponse()
+
+        # get arguments that satisfy an http rule for this method
+        sample_request = {"debuggee_id": "sample1", "breakpoint_": {"id": "sample2"}}
+
+        # get truthy value for each flattened field
+        mock_args = dict(
+            debuggee_id="debuggee_id_value",
+            breakpoint_=data.Breakpoint(id="id_value"),
+        )
+        mock_args.update(sample_request)
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        pb_return_value = controller.UpdateActiveBreakpointResponse.pb(return_value)
+        json_return_value = json_format.MessageToJson(pb_return_value)
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        client.update_active_breakpoint(**mock_args)
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(req.mock_calls) == 1
+        _, args, _ = req.mock_calls[0]
+        assert path_template.validate(
+            "%s/v2/controller/debuggees/{debuggee_id}/breakpoints/{breakpoint_.id}"
+            % client.transport._host,
+            args[1],
+        )
+
+
+def test_update_active_breakpoint_rest_flattened_error(transport: str = "rest"):
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.update_active_breakpoint(
+            controller.UpdateActiveBreakpointRequest(),
+            debuggee_id="debuggee_id_value",
+            breakpoint_=data.Breakpoint(id="id_value"),
+        )
+
+
+def test_update_active_breakpoint_rest_error():
+    client = Controller2Client(
+        credentials=ga_credentials.AnonymousCredentials(), transport="rest"
+    )
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.Controller2GrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = Controller2Client(
@@ -1420,28 +2262,30 @@
 
 
 @pytest.mark.parametrize(
     "transport_class",
     [
         transports.Controller2GrpcTransport,
         transports.Controller2GrpcAsyncIOTransport,
+        transports.Controller2RestTransport,
     ],
 )
 def test_transport_adc(transport_class):
     # Test default credentials are used if not provided.
     with mock.patch.object(google.auth, "default") as adc:
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport_class()
         adc.assert_called_once()
 
 
 @pytest.mark.parametrize(
     "transport_name",
     [
         "grpc",
+        "rest",
     ],
 )
 def test_transport_kind(transport_name):
     transport = Controller2Client.get_transport_class(transport_name)(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     assert transport.kind == transport_name
@@ -1574,14 +2418,15 @@
 
 
 @pytest.mark.parametrize(
     "transport_class",
     [
         transports.Controller2GrpcTransport,
         transports.Controller2GrpcAsyncIOTransport,
+        transports.Controller2RestTransport,
     ],
 )
 def test_controller2_transport_auth_gdch_credentials(transport_class):
     host = "https://language.com"
     api_audience_tests = [None, "https://language2.com"]
     api_audience_expect = [host, "https://language2.com"]
     for t, e in zip(api_audience_tests, api_audience_expect):
@@ -1671,48 +2516,97 @@
             )
             expected_cert, expected_key = client_cert_source_callback()
             mock_ssl_cred.assert_called_once_with(
                 certificate_chain=expected_cert, private_key=expected_key
             )
 
 
+def test_controller2_http_transport_client_cert_source_for_mtls():
+    cred = ga_credentials.AnonymousCredentials()
+    with mock.patch(
+        "google.auth.transport.requests.AuthorizedSession.configure_mtls_channel"
+    ) as mock_configure_mtls_channel:
+        transports.Controller2RestTransport(
+            credentials=cred, client_cert_source_for_mtls=client_cert_source_callback
+        )
+        mock_configure_mtls_channel.assert_called_once_with(client_cert_source_callback)
+
+
 @pytest.mark.parametrize(
     "transport_name",
     [
         "grpc",
         "grpc_asyncio",
+        "rest",
     ],
 )
 def test_controller2_host_no_port(transport_name):
     client = Controller2Client(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="clouddebugger.googleapis.com"
         ),
         transport=transport_name,
     )
-    assert client.transport._host == ("clouddebugger.googleapis.com:443")
+    assert client.transport._host == (
+        "clouddebugger.googleapis.com:443"
+        if transport_name in ["grpc", "grpc_asyncio"]
+        else "https://clouddebugger.googleapis.com"
+    )
 
 
 @pytest.mark.parametrize(
     "transport_name",
     [
         "grpc",
         "grpc_asyncio",
+        "rest",
     ],
 )
 def test_controller2_host_with_port(transport_name):
     client = Controller2Client(
         credentials=ga_credentials.AnonymousCredentials(),
         client_options=client_options.ClientOptions(
             api_endpoint="clouddebugger.googleapis.com:8000"
         ),
         transport=transport_name,
     )
-    assert client.transport._host == ("clouddebugger.googleapis.com:8000")
+    assert client.transport._host == (
+        "clouddebugger.googleapis.com:8000"
+        if transport_name in ["grpc", "grpc_asyncio"]
+        else "https://clouddebugger.googleapis.com:8000"
+    )
+
+
+@pytest.mark.parametrize(
+    "transport_name",
+    [
+        "rest",
+    ],
+)
+def test_controller2_client_transport_session_collision(transport_name):
+    creds1 = ga_credentials.AnonymousCredentials()
+    creds2 = ga_credentials.AnonymousCredentials()
+    client1 = Controller2Client(
+        credentials=creds1,
+        transport=transport_name,
+    )
+    client2 = Controller2Client(
+        credentials=creds2,
+        transport=transport_name,
+    )
+    session1 = client1.transport.register_debuggee._session
+    session2 = client2.transport.register_debuggee._session
+    assert session1 != session2
+    session1 = client1.transport.list_active_breakpoints._session
+    session2 = client2.transport.list_active_breakpoints._session
+    assert session1 != session2
+    session1 = client1.transport.update_active_breakpoint._session
+    session2 = client2.transport.update_active_breakpoint._session
+    assert session1 != session2
 
 
 def test_controller2_grpc_transport_channel():
     channel = grpc.secure_channel("http://localhost/", grpc.local_channel_credentials())
 
     # Check that channel is used if provided.
     transport = transports.Controller2GrpcTransport(
@@ -1967,14 +2861,15 @@
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
 def test_transport_close():
     transports = {
+        "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
         client = Controller2Client(
             credentials=ga_credentials.AnonymousCredentials(), transport=transport
         )
@@ -1984,14 +2879,15 @@
             with client:
                 close.assert_not_called()
             close.assert_called_once()
 
 
 def test_client_ctx():
     transports = [
+        "rest",
         "grpc",
     ]
     for transport in transports:
         client = Controller2Client(
             credentials=ga_credentials.AnonymousCredentials(), transport=transport
         )
         # Test client calls underlying transport.
```

