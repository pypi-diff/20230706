# Comparing `tmp/mlserver-1.4.0.dev2.tar.gz` & `tmp/mlserver-1.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-1.4.0.dev2.tar", last modified: Thu May  4 09:30:38 2023, max compression
+gzip compressed data, was "mlserver-1.4.0.dev3.tar", max compression
```

## Comparing `mlserver-1.4.0.dev2.tar` & `mlserver-1.4.0.dev3.tar`

### file list

```diff
@@ -1,123 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batch_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/batching/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/batching/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/init_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/cloudevents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/interceptors.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/servicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/grpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/handlers/model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/kafka/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/metrics/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/parallel/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.443136 mlserver-1.4.0.dev2/mlserver/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/repository/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/rest/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/dataplane.json
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/openapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/rest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/mlserver/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/types/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/mlserver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:30:38.439136 mlserver-1.4.0.dev2/mlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 09:30:38.000000 mlserver-1.4.0.dev2/mlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-04 09:30:38.447136 mlserver-1.4.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-04 09:29:59.000000 mlserver-1.4.0.dev2/setup.py
+-rw-r--r--   0        0        0    11354 2023-07-05 11:15:01.124882 mlserver-1.4.0.dev3/LICENSE
+-rw-r--r--   0        0        0     5366 2023-07-05 11:15:01.124882 mlserver-1.4.0.dev3/README.md
+-rw-r--r--   0        0        0      299 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/__init__.py
+-rw-r--r--   0        0        0    16370 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batch_processing.py
+-rw-r--r--   0        0        0      176 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batching/__init__.py
+-rw-r--r--   0        0        0     5529 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batching/adaptive.py
+-rw-r--r--   0        0        0     2227 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batching/hooks.py
+-rw-r--r--   0        0        0    10847 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batching/requests.py
+-rw-r--r--   0        0        0      911 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/batching/shape.py
+-rw-r--r--   0        0        0       43 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/__init__.py
+-rw-r--r--   0        0        0     1883 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/build.py
+-rw-r--r--   0        0        0     2448 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/constants.py
+-rw-r--r--   0        0        0      427 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/init_project.py
+-rw-r--r--   0        0        0     6813 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/main.py
+-rw-r--r--   0        0        0     1318 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cli/serve.py
+-rw-r--r--   0        0        0     3323 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/cloudevents.py
+-rw-r--r--   0        0        0     1197 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/__init__.py
+-rw-r--r--   0        0        0     9601 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/base.py
+-rw-r--r--   0        0        0     2717 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/base64.py
+-rw-r--r--   0        0        0     2597 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/datetime.py
+-rw-r--r--   0        0        0     7306 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/decorator.py
+-rw-r--r--   0        0        0     2056 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/errors.py
+-rw-r--r--   0        0        0      749 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/lists.py
+-rw-r--r--   0        0        0     5020 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/numpy.py
+-rw-r--r--   0        0        0     4566 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/pandas.py
+-rw-r--r--   0        0        0     2825 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/string.py
+-rw-r--r--   0        0        0     7722 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/codecs/utils.py
+-rw-r--r--   0        0        0     3814 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/env.py
+-rw-r--r--   0        0        0     1494 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/errors.py
+-rw-r--r--   0        0        0       57 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/__init__.py
+-rw-r--r--   0        0        0    16463 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/converters.py
+-rw-r--r--   0        0        0    31033 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/dataplane_pb2.py
+-rw-r--r--   0        0        0    45172 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/dataplane_pb2.pyi
+-rw-r--r--   0        0        0    15571 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/dataplane_pb2_grpc.py
+-rw-r--r--   0        0        0     8624 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/interceptors.py
+-rw-r--r--   0        0        0       92 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/logging.py
+-rw-r--r--   0        0        0     2021 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/model_repository.py
+-rw-r--r--   0        0        0     6507 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/model_repository_pb2.py
+-rw-r--r--   0        0        0     5344 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/model_repository_pb2.pyi
+-rw-r--r--   0        0        0     6338 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/model_repository_pb2_grpc.py
+-rw-r--r--   0        0        0     4260 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/server.py
+-rw-r--r--   0        0        0     4044 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/servicers.py
+-rw-r--r--   0        0        0     1679 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/grpc/utils.py
+-rw-r--r--   0        0        0      255 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/handlers/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/handlers/custom.py
+-rw-r--r--   0        0        0     3615 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/handlers/dataplane.py
+-rw-r--r--   0        0        0     2906 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/handlers/model_repository.py
+-rw-r--r--   0        0        0       59 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/errors.py
+-rw-r--r--   0        0        0     1624 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/handlers.py
+-rw-r--r--   0        0        0       85 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/logging.py
+-rw-r--r--   0        0        0     1694 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/message.py
+-rw-r--r--   0        0        0     3547 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/kafka/server.py
+-rw-r--r--   0        0        0     1589 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/logging.py
+-rw-r--r--   0        0        0      282 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/__init__.py
+-rw-r--r--   0        0        0     2244 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/context.py
+-rw-r--r--   0        0        0     1030 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/errors.py
+-rw-r--r--   0        0        0       87 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/logging.py
+-rw-r--r--   0        0        0     1961 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/prometheus.py
+-rw-r--r--   0        0        0      975 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/registry.py
+-rw-r--r--   0        0        0     2311 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/metrics/server.py
+-rw-r--r--   0        0        0     1478 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/middleware.py
+-rw-r--r--   0        0        0     8275 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/model.py
+-rw-r--r--   0        0        0      190 2023-07-05 11:15:01.288884 mlserver-1.4.0.dev3/mlserver/parallel/__init__.py
+-rw-r--r--   0        0        0     8798 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/dispatcher.py
+-rw-r--r--   0        0        0     1459 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/errors.py
+-rw-r--r--   0        0        0       96 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/logging.py
+-rw-r--r--   0        0        0     1506 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/messages.py
+-rw-r--r--   0        0        0     2607 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/model.py
+-rw-r--r--   0        0        0     6861 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/pool.py
+-rw-r--r--   0        0        0     8300 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/registry.py
+-rw-r--r--   0        0        0     1113 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/utils.py
+-rw-r--r--   0        0        0     6867 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/parallel/worker.py
+-rw-r--r--   0        0        0     3146 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/raw.py
+-rw-r--r--   0        0        0    11000 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/registry.py
+-rw-r--r--   0        0        0      302 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/repository/__init__.py
+-rw-r--r--   0        0        0      697 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/repository/factory.py
+-rw-r--r--   0        0        0     1587 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/repository/load.py
+-rw-r--r--   0        0        0     2560 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/repository/repository.py
+-rw-r--r--   0        0        0       57 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/__init__.py
+-rw-r--r--   0        0        0     5772 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/app.py
+-rw-r--r--   0        0        0     4450 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/endpoints.py
+-rw-r--r--   0        0        0      492 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/errors.py
+-rw-r--r--   0        0        0      876 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/logging.py
+-rw-r--r--   0        0        0      157 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/openapi/__init__.py
+-rw-r--r--   0        0        0    19065 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/openapi/dataplane.json
+-rw-r--r--   0        0        0     5385 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/openapi/model_repository.json
+-rw-r--r--   0        0        0     3258 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/openapi/schema.py
+-rw-r--r--   0        0        0      882 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/requests.py
+-rw-r--r--   0        0        0     1958 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/responses.py
+-rw-r--r--   0        0        0     3212 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/server.py
+-rw-r--r--   0        0        0      890 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/rest/utils.py
+-rw-r--r--   0        0        0     6534 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/server.py
+-rw-r--r--   0        0        0    12563 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/settings.py
+-rw-r--r--   0        0        0     1260 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/tracing.py
+-rw-r--r--   0        0        0     1096 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/types/__init__.py
+-rw-r--r--   0        0        0      655 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/types/base.py
+-rw-r--r--   0        0        0     2115 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/types/dataplane.py
+-rw-r--r--   0        0        0     1042 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/types/model_repository.py
+-rw-r--r--   0        0        0     3922 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/utils.py
+-rw-r--r--   0        0        0       27 2023-07-05 11:15:01.292884 mlserver-1.4.0.dev3/mlserver/version.py
+-rw-r--r--   0        0        0     3978 2023-07-05 11:15:01.296884 mlserver-1.4.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     6773 1970-01-01 00:00:00.000000 mlserver-1.4.0.dev3/PKG-INFO
```

### Comparing `mlserver-1.4.0.dev2/LICENSE` & `mlserver-1.4.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/PKG-INFO` & `mlserver-1.4.0.dev3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,114 @@
-Metadata-Version: 2.1
-Name: mlserver
-Version: 1.4.0.dev2
-Summary: ML server
-Home-page: https://github.com/SeldonIO/MLServer.git
-Author: Seldon Technologies Ltd.
-Author-email: hello@seldon.io
-License: Apache 2.0
-Description: # MLServer
-        
-        An open source inference server for your machine learning models.
-        
-        [![video_play_icon](https://user-images.githubusercontent.com/10466106/151803854-75d17c32-541c-4eee-b589-d45b07ea486d.png)](https://www.youtube.com/watch?v=aZHe3z-8C_w)
-        
-        ## Overview
-        
-        MLServer aims to provide an easy way to start serving your machine learning
-        models through a REST and gRPC interface, fully compliant with [KFServing's V2
-        Dataplane](https://docs.seldon.io/projects/seldon-core/en/latest/reference/apis/v2-protocol.html)
-        spec. Watch a quick video introducing the project [here](https://www.youtube.com/watch?v=aZHe3z-8C_w).
-        
-        - Multi-model serving, letting users run multiple models within the same
-          process.
-        - Ability to run [inference in parallel for vertical
-          scaling](https://mlserver.readthedocs.io/en/latest/user-guide/parallel-inference.html)
-          across multiple models through a pool of inference workers.
-        - Support for [adaptive
-          batching](https://mlserver.readthedocs.io/en/latest/user-guide/adaptive-batching.html),
-          to group inference requests together on the fly.
-        - Scalability with deployment in Kubernetes native frameworks, including
-          [Seldon Core](https://docs.seldon.io/projects/seldon-core/en/latest/graph/protocols.html#v2-kfserving-protocol) and
-          [KServe (formerly known as KFServing)](https://kserve.github.io/website/modelserving/v1beta1/sklearn/v2/), where
-          MLServer is the core Python inference server used to serve machine learning
-          models.
-        - Support for the standard [V2 Inference Protocol](https://docs.seldon.io/projects/seldon-core/en/latest/reference/apis/v2-protocol.html) on
-          both the gRPC and REST flavours, which has been standardised and adopted by
-          various model serving frameworks.
-        
-        You can read more about the goals of this project on the [inital design
-        document](https://docs.google.com/document/d/1C2uf4SaAtwLTlBCciOhvdiKQ2Eay4U72VxAD4bXe7iU/edit?usp=sharing).
-        
-        ## Usage
-        
-        You can install the `mlserver` package running:
-        
-        ```bash
-        pip install mlserver
-        ```
-        
-        Note that to use any of the optional [inference runtimes](#inference-runtimes),
-        you'll need to install the relevant package.
-        For example, to serve a `scikit-learn` model, you would need to install the
-        `mlserver-sklearn` package:
-        
-        ```bash
-        pip install mlserver-sklearn
-        ```
-        
-        For further information on how to use MLServer, you can check any of the
-        [available examples](#examples).
-        
-        ## Inference Runtimes
-        
-        Inference runtimes allow you to define how your model should be used within
-        MLServer.
-        You can think of them as the **backend glue** between MLServer and your machine
-        learning framework of choice.
-        You can read more about [inference runtimes in their documentation
-        page](./docs/runtimes/index.md).
-        
-        Out of the box, MLServer comes with a set of pre-packaged runtimes which let
-        you interact with a subset of common frameworks.
-        This allows you to start serving models saved in these frameworks straight
-        away.
-        However, it's also possible to **[write custom
-        runtimes](./docs/runtimes/custom.md)**.
-        
-        Out of the box, MLServer provides support for:
-        
-        | Framework     | Supported | Documentation                                                    |
-        | ------------- | --------- | ---------------------------------------------------------------- |
-        | Scikit-Learn  | ✅        | [MLServer SKLearn](./runtimes/sklearn)                           |
-        | XGBoost       | ✅        | [MLServer XGBoost](./runtimes/xgboost)                           |
-        | Spark MLlib   | ✅        | [MLServer MLlib](./runtimes/mllib)                               |
-        | LightGBM      | ✅        | [MLServer LightGBM](./runtimes/lightgbm)                         |
-        | Tempo         | ✅        | [`github.com/SeldonIO/tempo`](https://github.com/SeldonIO/tempo) |
-        | MLflow        | ✅        | [MLServer MLflow](./runtimes/mlflow)                             |
-        | Alibi-Detect  | ✅        | [MLServer Alibi Detect](./runtimes/alibi-detect)                 |
-        | Alibi-Explain | ✅        | [MLServer Alibi Explain](./runtimes/alibi-explain)               |
-        | HuggingFace   | ✅        | [MLServer HuggingFace](./runtimes/huggingface)                   |
-        
-        ## Examples
-        
-        To see MLServer in action, check out [our full list of
-        examples](./docs/examples/index.md).
-        You can find below a few selected examples showcasing how you can leverage
-        MLServer to start serving your machine learning models.
-        
-        - [Serving a `scikit-learn` model](./docs/examples/sklearn/README.md)
-        - [Serving a `xgboost` model](./docs/examples/xgboost/README.md)
-        - [Serving a `lightgbm` model](./docs/examples/lightgbm/README.md)
-        - [Serving a `tempo` pipeline](./docs/examples/tempo/README.md)
-        - [Serving a custom model](./docs/examples/custom/README.md)
-        - [Serving an `alibi-detect` model](./docs/examples/alibi-detect/README.md)
-        - [Serving a `HuggingFace` model](./docs/examples/huggingface/README.md)
-        - [Multi-Model Serving with multiple frameworks](./docs/examples/mms/README.md)
-        - [Loading / unloading models from a model repository](./docs/examples/model-repository/README.md)
-        
-        ## Developer Guide
-        
-        ### Versioning
-        
-        Both the main `mlserver` package and the [inference runtimes
-        packages](./docs/runtimes/index.md) try to follow the same versioning schema.
-        To bump the version across all of them, you can use the
-        [`./hack/update-version.sh`](./hack/update-version.sh) script.
-        
-        For example:
-        
-        ```bash
-        ./hack/update-version.sh 0.2.0.dev1
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# MLServer
+
+An open source inference server for your machine learning models.
+
+[![video_play_icon](https://user-images.githubusercontent.com/10466106/151803854-75d17c32-541c-4eee-b589-d45b07ea486d.png)](https://www.youtube.com/watch?v=aZHe3z-8C_w)
+
+## Overview
+
+MLServer aims to provide an easy way to start serving your machine learning
+models through a REST and gRPC interface, fully compliant with [KFServing's V2
+Dataplane](https://docs.seldon.io/projects/seldon-core/en/latest/reference/apis/v2-protocol.html)
+spec. Watch a quick video introducing the project [here](https://www.youtube.com/watch?v=aZHe3z-8C_w).
+
+- Multi-model serving, letting users run multiple models within the same
+  process.
+- Ability to run [inference in parallel for vertical
+  scaling](https://mlserver.readthedocs.io/en/latest/user-guide/parallel-inference.html)
+  across multiple models through a pool of inference workers.
+- Support for [adaptive
+  batching](https://mlserver.readthedocs.io/en/latest/user-guide/adaptive-batching.html),
+  to group inference requests together on the fly.
+- Scalability with deployment in Kubernetes native frameworks, including
+  [Seldon Core](https://docs.seldon.io/projects/seldon-core/en/latest/graph/protocols.html#v2-kfserving-protocol) and
+  [KServe (formerly known as KFServing)](https://kserve.github.io/website/modelserving/v1beta1/sklearn/v2/), where
+  MLServer is the core Python inference server used to serve machine learning
+  models.
+- Support for the standard [V2 Inference Protocol](https://docs.seldon.io/projects/seldon-core/en/latest/reference/apis/v2-protocol.html) on
+  both the gRPC and REST flavours, which has been standardised and adopted by
+  various model serving frameworks.
+
+You can read more about the goals of this project on the [inital design
+document](https://docs.google.com/document/d/1C2uf4SaAtwLTlBCciOhvdiKQ2Eay4U72VxAD4bXe7iU/edit?usp=sharing).
+
+## Usage
+
+You can install the `mlserver` package running:
+
+```bash
+pip install mlserver
+```
+
+Note that to use any of the optional [inference runtimes](#inference-runtimes),
+you'll need to install the relevant package.
+For example, to serve a `scikit-learn` model, you would need to install the
+`mlserver-sklearn` package:
+
+```bash
+pip install mlserver-sklearn
+```
+
+For further information on how to use MLServer, you can check any of the
+[available examples](#examples).
+
+## Inference Runtimes
+
+Inference runtimes allow you to define how your model should be used within
+MLServer.
+You can think of them as the **backend glue** between MLServer and your machine
+learning framework of choice.
+You can read more about [inference runtimes in their documentation
+page](./docs/runtimes/index.md).
+
+Out of the box, MLServer comes with a set of pre-packaged runtimes which let
+you interact with a subset of common frameworks.
+This allows you to start serving models saved in these frameworks straight
+away.
+However, it's also possible to **[write custom
+runtimes](./docs/runtimes/custom.md)**.
+
+Out of the box, MLServer provides support for:
+
+| Framework     | Supported | Documentation                                                    |
+| ------------- | --------- | ---------------------------------------------------------------- |
+| Scikit-Learn  | ✅        | [MLServer SKLearn](./runtimes/sklearn)                           |
+| XGBoost       | ✅        | [MLServer XGBoost](./runtimes/xgboost)                           |
+| Spark MLlib   | ✅        | [MLServer MLlib](./runtimes/mllib)                               |
+| LightGBM      | ✅        | [MLServer LightGBM](./runtimes/lightgbm)                         |
+| Tempo         | ✅        | [`github.com/SeldonIO/tempo`](https://github.com/SeldonIO/tempo) |
+| MLflow        | ✅        | [MLServer MLflow](./runtimes/mlflow)                             |
+| Alibi-Detect  | ✅        | [MLServer Alibi Detect](./runtimes/alibi-detect)                 |
+| Alibi-Explain | ✅        | [MLServer Alibi Explain](./runtimes/alibi-explain)               |
+| HuggingFace   | ✅        | [MLServer HuggingFace](./runtimes/huggingface)                   |
+
+## Examples
+
+To see MLServer in action, check out [our full list of
+examples](./docs/examples/index.md).
+You can find below a few selected examples showcasing how you can leverage
+MLServer to start serving your machine learning models.
+
+- [Serving a `scikit-learn` model](./docs/examples/sklearn/README.md)
+- [Serving a `xgboost` model](./docs/examples/xgboost/README.md)
+- [Serving a `lightgbm` model](./docs/examples/lightgbm/README.md)
+- [Serving a `tempo` pipeline](./docs/examples/tempo/README.md)
+- [Serving a custom model](./docs/examples/custom/README.md)
+- [Serving an `alibi-detect` model](./docs/examples/alibi-detect/README.md)
+- [Serving a `HuggingFace` model](./docs/examples/huggingface/README.md)
+- [Multi-Model Serving with multiple frameworks](./docs/examples/mms/README.md)
+- [Loading / unloading models from a model repository](./docs/examples/model-repository/README.md)
+
+## Developer Guide
+
+### Versioning
+
+Both the main `mlserver` package and the [inference runtimes
+packages](./docs/runtimes/index.md) try to follow the same versioning schema.
+To bump the version across all of them, you can use the
+[`./hack/update-version.sh`](./hack/update-version.sh) script.
+
+For example:
+
+```bash
+./hack/update-version.sh 0.2.0.dev1
+```
```

### Comparing `mlserver-1.4.0.dev2/mlserver/batch_processing.py` & `mlserver-1.4.0.dev3/mlserver/batch_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from functools import wraps
 import os
 from random import random
 import tritonclient.http.aio as httpclient
 
 import asyncio
+import numpy as np
 import aiofiles
 import logging
 import click
 import json
 import orjson
 
 from time import perf_counter as timer
@@ -97,25 +98,29 @@
     outputs: Optional[List[httpclient.InferRequestedOutput]]
 
     @classmethod
     def from_inference_request(
         cls, inference_request: InferenceRequest, binary_data: bool
     ) -> "TritonRequest":
         inputs = []
-
         for request_input in inference_request.inputs or []:
             new_input = httpclient.InferInput(
                 request_input.name, request_input.shape, request_input.datatype
             )
+            request_input_np = NumpyCodec.decode_input(request_input)
+
+            # Change datatype if BYTES to satisfy Tritonclient checks
+            if request_input.datatype == "BYTES":
+                request_input_np = request_input_np.astype(np.object_)
+
             new_input.set_data_from_numpy(
-                NumpyCodec.decode_input(request_input),
+                request_input_np,
                 binary_data=binary_data,
             )
             inputs.append(new_input)
-
         outputs = []
         for request_output in inference_request.outputs or []:
             new_output = httpclient.InferRequestedOutput(
                 request_output.name, binary_data=binary_data
             )
             outputs.append(new_output)
 
@@ -204,15 +209,14 @@
             item_indices[inference_request.id] = item.index
         except ValidationError as e:
             logger.error(
                 f"preprocessing error: batch_index={item.index}, error={repr(e)}"
             )
             invalid_inputs.append(_serialize_validation_error(item.index, e))
     batched = BatchedRequests(inference_requests)
-
     # Set `id` for batched requests - if only single request use its own id
     if len(inference_requests) == 1:
         batched.merged_request.id = inference_request.id
     else:
         batched.merged_request.id = generate_uuid()
     return (
         TritonRequest.from_inference_request(batched.merged_request, binary_data),
```

### Comparing `mlserver-1.4.0.dev2/mlserver/batching/adaptive.py` & `mlserver-1.4.0.dev3/mlserver/batching/adaptive.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/batching/hooks.py` & `mlserver-1.4.0.dev3/mlserver/batching/hooks.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/batching/requests.py` & `mlserver-1.4.0.dev3/mlserver/batching/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/batching/shape.py` & `mlserver-1.4.0.dev3/mlserver/batching/shape.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/cli/build.py` & `mlserver-1.4.0.dev3/mlserver/cli/build.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/cli/constants.py` & `mlserver-1.4.0.dev3/mlserver/cli/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     .
 RUN mkdir $(dirname $MLSERVER_ENV_TARBALL); \\
     for envFile in environment.yml environment.yaml conda.yml conda.yaml; do \\
         if [[ -f $envFile ]]; then \\
             conda env create \
                 --name $MLSERVER_ENV_NAME \\
                 --file $envFile; \\
-            conda-pack --ignore-missing-files \
+            conda-pack --ignore-missing-files --quiet \
                 -n $MLSERVER_ENV_NAME \\
                 -o $MLSERVER_ENV_TARBALL; \\
         fi \\
     done; \\
     chmod -R 776 $(dirname $MLSERVER_ENV_TARBALL)
 
 FROM seldonio/mlserver:{version}-slim
```

### Comparing `mlserver-1.4.0.dev2/mlserver/cli/main.py` & `mlserver-1.4.0.dev3/mlserver/cli/main.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/cli/serve.py` & `mlserver-1.4.0.dev3/mlserver/cli/serve.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/cloudevents.py` & `mlserver-1.4.0.dev3/mlserver/cloudevents.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/__init__.py` & `mlserver-1.4.0.dev3/mlserver/codecs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .numpy import NumpyCodec, NumpyRequestCodec
 from .pandas import PandasCodec
-from .string import StringCodec
+from .string import StringCodec, StringRequestCodec
 from .base64 import Base64Codec
 from .datetime import DatetimeCodec
 from .errors import CodecError
 from .decorator import decode_args
 from .base import (
     InputCodec,
     RequestCodec,
```

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/base.py` & `mlserver-1.4.0.dev3/mlserver/codecs/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/base64.py` & `mlserver-1.4.0.dev3/mlserver/codecs/base64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import binascii
 
 from typing import Any, List, Union
 from functools import partial
 
-from ..types import RequestInput, ResponseOutput
+from ..types import RequestInput, ResponseOutput, Parameters
 from .lists import is_list_of
 from .base import InputCodec, register_input_codec
 from .lists import as_list, ListElement
 
 _Base64StrCodec = "ascii"
 
 
@@ -60,14 +60,15 @@
         packed = map(partial(_encode_base64, use_bytes=use_bytes), payload)
         shape = [len(payload), 1]
         return ResponseOutput(
             name=name,
             datatype="BYTES",
             shape=shape,
             data=list(packed),
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> List[bytes]:
         packed = response_output.data.__root__
         return list(map(_decode_base64, as_list(packed)))
 
@@ -78,14 +79,15 @@
         # Assume that payload is already in b64, so we only need to pack it
         output = cls.encode_output(name, payload, use_bytes)
         return RequestInput(
             name=output.name,
             datatype=output.datatype,
             shape=output.shape,
             data=output.data,
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_input(cls, request_input: RequestInput) -> List[bytes]:
         packed = request_input.data.__root__
 
         return list(map(_decode_base64, as_list(packed)))
```

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/datetime.py` & `mlserver-1.4.0.dev3/mlserver/codecs/datetime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Union, List
 from datetime import datetime
 from functools import partial
 
-from ..types import RequestInput, ResponseOutput
+from ..types import RequestInput, ResponseOutput, Parameters
 from .lists import is_list_of, as_list, ListElement
 from .base import InputCodec, register_input_codec
 
 _Datetime = Union[str, datetime]
 _DatetimeStrCodec = "ascii"
 
 
@@ -58,14 +58,15 @@
         packed = map(partial(_encode_datetime, use_bytes=use_bytes), payload)
         shape = [len(payload), 1]
         return ResponseOutput(
             name=name,
             datatype="BYTES",
             shape=shape,
             data=list(packed),
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> List[datetime]:
         packed = response_output.data.__root__
 
         return list(map(_decode_datetime, as_list(packed)))
@@ -76,14 +77,15 @@
     ) -> RequestInput:
         output = cls.encode_output(name, payload, use_bytes=use_bytes)
         return RequestInput(
             name=output.name,
             datatype=output.datatype,
             shape=output.shape,
             data=output.data,
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_input(cls, request_input: RequestInput) -> List[datetime]:
         packed = request_input.data.__root__
 
         return list(map(_decode_datetime, as_list(packed)))
```

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/decorator.py` & `mlserver-1.4.0.dev3/mlserver/codecs/decorator.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/errors.py` & `mlserver-1.4.0.dev3/mlserver/codecs/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/lists.py` & `mlserver-1.4.0.dev3/mlserver/codecs/lists.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/numpy.py` & `mlserver-1.4.0.dev3/mlserver/codecs/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         shape = inject_batch_dimension(list(payload.shape))
 
         return ResponseOutput(
             name=name,
             datatype=datatype,
             shape=shape,
             data=_encode_data(payload, datatype),
+            parameters=Parameters(content_type=cls.ContentType),
         )
 
     @classmethod
     def decode_output(cls, response_output: ResponseOutput) -> np.ndarray:
         return cls.decode_input(response_output)  # type: ignore
 
     @classmethod
```

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/string.py` & `mlserver-1.4.0.dev3/mlserver/codecs/string.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/codecs/utils.py` & `mlserver-1.4.0.dev3/mlserver/codecs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,18 @@
                 f"No input codec found for {type(cls)} request codec"
             )
 
         output = cls.InputCodec.encode_output(
             f"{DefaultOutputPrefix}1", payload, **kwargs
         )
         return InferenceResponse(
-            model_name=model_name, model_version=model_version, outputs=[output]
+            model_name=model_name,
+            model_version=model_version,
+            parameters=Parameters(content_type=cls.ContentType),
+            outputs=[output],
         )
 
     @classmethod
     def decode_response(cls, response: InferenceResponse) -> Any:
         if len(response.outputs) != 1:
             raise CodecError(
                 f"The '{cls.ContentType}' codec only supports a single output tensor "
@@ -224,15 +227,17 @@
     def encode_request(cls, payload: Any, **kwargs) -> InferenceRequest:
         if cls.InputCodec is None:
             raise NotImplementedError(
                 f"No input codec found for {type(cls)} request codec"
             )
 
         inp = cls.InputCodec.encode_input(f"{DefaultInputPrefix}1", payload, **kwargs)
-        return InferenceRequest(inputs=[inp])
+        return InferenceRequest(
+            inputs=[inp], parameters=Parameters(content_type=cls.ContentType)
+        )
 
     @classmethod
     def decode_request(cls, request: InferenceRequest) -> Any:
         if len(request.inputs) != 1:
             raise CodecError(
                 f"The '{cls.ContentType}' codec only supports a single input tensor "
                 f"({len(request.inputs)} were received)"
```

### Comparing `mlserver-1.4.0.dev2/mlserver/env.py` & `mlserver-1.4.0.dev3/mlserver/env.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/errors.py` & `mlserver-1.4.0.dev3/mlserver/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/converters.py` & `mlserver-1.4.0.dev3/mlserver/grpc/converters.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2.py` & `mlserver-1.4.0.dev3/mlserver/grpc/dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/dataplane_pb2_grpc.py` & `mlserver-1.4.0.dev3/mlserver/grpc/dataplane_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/interceptors.py` & `mlserver-1.4.0.dev3/mlserver/grpc/interceptors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/model_repository.py` & `mlserver-1.4.0.dev3/mlserver/grpc/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2.py` & `mlserver-1.4.0.dev3/mlserver/grpc/model_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/model_repository_pb2_grpc.py` & `mlserver-1.4.0.dev3/mlserver/grpc/model_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/server.py` & `mlserver-1.4.0.dev3/mlserver/grpc/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from grpc import aio
 from concurrent.futures import ThreadPoolExecutor
 from typing import Optional, Any, List, Tuple
 
 from ..handlers import DataPlane, ModelRepositoryHandlers
 from ..settings import Settings
+from ..tracing import get_tracer_provider
 
 from .servicers import InferenceServicer
 from .model_repository import ModelRepositoryServicer
 from .dataplane_pb2_grpc import add_GRPCInferenceServiceServicer_to_server
 from .model_repository_pb2_grpc import add_ModelRepositoryServiceServicer_to_server
 from .interceptors import LoggingInterceptor, PromServerInterceptor
 from .logging import logger
 
+from opentelemetry.instrumentation.grpc import aio_server_interceptor, filters
+
 # Workers used for non-AsyncIO workloads (which aren't any in our case)
 DefaultGrpcWorkers = 5
 
 
 class GRPCServer:
     def __init__(
         self,
@@ -38,15 +41,36 @@
         interceptors = []
 
         if self._settings.debug:
             # If debug, enable access logs
             interceptors = [LoggingInterceptor()]
 
         if self._settings.metrics_endpoint:
-            interceptors.append(PromServerInterceptor())
+            interceptors.append(
+                PromServerInterceptor(enable_handling_time_histogram=True)
+            )
+
+        if self._settings.tracing_server:
+            tracer_provider = get_tracer_provider(self._settings)
+            excluded_urls = filters.negate(
+                filters.any_of(
+                    filters.full_method_name(
+                        "/inference.GRPCInferenceService/ServerLive"
+                    ),
+                    filters.full_method_name(
+                        "/inference.GRPCInferenceService/ServerReady"
+                    ),
+                )
+            )
+
+            interceptors.append(
+                aio_server_interceptor(
+                    tracer_provider=tracer_provider, filter_=excluded_urls
+                )
+            )
 
         self._server = aio.server(
             ThreadPoolExecutor(max_workers=DefaultGrpcWorkers),
             interceptors=tuple(interceptors),
             options=self._get_options(),
         )
```

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/servicers.py` & `mlserver-1.4.0.dev3/mlserver/grpc/servicers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/grpc/utils.py` & `mlserver-1.4.0.dev3/mlserver/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/handlers/custom.py` & `mlserver-1.4.0.dev3/mlserver/handlers/custom.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/handlers/dataplane.py` & `mlserver-1.4.0.dev3/mlserver/handlers/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/handlers/model_repository.py` & `mlserver-1.4.0.dev3/mlserver/handlers/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/kafka/handlers.py` & `mlserver-1.4.0.dev3/mlserver/kafka/handlers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/kafka/message.py` & `mlserver-1.4.0.dev3/mlserver/kafka/message.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/kafka/server.py` & `mlserver-1.4.0.dev3/mlserver/kafka/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/logging.py` & `mlserver-1.4.0.dev3/mlserver/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/metrics/context.py` & `mlserver-1.4.0.dev3/mlserver/metrics/context.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/metrics/errors.py` & `mlserver-1.4.0.dev3/mlserver/metrics/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/metrics/prometheus.py` & `mlserver-1.4.0.dev3/mlserver/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/metrics/registry.py` & `mlserver-1.4.0.dev3/mlserver/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/metrics/server.py` & `mlserver-1.4.0.dev3/mlserver/metrics/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,16 +29,14 @@
         app.add_route(self._settings.metrics_endpoint, self._endpoint.handle_metrics)
         return app
 
     async def on_worker_stop(self, worker: "Worker") -> None:
         if not worker.pid:
             return
 
-        # NOTE: If a worker gets restarted (instead of regular shutdown), we may
-        # not want to remove old files to keep counts intact
         await stop_metrics(self._settings, worker.pid)
 
     async def start(self):
         cfg = self._get_config()
         self._server = _NoSignalServer(cfg)
 
         metrics_server = f"http://{self._settings.host}:{self._settings.metrics_port}"
```

### Comparing `mlserver-1.4.0.dev2/mlserver/middleware.py` & `mlserver-1.4.0.dev3/mlserver/middleware.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/model.py` & `mlserver-1.4.0.dev3/mlserver/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,28 @@
 
 
         **This method should be overriden to implement your custom inference
         logic.**
         """
         raise NotImplementedError("predict() method not implemented")
 
+    async def unload(self) -> bool:
+        """
+        Method responsible for unloading the model, freeing any resources (e.g.
+        CPU memory, GPU memory, etc.).
+        This method will be called on each of the parallel workers (when
+        :doc:`parallel inference </user-guide/parallel-inference>`) is
+        enabled).
+        A return value of ``True`` will mean the model is now unloaded.
+
+        **This method should be overriden to implement your custom unload
+        logic.**
+        """
+        return True
+
     @property
     def name(self) -> str:
         """
         Model name, from the model settings.
         """
         return self._settings.name
```

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/dispatcher.py` & `mlserver-1.4.0.dev3/mlserver/parallel/dispatcher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,184 @@
 import asyncio
 
-from typing import Dict, List, Tuple
+from collections import defaultdict
+from typing import Dict, List, Tuple, Set, Iterator
 from itertools import cycle
 from multiprocessing import Queue
 from concurrent.futures import ThreadPoolExecutor
 from asyncio import Future
 
 from ..utils import schedule_with_callback, generate_uuid
 from ..metrics import REGISTRY
 
+from .errors import WorkerStop
 from .worker import Worker
 from .logging import logger
 from .utils import END_OF_QUEUE, cancel_task
 from .messages import (
     Message,
     ModelUpdateMessage,
     ModelRequestMessage,
     ModelResponseMessage,
 )
 from prometheus_client import Histogram
 
 QUEUE_METRIC_NAME = "parallel_request_queue"
 
 
-class Dispatcher:
-    def __init__(self, workers: Dict[int, Worker], responses: Queue):
-        self._responses = responses
-        self._workers = workers
-        self._workers_round_robin = cycle(self._workers.keys())
-        self._active = False
-        self._process_responses_task = None
-        self._executor = ThreadPoolExecutor()
-        self._async_responses: Dict[str, Future[ModelResponseMessage]] = {}
+class AsyncResponses:
+    def __init__(self) -> None:
+        self._futures: Dict[str, Future[ModelResponseMessage]] = {}
+
+        # _workers_map keeps track of which in-flight requests are being served
+        # by each worker
+        self._workers_map: Dict[int, Set[str]] = defaultdict(set)
+        # _futures_map keeps track of which worker is serving each in-flight
+        # request
+        self._futures_map: Dict[str, int] = {}
+
         self.parallel_request_queue_size = self._get_or_create_metric()
 
     def _get_or_create_metric(self) -> Histogram:
         if QUEUE_METRIC_NAME in REGISTRY:
             return REGISTRY[QUEUE_METRIC_NAME]  # type: ignore
 
         return Histogram(
             QUEUE_METRIC_NAME,
             "counter of request queue size for workers",
-            ["workerpid"],
             registry=REGISTRY,
         )
 
+    async def schedule_and_wait(
+        self, message: Message, worker: Worker
+    ) -> ModelResponseMessage:
+        """
+        Schedule a response and wait until it gets resolved.
+        """
+        message_id = message.id
+        self._schedule(message, worker)
+        return await self._wait(message_id)
+
+    def _schedule(self, message: Message, worker: Worker) -> Future:
+        """
+        Schedule a response to be resolved in the future.
+        """
+        loop = asyncio.get_running_loop()
+        future = loop.create_future()
+        message_id = message.id
+        self._futures[message_id] = future
+
+        # Keep track of allocation for in-flight requests
+        self._track_message(message, worker)
+
+        # Monitor current in-flight requests
+        in_flight_count = len(self._futures)
+        self.parallel_request_queue_size.observe(in_flight_count)
+
+        return future
+
+    def _track_message(self, message: Message, worker: Worker) -> None:
+        self._futures_map[message.id] = worker.pid  # type: ignore
+        self._workers_map[worker.pid].add(message.id)  # type: ignore
+
+    async def _wait(self, message_id: str) -> ModelResponseMessage:
+        future = self._futures[message_id]
+
+        try:
+            response_message = await future
+            return response_message
+        finally:
+            self._clear_message(message_id)
+
+    def _clear_message(self, message_id: str) -> None:
+        del self._futures[message_id]
+        worker_pid = self._futures_map.pop(message_id)
+        self._workers_map[worker_pid].remove(message_id)
+
+    def resolve(self, response: ModelResponseMessage):
+        """
+        Resolve a previously scheduled response future.
+        """
+        message_id = response.id
+        future = self._futures[message_id]
+
+        # NOTE: Use call_soon_threadsafe to cover cases where `model.predict()`
+        # (or other methods) get called from a separate thread (and a separate
+        # AsyncIO loop)
+        loop = future.get_loop()
+        if response.exception:
+            loop.call_soon_threadsafe(future.set_exception, response.exception)
+        else:
+            loop.call_soon_threadsafe(future.set_result, response)
+
+    def cancel(self, worker: Worker, exit_code: int):
+        """
+        Cancel in-flight requests for worker (e.g. because it died
+        unexpectedly).
+        """
+        in_flight = self._workers_map[worker.pid]  # type: ignore
+        if in_flight:
+            logger.info(
+                f"Cancelling {len(in_flight)} in-flight requests for "
+                "worker {worker.pid} which died unexpectedly with "
+                "exit code {exit_code}..."
+            )
+        for message_id in in_flight:
+            err = WorkerStop(exit_code)
+            future = self._futures[message_id]
+            loop = future.get_loop()
+            loop.call_soon_threadsafe(future.set_exception, err)
+
+
+class Dispatcher:
+    def __init__(self, workers: Dict[int, Worker], responses: Queue):
+        self._responses = responses
+        self._workers = workers
+        self._workers_round_robin = self._reset_round_robin()
+        self._worker_starting_lock = asyncio.Lock()
+        self._active = False
+        self._process_responses_task = None
+        self._executor = ThreadPoolExecutor()
+        self._async_responses = AsyncResponses()
+
+    def _reset_round_robin(self) -> Iterator[int]:
+        worker_pids = list(self._workers.keys())
+        self._workers_round_robin = cycle(worker_pids)
+        return self._workers_round_robin
+
+    async def on_worker_start(self, worker: Worker):
+        """
+        Handler for workers who have just started but are still not ready to
+        receive traffic.
+        This is used for workers that got restarted and need to reload all
+        models.
+        """
+        # Lock while worker is coming up to ensure no model updates get lost in
+        # translation
+        async with self._worker_starting_lock:
+            self._workers[worker.pid] = worker  # type: ignore
+
+    def on_worker_ready(self, worker: Worker):
+        """
+        Handler for workers who are now ready to receive traffic.
+        """
+        self._reset_round_robin()
+
+    def on_worker_stop(self, worker: Worker, exit_code: int):
+        """
+        Handler used for workers who stopped unexpectedly and there need to be
+        removed from the round robin rotation.
+        """
+        pid = worker.pid
+        if pid in self._workers:
+            del self._workers[pid]
+
+        self._reset_round_robin()
+        self._async_responses.cancel(worker, exit_code)
+
     def start(self):
         self._active = True
         self._process_responses_task = schedule_with_callback(
             self._process_responses(), self._process_responses_cb
         )
 
     def _process_responses_cb(self, process_responses):
@@ -70,93 +200,50 @@
             response = await loop.run_in_executor(self._executor, self._responses.get)
 
             # If the queue gets terminated, detect the "sentinel value" and
             # stop reading
             if response is END_OF_QUEUE:
                 return
 
-            await self._process_response(response)
-
-    async def _process_response(self, response: ModelResponseMessage):
-        internal_id = response.id
-
-        async_response = self._async_responses[internal_id]
-
-        # NOTE: Use call_soon_threadsafe to cover cases where `model.predict()`
-        # (or other methods) get called from a separate thread (and a separate
-        # AsyncIO loop)
-        response_loop = async_response.get_loop()
-        if response.exception:
-            response_loop.call_soon_threadsafe(
-                async_response.set_exception, response.exception
-            )
-        else:
-            response_loop.call_soon_threadsafe(async_response.set_result, response)
+            self._async_responses.resolve(response)
 
     async def dispatch_request(
         self, request_message: ModelRequestMessage
     ) -> ModelResponseMessage:
         worker, wpid = self._get_worker()
-        self._workers_queue_monitor(worker, wpid)
         worker.send_request(request_message)
 
-        return await self._dispatch(request_message)
+        return await self._async_responses.schedule_and_wait(request_message, worker)
 
     def _get_worker(self) -> Tuple[Worker, int]:
         """
         Get next available worker.
         By default, this is just a round-robin through all the workers.
         """
         worker_pid = next(self._workers_round_robin)
         return self._workers[worker_pid], worker_pid
 
-    def _workers_queue_monitor(self, worker: Worker, worker_pid: int):
-        """Get metrics from every worker request queue"""
-        queue_size = worker._requests.qsize()
-
-        self.parallel_request_queue_size.labels(workerpid=str(worker_pid)).observe(
-            float(queue_size)
-        )
-
     async def dispatch_update(
         self, model_update: ModelUpdateMessage
     ) -> List[ModelResponseMessage]:
-        return await asyncio.gather(
-            *[
-                self._dispatch_update(worker, model_update)
-                for worker in self._workers.values()
-            ]
-        )
+        async with self._worker_starting_lock:
+            return await asyncio.gather(
+                *[
+                    self.dispatch_update_to_worker(worker, model_update)
+                    for worker in self._workers.values()
+                ]
+            )
 
-    async def _dispatch_update(
+    async def dispatch_update_to_worker(
         self, worker: Worker, model_update: ModelUpdateMessage
     ) -> ModelResponseMessage:
         # NOTE: Need to rewrite the UUID to ensure each worker sends back a
         # unique result
         worker_update = model_update.copy()
         worker_update.id = generate_uuid()
         worker.send_update(worker_update)
-        return await self._dispatch(worker_update)
-
-    async def _dispatch(self, message: Message) -> ModelResponseMessage:
-        loop = asyncio.get_running_loop()
-        async_response = loop.create_future()
-        internal_id = message.id
-        self._async_responses[internal_id] = async_response
-
-        return await self._wait_response(internal_id)
-
-    async def _wait_response(self, internal_id: str) -> ModelResponseMessage:
-        async_response = self._async_responses[internal_id]
-
-        try:
-            inference_response = await async_response
-            return inference_response
-        finally:
-            del self._async_responses[internal_id]
-
-        return await async_response
+        return await self._async_responses.schedule_and_wait(worker_update, worker)
 
     async def stop(self):
         self._executor.shutdown()
         if self._process_responses_task is not None:
             await cancel_task(self._process_responses_task)
```

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/errors.py` & `mlserver-1.4.0.dev3/mlserver/parallel/errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
         if model.version:
             msg += f" with version '{model.version}'"
 
         super().__init__(msg, status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
 
 
+class WorkerStop(MLServerError):
+    def __init__(self, exit_code: int):
+        msg = f"Worker process stopped unexpectedly with exit code {exit_code}."
+        super().__init__(msg, status.HTTP_500_INTERNAL_SERVER_ERROR)
+
+
 class WorkerError(MLServerError):
     """
     Class used to wrap exceptions raised from the workers.
 
     All stacktrace details will be hidden, and the original class won't be
     returned. This is to avoid issues with custom exceptions, like:
```

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/messages.py` & `mlserver-1.4.0.dev3/mlserver/parallel/messages.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/model.py` & `mlserver-1.4.0.dev3/mlserver/parallel/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/registry.py` & `mlserver-1.4.0.dev3/mlserver/parallel/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import os
 import shutil
+import signal
 
 from typing import Optional, Dict, List
 
 from ..settings import ModelSettings
 from ..utils import to_absolute_path
 from ..model import MLModel
 from ..settings import Settings
@@ -52,14 +53,32 @@
         self._default_pool = InferencePool(
             self._settings, on_worker_stop=on_worker_stop
         )
         self._pools: Dict[str, InferencePool] = {}
 
         os.makedirs(self._settings.environments_dir, exist_ok=True)
 
+        # Register sigchld signal handler (saving original to restore it later)
+        self._original_sigchld_handler = signal.getsignal(signal.SIGCHLD)
+        signal.signal(
+            signal.SIGCHLD,
+            lambda *args: asyncio.create_task(self._handle_worker_stop(*args)),
+        )
+
+    async def _handle_worker_stop(self, signum, frame):
+        pid, exit_code = os.waitpid(-1, os.WNOHANG)
+        if pid == 0 or exit_code == 0:
+            # Worker terminated gracefully, nothing to do
+            return
+
+        await self._default_pool.on_worker_stop(pid, exit_code)
+        await asyncio.gather(
+            *[pool.on_worker_stop(pid) for pool in self._pools.values()]
+        )
+
     async def _get_or_create(self, model: MLModel) -> InferencePool:
         env_tarball = _get_env_tarball(model)
         if not env_tarball:
             return self._default_pool
 
         env_hash = await compute_hash(env_tarball)
         if env_hash in self._pools:
@@ -182,27 +201,27 @@
         if pool != self._default_pool and pool.empty():
             logger.info(f"Inference pool with hash '{pool.env_hash}' is now empty")
             await self._close_pool(pool.env_hash)
 
         return unloaded
 
     async def close(self):
+        # Reset signal handler
+        signal.signal(signal.SIGCHLD, self._original_sigchld_handler)
         await asyncio.gather(
             self._close_pool(None),
             *[self._close_pool(env_hash) for env_hash in self._pools],
         )
 
     async def _close_pool(self, env_hash: Optional[str] = None):
         pool = self._default_pool
-        pool_name = "default inference pool"
         if env_hash:
             pool = self._pools[env_hash]
-            pool_name = f"inference pool with hash '{env_hash}'"
 
-        logger.info(f"Waiting for shutdown of {pool_name}...")
+        logger.info(f"Waiting for shutdown of {pool.name}...")
         await pool.close()
-        logger.info(f"Shutdown of {pool_name} complete")
+        logger.info(f"Shutdown of {pool.name} complete")
 
         if env_hash:
             del self._pools[env_hash]
             env_path = self._get_env_path(env_hash)
             shutil.rmtree(env_path)
```

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/utils.py` & `mlserver-1.4.0.dev3/mlserver/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/parallel/worker.py` & `mlserver-1.4.0.dev3/mlserver/parallel/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         """
         self._model_registry = MultiModelRegistry()
         self._active = True
 
     async def coro_run(self):
         self.__inner_init__()
         loop = asyncio.get_event_loop()
-
         while self._active:
             readable = await loop.run_in_executor(self._executor, self._select)
             for r in readable:
                 if r is self._requests._reader:
                     request = self._requests.get()
 
                     schedule_with_callback(
```

### Comparing `mlserver-1.4.0.dev2/mlserver/raw.py` & `mlserver-1.4.0.dev3/mlserver/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/registry.py` & `mlserver-1.4.0.dev3/mlserver/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
         # deployment)
         new_model.ready = await new_model.load()
         self._register(new_model)
 
         if old_model == self.default:
             self._clear_default()
 
+        old_model.ready = not await old_model.unload()
         logger.info(f"Reloaded model '{new_model.name}' succesfully.")
 
     async def unload(self):
         models = await self.get_models()
         await asyncio.gather(*[self._unload_model(model) for model in models])
 
         self._versions.clear()
@@ -217,14 +218,16 @@
 
         if model.version:
             del self._versions[model.version]
 
         if model == self.default:
             self._clear_default()
 
+        model.ready = not await model.unload()
+
     def _find_model(self, version: Optional[str] = None) -> Optional[MLModel]:
         if version:
             if version not in self._versions:
                 return None
 
             return self._versions[version]
```

### Comparing `mlserver-1.4.0.dev2/mlserver/repository/factory.py` & `mlserver-1.4.0.dev3/mlserver/repository/factory.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/repository/load.py` & `mlserver-1.4.0.dev3/mlserver/repository/load.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/repository/repository.py` & `mlserver-1.4.0.dev3/mlserver/repository/repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/app.py` & `mlserver-1.4.0.dev3/mlserver/rest/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from typing import Callable
 from fastapi import FastAPI
 from fastapi.responses import Response as FastAPIResponse
 from fastapi.routing import APIRoute as FastAPIRoute
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.middleware.gzip import GZipMiddleware
+from opentelemetry.instrumentation.fastapi import FastAPIInstrumentor
+
 from starlette_exporter import PrometheusMiddleware
 
 from .endpoints import Endpoints, ModelRepositoryEndpoints
 from .requests import Request
 from .responses import Response
 from .errors import _EXCEPTION_HANDLERS
 
 from ..settings import Settings
 from ..handlers import DataPlane, ModelRepositoryHandlers
+from ..tracing import get_tracer_provider
 
 
 class APIRoute(FastAPIRoute):
     """
     Custom route to use our own Request handler.
     """
 
@@ -141,14 +144,30 @@
         debug=settings.debug,
         routes=routes,  # type: ignore
         default_response_class=Response,
         exception_handlers=_EXCEPTION_HANDLERS,  # type: ignore
         docs_url=None,
         redoc_url=None,
     )
+
+    if settings.tracing_server:
+        tracer_provider = get_tracer_provider(settings)
+        excluded_urls = ",".join(
+            [
+                "/v2/health/live",
+                "/v2/health/ready",
+            ]
+        )
+
+        FastAPIInstrumentor.instrument_app(
+            app,
+            tracer_provider=tracer_provider,
+            excluded_urls=excluded_urls,
+        )
+
     app.router.route_class = APIRoute
     app.add_middleware(GZipMiddleware)
     if settings.cors_settings is not None:
         app.add_middleware(
             CORSMiddleware,
             allow_origins=settings.cors_settings.allow_origins,
             allow_origin_regex=settings.cors_settings.allow_origin_regex,
```

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/endpoints.py` & `mlserver-1.4.0.dev3/mlserver/rest/endpoints.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/logging.py` & `mlserver-1.4.0.dev3/mlserver/rest/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/openapi/dataplane.json` & `mlserver-1.4.0.dev3/mlserver/rest/openapi/dataplane.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/openapi/model_repository.json` & `mlserver-1.4.0.dev3/mlserver/rest/openapi/model_repository.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/openapi/schema.py` & `mlserver-1.4.0.dev3/mlserver/rest/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/requests.py` & `mlserver-1.4.0.dev3/mlserver/rest/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/responses.py` & `mlserver-1.4.0.dev3/mlserver/rest/responses.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/server.py` & `mlserver-1.4.0.dev3/mlserver/rest/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/rest/utils.py` & `mlserver-1.4.0.dev3/mlserver/rest/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/server.py` & `mlserver-1.4.0.dev3/mlserver/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/settings.py` & `mlserver-1.4.0.dev3/mlserver/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,20 +220,24 @@
     used.
     """
 
     # Logging settings
     logging_settings: Optional[Union[str, Dict]] = None
     """Path to logging config file or dictionary configuration."""
 
-    # Kakfa Server settings
+    # Kafka Server settings
     kafka_enabled: bool = False
     kafka_servers: str = "localhost:9092"
     kafka_topic_input: str = "mlserver-input"
     kafka_topic_output: str = "mlserver-output"
 
+    # OpenTelemetry Tracing settings
+    tracing_server: Optional[str] = None
+    """Server name used to export OpenTelemetry tracing to collector service."""
+
     # Custom server settings
     _custom_rest_server_settings: Optional[dict] = None
     _custom_metrics_server_settings: Optional[dict] = None
     _custom_grpc_server_settings: Optional[dict] = None
 
 
 class ModelParameters(BaseSettings):
```

### Comparing `mlserver-1.4.0.dev2/mlserver/types/__init__.py` & `mlserver-1.4.0.dev3/mlserver/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/types/base.py` & `mlserver-1.4.0.dev3/mlserver/types/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/types/dataplane.py` & `mlserver-1.4.0.dev3/mlserver/types/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/types/model_repository.py` & `mlserver-1.4.0.dev3/mlserver/types/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.4.0.dev2/mlserver/utils.py` & `mlserver-1.4.0.dev3/mlserver/utils.py`

 * *Files identical despite different names*

