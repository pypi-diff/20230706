# Comparing `tmp/authedwig-9.1.0.tar.gz` & `tmp/authedwig-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/authedwig-9.1.0.tar", last modified: Mon Dec 12 07:35:59 2022, max compression
+gzip compressed data, was "authedwig-9.2.0.tar", last modified: Thu Jul  6 18:59:47 2023, max compression
```

## Comparing `authedwig-9.1.0.tar` & `authedwig-9.2.0.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.887891 authedwig-9.1.0/
--rw-r--r--   0 maru       (501) staff       (20)      348 2021-06-25 18:42:17.000000 authedwig-9.1.0/CONTRIBUTORS.txt
--rw-r--r--   0 maru       (501) staff       (20)      223 2021-06-25 18:42:16.000000 authedwig-9.1.0/MANIFEST.in
--rw-r--r--   0 maru       (501) staff       (20)     9280 2022-12-12 07:35:59.888085 authedwig-9.1.0/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     6501 2021-06-28 19:06:57.000000 authedwig-9.1.0/README.rst
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.851280 authedwig-9.1.0/authedwig.egg-info/
--rw-r--r--   0 maru       (501) staff       (20)     9280 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     2535 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/SOURCES.txt
--rw-r--r--   0 maru       (501) staff       (20)        1 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/dependency_links.txt
--rw-r--r--   0 maru       (501) staff       (20)       50 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/entry_points.txt
--rw-r--r--   0 maru       (501) staff       (20)      785 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/requires.txt
--rw-r--r--   0 maru       (501) staff       (20)        7 2022-12-12 07:35:59.000000 authedwig-9.1.0/authedwig.egg-info/top_level.txt
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.851500 authedwig-9.1.0/examples/
--rw-r--r--   0 maru       (501) staff       (20)     2507 2021-06-25 18:42:16.000000 authedwig-9.1.0/examples/README.md
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.854771 authedwig-9.1.0/hedwig/
--rw-r--r--   0 maru       (501) staff       (20)       87 2022-12-12 07:35:48.000000 authedwig-9.1.0/hedwig/__init__.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.857072 authedwig-9.1.0/hedwig/backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    12088 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/backends/aws.py
--rw-r--r--   0 maru       (501) staff       (20)    11178 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/backends/base.py
--rw-r--r--   0 maru       (501) staff       (20)      343 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/backends/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)    15978 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/backends/gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      573 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/backends/import_utils.py
--rw-r--r--   0 maru       (501) staff       (20)      907 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/backends/utils.py
--rw-r--r--   0 maru       (501) staff       (20)     2283 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/callback.py
--rw-r--r--   0 maru       (501) staff       (20)      653 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/commands.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.857514 authedwig-9.1.0/hedwig/conf/
--rw-r--r--   0 maru       (501) staff       (20)     8148 2021-06-28 20:51:54.000000 authedwig-9.1.0/hedwig/conf/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1759 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/consumer.py
--rw-r--r--   0 maru       (501) staff       (20)     1080 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/exceptions.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.858619 authedwig-9.1.0/hedwig/instrumentation/
--rw-r--r--   0 maru       (501) staff       (20)     1991 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/instrumentation/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1903 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/instrumentation/compat.py
--rw-r--r--   0 maru       (501) staff       (20)     7349 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/models.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.859624 authedwig-9.1.0/hedwig/protobuf/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-28 19:06:57.000000 authedwig-9.1.0/hedwig/protobuf/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     8828 2021-11-30 15:46:32.000000 authedwig-9.1.0/hedwig/protobuf/container_pb2.py
--rw-r--r--   0 maru       (501) staff       (20)     4137 2021-11-30 15:46:32.000000 authedwig-9.1.0/hedwig/protobuf/options_pb2.py
--rw-r--r--   0 maru       (501) staff       (20)      627 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/publisher.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.860781 authedwig-9.1.0/hedwig/testing/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)      218 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/config.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.862527 authedwig-9.1.0/hedwig/testing/factories/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/factories/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1585 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/factories/base.py
--rw-r--r--   0 maru       (501) staff       (20)      417 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/factories/jsonschema.py
--rw-r--r--   0 maru       (501) staff       (20)      984 2021-06-28 20:51:54.000000 authedwig-9.1.0/hedwig/testing/factories/protobuf.py
--rw-r--r--   0 maru       (501) staff       (20)     3130 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/testing/pytest_plugin.py
--rw-r--r--   0 maru       (501) staff       (20)      756 2021-06-28 20:51:54.000000 authedwig-9.1.0/hedwig/utils.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.865157 authedwig-9.1.0/hedwig/validators/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/validators/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    11581 2021-06-28 20:51:54.000000 authedwig-9.1.0/hedwig/validators/base.py
--rw-r--r--   0 maru       (501) staff       (20)    11146 2021-06-28 19:06:57.000000 authedwig-9.1.0/hedwig/validators/jsonschema.py
--rw-r--r--   0 maru       (501) staff       (20)     1776 2021-06-25 18:42:16.000000 authedwig-9.1.0/hedwig/validators/jsonschema_container_schema.json
--rw-r--r--   0 maru       (501) staff       (20)    11996 2022-12-12 07:35:04.000000 authedwig-9.1.0/hedwig/validators/protobuf.py
--rw-r--r--   0 maru       (501) staff       (20)      252 2021-06-25 18:42:16.000000 authedwig-9.1.0/pyproject.toml
--rw-r--r--   0 maru       (501) staff       (20)      375 2022-12-12 07:35:59.888590 authedwig-9.1.0/setup.cfg
--rw-r--r--   0 maru       (501) staff       (20)     3836 2022-12-12 07:35:04.000000 authedwig-9.1.0/setup.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.873375 authedwig-9.1.0/tests/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     4848 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/conftest.py
--rw-r--r--   0 maru       (501) staff       (20)      171 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/handlers.py
--rw-r--r--   0 maru       (501) staff       (20)      161 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/models.py
--rw-r--r--   0 maru       (501) staff       (20)      269 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/protobuf_factory.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.875952 authedwig-9.1.0/tests/schemas/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/schemas/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     4292 2021-06-28 19:06:57.000000 authedwig-9.1.0/tests/schemas/jsonschema.json
--rw-r--r--   0 maru       (501) staff       (20)      947 2021-06-28 20:51:54.000000 authedwig-9.1.0/tests/schemas/protobuf.proto
--rw-r--r--   0 maru       (501) staff       (20)      692 2021-06-28 20:51:54.000000 authedwig-9.1.0/tests/schemas/protobuf_bad.proto
--rw-r--r--   0 maru       (501) staff       (20)      725 2021-06-28 19:06:57.000000 authedwig-9.1.0/tests/schemas/protobuf_minor_versioned.proto
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.879686 authedwig-9.1.0/tests/schemas/protos/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/schemas/protos/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     6345 2021-11-30 15:46:32.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_bad_pb2.py
--rw-r--r--   0 maru       (501) staff       (20)     2506 2021-12-01 15:15:05.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_bad_pb2.pyi
--rw-r--r--   0 maru       (501) staff       (20)     8628 2021-11-30 15:46:32.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_minor_versioned_pb2.py
--rw-r--r--   0 maru       (501) staff       (20)     3117 2021-12-01 15:15:05.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_minor_versioned_pb2.pyi
--rw-r--r--   0 maru       (501) staff       (20)     8085 2021-11-30 15:46:32.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_pb2.py
--rw-r--r--   0 maru       (501) staff       (20)     2979 2021-12-01 15:15:05.000000 authedwig-9.1.0/tests/schemas/protos/protobuf_pb2.pyi
--rw-r--r--   0 maru       (501) staff       (20)     1137 2021-06-28 20:51:54.000000 authedwig-9.1.0/tests/settings.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.881425 authedwig-9.1.0/tests/test_backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    16534 2021-06-28 20:51:54.000000 authedwig-9.1.0/tests/test_backends/test_aws.py
--rw-r--r--   0 maru       (501) staff       (20)    15386 2022-12-12 07:35:04.000000 authedwig-9.1.0/tests/test_backends/test_base.py
--rw-r--r--   0 maru       (501) staff       (20)    13585 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_backends/test_gcp.py
--rw-r--r--   0 maru       (501) staff       (20)     2177 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_callback.py
--rw-r--r--   0 maru       (501) staff       (20)      388 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_commands.py
--rw-r--r--   0 maru       (501) staff       (20)     1083 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_consumer.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.883936 authedwig-9.1.0/tests/test_instrumentation/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_instrumentation/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1092 2021-12-01 15:15:05.000000 authedwig-9.1.0/tests/test_instrumentation/conftest.py
--rw-r--r--   0 maru       (501) staff       (20)     5529 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_instrumentation/test_aws.py
--rw-r--r--   0 maru       (501) staff       (20)      692 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_instrumentation/test_base.py
--rw-r--r--   0 maru       (501) staff       (20)     4562 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_instrumentation/test_gcp.py
--rw-r--r--   0 maru       (501) staff       (20)     1998 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_models.py
--rw-r--r--   0 maru       (501) staff       (20)      354 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_publisher.py
--rw-r--r--   0 maru       (501) staff       (20)     5872 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_pytest_plugin.py
--rw-r--r--   0 maru       (501) staff       (20)      591 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_settings.py
--rw-r--r--   0 maru       (501) staff       (20)     1983 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_utils.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.886054 authedwig-9.1.0/tests/test_validators/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/test_validators/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    17568 2021-06-28 19:06:57.000000 authedwig-9.1.0/tests/test_validators/test_jsonschema.py
--rw-r--r--   0 maru       (501) staff       (20)    15823 2021-12-01 15:15:05.000000 authedwig-9.1.0/tests/test_validators/test_protobuf.py
--rw-r--r--   0 maru       (501) staff       (20)     8952 2021-06-28 20:51:54.000000 authedwig-9.1.0/tests/test_validators/test_protobuf_json.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-12-12 07:35:59.887437 authedwig-9.1.0/tests/utils/
--rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/utils/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     1314 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/utils/gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      812 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/utils/mock.py
--rw-r--r--   0 maru       (501) staff       (20)      464 2021-06-25 18:42:16.000000 authedwig-9.1.0/tests/validator.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.373566 authedwig-9.2.0/
+-rw-r--r--   0 maru       (501) staff       (20)      348 2021-06-25 18:42:17.000000 authedwig-9.2.0/CONTRIBUTORS.txt
+-rw-r--r--   0 maru       (501) staff       (20)    11345 2021-06-25 21:01:35.000000 authedwig-9.2.0/LICENSE.md
+-rw-r--r--   0 maru       (501) staff       (20)      223 2021-06-25 18:42:16.000000 authedwig-9.2.0/MANIFEST.in
+-rw-r--r--   0 maru       (501) staff       (20)     7598 2023-07-06 18:59:47.373633 authedwig-9.2.0/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     6501 2021-06-28 19:06:57.000000 authedwig-9.2.0/README.rst
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.362226 authedwig-9.2.0/authedwig.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     7598 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     2546 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)       50 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/entry_points.txt
+-rw-r--r--   0 maru       (501) staff       (20)      785 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        7 2023-07-06 18:59:47.000000 authedwig-9.2.0/authedwig.egg-info/top_level.txt
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.362352 authedwig-9.2.0/examples/
+-rw-r--r--   0 maru       (501) staff       (20)     2507 2021-06-25 18:42:16.000000 authedwig-9.2.0/examples/README.md
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.363845 authedwig-9.2.0/hedwig/
+-rw-r--r--   0 maru       (501) staff       (20)       87 2023-07-06 18:59:46.000000 authedwig-9.2.0/hedwig/__init__.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.365021 authedwig-9.2.0/hedwig/backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    12208 2023-07-06 18:58:44.000000 authedwig-9.2.0/hedwig/backends/aws.py
+-rw-r--r--   0 maru       (501) staff       (20)    11953 2023-07-06 18:58:44.000000 authedwig-9.2.0/hedwig/backends/base.py
+-rw-r--r--   0 maru       (501) staff       (20)      343 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/backends/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)    16070 2023-07-06 18:58:44.000000 authedwig-9.2.0/hedwig/backends/gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      573 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/backends/import_utils.py
+-rw-r--r--   0 maru       (501) staff       (20)      907 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/backends/utils.py
+-rw-r--r--   0 maru       (501) staff       (20)     2283 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/callback.py
+-rw-r--r--   0 maru       (501) staff       (20)      653 2022-12-12 07:35:04.000000 authedwig-9.2.0/hedwig/commands.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.365147 authedwig-9.2.0/hedwig/conf/
+-rw-r--r--   0 maru       (501) staff       (20)     8270 2023-07-06 18:58:44.000000 authedwig-9.2.0/hedwig/conf/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1759 2022-12-12 07:35:04.000000 authedwig-9.2.0/hedwig/consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)     1080 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/exceptions.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.365544 authedwig-9.2.0/hedwig/instrumentation/
+-rw-r--r--   0 maru       (501) staff       (20)     1991 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/instrumentation/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1903 2023-01-04 18:11:02.000000 authedwig-9.2.0/hedwig/instrumentation/compat.py
+-rw-r--r--   0 maru       (501) staff       (20)     7349 2023-01-04 18:11:02.000000 authedwig-9.2.0/hedwig/models.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.365915 authedwig-9.2.0/hedwig/protobuf/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-28 19:06:57.000000 authedwig-9.2.0/hedwig/protobuf/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     8828 2021-11-30 15:46:32.000000 authedwig-9.2.0/hedwig/protobuf/container_pb2.py
+-rw-r--r--   0 maru       (501) staff       (20)     4137 2021-11-30 15:46:32.000000 authedwig-9.2.0/hedwig/protobuf/options_pb2.py
+-rw-r--r--   0 maru       (501) staff       (20)      627 2022-12-12 07:35:04.000000 authedwig-9.2.0/hedwig/publisher.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.366321 authedwig-9.2.0/hedwig/testing/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)      218 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/config.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.366805 authedwig-9.2.0/hedwig/testing/factories/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/factories/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1585 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/factories/base.py
+-rw-r--r--   0 maru       (501) staff       (20)      417 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/factories/jsonschema.py
+-rw-r--r--   0 maru       (501) staff       (20)      984 2021-06-28 20:51:54.000000 authedwig-9.2.0/hedwig/testing/factories/protobuf.py
+-rw-r--r--   0 maru       (501) staff       (20)     3130 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/testing/pytest_plugin.py
+-rw-r--r--   0 maru       (501) staff       (20)      756 2021-06-28 20:51:54.000000 authedwig-9.2.0/hedwig/utils.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.367555 authedwig-9.2.0/hedwig/validators/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/validators/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    11581 2021-06-28 20:51:54.000000 authedwig-9.2.0/hedwig/validators/base.py
+-rw-r--r--   0 maru       (501) staff       (20)    11146 2021-06-28 19:06:57.000000 authedwig-9.2.0/hedwig/validators/jsonschema.py
+-rw-r--r--   0 maru       (501) staff       (20)     1776 2021-06-25 18:42:16.000000 authedwig-9.2.0/hedwig/validators/jsonschema_container_schema.json
+-rw-r--r--   0 maru       (501) staff       (20)    11996 2022-12-12 07:35:04.000000 authedwig-9.2.0/hedwig/validators/protobuf.py
+-rw-r--r--   0 maru       (501) staff       (20)      252 2021-06-25 18:42:16.000000 authedwig-9.2.0/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      375 2023-07-06 18:59:47.373879 authedwig-9.2.0/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     3836 2022-12-12 07:35:04.000000 authedwig-9.2.0/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.369759 authedwig-9.2.0/tests/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     4848 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/conftest.py
+-rw-r--r--   0 maru       (501) staff       (20)      171 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/handlers.py
+-rw-r--r--   0 maru       (501) staff       (20)      161 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/models.py
+-rw-r--r--   0 maru       (501) staff       (20)      269 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/protobuf_factory.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.370366 authedwig-9.2.0/tests/schemas/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/schemas/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     4292 2021-06-28 19:06:57.000000 authedwig-9.2.0/tests/schemas/jsonschema.json
+-rw-r--r--   0 maru       (501) staff       (20)      947 2021-06-28 20:51:54.000000 authedwig-9.2.0/tests/schemas/protobuf.proto
+-rw-r--r--   0 maru       (501) staff       (20)      692 2021-06-28 20:51:54.000000 authedwig-9.2.0/tests/schemas/protobuf_bad.proto
+-rw-r--r--   0 maru       (501) staff       (20)      725 2021-06-28 19:06:57.000000 authedwig-9.2.0/tests/schemas/protobuf_minor_versioned.proto
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.371294 authedwig-9.2.0/tests/schemas/protos/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/schemas/protos/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     6345 2021-11-30 15:46:32.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_bad_pb2.py
+-rw-r--r--   0 maru       (501) staff       (20)     2506 2021-12-01 15:15:05.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_bad_pb2.pyi
+-rw-r--r--   0 maru       (501) staff       (20)     8628 2021-11-30 15:46:32.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_minor_versioned_pb2.py
+-rw-r--r--   0 maru       (501) staff       (20)     3117 2021-12-01 15:15:05.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_minor_versioned_pb2.pyi
+-rw-r--r--   0 maru       (501) staff       (20)     8085 2021-11-30 15:46:32.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_pb2.py
+-rw-r--r--   0 maru       (501) staff       (20)     2979 2021-12-01 15:15:05.000000 authedwig-9.2.0/tests/schemas/protos/protobuf_pb2.pyi
+-rw-r--r--   0 maru       (501) staff       (20)     1137 2021-06-28 20:51:54.000000 authedwig-9.2.0/tests/settings.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.371858 authedwig-9.2.0/tests/test_backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    16963 2023-07-06 18:58:44.000000 authedwig-9.2.0/tests/test_backends/test_aws.py
+-rw-r--r--   0 maru       (501) staff       (20)    16227 2023-07-06 18:58:44.000000 authedwig-9.2.0/tests/test_backends/test_base.py
+-rw-r--r--   0 maru       (501) staff       (20)    14084 2023-07-06 18:58:44.000000 authedwig-9.2.0/tests/test_backends/test_gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)     2177 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_callback.py
+-rw-r--r--   0 maru       (501) staff       (20)      388 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_commands.py
+-rw-r--r--   0 maru       (501) staff       (20)     1083 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_consumer.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.372479 authedwig-9.2.0/tests/test_instrumentation/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_instrumentation/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1092 2021-12-01 15:15:05.000000 authedwig-9.2.0/tests/test_instrumentation/conftest.py
+-rw-r--r--   0 maru       (501) staff       (20)     5529 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_instrumentation/test_aws.py
+-rw-r--r--   0 maru       (501) staff       (20)      692 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_instrumentation/test_base.py
+-rw-r--r--   0 maru       (501) staff       (20)     4562 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_instrumentation/test_gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)     1998 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_models.py
+-rw-r--r--   0 maru       (501) staff       (20)      354 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)     5872 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_pytest_plugin.py
+-rw-r--r--   0 maru       (501) staff       (20)      591 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_settings.py
+-rw-r--r--   0 maru       (501) staff       (20)     1983 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_utils.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.373081 authedwig-9.2.0/tests/test_validators/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/test_validators/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    17568 2021-06-28 19:06:57.000000 authedwig-9.2.0/tests/test_validators/test_jsonschema.py
+-rw-r--r--   0 maru       (501) staff       (20)    15823 2021-12-01 15:15:05.000000 authedwig-9.2.0/tests/test_validators/test_protobuf.py
+-rw-r--r--   0 maru       (501) staff       (20)     8952 2021-06-28 20:51:54.000000 authedwig-9.2.0/tests/test_validators/test_protobuf_json.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-07-06 18:59:47.373448 authedwig-9.2.0/tests/utils/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/utils/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     1314 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/utils/gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      812 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/utils/mock.py
+-rw-r--r--   0 maru       (501) staff       (20)      464 2021-06-25 18:42:16.000000 authedwig-9.2.0/tests/validator.py
```

### Comparing `authedwig-9.1.0/README.rst` & `authedwig-9.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/authedwig.egg-info/SOURCES.txt` & `authedwig-9.2.0/authedwig.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CONTRIBUTORS.txt
+LICENSE.md
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 authedwig.egg-info/PKG-INFO
 authedwig.egg-info/SOURCES.txt
