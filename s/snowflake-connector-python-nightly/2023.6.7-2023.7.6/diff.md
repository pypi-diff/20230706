# Comparing `tmp/snowflake-connector-python-nightly-2023.6.7.tar.gz` & `tmp/snowflake-connector-python-nightly-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-connector-python-nightly-2023.6.7.tar", last modified: Wed Jun  7 04:07:02 2023, max compression
+gzip compressed data, was "snowflake-connector-python-nightly-2023.7.6.tar", last modified: Thu Jul  6 04:07:31 2023, max compression
```

## Comparing `snowflake-connector-python-nightly-2023.6.7.tar` & `snowflake-connector-python-nightly-2023.7.6.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    47673 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 04:06:48.000000 snowflake-connector-python-nightly-2023.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-07 04:07:02.196873 snowflake-connector-python-nightly-2023.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-07 04:06:49.000000 snowflake-connector-python-nightly-2023.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.172872 snowflake-connector-python-nightly-2023.6.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.172872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.180872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-07 04:06:50.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/_query_context_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/arrow_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/arrow_iterator.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.180872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/by_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/idtoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/okta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/usrpwdmfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/webbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/azure_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/bind_upload_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    66742 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/connection_diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter_issue23517.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter_snowsql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.172872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.184872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.184872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-07 04:06:53.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.184872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.184872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/Logging/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/Logging/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/Logging/logging.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    57032 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/dbapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/encryption_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/errorcode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_compression_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    47199 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_transfer_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/gcs_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/gzip_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-07 04:06:51.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/local_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39886 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ocsp_asn1crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    68441 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ocsp_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/pandas_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/result_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/result_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/s3_storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/secret_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sf_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sfbinaryformat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sfdatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/snow_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sqlstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ssd_internal_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ssl_wrap_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/storage_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/telemetry_oob.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.184872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_ocsp_response_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/probe_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/url_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/util_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.188872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.188872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 04:06:54.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.188872 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-06-07 04:06:55.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-06-07 04:06:56.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 04:06:52.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:07:02.192873 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 04:07:02.000000 snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    48322 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-06 04:07:31.115971 snowflake-connector-python-nightly-2023.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-06 04:07:09.000000 snowflake-connector-python-nightly-2023.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.071971 snowflake-connector-python-nightly-2023.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.067971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.095970 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-06 04:07:12.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-06 04:07:12.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/_query_context_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 04:07:12.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-06 04:07:12.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/arrow_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/arrow_iterator.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.095970 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27245 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/by_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/idtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/okta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/usrpwdmfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/webbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/azure_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/bind_upload_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67296 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30347 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/connection_diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter_issue23517.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter_snowsql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.067971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.099971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14375 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-06 04:07:16.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/IColumnConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/IntConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.099971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-06 04:07:17.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.103971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.103971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/Logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/Logging/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/Logging/logging.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    57032 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/dbapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/encryption_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-06 04:07:13.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/errorcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_compression_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47199 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_transfer_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16068 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/gcs_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/gzip_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/local_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40861 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ocsp_asn1crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68441 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ocsp_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19498 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/pandas_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:14.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/result_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/s3_storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/secret_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sf_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sfbinaryformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12449 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sfdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/snow_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sqlstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ssd_internal_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ssl_wrap_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/storage_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/telemetry_oob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.103971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_ocsp_response_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/probe_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/util_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.103971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.103971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19602 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-06 04:07:18.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35231 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30180 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33450 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.107971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20300 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39128 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.107971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.107971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17632 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17055 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34416 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-06 04:07:19.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34665 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19786 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30761 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-06 04:07:20.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22003 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssltransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-06 04:07:22.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-06 04:07:21.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-06 04:07:15.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:07:31.111971 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 04:07:31.000000 snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/top_level.txt
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/CONTRIBUTING.md` & `snowflake-connector-python-nightly-2023.7.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/DESCRIPTION.md` & `snowflake-connector-python-nightly-2023.7.6/DESCRIPTION.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 
 Source code is also available at: https://github.com/snowflakedb/snowflake-connector-python
 
 # Release Notes
 
 - v3.0.5(TBD)
   - Added the ability to read Snowflake's central configuration file.
