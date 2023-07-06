# Comparing `tmp/clubbi_utils-5.0.2.tar.gz` & `tmp/clubbi_utils-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clubbi_utils-5.0.2.tar", last modified: Fri Jun 30 13:11:02 2023, max compression
+gzip compressed data, was "clubbi_utils-5.0.3.tar", last modified: Thu Jul  6 12:33:11 2023, max compression
```

## Comparing `clubbi_utils-5.0.2.tar` & `clubbi_utils-5.0.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.835073 clubbi_utils-5.0.2/clubbi_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/async_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/aws_http_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/aws_sqs_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/get_ssm_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/aws/lambda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/lambda/http_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/lambda_invoker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/aws/local_mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/local_mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/local_mocks/s3_object_storage_local_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/s3_object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/ses_mailer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/aws/sns_publisher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/cmds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/cmds/deploy_lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.843073 clubbi_utils-5.0.2/clubbi_utils/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/async_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/async_messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/batched_gather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.843073 clubbi_utils-5.0.2/clubbi_utils/common/csv_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/csv_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/csv_utils/base_model_collection_to_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/iter_as_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/timeit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.843073 clubbi_utils-5.0.2/clubbi_utils/common/typing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/typing/lambda_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/common/undefined.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/json_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/mailer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.843073 clubbi_utils-5.0.2/clubbi_utils/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/mysql/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/mysql/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/mysql/print_literal_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.843073 clubbi_utils-5.0.2/clubbi_utils/operators/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/operators/none_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/operators/none_coalesce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/clubbi_utils/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/postgres/advisory_locker.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/postgres/postgres_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/slack_messenger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.839073 clubbi_utils-5.0.2/clubbi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 13:11:02.000000 clubbi_utils-5.0.2/clubbi_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 13:11:02.847073 clubbi_utils-5.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/tests/test_json_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-30 13:10:41.000000 clubbi_utils-5.0.2/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/async_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/aws_http_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/aws_sqs_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/get_ssm_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/aws/lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/lambda/http_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/lambda_invoker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/aws/local_mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/local_mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/local_mocks/s3_object_storage_local_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/s3_object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/ses_mailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/aws/sns_publisher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/cmds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/cmds/deploy_lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/async_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/async_messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/batched_gather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/common/csv_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/csv_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/csv_utils/base_model_collection_to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/iter_as_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/timeit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/common/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/typing/lambda_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/common/undefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/json_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/mailer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/mysql/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/mysql/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/mysql/print_literal_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/operators/none_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/operators/none_coalesce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/postgres/advisory_locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/postgres/postgres_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/slack_messenger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.807551 clubbi_utils-5.0.3/clubbi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 12:33:11.000000 clubbi_utils-5.0.3/clubbi_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 12:33:11.815552 clubbi_utils-5.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:33:11.811551 clubbi_utils-5.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/tests/test_json_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-06 12:32:54.000000 clubbi_utils-5.0.3/tests/test_operators.py
```

### Comparing `clubbi_utils-5.0.2/LICENSE` & `clubbi_utils-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/README.md` & `clubbi_utils-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/aws_http_event.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/aws_http_event.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/decorator.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from functools import lru_cache, wraps
 from os import getenv
 from typing import Optional, Any, Callable
 
-import aiobotocore
-from aiobotocore import AioSession
+from aiobotocore.client import AioBaseClient
+from aiobotocore.config import AioConfig
+from aiobotocore.session import AioSession
 from aiobotocore.session import get_session
+from pydantic import BaseSettings
 
 from clubbi_utils.aws.local_mocks.s3_object_storage_local_mock import S3ObjectStorageLocalMock
 from clubbi_utils.aws.s3_object_storage import S3ObjectStorage
-from aiobotocore.client import AioBaseClient
-from aiobotocore.config import AioConfig
-from pydantic import BaseSettings
-from clubbi_utils.operators import none_coalesce
 
 
 @lru_cache
 def _get_session() -> AioSession:
     return get_session()
```

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/get_ssm_secret.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/get_ssm_secret.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/lambda_invoker.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/lambda_invoker.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/local_mocks/s3_object_storage_local_mock.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/local_mocks/s3_object_storage_local_mock.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/s3_object_storage.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/s3_object_storage.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/ses_mailer.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/ses_mailer.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/aws/sns_publisher.py` & `clubbi_utils-5.0.3/clubbi_utils/aws/sns_publisher.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/cmds/deploy_lambda_layer.py` & `clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/cmds/deploy_lambda_layer.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/cli/clubbi_sls_util/utils.py` & `clubbi_utils-5.0.3/clubbi_utils/cli/clubbi_sls_util/utils.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/common/async_lambda.py` & `clubbi_utils-5.0.3/clubbi_utils/common/async_lambda.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/common/batched_gather.py` & `clubbi_utils-5.0.3/clubbi_utils/common/batched_gather.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/common/csv_utils/base_model_collection_to_csv.py` & `clubbi_utils-5.0.3/clubbi_utils/common/csv_utils/base_model_collection_to_csv.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/common/timeit.py` & `clubbi_utils-5.0.3/clubbi_utils/common/timeit.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/common/typing/lambda_context.py` & `clubbi_utils-5.0.3/clubbi_utils/common/typing/lambda_context.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/json.py` & `clubbi_utils-5.0.3/clubbi_utils/json.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/json_logging.py` & `clubbi_utils-5.0.3/clubbi_utils/json_logging.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/logging.py` & `clubbi_utils-5.0.3/clubbi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/mysql/mysql_connector.py` & `clubbi_utils-5.0.3/clubbi_utils/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/postgres/advisory_locker.py` & `clubbi_utils-5.0.3/clubbi_utils/postgres/advisory_locker.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/postgres/postgres_connector.py` & `clubbi_utils-5.0.3/clubbi_utils/postgres/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/slack_messenger.py` & `clubbi_utils-5.0.3/clubbi_utils/slack_messenger.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/connector.py` & `clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/connector.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils/sqlalchemy/decorator.py` & `clubbi_utils-5.0.3/clubbi_utils/sqlalchemy/decorator.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/clubbi_utils.egg-info/SOURCES.txt` & `clubbi_utils-5.0.3/clubbi_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/setup.cfg` & `clubbi_utils-5.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clubbi_utils
-version = 5.0.2
+version = 5.0.3
 long_description = Several helper functions, decorators and layers
 long_description_content_type = text/plain
 
 [options]
 packages = find:
 install_requires = 
 	sqlalchemy>=1.4,<1.5
```

### Comparing `clubbi_utils-5.0.2/tests/test_json_logging.py` & `clubbi_utils-5.0.3/tests/test_json_logging.py`

 * *Files identical despite different names*

### Comparing `clubbi_utils-5.0.2/tests/test_operators.py` & `clubbi_utils-5.0.3/tests/test_operators.py`

 * *Files identical despite different names*