```

### Comparing `authedwig-9.1.0/authedwig.egg-info/requires.txt` & `authedwig-9.2.0/authedwig.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/examples/README.md` & `authedwig-9.2.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/backends/aws.py` & `authedwig-9.2.0/hedwig/backends/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,18 @@
             'MaxNumberOfMessages': num_messages,
             'WaitTimeSeconds': self.WAIT_TIME_SECONDS,
             'AttributeNames': ['All'],
             'MessageAttributeNames': ['All'],
         }
         if visibility_timeout is not None:
             params['VisibilityTimeout'] = visibility_timeout
-        return self._get_queue().receive_messages(**params)
+        try:
+            return self._get_queue().receive_messages(**params)
+        finally:
+            self._call_heartbeat_hook()
 
     def process_message(self, queue_message) -> None:
         attributes = {k: o['StringValue'] for k, o in (queue_message.message_attributes or {}).items()}
         # body is always UTF-8 string
         message_payload = queue_message.body
         if attributes.get("hedwig_encoding") == "base64":
             message_payload = base64.decodebytes(message_payload.encode())
@@ -208,14 +211,15 @@
         Extends visibility timeout of a message on a given priority queue for long running tasks.
         """
         receipt = metadata.receipt
         queue_url = self.sqs_client.get_queue_url(QueueName=self.queue_name)['QueueUrl']
         self.sqs_client.change_message_visibility(
             QueueUrl=queue_url, ReceiptHandle=receipt, VisibilityTimeout=visibility_timeout_s
         )
+        self._call_heartbeat_hook(force=True)
 
     def requeue_dead_letter(self, num_messages: int = 10, visibility_timeout: Optional[int] = None) -> None:
         """
         Re-queues everything in the Hedwig DLQ back into the Hedwig queue.
 
         :param num_messages: Maximum number of messages to fetch in one SQS call. Defaults to 10.
         :param visibility_timeout: The number of seconds the message should remain invisible to other queue readers.