+  - Bumped cryptography dependency from <41.0.0,>=3.1.0 to >=3.1.0,<42.0.0.
   - Improved OCSP response caching to remove tmp cache files on Windows.
+  - Added a parameter `server_session_keep_alive` in `SnowflakeConnection` that skips session deletion when client connection closes.
+  - Tightened our pinning of platformdirs, to prevent their new releases breaking us.
+  - Fixed a bug where SFPlatformDirs would incorrectly append application_name/version to its path.
+  - Added retry reason for queries that are retried by the client.
+  - Fixed a bug where `write_pandas` fails when user does not have the privilege to create stage or file format in the target schema, but has the right privilege for the current schema.
 
 - v3.0.4(May 23,2023)
   - Fixed a bug in which `cursor.execute()` could modify the argument statement_params dictionary object when executing a multistatement query.
   - Added the json_result_force_utf8_decoding connection parameter to force decoding JSON content in utf-8 when the result format is JSON.
   - Fixed a bug in which we cannot call `SnowflakeCursor.nextset` before fetching the result of the first query if the cursor runs an async multistatement query.
   - Bumped vendored library urllib3 to 1.26.15
   - Bumped vendored library requests to 2.29.0
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/LICENSE.txt` & `snowflake-connector-python-nightly-2023.7.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/MANIFEST.in` & `snowflake-connector-python-nightly-2023.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/PKG-INFO` & `snowflake-connector-python-nightly-2023.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.6.7
+Version: 2023.7.6
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/README.md` & `snowflake-connector-python-nightly-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/pyproject.toml` & `snowflake-connector-python-nightly-2023.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/setup.cfg` & `snowflake-connector-python-nightly-2023.7.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 [options]
 python_requires = >=3.7
 packages = find_namespace:
 install_requires = 
 	asn1crypto>0.24.0,<2.0.0
 	cffi>=1.9,<2.0.0
-	cryptography>=3.1.0,<41.0.0
+	cryptography>=3.1.0,<42.0.0
 	oscrypto<2.0.0
 	pyOpenSSL>=16.2.0,<24.0.0
 	pycryptodomex!=3.5.0,>=3.2,<4.0.0
 	pyjwt<3.0.0
 	pytz
 	requests<3.0.0
 	importlib-metadata; python_version < '3.8'
@@ -57,15 +57,15 @@
 	charset_normalizer>=2,<4
 	idna>=2.5,<4
 	urllib3>=1.21.1,<1.27
 	certifi>=2017.4.17
 	typing_extensions>=4.3,<5
 	filelock>=3.5,<4
 	sortedcontainers>=2.4.0
-	platformdirs>=2.6.0,<4.0.0
+	platformdirs>=2.6.0,<3.9.0
 	tomlkit
 include_package_data = True
 package_dir = 
 	=src
 zip_safe = False
 
 [options.packages.find]
@@ -81,26 +81,26 @@
 	snowflake-export-certs = snowflake.connector.tool.export_certs:main
 
 [options.extras_require]
 development = 
 	Cython
 	coverage
 	more-itertools
-	numpy<1.25.0
+	numpy<1.26.0
 	pendulum!=2.1.1
 	pexpect
 	pytest<7.4.0
 	pytest-cov
 	pytest-rerunfailures
 	pytest-timeout
 	pytest-xdist
 	pytzdata
 pandas = 
 	pandas>=1.0.0,<2.1.0
 	pyarrow>=10.0.1,<10.1.0
 secure-local-storage = 