```

### Comparing `authedwig-9.1.0/hedwig/backends/base.py` & `authedwig-9.2.0/hedwig/backends/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import logging
 import threading
 import uuid
 from concurrent.futures import Future
 from contextlib import contextmanager
+from datetime import datetime, timedelta
 from typing import Optional, Union, Generator, List, Any, Dict, Tuple, Iterator
 
 from hedwig.conf import settings
 from hedwig.exceptions import ValidationError, IgnoreException, LoggingException, RetryException
 from hedwig.models import Message
 from hedwig.utils import log
 
@@ -85,14 +86,19 @@
 
         return result
 
 
 class HedwigConsumerBaseBackend:
     def __init__(self) -> None:
         self._error_count = 0
+        self._heartbeat_called_at = datetime(1970, 1, 1)
+        self._heartbeat_interval_timedelta = timedelta(seconds=settings.HEDWIG_HEARTBEAT_INTERVAL_S)
+
+    def heartbeat_hook_kwargs(self) -> dict:
+        return {"error_count": self.error_count}
 
     @staticmethod
     def pre_process_hook_kwargs(queue_message) -> dict:
         return {}
 
     @staticmethod
     def post_process_hook_kwargs(queue_message) -> dict:
@@ -149,16 +155,15 @@
                             extra={'queue_message': queue_message},
                         )
                         self.nack_message(queue_message)
                         continue
 
                     try:
                         self.process_message(queue_message)
-                        if self._error_count:  # type: ignore
-                            self._error_count = 0
+                        self._error_count = 0
                     except IgnoreException:
                         log(__name__, logging.INFO, 'Ignoring task', extra={'queue_message': queue_message})
                     except LoggingException as e:
                         # log with message and extra
                         log(__name__, logging.ERROR, str(e), extra=e.extra, exc_info=True)
                         self.nack_message(queue_message)
                         continue
@@ -168,14 +173,16 @@
                         self.nack_message(queue_message)
                         continue
                     except Exception:
                         log(__name__, logging.ERROR, 'Exception while processing message', exc_info=True)
                         self.nack_message(queue_message)
                         self._error_count += 1
                         continue
+                    finally:
+                        self._call_heartbeat_hook()
 
                     try:
                         settings.HEDWIG_POST_PROCESS_HOOK(**self.post_process_hook_kwargs(queue_message))
                     except Exception:
                         log(
                             __name__,
                             logging.ERROR,
@@ -248,14 +255,24 @@
             # side-effect: validates the callback
             _ = message.callback
             return message
         except ValidationError:
             _log_invalid_message(message_payload)
             raise
 
+    def _call_heartbeat_hook(self, force: bool = False):
+        now = datetime.utcnow()
+        if force or self._heartbeat_called_at + self._heartbeat_interval_timedelta < now:
+            try:
+                settings.HEDWIG_HEARTBEAT_HOOK(**self.heartbeat_hook_kwargs())
+            except Exception:
+                log(__name__, logging.ERROR, 'Exception in heartbeat hook', exc_info=True)
+            finally:
+                self._heartbeat_called_at = now
+
     @property
     def error_count(self) -> int:
         """
         Returns the number of consecutive errors occurred when trying to process messages from the queue.
 
         Resets to 0 when a message is successfully processed.
```

### Comparing `authedwig-9.1.0/hedwig/backends/gcp.py` & `authedwig-9.2.0/hedwig/backends/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,25 +274,25 @@
             )
 
         while not shutdown_event.is_set():
             try:
                 message = work_queue.get(timeout=1)
                 yield message
             except Empty:
-                pass
+                self._call_heartbeat_hook()
 
         for future in futures:
             future.cancel()
 
         # drain the queue
         try:
             while True:
                 yield work_queue.get(block=False)
         except Empty:
-            pass
+            self._call_heartbeat_hook()
 
     def process_message(self, queue_message: MessageWrapper) -> None:
         # body is always bytes
         message_payload = queue_message.message.data
         attributes = queue_message.message.attributes
         if attributes.get("hedwig_encoding") == "utf8":
             message_payload = message_payload.decode('utf8')
@@ -329,14 +329,15 @@
         if visibility_timeout_s < 0 or visibility_timeout_s > 600:
             raise ValueError("Invalid visibility_timeout_s")
         self.subscriber.modify_ack_deadline(
             subscription=metadata.subscription_path,
             ack_ids=[metadata.ack_id],
             ack_deadline_seconds=visibility_timeout_s,
         )
+        self._call_heartbeat_hook(force=True)
 
     def requeue_dead_letter(self, num_messages: int = 10, visibility_timeout: Optional[int] = None) -> None:
         """
         Re-queues everything in the Hedwig DLQ back into the Hedwig queue.
 
         :param num_messages: Maximum number of messages to fetch in one call. Defaults to 10.
         :param visibility_timeout: The number of seconds the message should remain invisible to other queue readers.
```

### Comparing `authedwig-9.1.0/hedwig/backends/import_utils.py` & `authedwig-9.2.0/hedwig/backends/import_utils.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/backends/utils.py` & `authedwig-9.2.0/hedwig/backends/utils.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/callback.py` & `authedwig-9.2.0/hedwig/callback.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/commands.py` & `authedwig-9.2.0/hedwig/commands.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/conf/__init__.py` & `authedwig-9.2.0/hedwig/conf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     'GOOGLE_APPLICATION_CREDENTIALS': None,
     'GOOGLE_CLOUD_PROJECT': None,
     'GOOGLE_PUBSUB_READ_TIMEOUT_S': 5,
     'HEDWIG_CALLBACKS': {},
     'HEDWIG_CONSUMER_BACKEND': None,
     'HEDWIG_DATA_VALIDATOR_CLASS': 'hedwig.validators.jsonschema.JSONSchemaValidator',
     'HEDWIG_DEFAULT_HEADERS': 'hedwig.conf.default_headers_hook',
+    'HEDWIG_HEARTBEAT_INTERVAL_S': 15,
+    'HEDWIG_HEARTBEAT_HOOK': 'hedwig.conf.noop_hook',
     'HEDWIG_MESSAGE_ROUTING': {},
     'HEDWIG_PRE_PROCESS_HOOK': 'hedwig.conf.noop_hook',
     'HEDWIG_POST_PROCESS_HOOK': 'hedwig.conf.noop_hook',
     'HEDWIG_PUBLISHER': None,
     'HEDWIG_PUBLISHER_BACKEND': None,
     'HEDWIG_PUBLISHER_GCP_BATCH_SETTINGS': (),
     'HEDWIG_QUEUE': None,
@@ -56,14 +58,15 @@
 
 
 # List of settings that may be in string import notation.
 _IMPORT_STRINGS = (
     'HEDWIG_CONSUMER_BACKEND',
     'HEDWIG_DATA_VALIDATOR_CLASS',
     'HEDWIG_DEFAULT_HEADERS',
+    'HEDWIG_HEARTBEAT_HOOK',
     'HEDWIG_PRE_PROCESS_HOOK',
     'HEDWIG_POST_PROCESS_HOOK',
     'HEDWIG_PUBLISHER_BACKEND',
 )
 
 # List of settings that will be dicts with values as string import notation.
 _IMPORT_DICT_VALUES = ('HEDWIG_CALLBACKS',)
```

### Comparing `authedwig-9.1.0/hedwig/consumer.py` & `authedwig-9.2.0/hedwig/consumer.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/exceptions.py` & `authedwig-9.2.0/hedwig/exceptions.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/instrumentation/__init__.py` & `authedwig-9.2.0/hedwig/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/instrumentation/compat.py` & `authedwig-9.2.0/hedwig/instrumentation/compat.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/models.py` & `authedwig-9.2.0/hedwig/models.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/protobuf/container_pb2.py` & `authedwig-9.2.0/hedwig/protobuf/container_pb2.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/protobuf/options_pb2.py` & `authedwig-9.2.0/hedwig/protobuf/options_pb2.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/publisher.py` & `authedwig-9.2.0/hedwig/publisher.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/testing/factories/base.py` & `authedwig-9.2.0/hedwig/testing/factories/base.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/testing/factories/protobuf.py` & `authedwig-9.2.0/hedwig/testing/factories/protobuf.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/testing/pytest_plugin.py` & `authedwig-9.2.0/hedwig/testing/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/utils.py` & `authedwig-9.2.0/hedwig/utils.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/validators/base.py` & `authedwig-9.2.0/hedwig/validators/base.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/validators/jsonschema.py` & `authedwig-9.2.0/hedwig/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/validators/jsonschema_container_schema.json` & `authedwig-9.2.0/hedwig/validators/jsonschema_container_schema.json`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/hedwig/validators/protobuf.py` & `authedwig-9.2.0/hedwig/validators/protobuf.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/setup.py` & `authedwig-9.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/conftest.py` & `authedwig-9.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/jsonschema.json` & `authedwig-9.2.0/tests/schemas/jsonschema.json`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protobuf.proto` & `authedwig-9.2.0/tests/schemas/protobuf.proto`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protobuf_bad.proto` & `authedwig-9.2.0/tests/schemas/protobuf_bad.proto`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protobuf_minor_versioned.proto` & `authedwig-9.2.0/tests/schemas/protobuf_minor_versioned.proto`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_bad_pb2.py` & `authedwig-9.2.0/tests/schemas/protos/protobuf_bad_pb2.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_bad_pb2.pyi` & `authedwig-9.2.0/tests/schemas/protos/protobuf_bad_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_minor_versioned_pb2.py` & `authedwig-9.2.0/tests/schemas/protos/protobuf_minor_versioned_pb2.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_minor_versioned_pb2.pyi` & `authedwig-9.2.0/tests/schemas/protos/protobuf_minor_versioned_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_pb2.py` & `authedwig-9.2.0/tests/schemas/protos/protobuf_pb2.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/schemas/protos/protobuf_pb2.pyi` & `authedwig-9.2.0/tests/schemas/protos/protobuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/settings.py` & `authedwig-9.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_backends/test_aws.py` & `authedwig-9.2.0/tests/test_backends/test_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,33 +87,36 @@
         with pytest.raises(ValidationError) as exc_info:
             message.publish()
         assert isinstance(exc_info.value.__context__, CallbackNotFound)
 
 
 pre_process_hook = mock.MagicMock()
 post_process_hook = mock.MagicMock()
+heartbeat_hook = mock.MagicMock()
 
 
 @pytest.fixture(name='sqs_consumer')
 def _sqs_consumer(mock_boto3):
     return aws.AWSSQSConsumerBackend()
 
 
 @pytest.fixture(name='sns_consumer')
 def _sns_consumer(mock_boto3):
     return aws.AWSSNSConsumerBackend()
 
 
 @pytest.fixture(name='prepost_process_hooks')
 def _prepost_process_hooks(settings):
+    settings.HEDWIG_HEARTBEAT_HOOK = 'tests.test_backends.test_aws.heartbeat_hook'
     settings.HEDWIG_PRE_PROCESS_HOOK = 'tests.test_backends.test_aws.pre_process_hook'
     settings.HEDWIG_POST_PROCESS_HOOK = 'tests.test_backends.test_aws.post_process_hook'
     yield
-    pre_process_hook.reset_mock()
-    post_process_hook.reset_mock()
+    pre_process_hook.reset_mock(side_effect=True)
+    post_process_hook.reset_mock(side_effect=True)
+    heartbeat_hook.reset_mock(side_effect=True)
 
 
 class TestSQSConsumer:
     def test_client_and_resource_instantiation(self, sqs_consumer, mock_boto3):
         # make sure client and resource are initialized
         sqs_consumer.sqs_client
         sqs_consumer.sqs_resource
@@ -130,15 +133,15 @@
             region_name=hedwig_settings.AWS_REGION,
             aws_access_key_id=hedwig_settings.AWS_ACCESS_KEY,
             aws_secret_access_key=hedwig_settings.AWS_SECRET_KEY,
             aws_session_token=hedwig_settings.AWS_SESSION_TOKEN,
             endpoint_url=hedwig_settings.AWS_ENDPOINT_SQS,
         )
 
-    def test_pull_messages(self, sqs_consumer):
+    def test_pull_messages(self, sqs_consumer, prepost_process_hooks):
         num_messages = 1
         visibility_timeout = 10
         queue = mock.MagicMock()
         sqs_consumer.sqs_resource.get_queue_by_name = mock.MagicMock(return_value=queue)
 
         sqs_consumer.pull_messages(num_messages, visibility_timeout)
 
@@ -146,16 +149,17 @@
         queue.receive_messages.assert_called_once_with(
             MaxNumberOfMessages=num_messages,
             MessageAttributeNames=['All'],
             AttributeNames=['All'],
             VisibilityTimeout=visibility_timeout,
             WaitTimeSeconds=sqs_consumer.WAIT_TIME_SECONDS,
         )
+        heartbeat_hook.assert_called_once_with(error_count=0)
 
-    def test_extend_visibility_timeout(self, sqs_consumer):
+    def test_extend_visibility_timeout(self, sqs_consumer, prepost_process_hooks):
         visibility_timeout_s = 10
         receipt = "receipt"
         sent_time = datetime.now(timezone.utc)
         first_receive_time = datetime.now(timezone.utc)
         receive_count = 1
 
         sqs_consumer.sqs_client.get_queue_url = mock.MagicMock(return_value={"QueueUrl": "DummyQueueUrl"})
@@ -164,14 +168,15 @@
             visibility_timeout_s, AWSMetadata(receipt, first_receive_time, sent_time, receive_count)
         )
 
         sqs_consumer.sqs_client.get_queue_url.assert_called_once_with(QueueName=sqs_consumer.queue_name)
         sqs_consumer.sqs_client.change_message_visibility.assert_called_once_with(
             QueueUrl='DummyQueueUrl', ReceiptHandle='receipt', VisibilityTimeout=10
         )
+        heartbeat_hook.assert_called_once_with(error_count=0)
 
     def test_success_requeue_dead_letter(self, sqs_consumer):
         sqs_consumer = aws.AWSSQSConsumerBackend(dlq=True)
         num_messages = 3
         visibility_timeout = 4
 
         messages = [mock.MagicMock() for _ in range(num_messages)]
@@ -290,14 +295,15 @@
                 receive_count,
             ),
         )
         message_mock.exec_callback.assert_called_once_with()
         queue_message.delete.assert_called_once_with()
         pre_process_hook.assert_called_once_with(sqs_queue_message=queue_message)
         post_process_hook.assert_called_once_with(sqs_queue_message=queue_message)
+        heartbeat_hook.assert_called_once_with(error_count=0)
 
 
 class TestSNSConsumer:
     @mock.patch('hedwig.backends.aws.AWSSNSConsumerBackend.process_message')
     def test_process_messages(self, mock_process_message, sns_consumer):
         records = {"attributes": {}}, {"attributes": {}}
         event = {'Records': records}
```

### Comparing `authedwig-9.1.0/tests/test_backends/test_base.py` & `authedwig-9.2.0/tests/test_backends/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,26 @@
         mock_exec_callback.side_effect = Exception
         with pytest.raises(mock_exec_callback.side_effect):
             consumer_backend.message_handler(*message.serialize(), None)
 
 
 pre_process_hook = mock.MagicMock()
 post_process_hook = mock.MagicMock()
+heartbeat_hook = mock.MagicMock()
+
+
+@pytest.fixture(name='prepost_process_hooks')
+def _prepost_process_hooks(settings):
+    settings.HEDWIG_HEARTBEAT_HOOK = 'tests.test_backends.test_base.heartbeat_hook'
+    settings.HEDWIG_PRE_PROCESS_HOOK = 'tests.test_backends.test_base.pre_process_hook'
+    settings.HEDWIG_POST_PROCESS_HOOK = 'tests.test_backends.test_base.post_process_hook'
+    yield
+    pre_process_hook.reset_mock(side_effect=True)
+    post_process_hook.reset_mock(side_effect=True)
+    heartbeat_hook.reset_mock(side_effect=True)
 
 
 class TestFetchAndProcessMessages:
     def test_success(self, consumer_backend):
         num_messages = 3
         visibility_timeout = 4
         shutdown_event = threading.Event()
@@ -120,37 +132,33 @@
 
             logging_mock.assert_called_once_with(
                 'hedwig.backends.base', logging.ERROR, mock.ANY, exc_info=True, extra=mock.ANY
             )
 
         consumer_backend.ack_message.assert_called_once_with(queue_message)
 
-    def test_pre_process_hook(self, consumer_backend, settings):
+    def test_pre_process_hook(self, consumer_backend, prepost_process_hooks):
         shutdown_event = threading.Event()
-        pre_process_hook.reset_mock()
-        settings.HEDWIG_PRE_PROCESS_HOOK = 'tests.test_backends.test_base.pre_process_hook'
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock()
         mock_return_once(consumer_backend.pull_messages, [mock.MagicMock(), mock.MagicMock()], [], shutdown_event)
 
         consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
         pre_process_hook.assert_has_calls(
             [
                 mock.call(**consumer_backend.pre_process_hook_kwargs(x))
                 for x in consumer_backend.pull_messages.return_value
             ]
         )
 
-    def test_pre_process_hook_exception(self, consumer_backend, settings):
+    def test_pre_process_hook_exception(self, consumer_backend, prepost_process_hooks):
         shutdown_event = threading.Event()
-        pre_process_hook.reset_mock()
         pre_process_hook.side_effect = RuntimeError('fail')
         queue_message = mock.MagicMock()
-        settings.HEDWIG_PRE_PROCESS_HOOK = 'tests.test_backends.test_base.pre_process_hook'
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock()
         mock_return_once(consumer_backend.pull_messages, [queue_message], [], shutdown_event)
 
         with mock.patch('hedwig.backends.base.log') as logging_mock:
             consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
@@ -161,39 +169,35 @@
                 exc_info=True,
                 extra={'queue_message': queue_message},
             )
 
         pre_process_hook.assert_called_once_with(**consumer_backend.pre_process_hook_kwargs(queue_message))
         queue_message.delete.assert_not_called()
 