-	keyring!=16.1.0,<24.0.0
+	keyring!=16.1.0,<25.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/setup.py` & `snowflake-connector-python-nightly-2023.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,11 +204,11 @@
                 ret.append(source)
 
             return ret
 
     cmd_class = {"build_ext": MyBuildExt}
 
 setup(
-    version="2023.06.07",
+    version="2023.07.06",
     ext_modules=extensions,
     cmdclass=cmd_class,
 )
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/__init__.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/_query_context_cache.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/_query_context_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/_sql_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/_sql_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/arrow_context.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/arrow_context.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/arrow_iterator.pyx` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/arrow_iterator.pyx`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/__init__.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/_auth.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/_auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/by_plugin.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/by_plugin.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/default.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/default.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/idtoken.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/idtoken.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/keypair.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/keypair.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/oauth.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/okta.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/okta.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/usrpwdmfa.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/usrpwdmfa.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/auth/webbrowser.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/auth/webbrowser.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/azure_storage_client.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/bind_upload_agent.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/bind_upload_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cache.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/compat.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/config_manager.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/config_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,10 +335,11 @@
 )
 CONFIG_PARSER.add_option(
     name="connections",
     parse_str=tomlkit.parse,
 )
 
 __all__ = [
+    "ConfigOption",
     "ConfigManager",
     "CONFIG_PARSER",
 ]
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/connection.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,22 @@
         False,
         bool,
     ),  # Disable query context cache
     "json_result_force_utf8_decoding": (
         False,
         bool,
     ),  # Whether to force the JSON content to be decoded in utf-8, it is only effective when result format is JSON
+    "server_session_keep_alive": (
+        False,
+        bool,
+    ),  # Whether to keep session alive after connector shuts down
+    "enable_retry_reason_in_query_response": (
+        True,
+        bool,
+    ),  # Enable sending retryReason in response header for query-requests
 }
 
 APPLICATION_RE = re.compile(r"[\w\d_]+")
 
 # adding the exception class to Connection class
 for m in [method for method in dir(errors) if callable(getattr(errors, method))]:
     setattr(sys.modules[__name__], m, getattr(errors, m))
@@ -276,14 +284,16 @@
         enable_stage_s3_privatelink_for_us_east_1: when true, clients use regional s3 url to upload files.
         enable_connection_diag: when true, clients will generate a connectivity diagnostic report.
         connection_diag_log_path: path to location to create diag report with enable_connection_diag.
         connection_diag_whitelist_path: path to a whitelist.json file to test with enable_connection_diag.
         json_result_force_utf8_decoding: When true, json result will be decoded in utf-8,
           when false, the encoding of the content is auto-detected. Default value is false.
           This parameter is only effective when the result format is JSON.
+        server_session_keep_alive: When true, the connector does not destroy the session on the Snowflake server side
+          before the connector shuts down. Default value is false.
     """
 
     OCSP_ENV_LOCK = Lock()
 
     def __init__(
         self,
         connection_name: str | None = None,
@@ -619,15 +629,18 @@
             # CLIENT_SESSION_KEEP_ALIVE is set, because the heartbeat runs on
             # a separate thread.
             self._cancel_heartbeat()
 
             # close telemetry first, since it needs rest to send remaining data
             logger.info("closed")
             self._telemetry.close(send_on_close=retry)
-            if self._all_async_queries_finished():
+            if (
+                self._all_async_queries_finished()
+                and not self._server_session_keep_alive
+            ):
                 logger.info("No async queries seem to be running, deleting session")
                 self.rest.delete_session(retry=retry)
             else:
                 logger.info(
                     "There are {} async queries still running, not deleting session".format(
                         len(self._async_sfqids)
                     )
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/connection_diagnostic.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/connection_diagnostic.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/constants.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/constants.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter_issue23517.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter_issue23517.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/converter_snowsql.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/converter_snowsql.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BinaryConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/BooleanConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowChunkIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/CArrowTableIterator.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DateConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DateConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/DecimalConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/FloatConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/IntConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Common.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Python/Helpers.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/SnowflakeType.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/StringConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/StringConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/TimeStampConverter.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/time.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/ArrowIterator/Util/time.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/Logging/logging.cpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/Logging/logging.cpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cpp/Logging/logging.hpp` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cpp/Logging/logging.hpp`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/cursor.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/cursor.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/dbapi.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/dbapi.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/description.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/description.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/encryption_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/encryption_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/errorcode.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/errorcode.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/errors.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,14 +532,27 @@
             msg=kwargs.get("msg") or "HTTP 405: Method not allowed",
             errno=kwargs.get("errno"),
             sqlstate=kwargs.get("sqlstate"),
             sfqid=kwargs.get("sfqid"),
         )
 
 
+class TooManyRequests(Error):
+    """Exception for 429 HTTP error for retry."""
+
+    def __init__(self, **kwargs) -> None:
+        Error.__init__(
+            self,
+            msg=kwargs.get("msg") or "HTTP 429: Too Many Requests",
+            errno=kwargs.get("errno"),
+            sqlstate=kwargs.get("sqlstate"),
+            sfqid=kwargs.get("sfqid"),
+        )
+
+
 class OtherHTTPRetryableError(Error):
     """Exception for other HTTP error for retry."""
 
     def __init__(self, **kwargs) -> None:
         code = kwargs.get("code", "n/a")
         Error.__init__(
             self,
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_compression_type.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_compression_type.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_transfer_agent.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_transfer_agent.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/file_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/file_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/gcs_storage_client.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/gcs_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/gzip_decoder.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/gzip_decoder.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/local_storage_client.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/local_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/network.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
     InterfaceError,
     InternalServerError,
     MethodNotAllowed,
     OperationalError,
     OtherHTTPRetryableError,
     ProgrammingError,
     ServiceUnavailableError,
+    TooManyRequests,
 )
 from .sqlstate import (
     SQLSTATE_CONNECTION_NOT_EXISTS,
     SQLSTATE_CONNECTION_REJECTED,
     SQLSTATE_CONNECTION_WAS_NOT_ESTABLISHED,
     SQLSTATE_IO_ERROR,
 )
@@ -169,14 +170,15 @@
     INTERNAL_SERVER_ERROR: InternalServerError,
     FORBIDDEN: ForbiddenError,
     SERVICE_UNAVAILABLE: ServiceUnavailableError,
     GATEWAY_TIMEOUT: GatewayTimeoutError,
     BAD_REQUEST: BadRequest,
     BAD_GATEWAY: BadGatewayError,
     METHOD_NOT_ALLOWED: MethodNotAllowed,
+    TOO_MANY_REQUESTS: TooManyRequests,
 }
 
 DEFAULT_AUTHENTICATOR = "SNOWFLAKE"  # default authenticator name
 EXTERNAL_BROWSER_AUTHENTICATOR = "EXTERNALBROWSER"
 KEY_PAIR_AUTHENTICATOR = "SNOWFLAKE_JWT"
 OAUTH_AUTHENTICATOR = "OAUTH"
 ID_TOKEN_AUTHENTICATOR = "ID_TOKEN"
@@ -780,44 +782,65 @@
         data: dict[str, Any] | None = None,
         timeout: int | None = None,
         **kwargs,
     ) -> dict[Any, Any]:
         """Carry out API request with session management."""
 
         class RetryCtx:
-            def __init__(self, timeout, _include_retry_params: bool = False) -> None:
+            def __init__(
+                self,
+                timeout,
+                _include_retry_params: bool = False,
+                _include_retry_reason: bool = False,
+            ) -> None:
                 self.total_timeout = timeout
                 self.timeout = timeout
                 self.cnt = 0
+                self.reason = 0
                 self.sleeping_time = 1
                 self.start_time = get_time_millis()
                 self._include_retry_params = _include_retry_params
+                self._include_retry_reason = _include_retry_reason
                 # backoff between 1 and 16 seconds
                 self._backoff = DecorrelateJitterBackoff(1, 16)
 
+            def increment_retry(self, reason: int = 0) -> None:
+                """Increment retry count and update the reason for retry
+
+                Args:
+                    reason: HTTP response code that caused retry. Defaults to 0.
+                """
+                self.cnt += 1
+                self.reason = reason
+
             def next_sleep(self) -> int:
                 self.sleeping_time = self._backoff.next_sleep(
                     self.cnt, self.sleeping_time
                 )
                 return self.sleeping_time
 
             def add_retry_params(self, full_url: str) -> str:
                 if self._include_retry_params and self.cnt > 0:
-                    suffix = urlencode(
-                        {"clientStartTime": self.start_time, "retryCount": self.cnt}
-                    )
+                    retry_params = {
+                        "clientStartTime": self.start_time,
+                        "retryCount": self.cnt,
+                    }
+                    if self._include_retry_reason:
+                        retry_params.update({"retryReason": self.reason})
+                    suffix = urlencode(retry_params)
                     sep = "&" if urlparse(full_url).query else "?"
                     return full_url + sep + suffix
                 else:
                     return full_url
 
+        include_retry_reason = self._connection._enable_retry_reason_in_query_response
         include_retry_params = kwargs.pop("_include_retry_params", False)
 
         with self._use_requests_session(full_url) as session:
-            retry_ctx = RetryCtx(timeout, include_retry_params)
+            retry_ctx = RetryCtx(timeout, include_retry_params, include_retry_reason)
             while True:
                 ret = self._request_exec_wrapper(
                     session, method, full_url, headers, data, retry_ctx, **kwargs
                 )
                 if ret is not None:
                     return ret
 
@@ -928,15 +951,16 @@
                 "sleeping=%s(s)",
                 type(cause),
                 cause,
                 retry_ctx.cnt + 1,
                 sleeping_time,
             )
             time.sleep(sleeping_time)
-            retry_ctx.cnt += 1
+            reason = getattr(cause, "errno", 0)
+            retry_ctx.increment_retry(reason)
             if retry_ctx.timeout is not None:
                 retry_ctx.timeout -= sleeping_time
             return None  # retry
         except Exception as e:
             if not no_retry:
                 raise e
             logger.debug("Ignored error", exc_info=True)
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ocsp_asn1crypto.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ocsp_asn1crypto.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ocsp_snowflake.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ocsp_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/options.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/options.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/pandas_tools.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/pandas_tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from typing_extensions import Literal
 
 from snowflake.connector import ProgrammingError
 from snowflake.connector.options import pandas
 from snowflake.connector.telemetry import TelemetryData, TelemetryField
 from snowflake.connector.util_text import random_string
 
+from .cursor import SnowflakeCursor
+
 if TYPE_CHECKING:  # pragma: no cover
     from .connection import SnowflakeConnection
 
     try:
         import sqlalchemy
     except ImportError:
         sqlalchemy = None
@@ -58,14 +60,100 @@
             (database + "." if database else "")
             + (schema + "." if schema else "")
             + name
         )
     return location
 
 
+def _do_create_temp_stage(
+    cursor: SnowflakeCursor,
+    stage_location: str,
+    compression: str,
+    auto_create_table: bool,
+    overwrite: bool,
+) -> None:
+    create_stage_sql = f"CREATE TEMP STAGE /* Python:snowflake.connector.pandas_tools.write_pandas() */ {stage_location} FILE_FORMAT=(TYPE=PARQUET COMPRESSION={compression}{' BINARY_AS_TEXT=FALSE' if auto_create_table or overwrite else ''})"
+    logger.debug(f"creating stage with '{create_stage_sql}'")
+    cursor.execute(create_stage_sql, _is_internal=True).fetchall()
+
+
+def _create_temp_stage(
+    cursor: SnowflakeCursor,
+    database: str | None,
+    schema: str | None,
+    quote_identifiers: bool,
+    compression: str,
+    auto_create_table: bool,
+    overwrite: bool,
+) -> str:
+    stage_name = random_string()
+    stage_location = build_location_helper(
+        database=database,
+        schema=schema,
+        name=stage_name,
+        quote_identifiers=quote_identifiers,
+    )
+    try:
+        _do_create_temp_stage(
+            cursor, stage_location, compression, auto_create_table, overwrite
+        )
+    except ProgrammingError as e:
+        # User may not have the privilege to create stage on the target schema, so fall back to use current schema as
+        # the old behavior.
+        logger.debug(
+            f"creating stage {stage_location} failed. Exception {str(e)}. Fall back to use current schema"
+        )
+        stage_location = stage_name
+        _do_create_temp_stage(
+            cursor, stage_location, compression, auto_create_table, overwrite
+        )
+
+    return stage_location
+
+
+def _do_create_temp_file_format(
+    cursor: SnowflakeCursor, file_format_location: str, compression: str
+) -> None:
+    file_format_sql = (
+        f"CREATE TEMP FILE FORMAT {file_format_location} "
+        f"/* Python:snowflake.connector.pandas_tools.write_pandas() */ "
+        f"TYPE=PARQUET COMPRESSION={compression}"
+    )
+    logger.debug(f"creating file format with '{file_format_sql}'")
+    cursor.execute(file_format_sql, _is_internal=True)
+
+
+def _create_temp_file_format(
+    cursor: SnowflakeCursor,
+    database: str | None,
+    schema: str | None,
+    quote_identifiers: bool,
+    compression: str,
+) -> str:
+    file_format_name = random_string()
+    file_format_location = build_location_helper(
+        database=database,
+        schema=schema,
+        name=file_format_name,
+        quote_identifiers=quote_identifiers,
+    )
+    try:
+        _do_create_temp_file_format(cursor, file_format_location, compression)
+    except ProgrammingError as e:
+        # User may not have the privilege to create file format on the target schema, so fall back to use current schema
+        # as the old behavior.
+        logger.debug(
+            f"creating stage {file_format_location} failed. Exception {str(e)}. Fall back to use current schema"
+        )
+        file_format_location = file_format_name
+        _do_create_temp_file_format(cursor, file_format_location, compression)
+
+    return file_format_location
+
+
 def write_pandas(
     conn: SnowflakeConnection,
     df: pandas.DataFrame,
     table_name: str,
     database: str | None = None,
     schema: str | None = None,
     chunk_size: int | None = None,
@@ -182,23 +270,23 @@
             f" Consider changing the index to pd.RangeIndex(start=0,...,step=1) or "
             f"call reset_index() to keep index as column(s)",
             UserWarning,
             stacklevel=2,
         )
 
     cursor = conn.cursor()
-    stage_location = build_location_helper(
-        database=database,
-        schema=schema,
-        name=random_string(),
-        quote_identifiers=quote_identifiers,
+    stage_location = _create_temp_stage(
+        cursor,
+        database,
+        schema,
+        quote_identifiers,
+        compression,
+        auto_create_table,
+        overwrite,
     )
-    create_stage_sql = f"CREATE TEMP STAGE /* Python:snowflake.connector.pandas_tools.write_pandas() */ {stage_location}"
-    logger.debug(f"creating stage with '{create_stage_sql}'")
-    cursor.execute(create_stage_sql, _is_internal=True).fetchall()
 
     with TemporaryDirectory() as tmp_folder:
         for i, chunk in chunk_helper(df, chunk_size):
             chunk_path = os.path.join(tmp_folder, f"file{i}.txt")
             # Dump chunk into parquet file
             chunk.to_parquet(chunk_path, compression=compression, **kwargs)
             # Upload parquet file
@@ -229,28 +317,17 @@
 
     def drop_object(name: str, object_type: str) -> None:
         drop_sql = f"DROP {object_type.upper()} IF EXISTS {name} /* Python:snowflake.connector.pandas_tools.write_pandas() */"
         logger.debug(f"dropping {object_type} with '{drop_sql}'")
         cursor.execute(drop_sql, _is_internal=True)
 
     if auto_create_table or overwrite:
-        file_format_location = build_location_helper(
-            database=database,
-            schema=schema,
-            name=random_string(),
-            quote_identifiers=quote_identifiers,
-        )
-        file_format_sql = (
-            f"CREATE TEMP FILE FORMAT {file_format_location} "
-            f"/* Python:snowflake.connector.pandas_tools.write_pandas() */ "
-            f"TYPE=PARQUET COMPRESSION={compression_map[compression]}"
+        file_format_location = _create_temp_file_format(
+            cursor, database, schema, quote_identifiers, compression_map[compression]
         )
-        logger.debug(f"creating file format with '{file_format_sql}'")
-        cursor.execute(file_format_sql, _is_internal=True)
-
         infer_schema_sql = f"SELECT COLUMN_NAME, TYPE FROM table(infer_schema(location=>'@{stage_location}', file_format=>'{file_format_location}'))"
         logger.debug(f"inferring schema with '{infer_schema_sql}'")
         column_type_mapping = dict(
             cursor.execute(infer_schema_sql, _is_internal=True).fetchall()
         )
         # Infer schema can return the columns out of order depending on the chunking we do when uploading
         # so we have to iterate through the dataframe columns to make sure we create the table with its
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/proxy.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/result_batch.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/result_batch.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/result_set.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/result_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/s3_storage_client.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/s3_storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/secret_detector.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/secret_detector.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sf_dirs.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sf_dirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     defaults.
 
     This helper function was introduced to make this code testable.
     """
     platformdir_kwargs = {
         "appname": "snowflake",
         "appauthor": False,
-        "ensure_exists": True,
     }
     snowflake_home = os.path.expanduser(
         os.environ.get("SNOWFLAKE_HOME", "~/.snowflake/"),
     )
     if os.path.exists(snowflake_home):
         return SFPlatformDirs(
             snowflake_home,
@@ -70,15 +69,15 @@
             ensure_exists=ensure_exists,
         )
         self.single_dir = single_dir
 
     @property
     def user_data_dir(self) -> str:
         """data directory tied to to the user"""