-    def test_post_process_hook(self, consumer_backend, settings):
+    def test_post_process_hook(self, consumer_backend, prepost_process_hooks):
         shutdown_event = threading.Event()
-        post_process_hook.reset_mock()
-        settings.HEDWIG_POST_PROCESS_HOOK = 'tests.test_backends.test_base.post_process_hook'
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock()
         mock_return_once(consumer_backend.pull_messages, [mock.MagicMock(), mock.MagicMock()], [], shutdown_event)
 
         consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
         post_process_hook.assert_has_calls(
             [
                 mock.call(**consumer_backend.post_process_hook_kwargs(x))
                 for x in consumer_backend.pull_messages.return_value
             ]
         )
 
-    def test_post_process_hook_exception(self, consumer_backend, settings):
+    def test_post_process_hook_exception(self, consumer_backend, prepost_process_hooks):
         shutdown_event = threading.Event()
-        settings.HEDWIG_POST_PROCESS_HOOK = 'tests.test_backends.test_base.post_process_hook'
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock()
         queue_message = mock.MagicMock()
         mock_return_once(consumer_backend.pull_messages, [queue_message], [], shutdown_event)
-        post_process_hook.reset_mock()
         post_process_hook.side_effect = RuntimeError('fail')
 
         with mock.patch('hedwig.backends.base.log') as logging_mock:
             consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
             logging_mock.assert_called_once_with(
                 'hedwig.backends.base',
@@ -257,15 +261,15 @@
         # First message is processed normally, second and third raise an exception
         consumer_backend.process_message = mock.MagicMock(side_effect=[None, Exception, Exception])
 
         with mock.patch('hedwig.backends.base.log') as logging_mock:
             consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
             logging_mock.assert_called_with('hedwig.backends.base', logging.ERROR, mock.ANY, exc_info=True)
-            logging_mock.call_count == 2
+            assert logging_mock.call_count == 2
 
         assert consumer_backend.error_count == 2
 
     def test_success_reset_error_count(self, consumer_backend):
         shutdown_event = threading.Event()
         queue_message = mock.MagicMock()
         consumer_backend.pull_messages = mock.MagicMock()
@@ -277,14 +281,32 @@
         # process message normally
         consumer_backend.process_message = mock.MagicMock()
         consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
 
         # error count is reset to 0
         assert consumer_backend.error_count == 0
 
+    def test_heartbeat_hook_called_once_when_multiple_messages_are_processed(
+        self, consumer_backend, prepost_process_hooks
+    ):
+        shutdown_event = threading.Event()
+        queue_message = mock.MagicMock()
+        consumer_backend.pull_messages = mock.MagicMock()
+        mock_return_once(
+            consumer_backend.pull_messages, [queue_message, queue_message, queue_message], [], shutdown_event
+        )
+
+        # process message normally
+        consumer_backend.process_message = mock.MagicMock()
+        consumer_backend.fetch_and_process_messages(shutdown_event=shutdown_event)
+
+        assert pre_process_hook.call_count == 3
+        assert post_process_hook.call_count == 3
+        heartbeat_hook.assert_called_once_with(error_count=0)
+
 
 default_headers = mock.MagicMock(return_value={'mickey': 'mouse'})
 
 
 @pytest.fixture(name='default_headers_hook')
 def _default_headers_hook(settings):
     settings.HEDWIG_DEFAULT_HEADERS = 'tests.test_backends.test_base.default_headers'
```

### Comparing `authedwig-9.1.0/tests/test_backends/test_gcp.py` & `authedwig-9.2.0/tests/test_backends/test_gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         with pytest.raises(ValidationError) as exc_info:
             message.publish()
         assert isinstance(exc_info.value.__context__, CallbackNotFound)
 
 
 pre_process_hook = mock.MagicMock()
 post_process_hook = mock.MagicMock()
+heartbeat_hook = mock.MagicMock()
 
 
 @pytest.fixture(name='subscription_paths')
 def _subscription_paths(gcp_settings):
     return [mock.MagicMock() for _ in range(len(gcp_settings.HEDWIG_SUBSCRIPTIONS) + 1)]
 
 
@@ -122,23 +123,25 @@
 def _gcp_consumer(mock_pubsub_v1, gcp_settings, subscription_paths):
     mock_pubsub_v1.SubscriberClient.subscription_path.side_effect = subscription_paths
     return gcp.GooglePubSubConsumerBackend()
 
 
 @pytest.fixture(name='prepost_process_hooks')
 def _prepost_process_hooks(gcp_settings):
+    gcp_settings.HEDWIG_HEARTBEAT_HOOK = 'tests.test_backends.test_gcp.heartbeat_hook'
     gcp_settings.HEDWIG_PRE_PROCESS_HOOK = 'tests.test_backends.test_gcp.pre_process_hook'
     gcp_settings.HEDWIG_POST_PROCESS_HOOK = 'tests.test_backends.test_gcp.post_process_hook'
     yield
-    pre_process_hook.reset_mock()
-    post_process_hook.reset_mock()
+    pre_process_hook.reset_mock(side_effect=True)
+    post_process_hook.reset_mock(side_effect=True)
+    heartbeat_hook.reset_mock(side_effect=True)
 
 
 class TestGCPConsumer:
-    def test_pull_messages(self, mock_pubsub_v1, gcp_consumer, subscription_paths):
+    def test_pull_messages(self, mock_pubsub_v1, gcp_consumer, subscription_paths, prepost_process_hooks):
         shutdown_event = threading.Event()
         num_messages = 1
         visibility_timeout = 10
         messages = [mock.MagicMock(), mock.MagicMock(), mock.MagicMock(), mock.MagicMock()]
         futures = [mock.MagicMock(), mock.MagicMock(), mock.MagicMock(), mock.MagicMock()]
 
         def subscribe_side_effect(subscription_path, callback, flow_control, scheduler):
@@ -188,43 +191,46 @@
         # verify subscriber call for each path
         gcp_consumer.subscriber.subscribe.assert_has_calls(
             [
                 mock.call(subscription_paths[x], callback=None, flow_control=flow_control, scheduler=mock.ANY)
                 for x in range(4)
             ]
         )
+        heartbeat_hook.assert_called_once_with(error_count=0)
 
-    def test_success_extend_visibility_timeout(self, gcp_consumer):
+    def test_success_extend_visibility_timeout(self, gcp_consumer, prepost_process_hooks):
         visibility_timeout_s = 10
         ack_id = "dummy_ack_id"
         subscription_path = "subscriptions/foobar"
         publish_time = datetime.now(timezone.utc)
         delivery_attempt = 1
 
         gcp_consumer.extend_visibility_timeout(
             visibility_timeout_s, GoogleMetadata(ack_id, subscription_path, publish_time, delivery_attempt)
         )
 
         gcp_consumer.subscriber.modify_ack_deadline.assert_called_once_with(
             subscription=subscription_path, ack_ids=[ack_id], ack_deadline_seconds=visibility_timeout_s
         )
+        heartbeat_hook.assert_called_once_with(error_count=0)
 
     @pytest.mark.parametrize("visibility_timeout", [-1, 601])
-    def test_failure_extend_visibility_timeout(self, visibility_timeout, gcp_consumer):
+    def test_failure_extend_visibility_timeout(self, visibility_timeout, gcp_consumer, prepost_process_hooks):
         subscription_path = "subscriptions/foobar"
         publish_time = datetime.now(timezone.utc)
         delivery_attempt = 1
 
         with pytest.raises(ValueError):
             gcp_consumer.extend_visibility_timeout(
                 visibility_timeout, GoogleMetadata('dummy_ack_id', subscription_path, publish_time, delivery_attempt)
             )
 
         gcp_consumer.subscriber.subscription_path.assert_not_called()
         gcp_consumer.subscriber.modify_ack_deadline.assert_not_called()
+        heartbeat_hook.assert_not_called()
 
     def test_success_requeue_dead_letter(self, mock_pubsub_v1, message, use_transport_message_attrs):
         gcp_consumer = gcp.GooglePubSubConsumerBackend(dlq=True)
 
         num_messages = 1
         visibility_timeout = 4
         subscription_path = gcp_consumer._subscription_paths[0]
@@ -319,7 +325,8 @@
                 queue_message.publish_time,
                 queue_message.delivery_attempt,
             ),
         )
         queue_message.ack.assert_called_once_with()
         pre_process_hook.assert_called_once_with(google_pubsub_message=queue_message)
         post_process_hook.assert_called_once_with(google_pubsub_message=queue_message)