-        return self._append_app_name_and_version(self.single_dir)
+        return self.single_dir
 
     @property
     def site_data_dir(self) -> str:
         """data directory shared by users"""
         return self.user_data_dir
 
     @property
@@ -131,7 +130,12 @@
         """pictures directory tied to the user"""
         return self.user_data_dir
 
     @property
     def user_videos_dir(self) -> str:
         """videos directory tied to the user"""
         return self.user_data_dir
+
+    @property
+    def user_downloads_dir(self) -> str:
+        """downloads directory tied to the user"""
+        return self.user_data_dir
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sfbinaryformat.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sfbinaryformat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/sfdatetime.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/sfdatetime.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/snow_logging.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/snow_logging.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ssd_internal_keys.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ssd_internal_keys.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/ssl_wrap_socket.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/ssl_wrap_socket.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/storage_client.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/storage_client.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/telemetry.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/telemetry_oob.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/telemetry_oob.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/test_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/test_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/time_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/time_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_certs.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_certs.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_ocsp_response.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/dump_ocsp_response_cache.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/dump_ocsp_response_cache.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/tool/probe_connection.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/tool/probe_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/url_util.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/url_util.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/util_text.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/util_text.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/LICENSE` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/__init__.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/_internal_utils.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/adapters.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/api.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/auth.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/compat.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/cookies.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/exceptions.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/help.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/hooks.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/models.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/sessions.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/status_codes.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/structures.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/requests/utils.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/LICENSE.txt` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/__init__.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/_collections.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/connection.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/connectionpool.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/appengine.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/contrib/socks.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/exceptions.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/fields.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/filepost.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/packages/six.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/poolmanager.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/request.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/response.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/__init__.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/connection.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/proxy.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/request.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/response.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/retry.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssl_.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/ssltransport.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/timeout.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/url.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake/connector/vendored/urllib3/util/wait.py` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake/connector/vendored/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/PKG-INFO` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-connector-python-nightly
-Version: 2023.6.7
+Version: 2023.7.6
 Summary: Nigthly build of Snowflake Connector for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache-2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/user-guide/python-connector.html
 Project-URL: Source, https://github.com/keller00/snowflake-connector-python-nightlies/