+        heartbeat_hook.assert_called_once_with(error_count=0)
```

### Comparing `authedwig-9.1.0/tests/test_callback.py` & `authedwig-9.2.0/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_consumer.py` & `authedwig-9.2.0/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_instrumentation/conftest.py` & `authedwig-9.2.0/tests/test_instrumentation/conftest.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_instrumentation/test_aws.py` & `authedwig-9.2.0/tests/test_instrumentation/test_aws.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_instrumentation/test_base.py` & `authedwig-9.2.0/tests/test_instrumentation/test_base.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_instrumentation/test_gcp.py` & `authedwig-9.2.0/tests/test_instrumentation/test_gcp.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_models.py` & `authedwig-9.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_pytest_plugin.py` & `authedwig-9.2.0/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_settings.py` & `authedwig-9.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_utils.py` & `authedwig-9.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_validators/test_jsonschema.py` & `authedwig-9.2.0/tests/test_validators/test_jsonschema.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_validators/test_protobuf.py` & `authedwig-9.2.0/tests/test_validators/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/test_validators/test_protobuf_json.py` & `authedwig-9.2.0/tests/test_validators/test_protobuf_json.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/utils/gcp.py` & `authedwig-9.2.0/tests/utils/gcp.py`

 * *Files identical despite different names*

### Comparing `authedwig-9.1.0/tests/utils/mock.py` & `authedwig-9.2.0/tests/utils/mock.py`

 * *Files identical despite different names*