```

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snowflake-connector-python-nightly-2023.6.7/src/snowflake_connector_python_nightly.egg-info/requires.txt` & `snowflake-connector-python-nightly-2023.7.6/src/snowflake_connector_python_nightly.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 asn1crypto<2.0.0,>0.24.0
 cffi<2.0.0,>=1.9
-cryptography<41.0.0,>=3.1.0
+cryptography<42.0.0,>=3.1.0
 oscrypto<2.0.0
 pyOpenSSL<24.0.0,>=16.2.0
 pycryptodomex!=3.5.0,<4.0.0,>=3.2
 pyjwt<3.0.0
 pytz
 requests<3.0.0
 packaging
 charset_normalizer<4,>=2
 idna<4,>=2.5
 urllib3<1.27,>=1.21.1
 certifi>=2017.4.17
 typing_extensions<5,>=4.3
 filelock<4,>=3.5
 sortedcontainers>=2.4.0
-platformdirs<4.0.0,>=2.6.0
+platformdirs<3.9.0,>=2.6.0
 tomlkit
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [development]
 Cython
 coverage
 more-itertools
-numpy<1.25.0
+numpy<1.26.0
 pendulum!=2.1.1
 pexpect
 pytest<7.4.0
 pytest-cov
 pytest-rerunfailures
 pytest-timeout
 pytest-xdist
 pytzdata
 
 [pandas]
 pandas<2.1.0,>=1.0.0
 pyarrow<10.1.0,>=10.0.1
 
 [secure-local-storage]
-keyring!=16.1.0,<24.0.0
+keyring!=16.1.0,<25.0.0
```

