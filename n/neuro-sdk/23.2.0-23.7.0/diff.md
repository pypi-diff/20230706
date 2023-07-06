# Comparing `tmp/neuro-sdk-23.2.0.tar.gz` & `tmp/neuro-sdk-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-sdk-23.2.0.tar", last modified: Mon Feb 20 23:18:30 2023, max compression
+gzip compressed data, was "neuro-sdk-23.7.0.tar", last modified: Thu Jul  6 19:40:47 2023, max compression
```

## Comparing `neuro-sdk-23.2.0.tar` & `neuro-sdk-23.7.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.374735 neuro-sdk-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89475 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-20 23:18:30.374735 neuro-sdk-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.338735 neuro-sdk-23.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.338735 neuro-sdk-23.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/_static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.338735 neuro-sdk-23.2.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/_templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    24522 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/buckets_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/client_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/config_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/disks_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/functions_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/images_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35696 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/jobs_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/jobs_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/parse_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/plugin_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/secrets_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/service_accounts_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/storage_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/storage_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/docs/users_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-20 23:18:30.374735 neuro-sdk-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.322735 neuro-sdk-23.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.354735 neuro-sdk-23.2.0/src/neuro_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_azure_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_bucket_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28161 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_gcs_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    40630 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_parsing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_rewrite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_s3_bucket_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_server_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    37076 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6620 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_url_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/_version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/src/neuro_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.358735 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-20 23:18:30.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-02-20 23:18:30.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 23:18:30.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 23:17:52.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-20 23:18:30.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 23:18:30.000000 neuro-sdk-23.2.0/src/neuro_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.370736 neuro-sdk-23.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.374735 neuro-sdk-23.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/data/emptyfile.txt
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/data/file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.322735 neuro-sdk-23.2.0/tests/data/nested/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:30.374735 neuro-sdk-23.2.0/tests/data/nested/folder/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/data/nested/folder/file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_bucket_persistent_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19369 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    62588 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)   102853 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_login_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_public_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    78788 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_storage_filestatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_url_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-02-20 23:17:48.000000 neuro-sdk-23.2.0/tests/test_version_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.062079 neuro-sdk-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    92203 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-06 19:40:47.062079 neuro-sdk-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.034079 neuro-sdk-23.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.034079 neuro-sdk-23.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/_static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.034079 neuro-sdk-23.7.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/_templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    24522 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/buckets_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/client_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/config_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/disks_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/functions_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/images_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35696 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/jobs_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/jobs_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/parse_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/plugin_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/secrets_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/service_accounts_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/storage_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/storage_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/docs/users_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-06 19:40:47.066079 neuro-sdk-23.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.022079 neuro-sdk-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.046079 neuro-sdk-23.7.0/src/neuro_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_azure_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_bucket_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30600 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34493 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_gcs_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41551 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_parsing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_s3_bucket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_server_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37214 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_url_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/_version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/src/neuro_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.050079 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-06 19:40:47.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-06 19:40:47.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:40:47.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:39:53.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 19:40:47.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 19:40:47.000000 neuro-sdk-23.7.0/src/neuro_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.062079 neuro-sdk-23.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.062079 neuro-sdk-23.7.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/data/emptyfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/data/file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.026079 neuro-sdk-23.7.0/tests/data/nested/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:47.062079 neuro-sdk-23.7.0/tests/data/nested/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/data/nested/folder/file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_bucket_persistent_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41447 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16161 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63974 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110227 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_login_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_public_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80423 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_storage_filestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_url_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-07-06 19:39:48.000000 neuro-sdk-23.7.0/tests/test_version_check.py
```

### Comparing `neuro-sdk-23.2.0/CHANGELOG.md` & `neuro-sdk-23.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,46 @@
 [comment]: # (Please do not modify this file)
 [comment]: # (Put you comments to changelog.d and it will be moved to changelog in next release)
 
 [comment]: # (Clear the text on make release for canceling the release)
 
 [comment]: # (towncrier release notes start)
 
+Neuro SDK/CLI 23.7.0 (2023-07-03)
+=================================
+
+Features
+--------
+
+- Commands `neuro run`, `neuro logs`, `neuro attach` and `neuro exec` in non-quiet mode now prints details for cancelled and failed jobs. Also improved other indications of the job status. ([#2800](https://github.com/neuro-inc/platform-client-python/issues/2800))
+- Commands `neuro run` and `neuro attach` now re-attach to restarted jobs. Previously they waited until the job finished. ([#2802](https://github.com/neuro-inc/platform-client-python/issues/2802))
+- Added support of cluster energy schedules.
+  `neuro config show --energy` will display awailable energy schedule periods.
+  `neuro run --schedule-name <energy-schedule-name>` will run the job within the specified <energy-schedule-name>. Note - the selected preset should have an enabled scheduler.
+  `neuro status <job-id>` will include the energy schedule name if one was used for running the job. ([#2903](https://github.com/neuro-inc/platform-client-python/issues/2903))
+- Added Python 3.11 support. ([#2908](https://github.com/neuro-inc/platform-client-python/issues/2908))
+- Add `neuro config switch-project` command. ([#2940](https://github.com/neuro-inc/platform-client-python/issues/2940))
+- Support projects in storage commands, make project directory default instead of user home directory. ([#2949](https://github.com/neuro-inc/platform-client-python/issues/2949))
+- Support projects in image commands. ([#2950](https://github.com/neuro-inc/platform-client-python/issues/2950))
+- Support projects in `neuro secret` cli. ([#2952](https://github.com/neuro-inc/platform-client-python/issues/2952))
+- Support projects in `neuro blob` cli commands and `neuro-sdk`. ([#2954](https://github.com/neuro-inc/platform-client-python/issues/2954))
+- Add project support in `neuro job` commands. ([#2955](https://github.com/neuro-inc/platform-client-python/issues/2955))
+- Support projects in disk CLI commands and SDK methods. ([#2960](https://github.com/neuro-inc/platform-client-python/issues/2960))
+- Support projects in service account CLI commands and SDK methods. ([#2965](https://github.com/neuro-inc/platform-client-python/issues/2965))
+- Unhide remove-project command. ([#2976](https://github.com/neuro-inc/platform-client-python/issues/2976))
+- Align all `ls` command options. ([#2995](https://github.com/neuro-inc/platform-client-python/issues/2995))
+
+
+Bugfixes
+--------
+
+- Fix human-readable datetime formatter to correctly report jobs lifespan ending in future ([#2933](https://github.com/neuro-inc/platform-client-python/issues/2933))
+- Update projects after fetching config from server. ([#2992](https://github.com/neuro-inc/platform-client-python/issues/2992))
+
+
 Neuro SDK/CLI 22.7.1 (2022-07-27)
 =================================
 
 Features
 --------
 
 - Add update-node-pool command. Only idle_size update is available. ([#2740](https://github.com/neuro-inc/platform-client-python/issues/2740))
```

### Comparing `neuro-sdk-23.2.0/LICENSE` & `neuro-sdk-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/PKG-INFO` & `neuro-sdk-23.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-sdk
-Version: 23.2.0
+Version: 23.7.0
 Summary: Neu.ro SDK
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `neuro-sdk-23.2.0/README.md` & `neuro-sdk-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/Makefile` & `neuro-sdk-23.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/buckets_reference.rst` & `neuro-sdk-23.7.0/docs/buckets_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/client_reference.rst` & `neuro-sdk-23.7.0/docs/client_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/conf.py` & `neuro-sdk-23.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/config_reference.rst` & `neuro-sdk-23.7.0/docs/config_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/disks_reference.rst` & `neuro-sdk-23.7.0/docs/disks_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/functions_reference.rst` & `neuro-sdk-23.7.0/docs/functions_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/images_reference.rst` & `neuro-sdk-23.7.0/docs/images_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/index.rst` & `neuro-sdk-23.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/jobs_reference.rst` & `neuro-sdk-23.7.0/docs/jobs_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/jobs_usage.rst` & `neuro-sdk-23.7.0/docs/jobs_usage.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/make.bat` & `neuro-sdk-23.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/parse_reference.rst` & `neuro-sdk-23.7.0/docs/parse_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/plugin_reference.rst` & `neuro-sdk-23.7.0/docs/plugin_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/secrets_reference.rst` & `neuro-sdk-23.7.0/docs/secrets_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/service_accounts_reference.rst` & `neuro-sdk-23.7.0/docs/service_accounts_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/storage_reference.rst` & `neuro-sdk-23.7.0/docs/storage_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/storage_usage.rst` & `neuro-sdk-23.7.0/docs/storage_usage.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/docs/users_reference.rst` & `neuro-sdk-23.7.0/docs/users_reference.rst`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/setup.cfg` & `neuro-sdk-23.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuro-sdk
-version = 23.2.0
+version = 23.7.0
 description = Neu.ro SDK
 url = https://github.com/neuro-inc/platform-client-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Neu.ro Team
 author_email = team@neu.ro
 license = Apache 2
@@ -30,29 +30,29 @@
 	=src
 packages = find:
 zip_safe = False
 python_requires = >=3.8.0
 include_package_data = True
 install_requires = 
 	aiohttp>=3.8.1
-	yarl>=1.7.0
+	yarl>=1.7.0,<1.9.0
 	pyyaml>=5.0
 	python-jose>=3.3.0
 	python-dateutil>=2.7.0
 	aiobotocore>=2.3.0,<3.0
 	aiodocker>=0.21.0
 	typing_extensions>=3.7.4
 	certifi
 	toml>=0.10.0
 	azure-storage-blob>=12.8.1,!=12.9.0
 	google-auth>=2.0.2
 	importlib_metadata>=4.11.4; python_version<"3.11"
 	packaging>=20.4
-	neuro-admin-client>=22.7.2
-	neuro-config-client>=23.2.3
+	neuro-admin-client>=23.5.0
+	neuro-config-client>=23.3.0
 
 [options.packages.find]
 where = src
 
 [flake8]
 exclude = .git,.env,__pycache__,.eggs
 max-line-length = 88
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/__init__.py` & `neuro-sdk-23.7.0/src/neuro_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,23 +134,28 @@
     SecretFile,
     Volume,
     VolumeParseResult,
 )
 from ._parsing_utils import LocalImage, RemoteImage, Tag, TagOption
 from ._plugins import ConfigBuilder, ConfigScope, PluginManager, VersionChecker
 from ._secrets import Secret, Secrets
-from ._server_cfg import Cluster
+from ._server_cfg import Cluster, Project
 from ._service_accounts import ServiceAccount, ServiceAccounts
 from ._storage import DiskUsageInfo, FileStatus, FileStatusType, Storage
 from ._tracing import gen_trace_id
 from ._url_utils import CLUSTER_SCHEMES as SCHEMES
 from ._users import Action, Permission, Quota, Share, Users
-from ._utils import _ContextManager, find_project_root
+from ._utils import (
+    ORG_NAME_SENTINEL,
+    OrgNameSentinel,
+    _ContextManager,
+    find_project_root,
+)
 
-__version__ = "23.2.0"
+__version__ = "23.7.0"
 
 
 __all__ = (
     "AbstractDeleteProgress",
     "AbstractDockerImageProgress",
     "AbstractFileProgress",
     "AbstractRecursiveFileProgress",
@@ -202,20 +207,23 @@
     "JobStatusHistory",
     "JobStatusItem",
     "JobTelemetry",
     "Jobs",
     "LocalImage",
     "NDJSONError",
     "NotSupportedError",
+    "ORG_NAME_SENTINEL",
+    "OrgNameSentinel",
     "PASS_CONFIG_ENV_NAME",
     "Parser",
     "Permission",
     "PersistentBucketCredentials",
     "PluginManager",
     "Preset",
+    "Project",
     "Quota",
     "RemoteImage",
     "ResourceNotFound",
     "Resources",
     "SCHEMES",
     "Secret",
     "SecretFile",
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_abc.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_abc.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_admin.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_azure_bucket_provider.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_azure_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_bucket_base.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_bucket_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,26 +132,27 @@
 @rewrite_module
 @dataclass(frozen=True)
 class Bucket:
     id: str
     owner: str
     cluster_name: str
     org_name: Optional[str]
+    project_name: str
     provider: "Bucket.Provider"
     created_at: datetime
     imported: bool
     public: bool = False
     name: Optional[str] = None
 
     @property
     def uri(self) -> URL:
         base = f"blob://{self.cluster_name}"
         if self.org_name:
             base += f"/{self.org_name}"
-        return URL(f"{base}/{self.owner}/{self.name or self.id}")
+        return URL(f"{base}/{self.project_name}/{self.name or self.id}")
 
     def get_key_for_uri(self, uri: URL) -> str:
         self_uris = [self.uri]
         if self.name:
             self_uris.append(self.uri.parent / self.id)
         uri_str = str(uri)
         for self_uri in self_uris:
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_buckets.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_buckets.py`

 * *Files 9% similar despite different names*

```diff
@@ -192,14 +192,15 @@
             name=payload.get("name"),
             created_at=isoparse(payload["created_at"]),
             provider=Bucket.Provider(payload["provider"]),
             imported=payload.get("imported", False),
             public=payload.get("public", False),
             cluster_name=self._config.cluster_name,
             org_name=payload.get("org_name"),
+            project_name=payload["project_name"],
         )
 
     def _parse_bucket_credentials_payload(
         self, payload: Mapping[str, Any]
     ) -> BucketCredentials:
         return BucketCredentials(
             bucket_id=payload["bucket_id"],
@@ -208,20 +209,48 @@
         )
 
     def _get_buckets_url(self, cluster_name: Optional[str]) -> URL:
         if cluster_name is None:
             cluster_name = self._config.cluster_name
         return self._config.get_cluster(cluster_name).buckets_url / "buckets"
 
+    def _get_bucket_url_params(
+        self,
+        org_name: Union[Optional[str], OrgNameSentinel],
+        project_name: Optional[str],
+    ) -> Dict[str, Any]:
+        org_name_val = (
+            org_name
+            if not isinstance(org_name, OrgNameSentinel)
+            else self._config.org_name
+        )
+        params = {
+            "org_name": org_name_val or "NO_ORG",
+            "project_name": project_name or self._config.project_name_or_raise,
+        }
+        return params
+
     @asyncgeneratorcontextmanager
-    async def list(self, cluster_name: Optional[str] = None) -> AsyncIterator[Bucket]:
+    async def list(
+        self,
+        cluster_name: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
+    ) -> AsyncIterator[Bucket]:
         url = self._get_buckets_url(cluster_name)
         auth = await self._config._api_auth()
         headers = {"Accept": "application/x-ndjson"}
-        async with self._core.request("GET", url, headers=headers, auth=auth) as resp:
+        params = {}
+        if not isinstance(org_name, OrgNameSentinel):
+            params["org_name"] = org_name or "NO_ORG"
+        if project_name:
+            params["project_name"] = project_name
+        async with self._core.request(
+            "GET", url, headers=headers, auth=auth, params=params
+        ) as resp:
             if resp.headers.get("Content-Type", "").startswith("application/x-ndjson"):
                 async for line in resp.content:
                     server_message = json.loads(line)
                     if "error" in server_message:
                         raise NDJSONError(server_message["error"])
                     yield self._parse_bucket_payload(server_message)
             else:
@@ -230,123 +259,135 @@
                     yield self._parse_bucket_payload(bucket_data)
 
     async def create(
         self,
         name: Optional[str] = None,
         cluster_name: Optional[str] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> Bucket:
         url = self._get_buckets_url(cluster_name)
         auth = await self._config._api_auth()
         data = {
             "name": name,
             "org_name": org_name
             if not isinstance(org_name, OrgNameSentinel)
             else self._config.org_name,
+            "project_name": project_name or self._config.project_name_or_raise,
         }
         async with self._core.request("POST", url, auth=auth, json=data) as resp:
             payload = await resp.json()
             return self._parse_bucket_payload(payload)
 
     async def import_external(
         self,
         provider: Bucket.Provider,
         provider_bucket_name: str,
         credentials: Mapping[str, str],
         name: Optional[str] = None,
         cluster_name: Optional[str] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> Bucket:
         url = self._get_buckets_url(cluster_name) / "import" / "external"
         auth = await self._config._api_auth()
         data = {
             "name": name,
             "provider": provider.value,
             "provider_bucket_name": provider_bucket_name,
             "credentials": credentials,
             "org_name": org_name
             if not isinstance(org_name, OrgNameSentinel)
             else self._config.org_name,
+            "project_name": project_name or self._config.project_name_or_raise,
         }
         async with self._core.request("POST", url, auth=auth, json=data) as resp:
             payload = await resp.json()
             return self._parse_bucket_payload(payload)
 
     async def get(
         self,
         bucket_id_or_name: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> Bucket:
         url = self._get_buckets_url(cluster_name) / bucket_id_or_name
-        query = {"owner": bucket_owner} if bucket_owner else {}
+        params = self._get_bucket_url_params(org_name, project_name)
         auth = await self._config._api_auth()
-        async with self._core.request("GET", url, auth=auth, params=query) as resp:
+        async with self._core.request("GET", url, auth=auth, params=params) as resp:
             payload = await resp.json()
             return self._parse_bucket_payload(payload)
 
     async def rm(
         self,
         bucket_id_or_name: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         url = self._get_buckets_url(cluster_name) / bucket_id_or_name
-        query = {"owner": bucket_owner} if bucket_owner else {}
+        params = self._get_bucket_url_params(org_name, project_name)
         auth = await self._config._api_auth()
-        async with self._core.request("DELETE", url, auth=auth, params=query):
+        async with self._core.request("DELETE", url, auth=auth, params=params):
             pass
 
     async def set_public_access(
         self,
         bucket_id_or_name: str,
         public_access: bool,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> Bucket:
         url = self._get_buckets_url(cluster_name) / bucket_id_or_name
+        params = self._get_bucket_url_params(org_name, project_name)
         auth = await self._config._api_auth()
         data = {
             "public": public_access,
         }
-        query = {"owner": bucket_owner} if bucket_owner else {}
         async with self._core.request(
-            "PATCH", url, auth=auth, json=data, params=query
+            "PATCH", url, auth=auth, json=data, params=params
         ) as resp:
             payload = await resp.json()
             return self._parse_bucket_payload(payload)
 
     async def request_tmp_credentials(
         self,
         bucket_id_or_name: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> BucketCredentials:
         url = (
             self._get_buckets_url(cluster_name)
             / bucket_id_or_name
             / "make_tmp_credentials"
         )
+        params = self._get_bucket_url_params(org_name, project_name)
         auth = await self._config._api_auth()
-        query = {"owner": bucket_owner} if bucket_owner else {}
-        async with self._core.request("POST", url, auth=auth, params=query) as resp:
+        async with self._core.request("POST", url, auth=auth, params=params) as resp:
             payload = await resp.json()
             return self._parse_bucket_credentials_payload(payload)
 
     @asyncgeneratorcontextmanager
     async def get_disk_usage(
         self,
         bucket_id_or_name: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> AsyncIterator[BucketUsage]:
         total_bytes = 0
         obj_count = 0
         async with self._get_provider_by_exact(
-            bucket_id_or_name, cluster_name, bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         ) as provider:
             async with provider.list_blobs("", recursive=True) as it:
                 async for obj in it:
                     total_bytes += obj.size
                     obj_count += 1
                     yield BucketUsage(total_bytes, obj_count)
 
@@ -369,18 +410,22 @@
             yield provider
 
     @asynccontextmanager
     async def _get_provider_by_exact(
         self,
         bucket_id_or_name: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> AsyncIterator[BucketProvider]:
         bucket = await self.get(
-            bucket_id_or_name, cluster_name=cluster_name, bucket_owner=bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         )
         async with self._get_provider_for_bucket(bucket) as provider:
             yield provider
 
     @asynccontextmanager
     async def _get_provider_for_bucket(
         self, bucket: Bucket
@@ -420,59 +465,75 @@
     # Low level operations
 
     async def head_blob(
         self,
         bucket_id_or_name: str,
         key: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> BucketEntry:
         async with self._get_provider_by_exact(
-            bucket_id_or_name, cluster_name, bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         ) as provider:
             return await provider.head_blob(key)
 
     async def put_blob(
         self,
         bucket_id_or_name: str,
         key: str,
         body: Union[AsyncIterator[bytes], bytes],
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         async with self._get_provider_by_exact(
-            bucket_id_or_name, cluster_name, bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         ) as provider:
             await provider.put_blob(key, body)
 
     @asyncgeneratorcontextmanager
     async def fetch_blob(
         self,
         bucket_id_or_name: str,
         key: str,
         offset: int = 0,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> AsyncIterator[bytes]:
         async with self._get_provider_by_exact(
-            bucket_id_or_name, cluster_name, bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         ) as provider:
             async with provider.fetch_blob(key, offset=offset) as it:
                 async for chunk in it:
                     yield chunk
 
     async def delete_blob(
         self,
         bucket_id_or_name: str,
         key: str,
         cluster_name: Optional[str] = None,
-        bucket_owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         async with self._get_provider_by_exact(
-            bucket_id_or_name, cluster_name, bucket_owner
+            bucket_id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
         ) as provider:
             return await provider.delete_blob(key)
 
     # Listing operations
 
     @asyncgeneratorcontextmanager
     async def list_blobs(
@@ -581,15 +642,14 @@
         update: bool = False,
         continue_: bool = False,
         progress: Optional[AbstractFileProgress] = None,
     ) -> None:
         src = self._parser.normalize_uri(src, allowed_schemes=("blob",))
         dst = normalize_local_path_uri(dst)
         async with self._get_bucket_fs(src) as bucket_fs:
-
             src_key = bucket_fs.bucket.get_key_for_uri(src)
             transferer = FileTransferer(bucket_fs, LocalFS())
             await transferer.transfer_file(
                 src=PurePosixPath(src_key),
                 dst=_extract_path(dst),
                 update=update,
                 continue_=continue_,
@@ -605,15 +665,14 @@
         filter: Optional[AsyncFilterFunc] = None,
         ignore_file_names: AbstractSet[str] = frozenset(),
         progress: Optional[AbstractRecursiveFileProgress] = None,
     ) -> None:
         src = normalize_local_path_uri(src)
         dst = self._parser.normalize_uri(dst, allowed_schemes=("blob",))
         async with self._get_bucket_fs(dst) as bucket_fs:
-
             dst_key = bucket_fs.bucket.get_key_for_uri(dst)
             transferer = FileTransferer(LocalFS(), bucket_fs)
             await transferer.transfer_dir(
                 src=_extract_path(src),
                 dst=PurePosixPath(dst_key),
                 filter=filter,
                 ignore_file_names=ignore_file_names,
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_client.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_client.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_clusters.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_clusters.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_config.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from yarl import URL
 
 from ._core import _Core
 from ._errors import ConfigError
 from ._login import AuthTokenClient, _AuthConfig, _AuthToken
 from ._plugins import ConfigScope, PluginManager, _ParamType
 from ._rewrite import rewrite_module
-from ._server_cfg import Cluster, Preset, _ServerConfig, get_server_config
+from ._server_cfg import Cluster, Preset, Project, _ServerConfig, get_server_config
 from ._utils import NoPublicConstructor, find_project_root, flat
 
 WIN32 = sys.platform == "win32"
 CMD_RE = re.compile("[A-Za-z][A-Za-z0-9-]*")
 
 MALFORMED_CONFIG_MSG = "Malformed config. Please logout and login again."
 
@@ -37,17 +37,19 @@
         CREATE TABLE main (auth_config TEXT,
                            token TEXT,
                            expiration_time REAL,
                            refresh_token TEXT,
                            url TEXT,
                            admin_url TEXT,
                            version TEXT,
+                           project_name TEXT,
                            cluster_name TEXT,
                            org_name TEXT,
                            clusters TEXT,
+                           projects TEXT,
                            timestamp REAL)"""
     )
 }
 
 
 logger = logging.getLogger(__package__)
 
@@ -55,17 +57,19 @@
 @dataclass(frozen=True)
 class _ConfigData:
     auth_config: _AuthConfig
     auth_token: _AuthToken
     url: URL
     admin_url: Optional[URL]
     version: str
+    project_name: Optional[str]
     cluster_name: Optional[str]
     org_name: Optional[str]
     clusters: Mapping[str, Cluster]
+    projects: Mapping[Project.Key, Project]
 
 
 @dataclass(frozen=True)
 class _ConfigRecoveryData:
     url: URL
     cluster_name: str
     org_name: str
@@ -101,14 +105,18 @@
         return MappingProxyType(self._cluster.presets)
 
     @property
     def clusters(self) -> Mapping[str, Cluster]:
         return MappingProxyType(self._config_data.clusters)
 
     @property
+    def projects(self) -> Mapping[Project.Key, Project]:
+        return MappingProxyType(self._config_data.projects)
+
+    @property
     def cluster_name(self) -> str:
         if not self._config_data.clusters:
             raise RuntimeError(
                 "There are no clusters available. Please logout and login again."
             )
         name = self._get_user_cluster_name()
         if name is None:
@@ -140,14 +148,52 @@
         config = self._get_user_config()
         section = config.get("job")
         if section is not None:
             return section.get("org-name")
         return None
 
     @property
+    def project_name(self) -> Optional[str]:
+        name = self._get_user_project_name()
+        if name is None:
+            name = self._config_data.project_name
+        return name
+
+    @property
+    def project_name_or_raise(self) -> str:
+        name = self.project_name
+        if not name:
+            raise RuntimeError(
+                "The current project is not selected. "
+                "Please create one with 'neuro admin add-project', or "
+                "switch to the existing one with 'neuro config switch-project'."
+            )
+        return name
+
+    def _get_user_project_name(self) -> Optional[str]:
+        config = self._get_user_config()
+        section = config.get("job")
+        if section is not None:
+            return section.get("project-name")
+        return None
+
+    @property
+    def cluster_org_projects(self) -> List[Project]:
+        return self._get_cluster_org_projects(self.cluster_name, self.org_name)
+
+    def _get_cluster_org_projects(
+        self, cluster_name: str, org_name: Optional[str]
+    ) -> List[Project]:
+        projects = []
+        for project in self.projects.values():
+            if project.cluster_name == cluster_name and project.org_name == org_name:
+                projects.append(project)
+        return projects
+
+    @property
     def _cluster(self) -> Cluster:
         return self.get_cluster(self.cluster_name)
 
     def get_cluster(self, cluster_name: str) -> Cluster:
         try:
             return self._config_data.clusters[cluster_name]
         except KeyError:
@@ -187,15 +233,38 @@
             # if yes there is not way to switch cluster without relogin
             raise RuntimeError(
                 f"Cluster {self.cluster_name} doesn't exist in "
                 f"a list of available clusters "
                 f"{list(server_config.clusters)}. "
                 f"Please logout and login again."
             )
-        self.__config_data = replace(self._config_data, clusters=server_config.clusters)
+        self.__config_data = replace(
+            self._config_data,
+            clusters=server_config.clusters,
+            projects=server_config.projects,
+        )
+        _save(self._config_data, self._path)
+
+    async def switch_project(self, name: str) -> None:
+        if self._get_user_project_name() is not None:
+            raise RuntimeError(
+                "Cannot switch the project. Please edit the '.neuro.toml' file."
+            )
+        cluster_name = self.cluster_name
+        org_name = self.org_name
+        project_key = Project.Key(
+            cluster_name=cluster_name, org_name=org_name, project_name=name
+        )
+        if project_key not in self.projects:
+            projects = [p.name for p in self.cluster_org_projects]
+            raise RuntimeError(
+                f"Project {name} doesn't exist in a list of available "
+                f"tenant projects {projects}. "
+            )
+        self.__config_data = replace(self._config_data, project_name=name)
         _save(self._config_data, self._path)
 
     async def switch_cluster(self, name: str) -> None:
         if self._get_user_cluster_name() is not None:
             raise RuntimeError(
                 "Cannot switch the project cluster. "
                 "Please edit the '.neuro.toml' file."
@@ -212,15 +281,20 @@
             # If NO_ORG is available - use it
             # else use first in alphabetical order
             if None in cluster_orgs:
                 org_name = None
             else:
                 org_name = sorted(cluster_orgs, key=lambda it: it or "")[0]
         self.__config_data = replace(
-            self._config_data, cluster_name=name, org_name=org_name
+            self._config_data,
+            cluster_name=name,
+            org_name=org_name,
+            project_name=self._get_current_project_for_cluster_org(
+                cluster_name=name, org_name=org_name
+            ),
         )
         _save(self._config_data, self._path)
 
     async def switch_org(self, name: Optional[str]) -> None:
         if self._get_user_org_name() is not None:
             raise RuntimeError(
                 "Cannot switch the project org. Please edit the '.neuro.toml' file."
@@ -228,17 +302,47 @@
         if name not in self._cluster.orgs:
             cluster_org_names = [org or "NO_ORG" for org in self._cluster.orgs]
             raise RuntimeError(
                 f"Org {name or 'NO_ORG'} doesn't exist in "
                 f"a list of available orgs {list(cluster_org_names)} for "
                 f"cluster '{self.cluster_name}'. "
             )
-        self.__config_data = replace(self._config_data, org_name=name)
+        self.__config_data = replace(
+            self._config_data,
+            org_name=name,
+            project_name=self._get_current_project_for_cluster_org(
+                cluster_name=self.cluster_name, org_name=name
+            ),
+        )
         _save(self._config_data, self._path)
 
+    def _get_current_project_for_cluster_org(
+        self, cluster_name: str, org_name: Optional[str]
+    ) -> Optional[str]:
+        project_name = self.project_name
+        if project_name:
+            project_key = Project.Key(
+                cluster_name=cluster_name, org_name=org_name, project_name=project_name
+            )
+        else:
+            project_key = None
+        if not project_key or project_key not in self.projects:
+            # Use first in alphabetical order if any
+            cluster_org_projects = self._get_cluster_org_projects(
+                cluster_name, org_name
+            )
+            if cluster_org_projects:
+                cluster_org_projects = sorted(
+                    cluster_org_projects, key=lambda it: it.name
+                )
+                project_name = cluster_org_projects[0].name
+            else:
+                project_name = None
+        return project_name
+
     @property
     def api_url(self) -> URL:
         return self._config_data.url
 
     @property
     def admin_url(self) -> Optional[URL]:
         return self._config_data.admin_url
@@ -416,43 +520,48 @@
     try:
         with _open_db_ro(path) as db:
             cur = db.cursor()
             # only one row is always present normally
             cur.execute(
                 """
                 SELECT auth_config, token, expiration_time, refresh_token,
-                       url, admin_url, version, cluster_name, org_name, clusters
+                       url, admin_url, version, project_name, cluster_name,
+                       org_name, clusters, projects
                 FROM main ORDER BY timestamp DESC LIMIT 1"""
             )
             payload = cur.fetchone()
 
         api_url = URL(payload["url"])
         if not payload["admin_url"]:
             admin_url = None
         else:
             admin_url = URL(payload["admin_url"])
         auth_config = _deserialize_auth_config(payload)
         clusters = _deserialize_clusters(payload)
+        projects = _deserialize_projects(payload)
         version = payload["version"]
+        project_name = payload["project_name"]
         cluster_name = payload["cluster_name"]
         org_name = payload["org_name"]
 
         auth_token = _AuthToken(
             payload["token"], payload["expiration_time"], payload["refresh_token"]
         )
 
         return _ConfigData(
             auth_config=auth_config,
             auth_token=auth_token,
             url=api_url,
             admin_url=admin_url,
             version=version,
+            project_name=project_name,
             cluster_name=cluster_name,
             org_name=org_name,
             clusters=clusters,
+            projects=projects,
         )
     except (AttributeError, KeyError, TypeError, ValueError, sqlite3.DatabaseError):
         raise ConfigError(MALFORMED_CONFIG_MSG)
 
 
 def _load_recovery_data(path: Path) -> _ConfigRecoveryData:
     try:
@@ -498,14 +607,28 @@
         audience=auth_config["audience"],
         headless_callback_url=URL(auth_config["headless_callback_url"]),
         success_redirect_url=success_redirect_url,
         callback_urls=tuple(URL(u) for u in auth_config.get("callback_urls", [])),
     )
 
 
+def _deserialize_projects(payload: Dict[str, Any]) -> Dict[Project.Key, Project]:
+    projects = json.loads(payload["projects"])
+    ret: Dict[Project.Key, Project] = {}
+    for project_config in projects:
+        project = Project(
+            name=project_config["name"],
+            cluster_name=project_config["cluster_name"],
+            org_name=project_config["org_name"],
+            role=project_config["role"],
+        )
+        ret[project.key] = project
+    return ret
+
+
 def _deserialize_clusters(payload: Dict[str, Any]) -> Dict[str, Cluster]:
     clusters = json.loads(payload["clusters"])
     ret: Dict[str, Cluster] = {}
     for cluster_config in clusters:
         cluster = Cluster(
             name=cluster_config["name"],
             orgs=cluster_config.get("orgs", [None]),
@@ -567,43 +690,48 @@
         url = str(config.url)
         if not config.admin_url:
             admin_url = None
         else:
             admin_url = str(config.admin_url)
         auth_config = _serialize_auth_config(config.auth_config)
         clusters = _serialize_clusters(config.clusters)
+        projects = _serialize_projects(config.projects)
         version = config.version
+        project_name = config.project_name
         cluster_name = config.cluster_name
         org_name = config.org_name
         token = config.auth_token
     except (AttributeError, KeyError, TypeError, ValueError):
         raise ConfigError(MALFORMED_CONFIG_MSG)
 
     with _open_db_rw(path, suppress_errors) as db:
         _init_db_maybe(db)
 
         cur = db.cursor()
         cur.execute("DELETE FROM main")
         cur.execute(
             """
             INSERT INTO main
-            (auth_config, token, expiration_time, refresh_token,
-             url, admin_url, version, cluster_name, org_name, clusters, timestamp)
-            VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)""",
+            (auth_config, token, expiration_time, refresh_token, url, admin_url,
+             version, project_name, cluster_name, org_name, clusters, projects,
+             timestamp)
+            VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)""",
             (
                 auth_config,
                 token.token,
                 token.expiration_time,
                 token.refresh_token,
                 url,
                 admin_url,
                 version,
+                project_name,
                 cluster_name,
                 org_name,
                 clusters,
+                projects,
                 time.time(),
             ),
         )
         db.commit()
 
 
 def _serialize_auth_config(auth_config: _AuthConfig) -> str:
@@ -620,14 +748,27 @@
             "headless_callback_url": str(auth_config.headless_callback_url),
             "success_redirect_url": success_redirect_url,
             "callback_urls": [str(u) for u in auth_config.callback_urls],
         }
     )
 
 
+def _serialize_projects(projects: Mapping[Project.Key, Project]) -> str:
+    ret: List[Dict[str, Any]] = []
+    for project in projects.values():
+        project_config = {
+            "name": project.name,
+            "cluster_name": project.cluster_name,
+            "org_name": project.org_name,
+            "role": project.role,
+        }
+        ret.append(project_config)
+    return json.dumps(ret)
+
+
 def _serialize_clusters(clusters: Mapping[str, Cluster]) -> str:
     ret: List[Dict[str, Any]] = []
     for cluster in clusters.values():
         cluster_config = {
             "name": cluster.name,
             "orgs": cluster.orgs,
             "registry_url": str(cluster.registry_url),
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_config_factory.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_config_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     HeadlessNegotiator,
     _AuthToken,
     create_standalone_token,
     logout_from_browser,
 )
 from ._plugins import PluginManager
 from ._rewrite import rewrite_module
-from ._server_cfg import _ServerConfig, get_server_config
+from ._server_cfg import Project, _ServerConfig, get_server_config
 from ._tracing import _make_trace_config
 from ._utils import _ContextManager
 
 if sys.version_info >= (3, 11):
     from importlib.metadata import entry_points
 else:
     from importlib_metadata import entry_points
@@ -231,45 +231,68 @@
                     f"Config env variable {PASS_CONFIG_ENV_NAME} " "is not present"
                 )
         try:
             data = json.loads(base64.b64decode(config_data).decode())
             token = data["token"]
             cluster = data["cluster"]
             url = URL(data["url"])
+            org_name = data.get("org_name")
+            project_name = data.get("project_name")
         except (ValueError, KeyError):
             raise ConfigError(f"Data in passed config is malformed: {config_data}")
         await self.login_with_token(token, url=url, timeout=timeout)
         client = await self.get(timeout=timeout)
 
         await client.config.switch_cluster(cluster)
+        await client.config.switch_org(org_name)
+        if project_name:
+            await client.config.switch_project(project_name)
         await client.close()
 
     def _gen_config(
         self, server_config: _ServerConfig, token: _AuthToken, url: URL
     ) -> _ConfigData:
         from . import __version__
 
         if server_config.clusters:
             cluster_name = next(iter(server_config.clusters))
             org_name = server_config.clusters[cluster_name].orgs[0]
+            project_name = self._get_first_project(
+                server_config.projects, cluster_name, org_name
+            )
         else:
             cluster_name = None
             org_name = None
+            project_name = None
         config = _ConfigData(
             auth_config=server_config.auth_config,
             auth_token=token,
             url=url,
             admin_url=server_config.admin_url,
             version=__version__,
             cluster_name=cluster_name,
             org_name=org_name,
+            project_name=project_name,
             clusters=server_config.clusters,
+            projects=server_config.projects,
         )
         return config
 
+    def _get_first_project(
+        self,
+        projects: Mapping[Project.Key, Project],
+        cluster_name: str,
+        org_name: Optional[str],
+    ) -> Optional[str]:
+        cluster_org_projects = []
+        for project in projects.values():
+            if project.cluster_name == cluster_name and project.org_name == org_name:
+                cluster_org_projects.append(project.name)
+        return sorted(cluster_org_projects)[0] if cluster_org_projects else None
+
     async def logout(
         self,
         show_browser_cb: Optional[Callable[[URL], Awaitable[None]]] = None,
     ) -> None:
         if show_browser_cb is not None:
             try:
                 old_config = _load(self._path)
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_core.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_core.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_disks.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_disks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from enum import Enum
-from typing import Any, AsyncIterator, Mapping, Optional, Union
+from typing import Any, AsyncIterator, Dict, Mapping, Optional, Union
 
 from dateutil.parser import isoparse
 from yarl import URL
 
 from ._config import Config
 from ._core import _Core
 from ._rewrite import rewrite_module
@@ -24,27 +24,28 @@
 @dataclass(frozen=True)
 class Disk:
     id: str
     storage: int  # In bytes
     owner: str
     status: "Disk.Status"
     cluster_name: str
+    project_name: str
     org_name: Optional[str]
     created_at: datetime
     last_usage: Optional[datetime] = None
     name: Optional[str] = None
     timeout_unused: Optional[timedelta] = None
     used_bytes: Optional[int] = None
 
     @property
     def uri(self) -> URL:
         base = f"disk://{self.cluster_name}"
         if self.org_name:
             base += f"/{self.org_name}"
-        return URL(f"{base}/{self.owner}/{self.id}")
+        return URL(f"{base}/{self.project_name}/{self.id}")
 
     class Status(Enum):
         PENDING = "Pending"
         READY = "Ready"
         BROKEN = "Broken"
 
 
@@ -66,14 +67,15 @@
         else:
             timeout_unused = None
         return Disk(
             id=payload["id"],
             storage=payload["storage"],
             used_bytes=payload.get("used_bytes"),
             owner=payload["owner"],
+            project_name=payload["project_name"],
             name=payload.get("name"),
             status=Disk.Status(payload["status"]),
             cluster_name=self._config.cluster_name,
             org_name=payload.get("org_name"),
             created_at=isoparse(payload["created_at"]),
             last_usage=last_usage,
             timeout_unused=timeout_unused,
@@ -81,65 +83,93 @@
 
     def _get_disks_url(self, cluster_name: Optional[str]) -> URL:
         if cluster_name is None:
             cluster_name = self._config.cluster_name
         return self._config.get_cluster(cluster_name).disks_url
 
     @asyncgeneratorcontextmanager
-    async def list(self, cluster_name: Optional[str] = None) -> AsyncIterator[Disk]:
+    async def list(
+        self,
+        cluster_name: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
+    ) -> AsyncIterator[Disk]:
         url = self._get_disks_url(cluster_name)
+        params = {}
+        if not isinstance(org_name, OrgNameSentinel):
+            params["org_name"] = org_name or "NO_ORG"
+        if project_name:
+            params["project_name"] = project_name
+
         auth = await self._config._api_auth()
-        async with self._core.request("GET", url, auth=auth) as resp:
+        async with self._core.request("GET", url, auth=auth, params=params) as resp:
             ret = await resp.json()
             for disk_payload in ret:
                 yield self._parse_disk_payload(disk_payload)
 
     async def create(
         self,
         storage: int,
         timeout_unused: Optional[timedelta] = None,
         name: Optional[str] = None,
         cluster_name: Optional[str] = None,
+        project_name: Optional[str] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
     ) -> Disk:
         url = self._get_disks_url(cluster_name)
         auth = await self._config._api_auth()
         data = {
             "storage": storage,
             "life_span": timeout_unused.total_seconds() if timeout_unused else None,
             "name": name,
+            "project_name": project_name or self._config.project_name_or_raise,
             "org_name": org_name
             if not isinstance(org_name, OrgNameSentinel)
             else self._config.org_name,
         }
         async with self._core.request("POST", url, auth=auth, json=data) as resp:
             payload = await resp.json()
             return self._parse_disk_payload(payload)
 
     async def get(
         self,
         disk_id_or_name: str,
         cluster_name: Optional[str] = None,
-        owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> Disk:
         url = self._get_disks_url(cluster_name) / disk_id_or_name
         auth = await self._config._api_auth()
-        params = {}
-        if owner:
-            params["owner"] = owner
+        params = self._get_url_params(org_name, project_name)
         async with self._core.request("GET", url, auth=auth, params=params) as resp:
             payload = await resp.json()
             return self._parse_disk_payload(payload)
 
     async def rm(
         self,
         disk_id_or_name: str,
         cluster_name: Optional[str] = None,
-        owner: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         url = self._get_disks_url(cluster_name) / disk_id_or_name
         auth = await self._config._api_auth()
-        params = {}
-        if owner:
-            params["owner"] = owner
+        params = self._get_url_params(org_name, project_name)
         async with self._core.request("DELETE", url, auth=auth, params=params):
             pass
+
+    def _get_url_params(
+        self,
+        org_name: Union[Optional[str], OrgNameSentinel],
+        project_name: Optional[str],
+    ) -> Dict[str, str]:
+        params = {
+            "project_name": project_name or self._config.project_name_or_raise,
+        }
+        org_name_val = (
+            org_name
+            if not isinstance(org_name, OrgNameSentinel)
+            else self._config.org_name
+        )
+        if org_name_val:
+            params["org_name"] = org_name_val
+        return params
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_errors.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_errors.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_file_filter.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_file_filter.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_file_utils.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_file_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_gcs_bucket_provider.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_gcs_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_images.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,24 @@
         self._parse = parse
         self._temporary_images: Set[str] = set()
         self.__docker: Optional[aiodocker.Docker] = None
 
     def _get_image_url(self, remote: RemoteImage) -> URL:
         cluster_name = remote.cluster_name
         if cluster_name:
-            assert remote.owner
+            assert remote.project_name
             registry_url = self._config.get_cluster(cluster_name).registry_url
         else:
             registry_url = self._config.registry_url
         org_prefix = ""
         if remote.org_name:
             org_prefix = f"{remote.org_name}/"
         return (
-            registry_url.with_path("/v2/") / f"{org_prefix}{remote.owner}/{remote.name}"
+            registry_url.with_path("/v2/")
+            / f"{org_prefix}{remote.project_name}/{remote.name}"
         )
 
     @property
     def _docker(self) -> aiodocker.Docker:
         if not self.__docker:
             try:
                 self.__docker = aiodocker.Docker()
@@ -224,16 +225,16 @@
                 url = URL(resp.links["next"]["url"])
         return result
 
     def _validate_image_for_tags(self, image: RemoteImage) -> None:
         err = f"Invalid image `{image}`: "
         if image.tag is not None:
             raise ValueError(err + "tag is not allowed")
-        if not image.owner:
-            raise ValueError(err + "missing image owner")
+        if not image.project_name:
+            raise ValueError(err + "missing image project")
         if not image.name:
             raise ValueError(err + "missing image name")
 
     async def tags(self, image: RemoteImage) -> List[RemoteImage]:
         self._validate_image_for_tags(image)
         auth = await self._config._registry_auth()
         url = self._get_image_url(image) / "tags" / "list"
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_jobs.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 
 @rewrite_module
 @dataclass(frozen=True)
 class JobDescription:
     id: str
     owner: str
     cluster_name: str
+    project_name: str
     status: JobStatus
     history: JobStatusHistory
     container: Container
     scheduler_enabled: bool
     pass_config: bool
     uri: URL
     total_price_credits: Decimal
@@ -348,18 +349,22 @@
         pass_config: bool = False,
         wait_for_jobs_quota: bool = False,
         schedule_timeout: Optional[float] = None,
         restart_policy: JobRestartPolicy = JobRestartPolicy.NEVER,
         life_span: Optional[float] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
         priority: Optional[JobPriority] = None,
+        project_name: Optional[str] = None,
     ) -> JobDescription:
         url = self._config.api_url / "jobs"
+        if not project_name:
+            project_name = self._config.project_name_or_raise
         payload = _job_to_api(
             cluster_name=self._config.cluster_name,
+            project_name=project_name,
             name=name,
             tags=tags,
             description=description,
             pass_config=pass_config,
             wait_for_jobs_quota=wait_for_jobs_quota,
             schedule_timeout=schedule_timeout,
             restart_policy=restart_policy,
@@ -415,14 +420,15 @@
         wait_for_jobs_quota: bool = False,
         schedule_timeout: Optional[float] = None,
         restart_policy: JobRestartPolicy = JobRestartPolicy.NEVER,
         life_span: Optional[float] = None,
         privileged: bool = False,
         priority: Optional[JobPriority] = None,
         energy_schedule_name: Optional[str] = None,
+        project_name: Optional[str] = None,
     ) -> JobDescription:
         url = (self._config.api_url / "jobs").with_query("from_preset")
         container_payload = _container_to_api(
             config=self._config,
             image=image,
             entrypoint=entrypoint,
             command=command,
@@ -434,14 +440,15 @@
             secret_files=secret_files,
             disk_volumes=disk_volumes,
             tty=tty,
             shm=shm,
         )
         payload = _job_to_api(
             cluster_name=cluster_name or self._config.cluster_name,
+            project_name=project_name or self._config.project_name_or_raise,
             name=name,
             preset_name=preset_name,
             tags=tags,
             description=description,
             pass_config=pass_config,
             wait_for_jobs_quota=wait_for_jobs_quota,
             schedule_timeout=schedule_timeout,
@@ -469,14 +476,16 @@
         tags: Iterable[str] = (),
         owners: Iterable[str] = (),
         since: Optional[datetime] = None,
         until: Optional[datetime] = None,
         reverse: bool = False,
         limit: Optional[int] = None,
         cluster_name: Optional[str] = None,
+        org_names: Iterable[Optional[str]] = (),
+        project_names: Iterable[str] = (),
         _materialized: Optional[bool] = None,
         _being_dropped: Optional[bool] = False,
         _logs_removed: Optional[bool] = False,
     ) -> AsyncIterator[JobDescription]:
         url = self._config.api_url / "jobs"
         headers = {"Accept": "application/x-ndjson"}
         params: MultiDict[str] = MultiDict()
@@ -506,14 +515,18 @@
             params.add("limit", str(limit))
         if _materialized is not None:
             params.add("materialized", str(_materialized))
         if _being_dropped is not None:
             params.add("being_dropped", str(_being_dropped))
         if _logs_removed is not None:
             params.add("logs_removed", str(_logs_removed))
+        for org_name in org_names:
+            params.add("org_name", org_name or "NO_ORG")
+        for project_name in project_names:
+            params.add("project_name", project_name)
         auth = await self._config._api_auth()
         async with self._core.request(
             "GET", url, headers=headers, params=params, auth=auth
         ) as resp:
             if resp.headers.get("Content-Type", "").startswith("application/x-ndjson"):
                 async for line in resp.content:
                     server_message = json.loads(line)
@@ -643,15 +656,15 @@
             progress.commit_started(data_1)
 
             chunk_2 = await resp.content.readline()
             data_2 = _parse_commit_finished_chunk(id, _load_chunk(chunk_2))
             progress.commit_finished(data_2)
 
             # then, we expect stream for docker-push
-            src = LocalImage(f"{image.owner}/{image.name}", image.tag)
+            src = LocalImage(f"{image.project_name}/{image.name}", image.tag)
             progress.push(ImageProgressPush(src, dst=image))
             async for chunk in resp.content:
                 obj = _load_chunk(chunk)
                 push_step = _try_parse_image_progress_step(obj, image.tag)
                 if push_step:
                     progress.step(push_step)
 
@@ -963,15 +976,18 @@
         primitive["env"] = env
     if volumes:
         primitive["volumes"] = [_volume_to_api(v, config) for v in volumes]
     if secret_env:
         primitive["secret_env"] = {
             k: str(
                 normalize_secret_uri(
-                    v, config.username, config.cluster_name, config.org_name
+                    v,
+                    config.project_name_or_raise,
+                    config.cluster_name,
+                    config.org_name,
                 )
             )
             for k, v in secret_env.items()
         }
     if secret_files:
         primitive["secret_volumes"] = [
             _secret_file_to_api(v, config) for v in secret_files
@@ -1063,39 +1079,44 @@
         life_span=life_span,
         schedule_timeout=res.get("schedule_timeout", None),
         preset_name=res.get("preset_name"),
         total_price_credits=total_price_credits,
         price_credits_per_hour=price_credits_per_hour,
         priority=priority,
         energy_schedule_name=res.get("energy_schedule_name"),
+        project_name=res.get("project_name", owner),
         _internal=JobDescriptionInternal(
             materialized=res.get("materialized", False),
             being_dropped=res.get("being_dropped", False),
             logs_removed=res.get("logs_removed", False),
         ),
     )
 
 
 def _job_to_api(
     cluster_name: str,
+    project_name: str,
     name: Optional[str] = None,
     preset_name: Optional[str] = None,
     tags: Sequence[str] = (),
     description: Optional[str] = None,
     pass_config: bool = False,
     wait_for_jobs_quota: bool = False,
     schedule_timeout: Optional[float] = None,
     restart_policy: JobRestartPolicy = JobRestartPolicy.NEVER,
     life_span: Optional[float] = None,
     privileged: bool = False,
     org_name: Optional[str] = None,
     priority: Optional[JobPriority] = None,
     energy_schedule_name: Optional[str] = None,
 ) -> Dict[str, Any]:
-    primitive: Dict[str, Any] = {"pass_config": pass_config}
+    primitive: Dict[str, Any] = {
+        "pass_config": pass_config,
+        "project_name": project_name,
+    }
     if name:
         primitive["name"] = name
     if preset_name:
         primitive["preset_name"] = preset_name
     if tags:
         primitive["tags"] = tags
     if description:
@@ -1128,37 +1149,46 @@
         gpu_duty_cycle=value.get("gpu_duty_cycle"),
         gpu_memory_bytes=value.get("gpu_memory_bytes"),
     )
 
 
 def _volume_to_api(volume: Volume, config: Config) -> Dict[str, Any]:
     uri = normalize_storage_path_uri(
-        volume.storage_uri, config.username, config.cluster_name, config.org_name
+        volume.storage_uri,
+        config.project_name_or_raise,
+        config.cluster_name,
+        config.org_name,
     )
     resp: Dict[str, Any] = {
         "src_storage_uri": str(uri),
         "dst_path": volume.container_path,
         "read_only": bool(volume.read_only),
     }
     return resp
 
 
 def _secret_file_to_api(secret_file: SecretFile, config: Config) -> Dict[str, Any]:
     uri = normalize_secret_uri(
-        secret_file.secret_uri, config.username, config.cluster_name, config.org_name
+        secret_file.secret_uri,
+        config.project_name_or_raise,
+        config.cluster_name,
+        config.org_name,
     )
     return {
         "src_secret_uri": str(uri),
         "dst_path": secret_file.container_path,
     }
 
 
 def _disk_volume_to_api(volume: DiskVolume, config: Config) -> Dict[str, Any]:
     uri = normalize_disk_uri(
-        volume.disk_uri, config.username, config.cluster_name, config.org_name
+        volume.disk_uri,
+        config.project_name_or_raise,
+        config.cluster_name,
+        config.org_name,
     )
     resp: Dict[str, Any] = {
         "src_disk_uri": str(uri),
         "dst_path": volume.container_path,
         "read_only": bool(volume.read_only),
     }
     return resp
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_login.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_login.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_parser.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from yarl import URL
 
 from ._config import Config
 from ._parsing_utils import LocalImage, RemoteImage, TagOption, _ImageNameParser
 from ._rewrite import rewrite_module
 from ._url_utils import _check_scheme, _extract_path, _normalize_uri, uri_from_cli
-from ._utils import ORG_NAME_SENTINEL, NoPublicConstructor, OrgNameSentinel
+from ._utils import NoPublicConstructor
 
 
 @rewrite_module
 @dataclass(frozen=True)
 class SecretFile:
     secret_uri: URL
     container_path: str
@@ -79,15 +79,15 @@
         volume: str,
         cluster_name: Optional[str] = None,
         org_name: Union[str, None, _Unset] = _Unset(),
     ) -> Volume:
         raw_uri, container_path, read_only = self._parse_generic_volume(volume)
         storage_uri = uri_from_cli(
             raw_uri,
-            self._config.username,
+            self._config.project_name_or_raise,
             cluster_name or self._config.cluster_name,
             org_name if not isinstance(org_name, _Unset) else self._config.org_name,
             allowed_schemes=("storage",),
         )
         return Volume(
             storage_uri=storage_uri, container_path=container_path, read_only=read_only
         )
@@ -118,15 +118,15 @@
         self,
         uri: str,
         cluster_name: Optional[str] = None,
         org_name: Union[str, None, _Unset] = _Unset(),
     ) -> URL:
         return uri_from_cli(
             uri,
-            self._config.username,
+            self._config.project_name_or_raise,
             cluster_name or self._config.cluster_name,
             org_name if not isinstance(org_name, _Unset) else self._config.org_name,
             allowed_schemes=("secret",),
         )
 
     def _build_disk_volumes(
         self, input_volumes: List[str], cluster_name: Optional[str] = None
@@ -144,35 +144,29 @@
         self,
         uri: str,
         cluster_name: Optional[str] = None,
         org_name: Union[str, None, _Unset] = _Unset(),
     ) -> URL:
         return uri_from_cli(
             uri,
-            self._config.username,
+            self._config.project_name_or_raise,
             cluster_name or self._config.cluster_name,
             org_name if not isinstance(org_name, _Unset) else self._config.org_name,
             allowed_schemes=("disk",),
         )
 
-    def _get_image_parser(
-        self,
-        cluster_name: Optional[str] = None,
-        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
-    ) -> _ImageNameParser:
+    def _get_image_parser(self, cluster_name: Optional[str] = None) -> _ImageNameParser:
         registry = {
             cluster.name: cluster.registry_url
             for cluster in self._config.clusters.values()
         }
         return _ImageNameParser(
-            default_user=self._config.username,
             default_cluster=cluster_name or self._config.cluster_name,
-            default_org=org_name
-            if not isinstance(org_name, OrgNameSentinel)
-            else self._config.org_name,
+            default_org=self._config.org_name,
+            default_project=self._config.project_name_or_raise,
             registry_urls=registry,
         )
 
     def local_image(self, image: str) -> LocalImage:
         return self._get_image_parser().parse_as_local_image(image)
 
     def remote_image(
@@ -267,15 +261,15 @@
         allowed_schemes: Iterable[str] = (),
         cluster_name: Optional[str] = None,
         org_name: Union[None, str, _Unset] = _Unset(),
         short: bool = False,
     ) -> URL:
         ret = uri_from_cli(
             id_or_name_or_uri,
-            self._config.username,
+            self._config.project_name_or_raise,
             cluster_name or self._config.cluster_name,
             org_name if not isinstance(org_name, _Unset) else self._config.org_name,
             allowed_schemes=allowed_schemes,
         )
         if short:
             ret = self._short(ret)
         return ret
@@ -289,15 +283,15 @@
 
     def path_to_uri(
         self,
         path: Path,
     ) -> URL:
         return uri_from_cli(
             str(path),
-            self._config.username,
+            self._config.project_name_or_raise,
             self._config.cluster_name,
             self._config.org_name,
             allowed_schemes=("file",),
         )
 
     def normalize_uri(
         self,
@@ -307,31 +301,35 @@
         cluster_name: Optional[str] = None,
         org_name: Union[None, str, _Unset] = _Unset(),
         short: bool = False,
     ) -> URL:
         _check_scheme(uri.scheme, allowed_schemes)
         ret = _normalize_uri(
             uri,
-            self._config.username,
+            self._config.project_name_or_raise,
             cluster_name or self._config.cluster_name,
             org_name if not isinstance(org_name, _Unset) else self._config.org_name,
         )
         if short:
             ret = self._short(ret)
         return ret
 
     def _short(self, uri: URL) -> URL:
         ret = uri
         if uri.scheme != "file":
             if ret.host == self._config.cluster_name:
                 prefix: Tuple[str, ...]
                 if self._config.org_name is None:
-                    prefix = ("/", self._config.username)
+                    prefix = ("/", self._config.project_name_or_raise)
                 else:
-                    prefix = ("/", self._config.org_name, self._config.username)
+                    prefix = (
+                        "/",
+                        self._config.org_name,
+                        self._config.project_name_or_raise,
+                    )
                 if ret.parts[: len(prefix)] == prefix:
                     ret = URL.build(
                         scheme=ret.scheme,
                         host="",
                         path="/".join(ret.parts[len(prefix) :]),
                     )
         else:
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_parsing_utils.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_parsing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,67 +17,67 @@
 
 
 @rewrite_module
 @dataclass(frozen=True)
 class RemoteImage:
     name: str
     tag: Optional[str] = None
-    owner: Optional[str] = None
     registry: Optional[str] = None
     cluster_name: Optional[str] = None
     org_name: Optional[str] = None
+    project_name: Optional[str] = None
 
     @property
     def _is_in_neuro_registry(self) -> bool:
-        return bool(self.registry and self.owner and self.cluster_name)
+        return bool(self.registry and self.cluster_name and self.project_name)
 
     @classmethod
     def new_neuro_image(
         cls,
         name: str,
         registry: str,
         *,
-        owner: str,
         cluster_name: str,
         org_name: Optional[str],
+        project_name: str,
         tag: Optional[str] = None,
     ) -> "RemoteImage":
         return RemoteImage(
             name=name,
             tag=tag,
-            owner=owner,
             registry=registry,
             cluster_name=cluster_name,
             org_name=org_name,
+            project_name=project_name,
         )
 
     @classmethod
     def new_external_image(
         cls, name: str, registry: Optional[str] = None, *, tag: Optional[str] = None
     ) -> "RemoteImage":
         return RemoteImage(name=name, tag=tag, registry=registry)
 
     def __post_init__(self) -> None:
         if self.registry:
-            if self.owner:
+            if self.project_name:
                 if not self.cluster_name:
                     raise ValueError("required cluster name")
             else:
                 if self.cluster_name:
-                    raise ValueError("required owner")
+                    raise ValueError("required project")
         else:
-            if self.owner or self.cluster_name:
+            if self.project_name or self.cluster_name:
                 raise ValueError("required registry")
 
     def as_docker_url(self, with_scheme: bool = False) -> str:
         if self._is_in_neuro_registry:
             if self.org_name:
-                prefix = f"{self.registry}/{self.org_name}/{self.owner}/"
+                prefix = f"{self.registry}/{self.org_name}/{self.project_name}/"
             else:
-                prefix = f"{self.registry}/{self.owner}/"
+                prefix = f"{self.registry}/{self.project_name}/"
             prefix = "https://" + prefix if with_scheme else prefix
         else:
             prefix = ""
         suffix = f":{self.tag}" if self.tag else ""
         return f"{prefix}{self.name}{suffix}"
 
     def __str__(self) -> str:
@@ -89,15 +89,15 @@
             base = ""
             if self.org_name:
                 base = f"/{self.org_name}"
             result = str(
                 URL.build(
                     scheme="image",
                     host=self.cluster_name,
-                    path=f"{base}/{self.owner}/{result}",
+                    path=f"{base}/{self.project_name}/{result}",
                 )
             )
         return result
 
     def __rich__(self) -> str:
         return str(self)
 
@@ -115,22 +115,22 @@
     def __rich__(self) -> str:
         return str(self)
 
 
 class _ImageNameParser:
     def __init__(
         self,
-        default_user: str,
         default_cluster: str,
         default_org: Optional[str],
+        default_project: str,
         registry_urls: Dict[str, URL],
     ):
-        self._default_user = default_user
         self._default_cluster = default_cluster
         self._default_org_name = default_org
+        self._default_project_name = default_project
         self._registries = {}
         for cluster_name, registry_url in registry_urls.items():
             if not registry_url.host:
                 raise ValueError(
                     f"Empty hostname in registry URL '{registry_url}': "
                     f"please consider updating configuration"
                 )
@@ -174,31 +174,31 @@
             registry, name = name.split("/", 1)
 
         return RemoteImage.new_external_image(name=name, tag=img.tag, registry=registry)
 
     def convert_to_neuro_image(self, image: LocalImage) -> RemoteImage:
         cluster_name = self._default_cluster
         org_name = self._default_org_name
-        owner = self._default_user
+        project_name = self._default_project_name
         name = image.name
         res = self._find_by_registry(name)
         if res:
             cluster_name, path = res
             if path:
-                owner, _, name = path.partition("/")
+                project_name, _, name = path.partition("/")
                 if not name:
-                    owner = self._default_user
+                    project_name = self._default_project_name
                     name = path
 
         return RemoteImage.new_neuro_image(
             name=name,
             tag=image.tag,
-            owner=owner,
             cluster_name=cluster_name,
             org_name=org_name,
+            project_name=project_name,
             registry=self._registries[cluster_name],
         )
 
     def convert_to_local_image(self, image: RemoteImage) -> LocalImage:
         return LocalImage(name=image.name, tag=image.tag)
 
     def has_tag(self, image: str) -> bool:
@@ -211,15 +211,15 @@
         _, tag = self._split_image_name(image)
         return bool(tag)
 
     def _validate_image_name(self, image: str) -> None:
         if not image:
             raise ValueError("empty image name")
         if image.startswith("-"):
-            raise ValueError(f"image cannot start with dash")
+            raise ValueError("image cannot start with dash")
         if image == "image:latest":
             raise ValueError(
                 "ambiguous value: valid as both local and remote image name"
             )
 
     def _parse_as_local_image(self, image: str) -> LocalImage:
         if image.startswith("image:"):
@@ -237,59 +237,62 @@
             if not url.scheme and url.path.startswith("image:"):
                 prefix = ""
                 if self._default_org_name:
                     prefix = f"/{self._default_org_name}"
                 url = URL.build(
                     scheme="image",
                     host=self._default_cluster,
-                    path=f"{prefix}/{self._default_user}/{url.path[len('image:') :]}",
+                    path=(
+                        f"{prefix}/{self._default_project_name}"
+                        f"/{url.path[len('image:') :]}"
+                    ),
                 )
         else:
             res = self._find_by_registry(image)
             if not res:
                 raise ValueError("scheme 'image:' is required for remote images")
             cluster_name, path = res
             url = URL(f"image://{cluster_name}/{path}")
 
         if not url.path or url.path == "/":
             raise ValueError("no image name specified")
         _check_uri(url)
 
         name, tag = self._split_image_name(url.path.lstrip("/"), default_tag)
         if url.host is None:
-            # This is short url, either image:name or image:/username/name
+            # This is short url, either image:name or image:/project/name
             cluster_name = self._default_cluster
             org_name = self._default_org_name
         else:
             cluster_name = url.host
             org_name = None
         if url.path.startswith("/"):
-            owner, _, name = name.partition("/")
-            if owner == self._default_org_name and url.host:
-                # Long form with explicit org name (image://cluster/org/user/image)
-                org_name = owner
-                owner, _, name = name.partition("/")
+            project_name, _, name = name.partition("/")
+            if project_name == self._default_org_name and url.host:
+                # Long form with explicit org name (image://cluster/org/project/image)
+                org_name = project_name
+                project_name, _, name = name.partition("/")
             if not name:
                 raise ValueError("no image name specified")
         else:
-            owner = self._default_user
+            project_name = self._default_project_name
         if cluster_name not in self._registries:
             tip = "Please logout and login again."
             raise RuntimeError(
                 f"Cluster {cluster_name} doesn't exist in "
                 f"a list of available clusters "
                 f"{list(self._registries)}. {tip}"
             )
         return RemoteImage.new_neuro_image(
             name=name,
             tag=tag,
             registry=self._registries[cluster_name],
-            owner=owner,
             cluster_name=cluster_name,
             org_name=org_name,
+            project_name=project_name,
         )
 
     def _find_by_registry(self, image: str) -> Optional[Tuple[str, str]]:
         for cluster_name, registry in self._registries.items():
             if image.startswith(f"{registry}/"):
                 path = image[len(registry) :].lstrip("/")
                 return cluster_name, path
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_plugins.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_plugins.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_s3_bucket_provider.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_s3_bucket_provider.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_secrets.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_secrets.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,76 +18,93 @@
 @rewrite_module
 @dataclass(frozen=True)
 class Secret:
     key: str
     owner: str
     cluster_name: str
     org_name: Optional[str]
+    project_name: str
 
     @property
     def uri(self) -> URL:
         base = f"secret://{self.cluster_name}"
         if self.org_name:
             base += f"/{self.org_name}"
-        return URL(f"{base}/{self.owner}/{self.key}")
+        return URL(f"{base}/{self.project_name}/{self.key}")
 
 
 @rewrite_module
 class Secrets(metaclass=NoPublicConstructor):
     def __init__(self, core: _Core, config: Config) -> None:
         self._core = core
         self._config = config
 
     def _get_secrets_url(self, cluster_name: Optional[str]) -> URL:
         if cluster_name is None:
             cluster_name = self._config.cluster_name
         return self._config.get_cluster(cluster_name).secrets_url
 
     @asyncgeneratorcontextmanager
-    async def list(self, cluster_name: Optional[str] = None) -> AsyncIterator[Secret]:
+    async def list(
+        self,
+        cluster_name: Optional[str] = None,
+        org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
+    ) -> AsyncIterator[Secret]:
         url = self._get_secrets_url(cluster_name)
+        params = {}
+        if not isinstance(org_name, OrgNameSentinel):
+            params["org_name"] = org_name or "NO_ORG"
+        if project_name:
+            params["project_name"] = project_name
         auth = await self._config._api_auth()
-        async with self._core.request("GET", url, auth=auth) as resp:
+        async with self._core.request("GET", url, params=params, auth=auth) as resp:
             ret = await resp.json()
             for j in ret:
                 yield Secret(
                     key=j["key"],
                     owner=j["owner"],
                     cluster_name=cluster_name or self._config.cluster_name,
                     org_name=j.get("org_name"),
+                    project_name=j["project_name"],
                 )
 
     async def add(
         self,
         key: str,
         value: bytes,
         cluster_name: Optional[str] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         url = self._get_secrets_url(cluster_name)
         auth = await self._config._api_auth()
         data = {
             "key": key,
             "value": base64.b64encode(value).decode("ascii"),
             "org_name": org_name
             if not isinstance(org_name, OrgNameSentinel)
             else self._config.org_name,
+            "project_name": project_name or self._config.project_name_or_raise,
         }
         async with self._core.request("POST", url, auth=auth, json=data):
             pass
 
     async def rm(
         self,
         key: str,
         cluster_name: Optional[str] = None,
         org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+        project_name: Optional[str] = None,
     ) -> None:
         url = self._get_secrets_url(cluster_name) / key
         auth = await self._config._api_auth()
-        params = {}
+        params = {
+            "project_name": project_name or self._config.project_name_or_raise,
+        }
         org_name_val = (
             org_name
             if not isinstance(org_name, OrgNameSentinel)
             else self._config.org_name
         )
         if org_name_val:
             params["org_name"] = org_name_val
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_server_cfg.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_server_cfg.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,37 @@
     @property
     def memory_mb(self) -> int:
         return self.memory // 2**20
 
 
 @rewrite_module
 @dataclass(frozen=True)
+class Project:
+    @dataclass(frozen=True)
+    class Key:
+        cluster_name: str
+        org_name: Optional[str]
+        project_name: str
+
+    cluster_name: str
+    org_name: Optional[str]
+    name: str
+    role: str
+
+    @property
+    def key(self) -> Key:
+        return self.Key(
+            cluster_name=self.cluster_name,
+            org_name=self.org_name,
+            project_name=self.name,
+        )
+
+
+@rewrite_module
+@dataclass(frozen=True)
 class Cluster:
     name: str
     orgs: List[Optional[str]]
     registry_url: URL
     storage_url: URL
     users_url: URL
     monitoring_url: URL
@@ -44,14 +67,32 @@
 
 
 @dataclass(frozen=True)
 class _ServerConfig:
     admin_url: Optional[URL]
     auth_config: _AuthConfig
     clusters: Mapping[str, Cluster]
+    projects: Mapping[Project.Key, Project]
+
+
+def _parse_project_config(payload: Dict[str, Any]) -> Project:
+    return Project(
+        name=payload["name"],
+        cluster_name=payload["cluster_name"],
+        org_name=payload.get("org_name"),
+        role=payload["role"],
+    )
+
+
+def _parse_projects(payload: Dict[str, Any]) -> Dict[Project.Key, Project]:
+    ret: Dict[Project.Key, Project] = {}
+    for item in payload.get("projects", []):
+        project = _parse_project_config(item)
+        ret[project.key] = project
+    return ret
 
 
 def _parse_cluster_config(payload: Dict[str, Any]) -> Cluster:
     presets: Dict[str, Preset] = {}
     for data in payload["resource_presets"]:
         tpu_type = tpu_software_version = None
         if "tpu" in data:
@@ -83,15 +124,15 @@
         presets=presets,
     )
     return cluster_config
 
 
 def _parse_clusters(payload: Dict[str, Any]) -> Dict[str, Cluster]:
     ret: Dict[str, Cluster] = {}
-    for item in payload.get("clusters", {}):
+    for item in payload.get("clusters", []):
         cluster = _parse_cluster_config(item)
         ret[cluster.name] = cluster
     return ret
 
 
 async def get_server_config(
     client: aiohttp.ClientSession, url: URL, token: Optional[str] = None
@@ -119,18 +160,20 @@
             logout_url=URL(payload["logout_url"]),
             client_id=payload["client_id"],
             audience=payload["audience"],
             success_redirect_url=success_redirect_url,
             callback_urls=callback_urls,
             headless_callback_url=headless_callback_url,
         )
-        clusters = _parse_clusters(payload)
         admin_url: Optional[URL] = None
         if "admin_url" in payload:
             admin_url = URL(payload["admin_url"])
         if headers and not payload.get("authorized", False):
             raise AuthError("Cannot authorize user")
+        clusters = _parse_clusters(payload)
+        projects = _parse_projects(payload)
         return _ServerConfig(
             admin_url=admin_url,
             auth_config=auth_config,
             clusters=clusters,
+            projects=projects,
         )
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_service_accounts.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_service_accounts.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 class ServiceAccount:
     id: str
     name: Optional[str]
     owner: str
     default_cluster: str
     role: str
     created_at: datetime
+    default_project: str
+    default_org: Optional[str] = None
 
 
 @rewrite_module
 class ServiceAccounts(metaclass=NoPublicConstructor):
     def __init__(self, core: _Core, config: Config) -> None:
         self._core = core
         self._config = config
@@ -34,14 +36,16 @@
         return ServiceAccount(
             id=payload["id"],
             owner=payload["owner"],
             name=payload["name"],
             default_cluster=payload["default_cluster"],
             role=payload["role"],
             created_at=isoparse(payload["created_at"]),
+            default_project=payload["default_project"],
+            default_org=payload.get("default_org"),
         )
 
     @asyncgeneratorcontextmanager
     async def list(self) -> AsyncIterator[ServiceAccount]:
         url = self._config.service_accounts_url
         auth = await self._config._api_auth()
         async with self._core.request("GET", url, auth=auth) as resp:
@@ -49,21 +53,27 @@
             for item in ret:
                 yield self._parse_account_payload(item)
 
     async def create(
         self,
         name: Optional[str] = None,
         default_cluster: Optional[str] = None,
+        default_org: Optional[str] = None,
+        default_project: Optional[str] = None,
     ) -> Tuple[ServiceAccount, str]:
         url = self._config.service_accounts_url
         auth = await self._config._api_auth()
         data = {
             "name": name,
             "default_cluster": default_cluster or self._config.cluster_name,
+            "default_project": default_project or self._config.project_name_or_raise,
         }
+        default_org = default_org or self._config.org_name
+        if default_org:
+            data["default_org"] = default_org
         async with self._core.request("POST", url, auth=auth, json=data) as resp:
             payload = await resp.json()
             return self._parse_account_payload(payload), payload["token"]
 
     async def get(self, id_or_name: str) -> ServiceAccount:
         url = self._config.service_accounts_url / id_or_name
         auth = await self._config._api_auth()
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_storage.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,18 @@
         self._config = config
         self._file_sem = asyncio.BoundedSemaphore(MAX_OPEN_FILES)
         self._min_time_diff = 0.0
         self._max_time_diff = 0.0
 
     def _normalize_uri(self, uri: URL) -> URL:
         return normalize_storage_path_uri(
-            uri, self._config.username, self._config.cluster_name, self._config.org_name
+            uri,
+            self._config.project_name_or_raise,
+            self._config.cluster_name,
+            self._config.org_name,
         )
 
     def _get_storage_url(self, uri: URL, *, normalized: bool = False) -> URL:
         if not normalized:
             uri = self._normalize_uri(uri)
         assert uri.host is not None
         return self._config.get_cluster(uri.host).storage_url / uri.path.lstrip("/")
@@ -385,19 +388,22 @@
             return _disk_usage_from_api(cluster_name, org_name_val, uri, res)
 
     def _create_disk_usage_uri(
         self, cluster_name: Optional[str], org_name: Optional[str]
     ) -> URL:
         if org_name:
             uri = self._normalize_uri(
-                URL(f"storage://{cluster_name}/{org_name}/{self._config.username}")
+                URL(
+                    f"storage://{cluster_name}/{org_name}"
+                    f"/{self._config.project_name_or_raise}"
+                )
             )
         else:
             uri = self._normalize_uri(
-                URL(f"storage://{cluster_name}/{self._config.username}")
+                URL(f"storage://{cluster_name}/{self._config.project_name_or_raise}")
             )
         assert uri.host is not None
         return uri
 
     @asyncgeneratorcontextmanager
     async def open(
         self, uri: URL, offset: int = 0, size: Optional[int] = None
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_tracing.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_tracing.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_url_utils.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_url_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from yarl import URL
 
 CLUSTER_SCHEMES = ("storage", "image", "job", "secret", "disk", "blob", "flow")
 
 
 def uri_from_cli(
     path_or_uri: str,
-    username: str,
+    project_name: str,
     cluster_name: str,
     org_name: Optional[str],
     *,
     allowed_schemes: Iterable[str] = ("file", "storage"),
 ) -> URL:
     if not isinstance(allowed_schemes, tuple):
         allowed_schemes = tuple(allowed_schemes)
@@ -50,15 +50,16 @@
         )
     _check_scheme(uri.scheme, allowed_schemes)
     # Check string representation to detect also trailing "?" and "#".
     _check_uri_str(path_or_uri, uri.scheme)
     if uri.scheme == "file":
         uri = normalize_local_path_uri(uri)
     else:
-        uri = _normalize_uri(uri, username, cluster_name, org_name)
+        # TODO (y.s.): replace username to project_name
+        uri = _normalize_uri(uri, project_name, cluster_name, org_name)
     return uri
 
 
 def _check_scheme(scheme: str, allowed: Iterable[str]) -> None:
     if not isinstance(allowed, tuple):
         allowed = tuple(allowed)
     if not allowed:
@@ -71,61 +72,61 @@
             verb = "is"
         raise ValueError(
             f"Invalid scheme '{scheme}:' (only {allowed_str} {verb} allowed)"
         )
 
 
 def normalize_storage_path_uri(
-    uri: URL, username: str, cluster_name: str, org_name: Optional[str]
+    uri: URL, project_name: str, cluster_name: str, org_name: Optional[str]
 ) -> URL:
     """Normalize storage url."""
     if uri.scheme != "storage":
         raise ValueError(
             f"Invalid storage scheme '{uri.scheme}:' (only 'storage:' is allowed)"
         )
-    return _normalize_uri(uri, username, cluster_name, org_name)
+    return _normalize_uri(uri, project_name, cluster_name, org_name)
 
 
 def normalize_secret_uri(
-    uri: URL, username: str, cluster_name: str, org_name: Optional[str]
+    uri: URL, project_name: str, cluster_name: str, org_name: Optional[str]
 ) -> URL:
     """Normalize secret url."""
     if uri.scheme != "secret":
         raise ValueError(
             f"Invalid secret scheme '{uri.scheme}:' (only 'secret:' is allowed)"
         )
-    return _normalize_uri(uri, username, cluster_name, org_name)
+    return _normalize_uri(uri, project_name, cluster_name, org_name)
 
 
 def normalize_disk_uri(
-    uri: URL, username: str, cluster_name: str, org_name: Optional[str]
+    uri: URL, project_name: str, cluster_name: str, org_name: Optional[str]
 ) -> URL:
     """Normalize disk url."""
     if uri.scheme != "disk":
         raise ValueError(
             f"Invalid disk scheme '{uri.scheme}:' (only 'disk:' is allowed)"
         )
-    return _normalize_uri(uri, username, cluster_name, org_name)
+    return _normalize_uri(uri, project_name, cluster_name, org_name)
 
 
 def _normalize_uri(
-    uri: URL, username: str, cluster_name: str, org_name: Optional[str]
+    uri: URL, project_name: str, cluster_name: str, org_name: Optional[str]
 ) -> URL:
-    """Normalize all other user-bound URI's like jobs, storage, images, etc."""
+    """Normalize all other project-bound URI's like jobs, storage, images, etc."""
     _check_uri(uri)
     path = uri.path
     if (uri.host or path.lstrip("/")).startswith("~"):
         raise ValueError(f"Cannot expand user for {uri}")
     if not uri.host:
         if uri.scheme in CLUSTER_SCHEMES:
             host = cluster_name
             if path.startswith("/"):
                 path = path.lstrip("/")
             else:
-                path = f"{username}/{path}" if path else username
+                path = f"{project_name}/{path}" if path else project_name
             if org_name is not None:
                 path = f"{org_name}/{path}"
         else:
             raise ValueError(f"Absolute URI is required for scheme {uri.scheme}")
         uri = URL.build(scheme=uri.scheme, host=host, path="/" + path)
 
     return uri
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_users.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_users.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_utils.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk/_version_utils.py` & `neuro-sdk-23.7.0/src/neuro_sdk/_version_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk.egg-info/PKG-INFO` & `neuro-sdk-23.7.0/src/neuro_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-sdk
-Version: 23.2.0
+Version: 23.7.0
 Summary: Neu.ro SDK
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `neuro-sdk-23.2.0/src/neuro_sdk.egg-info/SOURCES.txt` & `neuro-sdk-23.7.0/src/neuro_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/__init__.py` & `neuro-sdk-23.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/conftest.py` & `neuro-sdk-23.7.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Callable, Dict, Optional
 
 import aiohttp
 import pytest
 from jose import jwt
 from yarl import URL
 
-from neuro_sdk import Client, Cluster, PluginManager, Preset, __version__
+from neuro_sdk import Client, Cluster, PluginManager, Preset, Project, __version__
 from neuro_sdk._config import _AuthConfig, _AuthToken, _ConfigData, _save
 from neuro_sdk._tracing import _make_trace_config
 
 
 @pytest.fixture
 def token() -> str:
     return jwt.encode({"identity": "user"}, "secret", algorithm="HS256")
@@ -86,17 +86,19 @@
 ) -> Callable[..., Client]:
     def go(
         url_str: str,
         *,
         registry_url: str = "https://registry-dev.neu.ro",
         trace_id: str = "bd7a977555f6b982",
         clusters: Optional[Dict[str, Cluster]] = None,
+        projects: Optional[Dict[Project.Key, Project]] = None,
         token_url: Optional[URL] = None,
         plugin_manager: Optional[PluginManager] = None,
         org_name: Optional[str] = None,
+        project_name: Optional[str] = None,
         **kwargs: Any,
     ) -> Client:
         url = URL(url_str)
         if clusters is None:
             cluster_config = Cluster(
                 registry_url=URL(registry_url),
                 monitoring_url=(url / "jobs"),
@@ -149,14 +151,33 @@
                 name="another",
                 orgs=[None, "some_org"],
             )
             clusters = {
                 cluster_config.name: cluster_config,
                 cluster2_config.name: cluster2_config,
             }
+        if projects is None:
+            projects = {}
+            for cluster in clusters.values():
+                project = Project(
+                    cluster_name=cluster.name,
+                    org_name=cluster.orgs[0],
+                    name="test-project",
+                    role="owner",
+                )
+                project_other = Project(
+                    cluster_name=cluster.name,
+                    org_name=cluster.orgs[0],
+                    name="other-test-project",
+                    role="owner",
+                )
+                projects.update(
+                    {project.key: project, project_other.key: project_other}
+                )
+            project_name = "test-project"
         if token_url is not None:
             real_auth_config = replace(auth_config, token_url=token_url)
         else:
             real_auth_config = auth_config
         if "admin_url" not in kwargs:
             admin_url = URL(url) / ".." / ".." / "apis" / "admin" / "v1"
         else:
@@ -173,15 +194,17 @@
             auth_config=real_auth_config,
             auth_token=_AuthToken.create_non_expiring(token),
             url=URL(url),
             admin_url=admin_url,
             version=__version__,
             cluster_name=cluster_name,
             org_name=org_name,
+            project_name=project_name,
             clusters=clusters,
+            projects=projects,
         )
         config_dir = tmp_path / ".neuro"
         _save(config, config_dir)
         session = aiohttp.ClientSession(trace_configs=[_make_trace_config()])
         return Client._create(session, config_dir, trace_id, None, plugin_manager)
 
     return go
```

### Comparing `neuro-sdk-23.2.0/tests/data/file.txt` & `neuro-sdk-23.7.0/tests/data/file.txt`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_admin.py` & `neuro-sdk-23.7.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_blob_storage.py` & `neuro-sdk-23.7.0/tests/test_blob_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         name="test-bucket",
         cluster_name="test-cluster",
         owner="test-user",
         created_at=datetime.now(timezone.utc),
         provider=Bucket.Provider.AWS,
         imported=False,
         org_name=None,
+        project_name="test-project",
     )
 
 
 @pytest.fixture()
 def mock_bucket_provider(mock_bucket: Bucket) -> MockBucketProvider:
     return MockBucketProvider(mock_bucket)
```

### Comparing `neuro-sdk-23.2.0/tests/test_bucket_persistent_credentials.py` & `neuro-sdk-23.7.0/tests/test_bucket_persistent_credentials.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_buckets.py` & `neuro-sdk-23.7.0/tests/test_buckets.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,23 +24,25 @@
                     "id": "bucket-1",
                     "owner": "user",
                     "name": None,
                     "provider": "aws",
                     "created_at": created_at.isoformat(),
                     "imported": False,
                     "org_name": None,
+                    "project_name": "test-project",
                 },
                 {
                     "id": "bucket-2",
                     "owner": "user",
                     "name": "test-bucket",
                     "provider": "aws",
                     "created_at": created_at.isoformat(),
                     "imported": True,
                     "org_name": "test-org",
+                    "project_name": "test-project",
                 },
             ]
         )
 
     app = web.Application()
     app.router.add_get("/buckets/buckets", handler)
 
@@ -59,24 +61,26 @@
             owner="user",
             cluster_name=cluster_config.name,
             name=None,
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-2",
             owner="user",
             cluster_name=cluster_config.name,
             name="test-bucket",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=True,
             org_name="test-org",
+            project_name="test-project",
         ),
     ]
 
 
 async def test_add(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
@@ -85,22 +89,24 @@
     created_at = datetime.now()
 
     async def handler(request: web.Request) -> web.Response:
         data = await request.json()
         assert data == {
             "name": "test-bucket",
             "org_name": None,
+            "project_name": "test-project",
         }
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "test-bucket",
                 "created_at": created_at.isoformat(),
                 "provider": "aws",
+                "project_name": "test-project",
             }
         )
 
     app = web.Application()
     app.router.add_post("/buckets/buckets", handler)
 
     srv = await aiohttp_server(app)
@@ -112,14 +118,15 @@
             owner="user",
             cluster_name=cluster_config.name,
             name="test-bucket",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         )
 
 
 async def test_add_with_org(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_config: Cluster,
@@ -127,23 +134,25 @@
     created_at = datetime.now()
 
     async def handler(request: web.Request) -> web.Response:
         data = await request.json()
         assert data == {
             "name": "test-bucket",
             "org_name": "test-org",
+            "project_name": "test-project",
         }
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "test-bucket",
                 "created_at": created_at.isoformat(),
                 "provider": "aws",
                 "org_name": "test-org",
+                "project_name": "test-project",
             }
         )
 
     app = web.Application()
     app.router.add_post("/buckets/buckets", handler)
 
     srv = await aiohttp_server(app)
@@ -155,14 +164,15 @@
             owner="user",
             cluster_name=cluster_config.name,
             name="test-bucket",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name="test-org",
+            project_name="test-project",
         )
 
 
 async def test_import(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_config: Cluster,
@@ -173,23 +183,25 @@
         data = await request.json()
         assert data == {
             "name": "test-bucket",
             "provider": "aws",
             "provider_bucket_name": "test-external",
             "credentials": {"key": "value"},
             "org_name": None,
+            "project_name": "test-project",
         }
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "test-bucket",
                 "created_at": created_at.isoformat(),
                 "provider": "aws",
                 "imported": True,
+                "project_name": "test-project",
             }
         )
 
     app = web.Application()
     app.router.add_post("/buckets/buckets/import/external", handler)
 
     srv = await aiohttp_server(app)
@@ -206,14 +218,15 @@
             owner="user",
             cluster_name=cluster_config.name,
             name="test-bucket",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=True,
             org_name=None,
+            project_name="test-project",
         )
 
 
 async def test_import_with_org(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_config: Cluster,
@@ -224,24 +237,26 @@
         data = await request.json()
         assert data == {
             "name": "test-bucket",
             "provider": "aws",
             "provider_bucket_name": "test-external",
             "credentials": {"key": "value"},
             "org_name": "test-org",
+            "project_name": "test-project",
         }
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "test-bucket",
                 "created_at": created_at.isoformat(),
                 "provider": "aws",
                 "imported": True,
                 "org_name": "test-org",
+                "project_name": "test-project",
             }
         )
 
     app = web.Application()
     app.router.add_post("/buckets/buckets/import/external", handler)
 
     srv = await aiohttp_server(app)
@@ -249,24 +264,26 @@
     async with make_client(srv.make_url("/")) as client:
         bucket = await client.buckets.import_external(
             provider=Bucket.Provider.AWS,
             provider_bucket_name="test-external",
             credentials={"key": "value"},
             name="test-bucket",
             org_name="test-org",
+            project_name="test-project",
         )
         assert bucket == Bucket(
             id="bucket-1",
             owner="user",
             cluster_name=cluster_config.name,
             name="test-bucket",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=True,
             org_name="test-org",
+            project_name="test-project",
         )
 
 
 async def test_get(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_config: Cluster,
@@ -276,14 +293,15 @@
     async def handler(request: web.Request) -> web.Response:
         assert request.match_info["key"] == "name"
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "name",
+                "project_name": "test-project",
                 "provider": "aws",
                 "created_at": created_at.isoformat(),
             }
         )
 
     app = web.Application()
     app.router.add_get("/buckets/buckets/{key}", handler)
@@ -297,14 +315,15 @@
             owner="user",
             cluster_name=cluster_config.name,
             name="name",
             created_at=created_at,
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         )
 
 
 async def test_set_public(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_config: Cluster,
@@ -316,14 +335,15 @@
         data = await request.json()
         assert data == {"public": True}
         return web.json_response(
             {
                 "id": "bucket-1",
                 "owner": "user",
                 "name": "name",
+                "project_name": "test-project",
                 "provider": "aws",
                 "created_at": created_at.isoformat(),
                 "public": True,
             }
         )
 
     app = web.Application()
```

### Comparing `neuro-sdk-23.2.0/tests/test_client.py` & `neuro-sdk-23.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_clusters.py` & `neuro-sdk-23.7.0/tests/test_clusters.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_config.py` & `neuro-sdk-23.7.0/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,23 @@
 from urllib.parse import parse_qsl
 
 import pytest
 import toml
 from aiohttp import web
 from yarl import URL
 
-from neuro_sdk import Client, Cluster, ConfigError, ConfigScope, PluginManager, Preset
+from neuro_sdk import (
+    Client,
+    Cluster,
+    ConfigError,
+    ConfigScope,
+    PluginManager,
+    Preset,
+    Project,
+)
 from neuro_sdk._config import (
     _check_sections,
     _merge_user_configs,
     _validate_user_config,
 )
 from neuro_sdk._login import _AuthToken
 
@@ -403,14 +411,50 @@
                 disks_url=srv.make_url("/disk2"),
                 buckets_url=srv.make_url("/buckets2"),
                 presets=mock.ANY,
             ),
         }
 
 
+async def test_project_name(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    app = web.Application()
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        assert client.config.project_name == "test-project"
+
+
+async def test_projects(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    app = web.Application()
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        projects = {}
+        for cluster in client.config.clusters.values():
+            project = Project(
+                cluster_name=cluster.name,
+                org_name=cluster.orgs[0],
+                name="test-project",
+                role="owner",
+            )
+            project_other = Project(
+                cluster_name=cluster.name,
+                org_name=cluster.orgs[0],
+                name="other-test-project",
+                role="owner",
+            )
+            projects.update({project.key: project, project_other.key: project_other})
+
+        assert dict(client.config.projects) == projects
+
+
 async def test_fetch(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     admin_url = "https://admin-dev.neu.ro"
     registry_url = "https://registry2-dev.neu.ro"
     storage_url = "https://storage2-dev.neu.ro"
     users_url = "https://users2-dev.neu.ro"
@@ -452,14 +496,22 @@
                         "credits_per_hour": "10",
                         "cpu": 2,
                         "memory": 2 * 2**30,
                     }
                 ],
             }
         ],
+        "projects": [
+            {
+                "name": "some-project",
+                "cluster_name": "default",
+                "org_name": None,
+                "role": "admin",
+            }
+        ],
     }
 
     async def handler(request: web.Request) -> web.Response:
         return web.json_response(JSON)
 
     app = web.Application()
     app.add_routes([web.get("/config", handler)])
@@ -489,14 +541,22 @@
                         tpu_type=None,
                         tpu_software_version=None,
                     )
                 },
             )
         }
 
+        project = Project(
+            name="some-project",
+            cluster_name="default",
+            org_name=None,
+            role="admin",
+        )
+        assert client.config.projects == {project.key: project}
+
 
 async def test_fetch_without_admin_url(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     registry_url = "https://registry2-dev.neu.ro"
     storage_url = "https://storage2-dev.neu.ro"
     users_url = "https://users2-dev.neu.ro"
@@ -670,25 +730,85 @@
         assert client.config.cluster_name == "default"
         assert client.config.org_name == "test-org"
         await client.config.switch_cluster("third")
         assert client.config.cluster_name == "third"
         assert client.config.org_name == "a-org"
 
 
+async def test_switch_cluster_keep_project(make_client: _MakeClient) -> None:
+    async with make_client("https://example.org") as client:
+        assert client.config.cluster_name == "default"
+        assert client.config.project_name == "test-project"
+        await client.config.switch_cluster("another")
+        assert client.config.cluster_name == "another"
+        assert client.config.project_name == "test-project"
+
+
+async def test_switch_cluster_cant_keep_project_use_none(
+    make_client: _MakeClient, multiple_clusters_config: Dict[str, Cluster]
+) -> None:
+    async with make_client(
+        "https://example.org", clusters=multiple_clusters_config
+    ) as client:
+        assert client.config.cluster_name == "default"
+        assert client.config.project_name == "test-project"
+        await client.config.switch_cluster("another")
+        assert client.config.cluster_name == "another"
+        assert client.config.project_name is None
+
+
+async def test_switch_cluster_cant_keep_project_use_alphabetical(
+    make_client: _MakeClient,
+) -> None:
+    async with make_client("https://example.org") as client:
+        assert client.config.cluster_name == "default"
+        assert client.config.project_name == "test-project"
+        await client.config.switch_cluster("another")
+        await client.config.switch_org("some_org")
+        assert client.config.cluster_name == "another"
+        assert client.config.project_name is None
+        await client.config.switch_cluster("default")
+        assert client.config.cluster_name == "default"
+        assert client.config.project_name == "other-test-project"
+
+
 async def test_switch_org(
     make_client: _MakeClient, multiple_clusters_config: Dict[str, Cluster]
 ) -> None:
     async with make_client(
         "https://example.org", clusters=multiple_clusters_config
     ) as client:
         assert client.config.org_name is None
         await client.config.switch_org("test-org")
         assert client.config.org_name == "test-org"
 
 
+async def test_switch_org_keep_project_use_none(make_client: _MakeClient) -> None:
+    async with make_client("https://example.org") as client:
+        await client.config.switch_cluster("another")
+        assert client.config.org_name is None
+        assert client.config.project_name == "test-project"
+        await client.config.switch_org("some_org")
+        assert client.config.org_name == "some_org"
+        assert client.config.project_name is None
+
+
+async def test_switch_org_keep_project_use_alphabetical(
+    make_client: _MakeClient,
+) -> None:
+    async with make_client("https://example.org") as client:
+        await client.config.switch_cluster("another")
+        await client.config.switch_org("some_org")
+        assert client.config.org_name == "some_org"
+        assert client.config.project_name is None
+        await client.config.switch_org(None)
+        assert client.config.org_name is None
+        assert client.config.project_name == "other-test-project"
+
+
 async def test_switch_clusters_unknown(make_client: _MakeClient) -> None:
     async with make_client("https://example.org") as client:
         assert client.config.cluster_name == "default"
         with pytest.raises(RuntimeError, match="Cluster unknown doesn't exist"):
             await client.config.switch_cluster("unknown")
         assert client.config.cluster_name == "default"
 
@@ -773,14 +893,49 @@
         local_dir.mkdir(parents=True, exist_ok=True)
         monkeypatch.chdir(local_dir)
         local_conf = proj_dir / ".neuro.toml"
         local_conf.write_text(toml.dumps({"job": {"org-name": "NO_ORG"}}))
         assert client.config.org_name is None
 
 
+async def test_switch_project(make_client: _MakeClient) -> None:
+    async with make_client("https://example.org") as client:
+        assert client.config.project_name == "test-project"
+        await client.config.switch_project("other-test-project")
+        assert client.config.project_name == "other-test-project"
+
+
+async def test_switch_project_unknown(make_client: _MakeClient) -> None:
+    async with make_client("https://example.org") as client:
+        assert client.config.project_name == "test-project"
+        with pytest.raises(RuntimeError, match="Project unknown doesn't exist"):
+            await client.config.switch_project("unknown")
+        assert client.config.project_name == "test-project"
+
+
+async def test_switch_project_local(
+    monkeypatch: Any, tmp_path: Path, make_client: _MakeClient
+) -> None:
+    plugin_manager = PluginManager()
+    plugin_manager.config.define_str("job", "project-name", scope=ConfigScope.LOCAL)
+    async with make_client(
+        "https://example.org", plugin_manager=plugin_manager
+    ) as client:
+        proj_dir = tmp_path / "project"
+        local_dir = proj_dir / "folder"
+        local_dir.mkdir(parents=True, exist_ok=True)
+        monkeypatch.chdir(local_dir)
+        local_conf = proj_dir / ".neuro.toml"
+        local_conf.write_text(toml.dumps({"job": {"project-name": "test-project"}}))
+        assert client.config.project_name == "test-project"
+        with pytest.raises(RuntimeError, match=r"\.neuro\.toml"):
+            await client.config.switch_project("test-project")
+        assert client.config.project_name == "test-project"
+
+
 async def test_check_server_mismatch_clusters(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     # the test returns the same as for valid answer but the cluster name is different
 
     admin_url = "https://admin-dev.neu.ro"
     registry_url = "https://registry2-dev.neu.ro"
@@ -833,15 +988,14 @@
         return web.json_response(JSON)
 
     app = web.Application()
     app.add_routes([web.get("/config", handler)])
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-
         # Set expired version
         client.config._config_data.__dict__["version"] = "18.1.1"
 
         with pytest.raises(ConfigError, match="Neuro Platform CLI was updated"):
             await client.config.check_server()
 
 
@@ -900,15 +1054,14 @@
         return web.json_response(JSON)
 
     app = web.Application()
     app.add_routes([web.get("/config", handler)])
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-
         # Set expired version
         client.config._config_data.__dict__["version"] = "18.1.1"
 
         with pytest.raises(ConfigError, match="Neuro Platform CLI was updated"):
             await client.config.check_server()
 
 
@@ -933,15 +1086,14 @@
     app = web.Application()
     app.add_routes([web.post("/oauth/token", handler)])
     srv = await aiohttp_server(app)
 
     async with make_client(
         srv.make_url("/"), token_url=srv.make_url("/oauth/token")
     ) as client:
-
         token1 = await client.config.token()
 
         # Set expired version to far ago
         client.config._config_data.__dict__["auth_token"] = replace(
             _AuthToken.create(token, 3600, "REFRESH_TOKEN"), expiration_time=200
         )
```

### Comparing `neuro-sdk-23.2.0/tests/test_config_factory.py` & `neuro-sdk-23.7.0/tests/test_config_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import base64
 import json
 import os
 import sys
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Awaitable, Callable, Dict
+from typing import Any, Awaitable, Callable, Dict, Optional
 from unittest import mock
 
 import aiohttp
 import pytest
 from aiohttp import web
 from aiohttp.test_utils import TestServer as _TestServer
 from jose import jws
@@ -17,14 +17,15 @@
 
 from neuro_sdk import (
     PASS_CONFIG_ENV_NAME,
     AuthError,
     Cluster,
     ConfigError,
     Factory,
+    Project,
     __version__,
 )
 from neuro_sdk._config import _AuthConfig, _AuthToken, _ConfigData
 from neuro_sdk._login import JWT_STANDALONE_SECRET
 
 from tests import _TestServerFactory
 
@@ -46,25 +47,31 @@
 ) -> Path:
     config_path = tmp_home / ".neuro"
     _create_config(config_path, token, auth_config, cluster_config)
     return config_path
 
 
 def _create_config(
-    nmrc_path: Path, token: str, auth_config: _AuthConfig, cluster_config: Cluster
+    nmrc_path: Path,
+    token: str,
+    auth_config: _AuthConfig,
+    cluster_config: Cluster,
+    project: Optional[Project] = None,
 ) -> str:
     config = _ConfigData(
         auth_config=auth_config,
         auth_token=_AuthToken.create_non_expiring(token),
         url=URL("https://dev.neu.ro/api/v1"),
         admin_url=URL("https://dev.neu.ro/apis/admin/v1"),
         version=__version__,
         cluster_name=cluster_config.name,
         org_name=cluster_config.orgs[0],
         clusters={cluster_config.name: cluster_config},
+        projects={project.key: project} if project else {},
+        project_name=project.name if project else None,
     )
     Factory(nmrc_path)._save(config)
     assert nmrc_path.exists()
     return token
 
 
 @dataclass
@@ -140,21 +147,31 @@
                             "name": "cpu-large",
                             "credits_per_hour": "10",
                             "cpu": 3,
                             "memory": 14 * 2**30,
                         },
                     ],
                 }
+                project_config: Dict[str, Any] = {
+                    "cluster_name": "default",
+                    "org_name": None,
+                    "name": "default",
+                    "role": "owner",
+                }
                 config_json.update(
                     {
                         "authorized": True,
                         "clusters": [
                             {**cluster_config, "name": "default"},
                             {**cluster_config, "name": "default2"},
                         ],
+                        "projects": [
+                            project_config,
+                            {**project_config, "name": "default2"},
+                        ],
                     }
                 )
             else:
                 config_json["authorized"] = False
             return web.json_response(config_json)
 
         async def show_code(request: web.Request) -> web.Response:
@@ -228,14 +245,30 @@
         await client.close()
         assert len(client.presets) > 0
         assert not client.presets["cpu-large"].scheduler_enabled
         assert not client.presets["cpu-large"].preemptible_node
         assert client.presets["cpu-large-p"].scheduler_enabled
         assert client.presets["cpu-large-p"].preemptible_node
 
+    async def test_project_serialization(
+        self,
+        tmp_home: Path,
+        token: str,
+        auth_config: _AuthConfig,
+        cluster_config: Cluster,
+    ) -> None:
+        project = Project(
+            cluster_name="default", org_name=None, name="test-project", role="owner"
+        )
+        _create_config(tmp_home / ".neuro", token, auth_config, cluster_config, project)
+        client = await Factory().get()
+        await client.close()
+        assert client.config.project_name == project.name
+        assert dict(client.config.projects) == {project.key: project}
+
     async def test_shorten_path(
         self,
         tmp_home: Path,
         token: str,
         auth_config: _AuthConfig,
         cluster_config: Cluster,
     ) -> None:
@@ -330,31 +363,41 @@
             )
         nmrc_path = tmp_home / ".neuro"
         assert not Path(nmrc_path).exists(), "Config file not written after login "
 
 
 class TestLoginPassedConfig:
     @pytest.fixture()
-    def make_conf_data(self, mock_for_login: _TestServer) -> Callable[[str], str]:
-        def _make_config(token: str) -> str:
+    def make_conf_data(
+        self, mock_for_login: _TestServer
+    ) -> Callable[[str, Optional[str], Optional[str]], str]:
+        def _make_config(
+            token: str,
+            project_name: Optional[str] = "default",
+            org_name: Optional[str] = None,
+        ) -> str:
             data = {
                 "token": token,
                 "cluster": "default",
                 "url": str(mock_for_login.make_url("/")),
+                "org_name": org_name,
+                "project_name": project_name,
             }
             return base64.b64encode(json.dumps(data).encode()).decode()
 
         return _make_config
 
     @pytest.fixture()
     def set_conf_to_env(
-        self, monkeypatch: Any, make_conf_data: Callable[[str], str]
+        self,
+        monkeypatch: Any,
+        make_conf_data: Callable[[str, Optional[str], Optional[str]], str],
     ) -> Callable[[str], None]:
         def _set_env(token: str) -> None:
-            config_data = make_conf_data(token)
+            config_data = make_conf_data(token)  # type: ignore
             monkeypatch.setenv(PASS_CONFIG_ENV_NAME, config_data)
 
         return _set_env
 
     async def test_login_with_passed_config_already_logged(
         self, set_conf_to_env: Callable[[str], None], config_dir: Path
     ) -> None:
@@ -385,17 +428,19 @@
     ) -> None:
         set_conf_to_env("tokenstr")
         await Factory().login_with_passed_config()
         nmrc_path = tmp_home / ".neuro"
         assert Path(nmrc_path).exists(), "Config file not written after login "
 
     async def test_normal_login_direct_token(
-        self, tmp_home: Path, make_conf_data: Callable[[str], str]
+        self,
+        tmp_home: Path,
+        make_conf_data: Callable[[str, Optional[str], Optional[str]], str],
     ) -> None:
-        token_data = make_conf_data("tokenstr")
+        token_data = make_conf_data("tokenstr")  # type: ignore
         await Factory().login_with_passed_config(token_data)
         nmrc_path = tmp_home / ".neuro"
         assert Path(nmrc_path).exists(), "Config file not written after login "
 
     async def test_incorrect_token(
         self, tmp_home: Path, set_conf_to_env: Callable[[str], None]
     ) -> None:
@@ -422,14 +467,29 @@
         monkeypatch: Any,
     ) -> None:
         with pytest.raises(ConfigError):
             await Factory().login_with_passed_config()
         nmrc_path = tmp_home / ".neuro"
         assert not Path(nmrc_path).exists(), "Config file written after bad login "
 
+    async def test_login_project_set(
+        self,
+        tmp_home: Path,
+        monkeypatch: Any,
+        make_conf_data: Callable[[str, Optional[str]], str],
+    ) -> None:
+        pass_cfg_data = make_conf_data("tokenstr", "default2")
+        monkeypatch.setenv(PASS_CONFIG_ENV_NAME, pass_cfg_data)
+        client = await Factory().get()
+        await client.close()
+        nmrc_path = tmp_home / ".neuro"
+        assert Path(nmrc_path).exists(), "Config file not written after login "
+        assert client.config.project_name == "default2"
+        assert not client.config.org_name
+
 
 class TestHeadlessLogin:
     async def test_login_headless_already_logged(self, config_dir: Path) -> None:
         async def get_auth_code_cb(url: URL) -> str:
             return ""
 
         with pytest.raises(ConfigError, match=r"already exists"):
```

### Comparing `neuro-sdk-23.2.0/tests/test_core.py` & `neuro-sdk-23.7.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_file_filter.py` & `neuro-sdk-23.7.0/tests/test_file_filter.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_file_utils.py` & `neuro-sdk-23.7.0/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_images.py` & `neuro-sdk-23.7.0/tests/test_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,37 +31,37 @@
 def patch_docker_host() -> Iterator[None]:
     with mock.patch.dict(os.environ, values={"DOCKER_HOST": "http://localhost:45678"}):
         yield
 
 
 class TestImageParser:
     parser = _ImageNameParser(
-        default_user="alice",
         default_cluster="default",
         default_org=None,
+        default_project="test-project",
         registry_urls={
             "default": URL("https://reg.neu.ro"),
             "another": URL("https://example.org"),
         },
     )
     parser_with_org = _ImageNameParser(
-        default_user="alice",
         default_cluster="default",
         default_org="test-org",
+        default_project="test-project",
         registry_urls={
             "default": URL("https://reg.neu.ro"),
             "another": URL("https://example.org"),
         },
     )
 
     @pytest.mark.parametrize(
         "image",
         [
-            "image://default/me/ubuntu:v10.04",
-            "image://another/me/ubuntu:v10.04",
+            "image://default/project/ubuntu:v10.04",
+            "image://another/project/ubuntu:v10.04",
             "image:ubuntu:v10.04",
             "image:///ubuntu:v10.04",
             "image:ubuntu:v10.04",
             "ubuntu:v10.04",
         ],
     )
     def test_has_tag_ok(self, image: str) -> None:
@@ -106,45 +106,45 @@
 
     @pytest.mark.parametrize(
         "registry_url",
         ["http://reg.neu.ro", "https://reg.neu.ro", "https://reg.neu.ro/bla/bla"],
     )
     def test_get_registry_hostname(self, registry_url: str) -> None:
         parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL(registry_url)},
         )
         assert parser._registries == {"test-cluster": "reg.neu.ro"}
 
     @pytest.mark.parametrize(
         "registry_url", ["http://reg.neu.ro:5000", "http://reg.neu.ro:5000/bla/bla"]
     )
     def test_get_registry_hostname_with_port(self, registry_url: str) -> None:
         parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL(registry_url)},
         )
         assert parser._registries == {"test-cluster": "reg.neu.ro:5000"}
 
     @pytest.mark.parametrize(
         "registry_url",
         ["", "reg.neu.ro", "reg.neu.ro:5000", "https://", "https:///bla/bla"],
     )
     def test_get_registry_hostname__bad_url_empty_hostname(
         self, registry_url: str
     ) -> None:
         with pytest.raises(ValueError, match="Empty hostname in registry URL"):
             _ImageNameParser(
-                default_user="alice",
                 default_cluster="test-cluster",
                 default_org=None,
+                default_project="test-project",
                 registry_urls={"test-cluster": URL(registry_url)},
             )
 
     def test_split_image_name_no_tag(self) -> None:
         splitted = self.parser._split_image_name("ubuntu", "latest")
         assert splitted == ("ubuntu", "latest")
 
@@ -185,16 +185,16 @@
     # public method: parse_local
 
     @pytest.mark.parametrize(
         "url",
         [
             "image://",
             "image:///",
-            "image://default/bob",
-            "image://default/bob/",
+            "image://default/project",
+            "image://default/project/",
         ],
     )
     def test_parse_as_neuro_image__no_image_name(self, url: str) -> None:
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_local_image_empty_fail(self) -> None:
@@ -241,60 +241,60 @@
             self.parser.parse_as_local_image(image)
 
     # public method: parse_remote
 
     @pytest.mark.parametrize(
         "url",
         [
-            "image://default/bob/ubuntu:v10.04?key=value",
-            "image://default/bob/ubuntu?key=value",
+            "image://default/project/ubuntu:v10.04?key=value",
+            "image://default/project/ubuntu?key=value",
             "image:///ubuntu?key=value",
             "image:ubuntu?key=value",
             "image:5000?key=value",
-            "image://default/bob/ubuntu:v10.04?",
+            "image://default/project/ubuntu:v10.04?",
         ],
     )
     def test_parse_as_neuro_image__with_query__fail(self, url: str) -> None:
         with pytest.raises(ValueError, match="Query part is not allowed in image URI"):
             self.parser.parse_as_neuro_image(url)
 
     @pytest.mark.parametrize(
         "url",
         [
-            "image://default/bob/ubuntu:v10.04#fragment",
-            "image://default/bob/ubuntu#fragment",
+            "image://default/project/ubuntu:v10.04#fragment",
+            "image://default/project/ubuntu#fragment",
             "image:///ubuntu#fragment",
             "image:ubuntu#fragment",
             "image:5000#fragment",
-            "image://default/bob/ubuntu:v10.04#",
+            "image://default/project/ubuntu:v10.04#",
         ],
     )
     def test_parse_as_neuro_image__with_fragment__fail(self, url: str) -> None:
         with pytest.raises(
             ValueError, match="Fragment part is not allowed in image URI"
         ):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_neuro_image__with_user__fail(self) -> None:
-        url = "image://user@default/bob/ubuntu"
+        url = "image://user@default/project/ubuntu"
         with pytest.raises(ValueError, match="User is not allowed in image URI"):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_neuro_image__with_password__fail(self) -> None:
-        url = "image://:password@default/bob/ubuntu"
+        url = "image://:password@default/project/ubuntu"
         with pytest.raises(ValueError, match="Password is not allowed in image URI"):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_neuro_image__with_empty_password__fail(self) -> None:
-        url = "image://:@default/bob/ubuntu"
+        url = "image://:@default/project/ubuntu"
         with pytest.raises(ValueError, match="Password is not allowed in image URI"):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_neuro_image__with_port__fail(self) -> None:
-        url = "image://default:443/bob/ubuntu"
+        url = "image://default:443/project/ubuntu"
         with pytest.raises(ValueError, match="Port is not allowed in image URI"):
             self.parser.parse_as_neuro_image(url)
 
     def test_parse_as_neuro_image_empty__fail(self) -> None:
         image = ""
         with pytest.raises(ValueError, match="empty image name"):
             self.parser.parse_as_neuro_image(image)
@@ -322,416 +322,418 @@
         image = "http://ubuntu"
         with pytest.raises(
             ValueError, match="scheme 'image:' is required for remote images"
         ):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_default_org_no_org(self) -> None:
-        image = "image://another/bob/ubuntu:v10.04"
+        image = "image://another/project/ubuntu:v10.04"
         parsed = self.parser_with_org.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_default_org_no_cluster_no_org(self) -> None:
-        image = "image:/bob/ubuntu:v10.04"
+        image = "image:/project/ubuntu:v10.04"
         parsed = self.parser_with_org.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name="test-org",
+            project_name="project",
         )
 
-    def test_parse_as_neuro_image_with_default_org_no_cluster_no_user(self) -> None:
+    def test_parse_as_neuro_image_with_default_org_no_cluster_no_project(self) -> None:
         image = "image:ubuntu:v10.04"
         parsed = self.parser_with_org.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name="test-org",
+            project_name="test-project",
         )
 
     def test_parse_as_neuro_image_with_default_org_same_org(self) -> None:
-        image = "image://another/test-org/bob/ubuntu:v10.04"
+        image = "image://another/test-org/project/ubuntu:v10.04"
         parsed = self.parser_with_org.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name="test-org",
+            project_name="project",
         )
 
     # XXX: Ambigious URI
     def test_parse_as_neuro_image_with_default_org_other_org(self) -> None:
-        image = "image://another/org/bob/ubuntu:v10.04"
+        image = "image://another/org/project/ubuntu:v10.04"
         parsed = self.parser_with_org.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
-            name="bob/ubuntu",
+            name="project/ubuntu",
             tag="v10.04",
-            owner="org",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="org",
         )
 
     # XXX: Ambigious URI
     def test_parse_as_neuro_image_without_default_org_with_org(self) -> None:
-        image = "image://another/test-org/bob/ubuntu:v10.04"
+        image = "image://another/test-org/project/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
-            name="bob/ubuntu",
+            name="project/ubuntu",
             tag="v10.04",
-            owner="test-org",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="test-org",
         )
 
-    def test_parse_as_neuro_image_with_scheme_with_cluster_with_user_with_tag(
+    def test_parse_as_neuro_image_with_scheme_with_cluster_with_project_with_tag(
         self,
     ) -> None:
-        image = "image://another/bob/ubuntu:v10.04"
+        image = "image://another/project/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_with_cluster_with_user_with_tag_2(
+    def test_parse_as_neuro_image_with_scheme_with_cluster_with_project_with_tag_2(
         self,
     ) -> None:
-        image = "image://another/bob/library/ubuntu:v10.04"
+        image = "image://another/project/library/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_with_cluster_with_user_no_tag(
+    def test_parse_as_neuro_image_with_scheme_with_cluster_with_project_no_tag(
         self,
     ) -> None:
-        image = "image://another/bob/ubuntu"
+        image = "image://another/project/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_with_cluster_with_user_no_tag_2(
+    def test_parse_as_neuro_image_with_scheme_with_cluster_with_project_no_tag_2(
         self,
     ) -> None:
-        image = "image://another/bob/library/ubuntu"
+        image = "image://another/project/library/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="another",
             registry="example.org",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_unknown_cluster(self) -> None:
-        image = "image://unknown-cluster/bob/ubuntu"
+        image = "image://unknown-cluster/project/ubuntu"
         with pytest.raises(
             RuntimeError,
             match="Cluster unknown-cluster doesn't exist "
             "in a list of available clusters",
         ):
             self.parser.parse_as_neuro_image(image)
 
-    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_user_no_tag(
+    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_project_no_tag(
         self,
     ) -> None:
         image = "image:ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_user_no_tag_2(
+    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_project_no_tag_2(
         self,
     ) -> None:
         image = "image:library/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="latest",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_user_with_tag(
+    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_project_with_tag(
         self,
     ) -> None:
         image = "image:ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_user_with_tag_2(
+    def test_parse_as_neuro_image_with_scheme_no_slash_no_cluster_no_project_with_tag_2(
         self,
     ) -> None:
         image = "image:library/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_no_name_no_tag(
         self,
     ) -> None:
         image = "image:/ubuntu"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_no_tag(self) -> None:
-        image = "image:/bob/ubuntu"
+        image = "image:/project/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_no_tag_2(self) -> None:
-        image = "image:/bob/library/ubuntu"
+        image = "image:/project/library/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_no_name_with_tag(
         self,
     ) -> None:
         image = "image:/ubuntu:v10.04"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_with_tag(self) -> None:
-        image = "image:/bob/ubuntu:v10.04"
+        image = "image:/project/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_1_slash_no_cluster_with_tag_2(
         self,
     ) -> None:
-        image = "image:/bob/library/ubuntu:v10.04"
+        image = "image:/project/library/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
-    def test_parse_as_neuro_image_with_scheme_2_slash_cluster_user_no_name_no_tag_fail(
+    def test_parse_as_neuro_image_with_scheme_2_slash_cluster_proj_no_name_no_tag_fail(
         self,
     ) -> None:
         image = "image://another/ubuntu"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
-    def test_parse_as_neuro_image_with_scheme_2_slash_cluster_no_user_with_tag_fail(
+    def test_parse_as_neuro_image_with_scheme_2_slash_cluster_no_project_with_tag_fail(
         self,
     ) -> None:
         image = "image://ubuntu:v10.04"
         with pytest.raises(ValueError, match="port can't be converted to integer"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_no_name_no_tag(
         self,
     ) -> None:
         image = "image:///ubuntu"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_no_tag(self) -> None:
-        image = "image:///bob/ubuntu"
+        image = "image:///project/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_no_tag_2(self) -> None:
-        image = "image:///bob/library/ubuntu"
+        image = "image:///project/library/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_no_name_with_tag(
         self,
     ) -> None:
         image = "image:///ubuntu:v10.04"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_with_tag(self) -> None:
-        image = "image:///bob/ubuntu:v10.04"
+        image = "image:///project/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_3_slash_no_cluster_with_tag_2(
         self,
     ) -> None:
-        image = "image:///bob/library/ubuntu:v10.04"
+        image = "image:///project/library/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_no_name_with_tag(
         self,
     ) -> None:
         image = "image:////ubuntu:v10.04"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_with_tag(self) -> None:
-        image = "image:////bob/ubuntu:v10.04"
+        image = "image:////project/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_with_tag_2(
         self,
     ) -> None:
-        image = "image:////bob/library/ubuntu:v10.04"
+        image = "image:////project/library/ubuntu:v10.04"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_no_name_no_tag(
         self,
     ) -> None:
         image = "image:////ubuntu"
         with pytest.raises(ValueError, match="no image name specified"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_no_tag(self) -> None:
-        image = "image:////bob/ubuntu"
+        image = "image:////project/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_4_slash_no_cluster_no_tag_2(self) -> None:
-        image = "image:////bob/library/ubuntu"
+        image = "image:////project/library/ubuntu"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="latest",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image_with_scheme_special_chars(self) -> None:
-        image = "image://another/bob/ubuntu%23%252d%3F%C3%9F:v10.04%23%252d%3F%C3%9F"
+        image = (
+            "image://another/project/ubuntu%23%252d%3F%C3%9F:v10.04%23%252d%3F%C3%9F"
+        )
         with pytest.raises(ValueError, match="invalid image name"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_no_scheme_no_slash_no_tag_fail(self) -> None:
         image = "ubuntu"
         with pytest.raises(ValueError, match="scheme 'image:' is required"):
             self.parser.parse_as_neuro_image(image)
@@ -763,38 +765,38 @@
 
     def test_parse_as_neuro_image_no_scheme_3_slash_no_tag_fail(self) -> None:
         image = "something/docker.io/library/ubuntu"
         with pytest.raises(ValueError, match="scheme 'image:' is required"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_with_registry_prefix(self) -> None:
-        image = self.parser.parse_as_neuro_image("reg.neu.ro/user/image:tag")
-        assert str(image) == "image://default/user/image:tag"
+        image = self.parser.parse_as_neuro_image("reg.neu.ro/project/image:tag")
+        assert str(image) == "image://default/project/image:tag"
 
     def test_parse_as_neuro_image_with_registry_prefix_special_chars(self) -> None:
         with pytest.raises(ValueError, match="invalid image name"):
             self.parser.parse_as_neuro_image(
-                "reg.neu.ro/user/image%23%252d%3F%C3%9F:tag%23%252d%3F%C3%9F"
+                "reg.neu.ro/project/image%23%252d%3F%C3%9F:tag%23%252d%3F%C3%9F"
             )
 
     def test_parse_as_neuro_image_no_scheme_3_slash_with_tag_fail(self) -> None:
         image = "something/docker.io/library/ubuntu:v10.04"
         with pytest.raises(ValueError, match="scheme 'image:' is required"):
             self.parser.parse_as_neuro_image(image)
 
     def test_parse_as_neuro_image_allow_tag_false_with_scheme_no_tag(self) -> None:
         image = "image:ubuntu"
         parsed = self.parser.parse_as_neuro_image(image, tag_option=TagOption.DENY)
         assert parsed == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag=None,
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
     def test_parse_as_neuro_image_allow_tag_false_no_scheme_no_tag(self) -> None:
         image = "ubuntu"
         with pytest.raises(ValueError, match="scheme 'image:' is required"):
             self.parser.parse_as_neuro_image(image, tag_option=TagOption.DENY)
 
@@ -814,80 +816,80 @@
         with pytest.raises(ValueError, match="too many tags"):
             self.parser.parse_as_neuro_image(image, tag_option=TagOption.DENY)
 
     def test_convert_to_local_image(self) -> None:
         neuro_image = RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="artem",
             cluster_name="default",
             registry="reg.com",
             org_name=None,
+            project_name="project",
         )
         local_image = self.parser.convert_to_local_image(neuro_image)
         assert local_image == LocalImage(name="ubuntu", tag="latest")
 
     def test_convert_to_neuro_image(self) -> None:
         local_image = LocalImage(name="ubuntu", tag="latest")
         neuro_image = self.parser.convert_to_neuro_image(local_image)
         assert neuro_image == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
-    def test_convert_to_neuro_image_with_defualt_org(self) -> None:
+    def test_convert_to_neuro_image_with_default_org(self) -> None:
         local_image = LocalImage(name="ubuntu", tag="latest")
         neuro_image = self.parser_with_org.convert_to_neuro_image(local_image)
         assert neuro_image == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="latest",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name="test-org",
+            project_name="test-project",
         )
 
     def test_convert_to_neuro_image__neuro_registry(self) -> None:
-        local_image = LocalImage(name="reg.neu.ro/bob/ubuntu", tag="v20.04")
+        local_image = LocalImage(name="reg.neu.ro/project/ubuntu", tag="v20.04")
         neuro_image = self.parser.convert_to_neuro_image(local_image)
         assert neuro_image == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v20.04",
-            owner="bob",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="project",
         )
 
-    def test_convert_to_neuro_image__neuro_registry__no_user(self) -> None:
+    def test_convert_to_neuro_image__neuro_registry__no_project(self) -> None:
         local_image = LocalImage(name="reg.neu.ro/ubuntu", tag="v20.04")
         neuro_image = self.parser.convert_to_neuro_image(local_image)
         assert neuro_image == RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v20.04",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
     def test_convert_to_neuro_image__neuro_registry__no_path(self) -> None:
         local_image = LocalImage(name="reg.neu.ro/", tag="v20.04")
         neuro_image = self.parser.convert_to_neuro_image(local_image)
         assert neuro_image == RemoteImage.new_neuro_image(
             name="reg.neu.ro/",
             tag="v20.04",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
     # corner case 'image:latest'
 
     def test_parse_as_neuro_image__ambiguous_case__fail(self) -> None:
         url = "image:latest"
         with pytest.raises(ValueError, match="ambiguous value"):
@@ -902,175 +904,175 @@
 
     def test_parse_as_neuro_image__numeric_name(self) -> None:
         image = "image:5000"
         parsed = self.parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="5000",
             tag="latest",
-            owner="alice",
             cluster_name="default",
             registry="reg.neu.ro",
             org_name=None,
+            project_name="test-project",
         )
 
     def test_parse_as_local_image__neuro_registry(self) -> None:
-        image = "reg.neu.ro/bob/ubuntu:v10.04"
+        image = "reg.neu.ro/project/ubuntu:v10.04"
         parsed = self.parser.parse_as_local_image(image)
-        assert parsed == LocalImage(name="reg.neu.ro/bob/ubuntu", tag="v10.04")
+        assert parsed == LocalImage(name="reg.neu.ro/project/ubuntu", tag="v10.04")
 
     def test_parse_as_local_image__registry_has_port__neuro_registry(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "localhost:5000/bob/ubuntu:v10.04"
+        image = "localhost:5000/project/ubuntu:v10.04"
         parsed = my_parser.parse_as_local_image(image)
-        assert parsed == LocalImage(name="localhost:5000/bob/ubuntu", tag="v10.04")
+        assert parsed == LocalImage(name="localhost:5000/project/ubuntu", tag="v10.04")
 
     def test_parse_as_neuro_image__registry_has_port__neuro_image(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "image://test-cluster/bob/library/ubuntu:v10.04"
+        image = "image://test-cluster/project/library/ubuntu:v10.04"
         parsed = my_parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="test-cluster",
             registry="localhost:5000",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image__registry_has_port__image_in_good_repo(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "localhost:5000/bob/library/ubuntu:v10.04"
+        image = "localhost:5000/project/library/ubuntu:v10.04"
         parsed = my_parser.parse_as_neuro_image(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="test-cluster",
             registry="localhost:5000",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_as_neuro_image__registry_has_port__image_in_bad_repo(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "localhost:9999/bob/library/ubuntu:v10.04"
+        image = "localhost:9999/project/library/ubuntu:v10.04"
         with pytest.raises(ValueError, match="scheme 'image:' is required"):
             my_parser.parse_as_neuro_image(image)
 
     def test_parse_remote__registry_has_port__neuro_image(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "image://test-cluster/bob/library/ubuntu:v10.04"
+        image = "image://test-cluster/project/library/ubuntu:v10.04"
         parsed = my_parser.parse_remote(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="test-cluster",
             registry="localhost:5000",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_remote__registry_has_port__image_in_good_repo(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "localhost:5000/bob/library/ubuntu:v10.04"
+        image = "localhost:5000/project/library/ubuntu:v10.04"
         parsed = my_parser.parse_remote(image)
         assert parsed == RemoteImage.new_neuro_image(
             name="library/ubuntu",
             tag="v10.04",
-            owner="bob",
             cluster_name="test-cluster",
             registry="localhost:5000",
             org_name=None,
+            project_name="project",
         )
 
     def test_parse_remote__registry_has_port__image_in_other_repo(self) -> None:
         my_parser = _ImageNameParser(
-            default_user="alice",
             default_cluster="test-cluster",
             default_org=None,
+            default_project="test-project",
             registry_urls={"test-cluster": URL("http://localhost:5000")},
         )
-        image = "example.com:9999/bob/library/ubuntu:v10.04"
+        image = "example.com:9999/project/library/ubuntu:v10.04"
         parsed = my_parser.parse_remote(image)
         # NOTE: "owner" is parsed only for images in neuro registry
         assert parsed == RemoteImage.new_external_image(
-            name="bob/library/ubuntu",
+            name="project/library/ubuntu",
             tag="v10.04",
             registry="example.com:9999",
         )
 
 
 class TestRemoteImage:
     def test_as_str_in_neuro_registry_tag_none(self) -> None:
         image = RemoteImage.new_neuro_image(
             name="ubuntu",
             tag=None,
-            owner="me",
             cluster_name="test-cluster",
             org_name=None,
             registry="registry.io",
+            project_name="test-project",
         )
-        assert str(image) == "image://test-cluster/me/ubuntu"
-        assert image.as_docker_url() == "registry.io/me/ubuntu"
+        assert str(image) == "image://test-cluster/test-project/ubuntu"
+        assert image.as_docker_url() == "registry.io/test-project/ubuntu"
 
     def test_as_str_in_neuro_registry_tag_yes(self) -> None:
         image = RemoteImage.new_neuro_image(
             name="ubuntu",
             tag="v10.04",
-            owner="me",
             cluster_name="test-cluster",
             registry="registry.io",
             org_name=None,
+            project_name="test-project",
         )
-        assert str(image) == "image://test-cluster/me/ubuntu:v10.04"
-        assert image.as_docker_url() == "registry.io/me/ubuntu:v10.04"
+        assert str(image) == "image://test-cluster/test-project/ubuntu:v10.04"
+        assert image.as_docker_url() == "registry.io/test-project/ubuntu:v10.04"
 
     def test_as_str_in_neuro_registry_tag_special_chars(self) -> None:
         image = RemoteImage.new_neuro_image(
             name="image#%2d?ß",
             tag="tag#%2d?ß",
-            owner="me",
             cluster_name="test-cluster",
             registry="registry.io",
             org_name=None,
+            project_name="test-project",
         )
-        assert (
-            str(image)
-            == "image://test-cluster/me/image%23%252d%3F%C3%9F:tag%23%252d%3F%C3%9F"
+        assert str(image) == (
+            "image://test-cluster/test-project/"
+            "image%23%252d%3F%C3%9F:tag%23%252d%3F%C3%9F"
         )
-        assert image.as_docker_url() == "registry.io/me/image#%2d?ß:tag#%2d?ß"
+        assert image.as_docker_url() == "registry.io/test-project/image#%2d?ß:tag#%2d?ß"
 
     def test_as_str_not_in_neuro_registry_tag_none(self) -> None:
         image = RemoteImage.new_external_image(name="ubuntu")
         assert str(image) == "ubuntu"
         assert image.as_docker_url() == "ubuntu"
 
     def test_as_str_not_in_neuro_registry_tag_yes(self) -> None:
@@ -1078,83 +1080,87 @@
         assert str(image) == "ubuntu:v10.04"
         assert image.as_docker_url() == "ubuntu:v10.04"
 
     def test_as_docker_url_in_neuro_registry(self) -> None:
         image = RemoteImage(
             name="ubuntu",
             tag="v10.04",
-            owner="me",
             cluster_name="test-cluster",
             registry="registry.io",
+            project_name="test-project",
         )
-        assert image.as_docker_url() == "registry.io/me/ubuntu:v10.04"
+        assert image.as_docker_url() == "registry.io/test-project/ubuntu:v10.04"
 
     def test_as_docker_url_not_in_neuro_registry(self) -> None:
-        image = RemoteImage(name="ubuntu", tag="v10.04", owner=None, registry=None)
+        image = RemoteImage(name="ubuntu", tag="v10.04", registry=None)
         assert image.as_docker_url() == "ubuntu:v10.04"
 
 
 @pytest.mark.usefixtures("patch_docker_host")
 class TestImages:
     parser = _ImageNameParser(
-        default_user="user",
         default_cluster="default",
         default_org=None,
+        default_project="test-project",
         registry_urls={"default": URL("https://registry-dev.neu.ro")},
     )
 
     @mock.patch(
         "aiodocker.Docker.__init__",
         side_effect=ValueError(
             "text Either DOCKER_HOST or local sockets are not available text"
         ),
     )
     async def test_unavailable_docker(
         self, patched_init: Any, make_client: _MakeClient
     ) -> None:
-        image = self.parser.parse_as_neuro_image("image://default/bob/image:bananas")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/project/image:bananas"
+        )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(DockerError, match=r"Docker engine is not available.+"):
                 await client.images.pull(image, local_image)
 
     @mock.patch(
         "aiodocker.Docker.__init__", side_effect=ValueError("something went wrong")
     )
     async def test_unknown_docker_error(
         self, patched_init: Any, make_client: _MakeClient
     ) -> None:
-        image = self.parser.parse_as_neuro_image("image://default/bob/image:bananas")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/project/image:bananas"
+        )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(ValueError, match=r"something went wrong"):
                 await client.images.pull(image, local_image)
 
     @mock.patch("aiodocker.images.DockerImages.tag")
     async def test_push_non_existent_image(
         self, patched_tag: Any, make_client: _MakeClient
     ) -> None:
         patched_tag.side_effect = DockerError(404, {"message": "Mocked error"})
         image = self.parser.parse_as_neuro_image(
-            "image://default/bob/image:bananas-no-more"
+            "image://default/project/image:bananas-no-more"
         )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(ValueError, match=r"not found"):
                 await client.images.push(local_image, image)
 
     @mock.patch("aiodocker.images.DockerImages.tag")
     @mock.patch("aiodocker.images.DockerImages.push")
     async def test_push_image_to_foreign_repo(
         self, patched_push: Any, patched_tag: Any, make_client: _MakeClient
     ) -> None:
         patched_tag.return_value = True
         patched_push.side_effect = DockerError(403, {"message": "Mocked error"})
         image = self.parser.parse_as_neuro_image(
-            "image://default/bob/image:bananas-no-more"
+            "image://default/project/image:bananas-no-more"
         )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(AuthorizationError):
                 await client.images.push(local_image, image)
 
     @mock.patch("aiodocker.images.DockerImages.tag")
@@ -1164,15 +1170,15 @@
     ) -> None:
         async def error_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {"error": True, "errorDetail": {"message": "Mocked message"}}
 
         patched_tag.return_value = True
         patched_push.return_value = error_generator()
         image = self.parser.parse_as_neuro_image(
-            "image://default/bob/image:bananas-wrong-food"
+            "image://default/project/image:bananas-wrong-food"
         )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(DockerError) as exc_info:
                 await client.images.push(local_image, image)
         assert exc_info.value.status == 900
         assert exc_info.value.message == "Mocked message"
@@ -1184,15 +1190,15 @@
     ) -> None:
         async def message_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {}
 
         patched_tag.return_value = True
         patched_push.return_value = message_generator()
         image = self.parser.parse_as_neuro_image(
-            "image://default/bob/image:bananas-is-here"
+            "image://default/project/image:bananas-is-here"
         )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             result = await client.images.push(local_image, image)
         assert result == image
 
     @mock.patch("aiodocker.images.DockerImages.tag")
@@ -1201,55 +1207,59 @@
         self, patched_push: Any, patched_tag: Any, make_client: _MakeClient
     ) -> None:
         async def message_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {}
 
         patched_tag.return_value = True
         patched_push.return_value = message_generator()
-        image = self.parser.parse_as_neuro_image("image://default/user/bananas:latest")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/test-project/bananas:latest"
+        )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             result = await client.images.push(local_image)
         assert result == image
 
     @mock.patch("aiodocker.images.DockerImages.pull")
     async def test_pull_non_existent_image(
         self, patched_pull: Any, make_client: _MakeClient
     ) -> None:
         patched_pull.side_effect = DockerError(404, {"message": "Mocked error"})
         async with make_client("https://api.localhost.localdomain") as client:
             image = self.parser.parse_as_neuro_image(
-                "image://default/bob/image:no-bananas-here"
+                "image://default/project/image:no-bananas-here"
             )
             local_image = self.parser.parse_as_local_image("bananas:latest")
             with pytest.raises(ValueError, match=r"not found"):
                 await client.images.pull(image, local_image)
 
     @mock.patch("aiodocker.images.DockerImages.pull")
     async def test_pull_image_from_foreign_repo(
         self, patched_pull: Any, make_client: _MakeClient
     ) -> None:
         patched_pull.side_effect = DockerError(403, {"message": "Mocked error"})
         image = self.parser.parse_as_neuro_image(
-            "image://default/bob/image:not-your-bananas"
+            "image://default/project/image:not-your-bananas"
         )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(AuthorizationError):
                 await client.images.pull(image, local_image)
 
     @mock.patch("aiodocker.images.DockerImages.pull")
     async def test_pull_image_with_docker_api_error(
         self, patched_pull: Any, make_client: Any
     ) -> None:
         async def error_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {"error": True, "errorDetail": {"message": "Mocked message"}}
 
         patched_pull.return_value = error_generator()
-        image = self.parser.parse_as_neuro_image("image://default/bob/image:nuts-here")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/project/image:nuts-here"
+        )
         async with make_client("https://api.localhost.localdomain") as client:
             with pytest.raises(DockerError) as exc_info:
                 await client.images.pull(image, image)
         assert exc_info.value.status == 900
         assert exc_info.value.message == "Mocked message"
 
     @mock.patch("aiodocker.images.DockerImages.tag")
@@ -1258,15 +1268,17 @@
         self, patched_pull: Any, patched_tag: Any, make_client: _MakeClient
     ) -> None:
         async def message_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {}
 
         patched_tag.return_value = True
         patched_pull.return_value = message_generator()
-        image = self.parser.parse_as_neuro_image("image://default/bob/image:bananas")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/project/image:bananas"
+        )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             result = await client.images.pull(image, local_image)
         assert result == local_image
 
     @mock.patch("aiodocker.images.DockerImages.tag")
     @mock.patch("aiodocker.images.DockerImages.pull")
@@ -1274,29 +1286,31 @@
         self, patched_pull: Any, patched_tag: Any, make_client: _MakeClient
     ) -> None:
         async def message_generator() -> AsyncIterator[Dict[str, Any]]:
             yield {}
 
         patched_tag.return_value = True
         patched_pull.return_value = message_generator()
-        image = self.parser.parse_as_neuro_image("image://default/bob/bananas:latest")
+        image = self.parser.parse_as_neuro_image(
+            "image://default/project/bananas:latest"
+        )
         local_image = self.parser.parse_as_local_image("bananas:latest")
         async with make_client("https://api.localhost.localdomain") as client:
             result = await client.images.pull(image)
         assert result == local_image
 
 
 class TestRegistry:
     @pytest.mark.skipif(
         sys.platform == "win32", reason="aiodocker doesn't support Windows pipes yet"
     )
     async def test_ls_repositories(
         self, aiohttp_server: _TestServerFactory, make_client: _MakeClient
     ) -> None:
-        JSON = {"repositories": ["bob/alpine", "jill/bananas"]}
+        JSON = {"repositories": ["project1/alpine", "project2/bananas"]}
 
         async def handler(request: web.Request) -> web.Response:
             assert "n" in request.query
             assert "last" not in request.query
             return web.json_response(JSON)
 
         app = web.Application()
@@ -1311,26 +1325,26 @@
 
         registry = _get_url_authority(registry_url)
         assert registry is not None
         assert set(ret) == {
             RemoteImage.new_neuro_image(
                 "alpine",
                 tag=None,
-                owner="bob",
                 cluster_name="default",
                 registry=registry,
                 org_name=None,
+                project_name="project1",
             ),
             RemoteImage.new_neuro_image(
                 "bananas",
                 tag=None,
-                owner="jill",
                 cluster_name="default",
                 registry=registry,
                 org_name=None,
+                project_name="project2",
             ),
         }
 
     async def test_ls_repositories_chunked(
         self, aiohttp_server: _TestServerFactory, make_client: _MakeClient
     ) -> None:
         step = 0
@@ -1338,20 +1352,20 @@
         async def handler(request: web.Request) -> web.Response:
             nonlocal step
             step += 1
             headers: Dict[str, str]
             assert "n" in request.query
             if step == 1:
                 assert "last" not in request.query
-                payload = {"repositories": ["bob/alpine", "jill/bananas"]}
+                payload = {"repositories": ["project1/alpine", "project2/bananas"]}
                 headers = {LINK: f'<{catalog_url}?last=lsttkn>; rel="next"'}
                 return web.json_response(payload, headers=headers)
             elif step == 2:
                 assert request.query["last"] == "lsttkn"
-                payload = {"repositories": ["alice/library/ubuntu"]}
+                payload = {"repositories": ["project3/library/ubuntu"]}
                 headers = {LINK: f'<{catalog_url}?last=lsttkn2>; rel="next"'}
                 return web.json_response(payload, headers=headers)
             elif step == 3:
                 assert request.query["last"] == "lsttkn2"
                 payload = {"repositories": []}
                 headers = {LINK: f'<{catalog_url}?last=lsttkn3>; rel="next"'}
                 return web.json_response(payload, headers=headers)
@@ -1368,34 +1382,34 @@
 
         registry = _get_url_authority(registry_url)
         assert registry is not None
         expected = {
             RemoteImage.new_neuro_image(
                 "alpine",
                 tag=None,
-                owner="bob",
                 cluster_name="default",
                 registry=registry,
                 org_name=None,
+                project_name="project1",
             ),
             RemoteImage.new_neuro_image(
                 "library/ubuntu",
                 tag=None,
-                owner="alice",
                 cluster_name="default",
                 registry=registry,
                 org_name=None,
+                project_name="project3",
             ),
             RemoteImage.new_neuro_image(
                 "bananas",
                 tag=None,
-                owner="jill",
                 cluster_name="default",
                 registry=registry,
                 org_name=None,
+                project_name="project2",
             ),
         }
 
         async with make_client(url, registry_url=registry_url) as client:
             ret = await client.images.list()
         assert step == 3  # All steps are passed
         assert set(ret) == expected
@@ -1410,55 +1424,55 @@
 
         async def handler(request: web.Request) -> web.Response:
             assert "n" in request.query
             assert "last" not in request.query
             return web.json_response(JSON)
 
         app = web.Application()
-        app.router.add_get("/v2/me/test/tags/list", handler)
+        app.router.add_get("/v2/project/test/tags/list", handler)
 
         srv = await aiohttp_server(app)
         url = "http://platform"
         registry_url = srv.make_url("/v2/")
 
         async with make_client(url, registry_url=registry_url) as client:
             image = RemoteImage.new_neuro_image(
                 name="test",
                 tag=None,
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             )
             ret = await client.images.tags(image)
 
         assert set(ret) == {
             RemoteImage.new_neuro_image(
                 "test",
                 tag="alpha",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
             RemoteImage.new_neuro_image(
                 "test",
                 tag="beta",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
             RemoteImage.new_neuro_image(
                 "test",
                 tag="gamma",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
         }
 
     async def test_ls_tags_chunked(
         self, aiohttp_server: _TestServerFactory, make_client: _MakeClient
     ) -> None:
         step = 0
@@ -1483,57 +1497,57 @@
                 payload = {"name": "test", "tags": []}
                 headers = {LINK: f'<{tags_list_url}?last=lsttkn3>; rel="next"'}
                 return web.json_response(payload, headers=headers)
             else:  # pragma: no cover
                 assert False
 
         app = web.Application()
-        app.router.add_get("/v2/me/test/tags/list", handler)
+        app.router.add_get("/v2/project/test/tags/list", handler)
 
         srv = await aiohttp_server(app)
         url = "http://platform"
         registry_url = srv.make_url("/v2/")
-        tags_list_url = registry_url / "me/test/tags/list"
+        tags_list_url = registry_url / "project/test/tags/list"
 
         async with make_client(url, registry_url=registry_url) as client:
             image = RemoteImage.new_neuro_image(
                 name="test",
                 tag=None,
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             )
             ret = await client.images.tags(image)
         assert step == 3  # All steps are passed
 
         assert set(ret) == {
             RemoteImage.new_neuro_image(
                 "test",
                 tag="alpha",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
             RemoteImage.new_neuro_image(
                 "test",
                 tag="beta",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
             RemoteImage.new_neuro_image(
                 "test",
                 tag="gamma",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             ),
         }
 
     @pytest.mark.skipif(
         sys.platform == "win32", reason="aiodocker doesn't support Windows pipes yet"
     )
     async def test_tag_info(
@@ -1565,28 +1579,28 @@
             assert (
                 request.headers["Accept"]
                 == "application/vnd.docker.distribution.manifest.v2+json"
             )
             return web.json_response(JSON)
 
         app = web.Application()
-        app.router.add_get("/v2/me/test/manifests/test_tag", handler)
+        app.router.add_get("/v2/project/test/manifests/test_tag", handler)
 
         srv = await aiohttp_server(app)
         url = "http://platform"
         registry_url = srv.make_url("/v2/")
 
         async with make_client(url, registry_url=registry_url) as client:
             image = RemoteImage.new_neuro_image(
                 name="test",
                 tag="test_tag",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             )
             ret = await client.images.tag_info(image)
             assert image.tag
 
         assert ret == Tag(name=image.tag, size=32890532)
 
     @pytest.mark.skipif(
@@ -1595,32 +1609,32 @@
     async def test_tags_bad_image_with_tag(self, make_client: _MakeClient) -> None:
         url = URL("http://whatever")
         registry_url = URL("http://whatever-registry")
         async with make_client(url, registry_url=registry_url) as client:
             image = RemoteImage.new_neuro_image(
                 name="ubuntu",
                 tag="latest",
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             )
             with pytest.raises(ValueError, match="tag is not allowed"):
                 await client.images.tags(image)
 
     @pytest.mark.skipif(
         sys.platform == "win32", reason="aiodocker doesn't support Windows pipes yet"
     )
     async def test_tags_bad_image_without_name(self, make_client: _MakeClient) -> None:
         url = URL("http://whatever")
         registry_url = URL("http://whatever-registry")
         async with make_client(url, registry_url=registry_url) as client:
             image = RemoteImage.new_neuro_image(
                 name="",
                 tag=None,
-                owner="me",
                 cluster_name="default",
                 registry="reg",
                 org_name=None,
+                project_name="project",
             )
             with pytest.raises(ValueError, match="missing image name"):
                 await client.images.tags(image)
```

### Comparing `neuro-sdk-23.2.0/tests/test_jobs.py` & `neuro-sdk-23.7.0/tests/test_jobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -349,18 +349,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         await client.jobs.save("job-id", image)
 
 
 async def test_save_commit_started_invalid_status_fails(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
@@ -388,18 +388,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         with pytest.raises(
             DockerError,
             match=f"Invalid commit status: '{invalid}', expecting: 'CommitStarted'",
         ):
             await client.jobs.save("job-id", image)
 
@@ -430,18 +430,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         with pytest.raises(DockerError, match="Missing required details: 'image'"):
             await client.jobs.save("job-id", image)
 
 
 async def test_save_commit_finished_invalid_status_fails(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
@@ -469,18 +469,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         with pytest.raises(
             DockerError,
             match=(f"Invalid commit status: '{invalid}', expecting: 'CommitFinished'"),
         ):
             await client.jobs.save("job-id", image)
 
@@ -510,18 +510,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         with pytest.raises(DockerError, match='Missing required field: "status"'):
             await client.jobs.save("job-id", image)
 
 
 async def test_save_commit_finished_missing_status_fails(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
@@ -548,18 +548,18 @@
     app.router.add_post("/jobs/job-id/save", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         image = RemoteImage.new_neuro_image(
             registry="gcr.io",
-            owner="me",
             cluster_name="test-cluster",
             name="img",
             org_name=None,
+            project_name="test-project",
         )
         with pytest.raises(DockerError, match='Missing required field: "status"'):
             await client.jobs.save("job-id", image)
 
 
 async def test_status_failed(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
@@ -815,14 +815,33 @@
         ret = await client.jobs.status("job-id")
 
         assert ret == _job_description_from_api(JSON, client.parse)
         assert ret.container.resources.tpu_type == "v3-8"
         assert ret.container.resources.tpu_software_version == "1.14"
 
 
+async def test_status_wo_project(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    JSON = create_job_response("job-id", "running", project_name=None)
+
+    async def handler(request: web.Request) -> web.Response:
+        return web.json_response(JSON)
+
+    app = web.Application()
+    app.router.add_get("/jobs/job-id", handler)
+
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        ret = await client.jobs.status("job-id")
+        assert ret == _job_description_from_api(JSON, client.parse)
+        assert ret.project_name == "owner"
+
+
 async def test_job_start(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     JSON = {
         "id": "job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "status": "failed",
         "history": {
@@ -830,14 +849,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -874,14 +894,15 @@
                     "dst_path": "/container/path_read_write",
                     "read_only": False,
                 },
             ],
             "pass_config": False,
             "cluster_name": "default",
             "preset_name": "cpu-small",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -921,14 +942,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -951,14 +973,15 @@
         assert data == {
             "image": "submit-image-name",
             "command": "submit-command",
             "pass_config": False,
             "cluster_name": "default",
             "preset_name": "cpu-small",
             "privileged": True,
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -986,14 +1009,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1017,14 +1041,15 @@
         assert data == {
             "image": "submit-image-name",
             "command": "submit-command",
             "pass_config": False,
             "cluster_name": "default",
             "preset_name": "cpu-small",
             "priority": "high",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1037,14 +1062,50 @@
             preset_name="cpu-small",
             priority=JobPriority.HIGH,
         )
 
         assert ret == _job_description_from_api(JSON, client.parse)
 
 
+@pytest.mark.parametrize(
+    "project_name",
+    [None, "", "test-project", "other-test-project", "non-existing-project"],
+)
+async def test_job_start_with_project(
+    aiohttp_server: _TestServerFactory,
+    make_client: _MakeClient,
+    project_name: Optional[str],
+) -> None:
+    JSON = create_job_response("qwerty", "running", project_name=project_name)
+
+    async def handler(request: web.Request) -> web.Response:
+        data = await request.json()
+        assert data == {
+            "image": "submit-image-name",
+            "pass_config": False,
+            "cluster_name": "default",
+            "preset_name": "cpu-small",
+            # if project_name is not provided, SDK falls back to current project
+            "project_name": project_name or "test-project",
+        }
+        return web.json_response(JSON)
+
+    app = web.Application()
+    app.router.add_post("/jobs", handler)
+
+    srv = await aiohttp_server(app)
+    async with make_client(srv.make_url("/")) as client:
+        ret = await client.jobs.start(
+            image=RemoteImage.new_external_image(name="submit-image-name"),
+            preset_name="cpu-small",
+            project_name=project_name,
+        )
+        assert ret == _job_description_from_api(JSON, client.parse)
+
+
 async def test_job_run(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     JSON = {
         "id": "job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "status": "failed",
         "history": {
@@ -1054,14 +1115,15 @@
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
         "cluster_name": "default",
         "org_name": "my-test-org",
+        "project_name": "test-project",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
@@ -1103,14 +1165,15 @@
                         "read_only": False,
                     },
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1152,14 +1215,15 @@
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
         "cluster_name": "default",
+        "project_name": "test-project",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
@@ -1189,14 +1253,15 @@
                     "gpu_model": "test-gpu-model",
                 },
             },
             "scheduler_enabled": False,
             "wait_for_jobs_quota": True,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1229,14 +1294,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1281,14 +1347,15 @@
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "name": "test-job-name",
             "description": "job description",
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1335,14 +1402,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1386,14 +1454,15 @@
                     },
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "tags": ["t1", "t2", "t3"],
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1439,14 +1508,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1479,14 +1549,15 @@
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "name": "test-job-name",
             "description": "job description",
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1521,14 +1592,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1557,53 +1629,54 @@
                     "cpu": 7.0,
                     "shm": True,
                     "gpu": 1,
                     "gpu_model": "test-gpu-model",
                 },
                 "volumes": [
                     {
-                        "src_storage_uri": "storage://default/user/path",
+                        "src_storage_uri": "storage://default/test-project/path",
                         "dst_path": "/container/my_path",
                         "read_only": False,
                     },
                     {
-                        "src_storage_uri": "storage://default/otheruser/path",
+                        "src_storage_uri": "storage://default/otherproject/path",
                         "dst_path": "/container/other_user_path",
                         "read_only": True,
                     },
                     {
-                        "src_storage_uri": "storage://othercluster/otheruser/path",
+                        "src_storage_uri": "storage://othercluster/otherproject/path",
                         "dst_path": "/container/other_cluster_path",
                         "read_only": True,
                     },
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         resources = Resources(16384 * 2**20, 7, 1, "test-gpu-model", True, None, None)
         volumes: List[Volume] = [
             Volume(URL("storage:path"), "/container/my_path", False),
             Volume(
-                URL("storage:/otheruser/path"),
+                URL("storage:/otherproject/path"),
                 "/container/other_user_path",
                 True,
             ),
             Volume(
-                URL("storage://othercluster/otheruser/path"),
+                URL("storage://othercluster/otherproject/path"),
                 "/container/other_cluster_path",
                 True,
             ),
         ]
         container = Container(
             image=RemoteImage.new_external_image(name="submit-image-name"),
             command="submit-command",
@@ -1627,14 +1700,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1662,32 +1736,33 @@
                     "memory": 16384 * 2**20,
                     "cpu": 7.0,
                     "shm": True,
                     "gpu": 1,
                     "gpu_model": "test-gpu-model",
                 },
                 "env": {"VAR": "VAL"},
-                "secret_env": {"SECRET_VAR": "secret://default/user/secret"},
+                "secret_env": {"SECRET_VAR": "secret://default/test-project/secret"},
                 "volumes": [
                     {
-                        "src_storage_uri": "storage://default/user/path",
+                        "src_storage_uri": "storage://default/test-project/path",
                         "dst_path": "/container/my_path",
                         "read_only": False,
                     }
                 ],
                 "secret_volumes": [
                     {
-                        "src_secret_uri": "secret://default/user/secret",
+                        "src_secret_uri": "secret://default/test-project/secret",
                         "dst_path": "/secrets/my_path",
                     }
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1728,14 +1803,15 @@
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
         "cluster_name": "default",
+        "project_name": "test-project",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
             "resources": {
@@ -1743,15 +1819,15 @@
                 "memory": 16384 * 2**20,
                 "gpu": 1,
                 "shm": False,
                 "gpu_model": "nvidia-tesla-p4",
             },
             "disk_volumes": [
                 {
-                    "src_disk_uri": "disk://default/user/disk-1",
+                    "src_disk_uri": "disk://default/test-project/disk-1",
                     "dst_path": "/container/my_path",
                     "read_only": False,
                 }
             ],
         },
         "http_url": "http://my_host:8889",
         "scheduler_enabled": False,
@@ -1770,23 +1846,24 @@
                     "cpu": 7.0,
                     "shm": True,
                     "gpu": 1,
                     "gpu_model": "test-gpu-model",
                 },
                 "disk_volumes": [
                     {
-                        "src_disk_uri": "disk://default/user/disk-1",
+                        "src_disk_uri": "disk://default/test-project/disk-1",
                         "dst_path": "/container/my_path",
                         "read_only": False,
                     }
                 ],
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1821,14 +1898,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1873,14 +1951,15 @@
                 ],
             },
             "scheduler_enabled": True,
             "pass_config": False,
             "name": "test-job-name",
             "description": "job description",
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -1926,14 +2005,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -1965,14 +2045,15 @@
                     "gpu_model": "test-gpu-model",
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "schedule_timeout": 5,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -2001,14 +2082,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -2041,14 +2123,15 @@
                     "tpu": {"type": "v3-8", "software_version": "1.14"},
                 },
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "schedule_timeout": 5,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -2084,14 +2167,15 @@
                 "command": "submit-command",
                 "resources": {"memory": 16384 * 2**20, "cpu": 0.5, "shm": True},
                 "tty": True,
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
@@ -2107,24 +2191,66 @@
         )
         ret = await client.jobs.run(container=container)
 
         assert ret == _job_description_from_api(JSON, client.parse)
         assert ret.container.tty is True
 
 
+@pytest.mark.parametrize(
+    "project_name",
+    [None, "", "test-project", "other-test-project", "non-existing-project"],
+)
+async def test_job_run_with_project(
+    aiohttp_server: _TestServerFactory,
+    make_client: _MakeClient,
+    project_name: Optional[str],
+) -> None:
+    JSON = create_job_response("qwerty", "running", project_name=project_name)
+
+    async def handler(request: web.Request) -> web.Response:
+        data = await request.json()
+        assert data == {
+            "container": {
+                "image": "submit-image-name",
+                "resources": {"memory": 16384 * 2**20, "cpu": 0.5, "shm": True},
+            },
+            "scheduler_enabled": False,
+            "pass_config": False,
+            "cluster_name": "default",
+            "project_name": project_name or "test-project",
+        }
+        return web.json_response(JSON)
+
+    app = web.Application()
+    app.router.add_post("/jobs", handler)
+    srv = await aiohttp_server(app)
+
+    container = Container(
+        image=RemoteImage.new_external_image(name="submit-image-name"),
+        resources=Resources(16384 * 2**20, 0.5),
+    )
+    async with make_client(srv.make_url("/")) as client:
+        ret = await client.jobs.run(
+            container,
+            project_name=project_name,
+        )
+        assert ret == _job_description_from_api(JSON, client.parse)
+
+
 def create_job_response(
     id: str,
     status: str,
     owner: str = "owner",
     name: Optional[str] = None,
     org_name: Optional[str] = None,
     image: str = "submit-image-name",
     tags: Optional[List[str]] = None,
     total_price_credits: str = "10.01",
     price_credits_per_hour: str = "20",
+    project_name: Optional[str] = "myproject",
 ) -> Dict[str, Any]:
     result = {
         "id": id,
         "status": status,
         "history": {
             "status": "failed",
             "reason": "Error",
@@ -2153,14 +2279,16 @@
     }
     if name:
         result["name"] = name
     if tags:
         result["tags"] = tags
     if org_name:
         result["org_name"] = org_name
+    if project_name:
+        result["project_name"] = project_name
     return result
 
 
 async def test_list_error_in_stream_response(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     error_result = {"error": "Failed"}
@@ -2302,15 +2430,14 @@
             "job-id-3", "failed", image="registry-dev.neu.ro/path/:tag"
         ),
         create_job_response("job-id-4", "failed", image=""),
         create_job_response("job-id-5", "failed", image=":"),
     ]
 
     async def handler(request: web.Request) -> web.Response:
-
         JSON = {"jobs": jobs}
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
     srv = await aiohttp_server(app)
 
@@ -2346,57 +2473,57 @@
             with pytest.raises(ValueError, match=r"Wrong ReadWrite/ReadOnly mode spec"):
                 client.parse.volume(volume_param)
 
     @pytest.mark.parametrize(
         "volume_param,volume",
         [
             (
-                "storage://default/user/dir:/var/www",
+                "storage://default/test-project/dir:/var/www",
                 Volume(
-                    storage_uri=URL("storage://default/user/dir"),
+                    storage_uri=URL("storage://default/test-project/dir"),
                     container_path="/var/www",
                     read_only=False,
                 ),
             ),
             (
-                "storage://default/user/dir:/var/www:rw",
+                "storage://default/test-project/dir:/var/www:rw",
                 Volume(
-                    storage_uri=URL("storage://default/user/dir"),
+                    storage_uri=URL("storage://default/test-project/dir"),
                     container_path="/var/www",
                     read_only=False,
                 ),
             ),
             (
-                "storage://default/user:/var/www:ro",
+                "storage://default/test-project:/var/www:ro",
                 Volume(
-                    storage_uri=URL("storage://default/user"),
+                    storage_uri=URL("storage://default/test-project"),
                     container_path="/var/www",
                     read_only=True,
                 ),
             ),
             (
                 "storage::/var/www:ro",
                 Volume(
-                    storage_uri=URL("storage://default/user"),
+                    storage_uri=URL("storage://default/test-project"),
                     container_path="/var/www",
                     read_only=True,
                 ),
             ),
             (
                 "storage:dir:/var/www:ro",
                 Volume(
-                    storage_uri=URL("storage://default/user/dir"),
+                    storage_uri=URL("storage://default/test-project/dir"),
                     container_path="/var/www",
                     read_only=True,
                 ),
             ),
             (
                 "storage::/var/www:ro",
                 Volume(
-                    storage_uri=URL("storage://default/user"),
+                    storage_uri=URL("storage://default/test-project"),
                     container_path="/var/www",
                     read_only=True,
                 ),
             ),
         ],
     )
     async def test_positive(
@@ -2594,14 +2721,67 @@
         assert {job.id for job in ret} == {"job-id-2", "job-id-3"}
 
         async with client.jobs.list(until=t2naive) as it:
             ret = [job async for job in it]
         assert {job.id for job in ret} == {"job-id-1", "job-id-2"}
 
 
+async def test_list_filter_by_project(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    proj_1 = "proj-name-1"
+    proj_2 = "proj-name-2"
+    jobs = [
+        create_job_response("job-id-1", "pending", project_name=proj_1),
+        create_job_response("job-id-2", "succeeded", project_name=proj_1),
+        create_job_response("job-id-3", "failed", project_name=proj_1),
+        create_job_response("job-id-4", "running", project_name=proj_2),
+        create_job_response("job-id-5", "succeeded", project_name=proj_2),
+        create_job_response("job-id-6", "failed", project_name=proj_2),
+        create_job_response("job-id-7", "running"),
+        create_job_response("job-id-8", "pending"),
+        create_job_response("job-id-9", "succeeded"),
+        create_job_response("job-id-10", "failed"),
+    ]
+
+    async def handler(request: web.Request) -> web.Response:
+        projects = request.query.getall("project_name", None)
+        if projects:
+            filtered_jobs = [job for job in jobs if job["project_name"] in projects]
+        else:
+            filtered_jobs = jobs
+        JSON = {"jobs": filtered_jobs}
+        return web.json_response(JSON)
+
+    app = web.Application()
+    app.router.add_get("/jobs", handler)
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        job_descriptions = [
+            _job_description_from_api(job, client.parse) for job in jobs
+        ]
+        # default -- lists all available jobs
+        async with client.jobs.list() as it:
+            ret = [job async for job in it]
+        assert ret == job_descriptions
+        # filter by one project
+        async with client.jobs.list(project_names=(proj_1,)) as it:
+            ret = [job async for job in it]
+        assert ret == job_descriptions[:3]
+        # filter by two projects
+        async with client.jobs.list(project_names=(proj_1, proj_2)) as it:
+            ret = [job async for job in it]
+        assert ret == job_descriptions[:6]
+        # filter by non-existing project
+        async with client.jobs.list(project_names=("non-existing",)) as it:
+            ret = [job async for job in it]
+        assert ret == []
+
+
 async def test_job_run_life_span(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
         data = await request.json()
         assert data == {
             "container": {
@@ -2609,14 +2789,15 @@
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
                 "command": "submit-command",
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "max_run_time_minutes": 10,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
         return web.json_response(create_job_response("job-id-1", "running"))
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
@@ -2642,14 +2823,15 @@
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
                 "command": "submit-command",
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "restart_policy": "always",
             "cluster_name": "default",
+            "project_name": "test-project",
         }
         return web.json_response(create_job_response("job-id-1", "running"))
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
@@ -2677,14 +2859,15 @@
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
                 "command": "submit-command",
                 "working_dir": "/working/dir",
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
         result = create_job_response("job-id-1", "running")
         result["container"]["working_dir"] = "/working/dir"
         return web.json_response(result)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
@@ -2827,14 +3010,15 @@
             "container": {
                 "image": "submit-image-name",
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
         api_responce = create_job_response(
             "job-id-1",
             "running",
             total_price_credits=total_price_credits,
             price_credits_per_hour=price_credits_per_hour,
         )
@@ -2866,14 +3050,15 @@
             "container": {
                 "image": "submit-image-name",
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
             "org_name": org_name,
         }
         api_responce = create_job_response(
             "job-id-1",
             "running",
             org_name=org_name,
         )
@@ -2902,14 +3087,15 @@
             "container": {
                 "image": "submit-image-name",
                 "resources": {"memory": 16 * 2**20, "cpu": 0.5, "shm": True},
             },
             "scheduler_enabled": False,
             "pass_config": False,
             "cluster_name": "default",
+            "project_name": "test-project",
         }
         return web.json_response(create_job_response("job-id-1", "running"))
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
 
     srv = await aiohttp_server(app)
@@ -2934,14 +3120,15 @@
             "reason": "Error",
             "description": "Mounted on Avail\\n/dev/shm     " "64M\\n\\nExit code: 1",
             "created_at": "2018-09-25T12:28:21.298672+00:00",
             "started_at": "2018-09-25T12:28:59.759433+00:00",
             "finished_at": "2018-09-25T12:28:59.759433+00:00",
         },
         "owner": "owner",
+        "project_name": "test-project",
         "cluster_name": "default",
         "uri": "job://default/owner/job-cf519ed3-9ea5-48f6-a8c5-492b810eb56f",
         "total_price_credits": "10.01",
         "price_credits_per_hour": "20",
         "container": {
             "image": "gcr.io/light-reality-205619/ubuntu:latest",
             "command": "date",
@@ -2962,14 +3149,15 @@
         assert data == {
             "image": "submit-image-name",
             "command": "submit-command",
             "cluster_name": "default",
             "preset_name": "cpu-large-p",
             "energy_schedule_name": "some-schedule",
             "pass_config": False,
+            "project_name": "test-project",
         }
 
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_post("/jobs", handler)
```

### Comparing `neuro-sdk-23.2.0/tests/test_login.py` & `neuro-sdk-23.7.0/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_login_utils.py` & `neuro-sdk-23.7.0/tests/test_login_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 
 import aiohttp
 import pytest
 from aiohttp import web
 from yarl import URL
 
-from neuro_sdk import AuthError, Cluster, Preset
+from neuro_sdk import AuthError, Cluster, Preset, Project
 from neuro_sdk._login import _AuthConfig
 from neuro_sdk._server_cfg import _ServerConfig, get_server_config
 
 from tests import _TestClientFactory
 
 
 async def test_get_server_config_no_clusters(
@@ -55,22 +55,22 @@
             client_id=client_id,
             audience=audience,
             headless_callback_url=URL(headless_callback_url),
             callback_urls=tuple(URL(u) for u in callback_urls),
             success_redirect_url=URL(success_redirect_url),
         ),
         clusters={},
+        projects={},
         admin_url=None,
     )
 
 
 async def test_get_server_config_no_callback_urls(
     aiohttp_client: _TestClientFactory,
 ) -> None:
-
     auth_url = "https://dev-neuro.auth0.com/authorize"
     token_url = "https://dev-neuro.auth0.com/oauth/token"
     logout_url = "https://dev-neuro.auth0.com/v2/logout"
     client_id = "this_is_client_id"
     audience = "https://platform.dev.neu.ro"
     headless_callback_url = "https://dev.neu.ro/oauth/show-code"
     success_redirect_url = "https://platform.neu.ro"
@@ -100,22 +100,22 @@
             logout_url=URL(logout_url),
             client_id=client_id,
             audience=audience,
             headless_callback_url=URL(headless_callback_url),
             success_redirect_url=URL(success_redirect_url),
         ),
         clusters={},
+        projects={},
         admin_url=None,
     )
 
 
 async def test_get_server_config_with_token(
     aiohttp_client: _TestClientFactory,
 ) -> None:
-
     admin_url = "https://admin-dev.neu.ro"
     registry_url = "https://registry.dev.neu.ro"
     storage_url = "https://storage.dev.neu.ro"
     users_url = "https://dev.neu.ro/users"
     monitoring_url = "https://dev.neu.ro/monitoring"
     secrets_url = "https://dev.neu.ro/secrets"
     disks_url = "https://dev.neu.ro/disks"
@@ -183,27 +183,38 @@
                         "memory": 14 * 2**30,
                         "scheduler_enabled": True,
                         "preemptible_node": True,
                     },
                 ],
             }
         ],
+        "projects": [
+            {
+                "cluster_name": "default",
+                "org_name": None,
+                "name": "test-project",
+                "role": "owner",
+            }
+        ],
     }
 
     async def handler(request: web.Request) -> web.Response:
         assert request.headers["Authorization"] == "Bearer bananatoken"
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/config", handler)
     client = await aiohttp_client(app)
 
     config = await get_server_config(
         client.session, client.make_url("/"), token="bananatoken"
     )
+    project = Project(
+        cluster_name="default", org_name=None, name="test-project", role="owner"
+    )
     assert config == _ServerConfig(
         auth_config=_AuthConfig(
             auth_url=URL(auth_url),
             token_url=URL(token_url),
             logout_url=URL(logout_url),
             client_id=client_id,
             audience=audience,
@@ -249,14 +260,15 @@
                         preemptible_node=True,
                     ),
                 },
                 name="default",
                 orgs=[None],
             )
         },
+        projects={project.key: project},
     )
 
 
 async def test_get_server_config_with_token_no_clusters(
     aiohttp_client: _TestClientFactory,
 ) -> None:
     auth_url = "https://dev-neuro.auth0.com/authorize"
@@ -302,14 +314,15 @@
             client_id=client_id,
             audience=audience,
             headless_callback_url=URL(headless_callback_url),
             callback_urls=tuple(URL(u) for u in callback_urls),
             success_redirect_url=URL(success_redirect_url),
         ),
         clusters={},
+        projects={},
         admin_url=None,
     )
 
 
 async def test_get_server_config_unauthorized(
     aiohttp_client: _TestClientFactory,
 ) -> None:
```

### Comparing `neuro-sdk-23.2.0/tests/test_parser.py` & `neuro-sdk-23.7.0/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,59 +13,59 @@
     "volume",
     [
         "storage:///",
         ":",
         "::::",
         "",
         "storage:///data/:/data/rest:wrong",
-        "storage://cluster/user/path:to:/storage/location",
-        "storage://cluster/user/path/to:/storage/loca:tion",
-        "storage://cluster/user/path/to#fragment:/storage/location",
-        "storage://cluster/user/path/to#:/storage/location",
-        "storage://cluster/user/path/to?key=value:/storage/location",
-        "storage://cluster/user/path/to?:/storage/location",
-        "storage://user@cluster/user/path/to:/storage/location",
-        "storage://:password@cluster/user/path/to:/storage/location",
-        "storage://:@cluster/user/path/to:/storage/location",
-        "storage://cluster:1234/user/path/to:/storage/location",
+        "storage://cluster/project/path:to:/storage/location",
+        "storage://cluster/project/path/to:/storage/loca:tion",
+        "storage://cluster/project/path/to#fragment:/storage/location",
+        "storage://cluster/project/path/to#:/storage/location",
+        "storage://cluster/project/path/to?key=value:/storage/location",
+        "storage://cluster/project/path/to?:/storage/location",
+        "storage://user@cluster/project/path/to:/storage/location",
+        "storage://:password@cluster/project/path/to:/storage/location",
+        "storage://:@cluster/project/path/to:/storage/location",
+        "storage://cluster:1234/project/path/to:/storage/location",
     ],
 )
 async def test_volume_from_str_fail(volume: str, make_client: _MakeClient) -> None:
     async with make_client("https://example.com") as client:
         with pytest.raises(ValueError):
             client.parse.volume(volume)
 
 
 @pytest.mark.parametrize(
     "volume",
     [
         "disk://",
-        "disk://cluster/user/name:/disk/location:rw:more",
-        "disk://cluster/user/name:/disk/location:rwo",
-        "disk://cluster/user/na:me:/disk/location",
-        "disk://cluster/user/name:/disk/loca:tion",
-        "disk://cluster/user/name#fragment:/disk/location",
-        "disk://cluster/user/name#:/disk/location",
-        "disk://cluster/user/name?key=value:/disk/location",
-        "disk://cluster/user/name?:/disk/location",
-        "disk://user@cluster/user/name:/disk/location",
-        "disk://:password@cluster/user/name:/disk/location",
-        "disk://:@cluster/user/name:/disk/location",
-        "disk://cluster:1234/user/name:/disk/location",
-        "secret://cluster/user/secret:/var/secret:ro",
-        "secret://cluster/user/sec:ret:/secret/location",
-        "secret://cluster/user/secret:/secret/loca:tion",
-        "secret://cluster/user/secret#fragment:/secret/location",
-        "secret://cluster/user/secret#:/secret/location",
-        "secret://cluster/user/secret?key=value:/secret/location",
-        "secret://cluster/user/secret?:/secret/location",
-        "secret://user@cluster/user/secret:/secret/location",
-        "secret://:password@cluster/user/secret:/secret/location",
-        "secret://:@cluster/user/secret:/secret/location",
-        "secret://cluster:1234/user/secret:/secret/location",
+        "disk://cluster/project/name:/disk/location:rw:more",
+        "disk://cluster/project/name:/disk/location:rwo",
+        "disk://cluster/project/na:me:/disk/location",
+        "disk://cluster/project/name:/disk/loca:tion",
+        "disk://cluster/project/name#fragment:/disk/location",
+        "disk://cluster/project/name#:/disk/location",
+        "disk://cluster/project/name?key=value:/disk/location",
+        "disk://cluster/project/name?:/disk/location",
+        "disk://user@cluster/project/name:/disk/location",
+        "disk://:password@cluster/project/name:/disk/location",
+        "disk://:@cluster/project/name:/disk/location",
+        "disk://cluster:1234/project/name:/disk/location",
+        "secret://cluster/project/secret:/var/secret:ro",
+        "secret://cluster/project/sec:ret:/secret/location",
+        "secret://cluster/project/secret:/secret/loca:tion",
+        "secret://cluster/project/secret#fragment:/secret/location",
+        "secret://cluster/project/secret#:/secret/location",
+        "secret://cluster/project/secret?key=value:/secret/location",
+        "secret://cluster/project/secret?:/secret/location",
+        "secret://user@cluster/project/secret:/secret/location",
+        "secret://:password@cluster/project/secret:/secret/location",
+        "secret://:@cluster/project/secret:/secret/location",
+        "secret://cluster:1234/project/secret:/secret/location",
         "dissk://f1/f2/f3:/f1:rw",
     ],
 )
 async def test_parse_volumes_fail(volume: str, make_client: _MakeClient) -> None:
     async with make_client("https://example.com") as client:
         with pytest.raises(ValueError):
             client.parse.volumes([volume])
@@ -131,37 +131,39 @@
     async with make_client("https://api.localhost.localdomain") as client:
         result = client.parse.local_image("bananas:latest")
     assert result == LocalImage("bananas", "latest")
 
 
 async def test_parse_remote(make_client: _MakeClient) -> None:
     async with make_client("https://api.localhost.localdomain") as client:
-        result = client.parse.remote_image("image://default/bob/bananas:latest")
+        result = client.parse.remote_image("image://default/project/bananas:latest")
     assert result == RemoteImage.new_neuro_image(
         name="bananas",
         tag="latest",
-        owner="bob",
         registry="registry-dev.neu.ro",
         cluster_name="default",
         org_name=None,
+        project_name="project",
     )
 
 
 async def test_parse_remote_registry_image(make_client: _MakeClient) -> None:
     async with make_client(
         "https://api.localhost.localdomain", registry_url="http://localhost:5000"
     ) as client:
-        result = client.parse.remote_image("localhost:5000/bob/library/bananas:latest")
+        result = client.parse.remote_image(
+            "localhost:5000/project/library/bananas:latest"
+        )
     assert result == RemoteImage.new_neuro_image(
         name="library/bananas",
         tag="latest",
-        owner="bob",
         registry="localhost:5000",
         cluster_name="default",
         org_name=None,
+        project_name="project",
     )
 
 
 async def test_parse_remote_public(make_client: _MakeClient) -> None:
     async with make_client(
         "https://api.localhost.localdomain", registry_url="http://localhost:5000"
     ) as client:
@@ -197,17 +199,26 @@
         "secret:second:/var/secrets/second",
         "secret:third:/var/secrets/third",
     ]
     async with make_client("https://example.com") as client:
         volumes_parsed = client.parse.volumes(volumes)
 
     assert volumes_parsed.secret_files == [
-        SecretFile(URL("secret://default/user/first"), "/var/secrets/first"),
-        SecretFile(URL("secret://default/user/second"), "/var/secrets/second"),
-        SecretFile(URL("secret://default/user/third"), "/var/secrets/third"),
+        SecretFile(
+            URL(f"secret://default/{client.config.project_name}/first"),
+            "/var/secrets/first",
+        ),
+        SecretFile(
+            URL(f"secret://default/{client.config.project_name}/second"),
+            "/var/secrets/second",
+        ),
+        SecretFile(
+            URL(f"secret://default/{client.config.project_name}/third"),
+            "/var/secrets/third",
+        ),
     ]
 
 
 async def test_normalize_uri_short_from_short(make_client: _MakeClient) -> None:
     async with make_client("https://example.com") as client:
         ret = client.parse.normalize_uri(URL("storage:dir"), short=True)
         assert ret == URL("storage:dir")
```

### Comparing `neuro-sdk-23.2.0/tests/test_plugins.py` & `neuro-sdk-23.7.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_public_names.py` & `neuro-sdk-23.7.0/tests/test_public_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from yarl import URL
 
 import neuro_sdk
+from neuro_sdk._utils import OrgNameSentinel
 
 
 def test_public_version() -> None:
     assert "__version__" in neuro_sdk.__all__
 
 
 def test_module_for_public_names() -> None:
     for name in neuro_sdk.__all__:
         obj = getattr(neuro_sdk, name)
         if isinstance(obj, URL):
             # Default API url
             continue
+        if obj == OrgNameSentinel:
+            continue
+        if isinstance(obj, OrgNameSentinel):
+            continue
         if hasattr(obj, "__module__"):
             assert obj.__module__ in (
                 "neuro_sdk",
                 # objects from typing are public type hint aliases,
                 # e.g. Callable[...]
                 "typing",
                 # We re-export entities from admin client
```

### Comparing `neuro-sdk-23.2.0/tests/test_retry.py` & `neuro-sdk-23.7.0/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_secrets.py` & `neuro-sdk-23.7.0/tests/test_secrets.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,16 +12,25 @@
 
 async def test_list(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
         return web.json_response(
             [
-                {"key": "name1", "owner": "test"},
-                {"key": "name2", "owner": "test", "org_name": "test-org"},
+                {
+                    "key": "name1",
+                    "owner": "test",
+                    "project_name": "test-project",
+                },
+                {
+                    "key": "name2",
+                    "owner": "test",
+                    "org_name": "test-org",
+                    "project_name": "test-project",
+                },
             ]
         )
 
     app = web.Application()
     app.router.add_get("/secrets", handler)
 
     srv = await aiohttp_server(app)
@@ -30,28 +39,41 @@
 
     async with make_client(srv.make_url("/")) as client:
         async with client.secrets.list() as it:
             async for s in it:
                 ret.append(s)
 
     assert ret == [
-        Secret(key="name1", owner="test", cluster_name="default", org_name=None),
-        Secret(key="name2", owner="test", cluster_name="default", org_name="test-org"),
+        Secret(
+            key="name1",
+            owner="test",
+            cluster_name="default",
+            org_name=None,
+            project_name="test-project",
+        ),
+        Secret(
+            key="name2",
+            owner="test",
+            cluster_name="default",
+            org_name="test-org",
+            project_name="test-project",
+        ),
     ]
 
 
 async def test_add(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
         data = await request.json()
         assert data == {
             "key": "name",
             "value": base64.b64encode(b"data").decode("ascii"),
             "org_name": None,
+            "project_name": "test-project",
         }
         raise web.HTTPCreated
 
     app = web.Application()
     app.router.add_post("/secrets", handler)
 
     srv = await aiohttp_server(app)
@@ -65,26 +87,49 @@
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
         data = await request.json()
         assert data == {
             "key": "name",
             "value": base64.b64encode(b"data").decode("ascii"),
             "org_name": "test-org",
+            "project_name": "test-project",
         }
         raise web.HTTPCreated
 
     app = web.Application()
     app.router.add_post("/secrets", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.secrets.add("name", b"data", org_name="test-org")
 
 
+async def test_add_with_project(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    async def handler(request: web.Request) -> web.Response:
+        data = await request.json()
+        assert data == {
+            "key": "name",
+            "value": base64.b64encode(b"data").decode("ascii"),
+            "org_name": None,
+            "project_name": "project",
+        }
+        raise web.HTTPCreated
+
+    app = web.Application()
+    app.router.add_post("/secrets", handler)
+
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        await client.secrets.add("name", b"data", project_name="project")
+
+
 async def test_rm(aiohttp_server: _TestServerFactory, make_client: _MakeClient) -> None:
     async def handler(request: web.Request) -> web.Response:
         assert request.match_info["key"] == "name"
         raise web.HTTPNoContent
 
     app = web.Application()
     app.router.add_delete("/secrets/{key}", handler)
@@ -106,7 +151,24 @@
     app = web.Application()
     app.router.add_delete("/secrets/{key}", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.secrets.rm("name", org_name="test-org")
+
+
+async def test_rm_with_project(
+    aiohttp_server: _TestServerFactory, make_client: _MakeClient
+) -> None:
+    async def handler(request: web.Request) -> web.Response:
+        assert request.match_info["key"] == "name"
+        assert request.query.get("project_name") == "project"
+        raise web.HTTPNoContent
+
+    app = web.Application()
+    app.router.add_delete("/secrets/{key}", handler)
+
+    srv = await aiohttp_server(app)
+
+    async with make_client(srv.make_url("/")) as client:
+        await client.secrets.rm("name", project_name="project")
```

### Comparing `neuro-sdk-23.2.0/tests/test_storage.py` & `neuro-sdk-23.7.0/tests/test_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     return ret
 
 
 @pytest.fixture
 async def storage_server(
     aiohttp_raw_server: _RawTestServerFactory, storage_path: Path
 ) -> Any:
-    PREFIX = "/storage/user"
+    PREFIX = "/storage/test-project"
     PREFIX_LEN = len(PREFIX)
 
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
         op = request.query["op"]
         path = request.path
         assert path.startswith(PREFIX)
@@ -213,56 +213,56 @@
                 },
             ]
         }
     }
 
     async def handler(request: web.Request) -> web.Response:
         assert "b3" in request.headers
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "LISTSTATUS"}
         return web.json_response(JSON)
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", handler)
+    app.router.add_get("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     expected = [
         FileStatus(
             path="foo",
             size=1024,
             type=FileStatusType.FILE,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/foo"),
+            uri=URL("storage://default/test-project/folder/foo"),
         ),
         FileStatus(
             path="bar",
             size=4 * 1024,
             type=FileStatusType.DIRECTORY,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/bar"),
+            uri=URL("storage://default/test-project/folder/bar"),
         ),
         FileStatus(
             path="baz",
             size=1,
             type=FileStatusType.SYMLINK,
             modification_time=0,
             permission=Action.READ,
             target="foo",
-            uri=URL("storage://default/user/folder/baz"),
+            uri=URL("storage://default/test-project/folder/baz"),
         ),
         FileStatus(
             path="spam",
             size=1,
             type=FileStatusType.UNKNOWN,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/spam"),
+            uri=URL("storage://default/test-project/folder/spam"),
         ),
     ]
 
     async with make_client(srv.make_url("/")) as client:
         async with client.storage.list(URL("storage:folder")) as it:
             ret = [file async for file in it]
             assert ret == expected
@@ -314,115 +314,122 @@
             "modificationTime": 0,
             "permission": "read",
         },
     ]
 
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "LISTSTATUS"}
         return await make_listiter_response(request, file_statuses)
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", handler)
+    app.router.add_get("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         async with client.storage.list(URL("storage:folder")) as it:
             ret = [file async for file in it]
 
     assert ret == [
         FileStatus(
             path="foo",
             size=1024,
             type=FileStatusType.FILE,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/foo"),
+            uri=URL("storage://default/test-project/folder/foo"),
         ),
         FileStatus(
             path="bar",
             size=4 * 1024,
             type=FileStatusType.DIRECTORY,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/bar"),
+            uri=URL("storage://default/test-project/folder/bar"),
         ),
         FileStatus(
             path="baz",
             size=1,
             type=FileStatusType.SYMLINK,
             modification_time=0,
             permission=Action.READ,
             target="foo",
-            uri=URL("storage://default/user/folder/baz"),
+            uri=URL("storage://default/test-project/folder/baz"),
         ),
         FileStatus(
             path="spam",
             size=1,
             type=FileStatusType.UNKNOWN,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder/spam"),
+            uri=URL("storage://default/test-project/folder/spam"),
         ),
     ]
 
 
+async def test_storage_ls_without_project(make_client: _MakeClient) -> None:
+    async with make_client("https://example.com", projects={}) as client:
+        with pytest.raises(RuntimeError, match="The current project is not selected"):
+            async with client.storage.list(URL("storage:folder")) as it:
+                [file async for file in it]
+
+
 async def test_storage_disk_usage(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/user"
+        assert request.path == "/storage/test-project"
         assert request.query == {"op": "GETDISKUSAGE"}
         return web.json_response({"total": 100, "used": 20, "free": 80})
 
     app = web.Application()
-    app.router.add_get("/storage/user", handler)
+    app.router.add_get("/storage/test-project", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         res = await client.storage.disk_usage()
 
     assert res == DiskUsageInfo(total=100, used=20, free=80, cluster_name="default")
 
 
 async def test_storage_disk_usage_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage2/user"
+        assert request.path == "/storage2/test-project"
         assert request.query == {"op": "GETDISKUSAGE"}
         return web.json_response({"total": 100, "used": 20, "free": 80})
 
     app = web.Application()
-    app.router.add_get("/storage2/user", handler)
+    app.router.add_get("/storage2/test-project", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         res = await client.storage.disk_usage(cluster_name="another")
 
     assert res == DiskUsageInfo(total=100, used=20, free=80, cluster_name="another")
 
 
 async def test_storage_disk_usage_another_org(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/org/user"
+        assert request.path == "/storage/org/test-project"
         assert request.query == {"op": "GETDISKUSAGE"}
         return web.json_response({"total": 100, "used": 20, "free": 80})
 
     app = web.Application()
-    app.router.add_get("/storage/org/user", handler)
+    app.router.add_get("/storage/org/test-project", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         res = await client.storage.disk_usage(org_name="org")
 
     assert res == DiskUsageInfo(
@@ -431,20 +438,20 @@
 
 
 async def test_storage_disk_usage_path(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/user/dir"
+        assert request.path == "/storage/test-project/dir"
         assert request.query == {"op": "GETDISKUSAGE"}
         return web.json_response({"total": 100, "used": 20, "free": 80})
 
     app = web.Application()
-    app.router.add_get("/storage/user/dir", handler)
+    app.router.add_get("/storage/test-project/dir", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         res = await client.storage.disk_usage(uri=URL("storage:dir"))
 
     assert res == DiskUsageInfo(
@@ -485,81 +492,83 @@
             "modificationTime": 0,
             "permission": "read",
         },
     ]
 
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage2/user/folder"
+        assert request.path == "/storage2/test-project/folder"
         assert request.query == {"op": "LISTSTATUS"}
         return await make_listiter_response(request, file_statuses)
 
     app = web.Application()
-    app.router.add_get("/storage2/user/folder", handler)
+    app.router.add_get("/storage2/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        async with client.storage.list(URL("storage://another/user/folder")) as it:
+        async with client.storage.list(
+            URL("storage://another/test-project/folder")
+        ) as it:
             ret = [file async for file in it]
 
     assert ret == [
         FileStatus(
             path="foo",
             size=1024,
             type=FileStatusType.FILE,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://another/user/folder/foo"),
+            uri=URL("storage://another/test-project/folder/foo"),
         ),
         FileStatus(
             path="bar",
             size=4 * 1024,
             type=FileStatusType.DIRECTORY,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://another/user/folder/bar"),
+            uri=URL("storage://another/test-project/folder/bar"),
         ),
         FileStatus(
             path="baz",
             size=1,
             type=FileStatusType.SYMLINK,
             modification_time=0,
             permission=Action.READ,
             target="foo",
-            uri=URL("storage://another/user/folder/baz"),
+            uri=URL("storage://another/test-project/folder/baz"),
         ),
         FileStatus(
             path="spam",
             size=1,
             type=FileStatusType.UNKNOWN,
             modification_time=0,
             permission=Action.READ,
-            uri=URL("storage://another/user/folder/spam"),
+            uri=URL("storage://another/test-project/folder/spam"),
         ),
     ]
 
 
 async def test_storage_ls_error_in_server_response(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     error_result = {"error": "Server is to busy", "errno": "EBUSY"}
 
     async def handler(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "LISTSTATUS"}
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(error_result).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", handler)
+    app.router.add_get("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(OSError) as err:
             async with client.storage.list(URL("storage:folder")) as it:
                 async for _ in it:
@@ -569,15 +578,15 @@
 
 
 async def test_storage_glob(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler_home(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path == "/storage/user"
+        assert request.path == "/storage/test-project"
         assert request.query == {"op": "LISTSTATUS"}
         return await make_listiter_response(
             request,
             [
                 {
                     "path": "folder",
                     "length": 0,
@@ -586,21 +595,21 @@
                     "permission": "read",
                 }
             ],
         )
 
     async def handler_folder(request: web.Request) -> web.StreamResponse:
         assert "b3" in request.headers
-        assert request.path.rstrip("/") == "/storage/user/folder"
+        assert request.path.rstrip("/") == "/storage/test-project/folder"
         assert request.query["op"] in ("GETFILESTATUS", "LISTSTATUS")
         if request.query["op"] == "GETFILESTATUS":
             return web.json_response(
                 {
                     "FileStatus": {
-                        "path": "/user/folder",
+                        "path": "/test-project/folder",
                         "type": "DIRECTORY",
                         "length": 0,
                         "modificationTime": 0,
                         "permission": "read",
                     }
                 }
             )
@@ -625,35 +634,35 @@
                 ],
             )
         else:
             raise web.HTTPInternalServerError
 
     async def handler_foo(request: web.Request) -> web.Response:
         assert "b3" in request.headers
-        assert request.path == "/storage/user/folder/foo"
+        assert request.path == "/storage/test-project/folder/foo"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder/foo",
+                    "path": "/test-project/folder/foo",
                     "length": 1024,
                     "type": "FILE",
                     "modificationTime": 0,
                     "permission": "read",
                 }
             }
         )
 
     async def handler_bar(request: web.Request) -> web.StreamResponse:
-        assert request.path.rstrip("/") == "/storage/user/folder/bar"
+        assert request.path.rstrip("/") == "/storage/test-project/folder/bar"
         if request.query["op"] == "GETFILESTATUS":
             return web.json_response(
                 {
                     "FileStatus": {
-                        "path": "/user/folder/bar",
+                        "path": "/test-project/folder/bar",
                         "length": 0,
                         "type": "DIRECTORY",
                         "modificationTime": 0,
                         "permission": "read",
                     }
                 }
             )
@@ -670,22 +679,22 @@
                     }
                 ],
             )
         else:
             raise web.HTTPInternalServerError
 
     app = web.Application()
-    app.router.add_get("/storage/user", handler_home)
-    app.router.add_get("/storage/user/", handler_home)
-    app.router.add_get("/storage/user/folder", handler_folder)
-    app.router.add_get("/storage/user/folder/", handler_folder)
-    app.router.add_get("/storage/user/folder/foo", handler_foo)
-    app.router.add_get("/storage/user/folder/foo/", handler_foo)
-    app.router.add_get("/storage/user/folder/bar", handler_bar)
-    app.router.add_get("/storage/user/folder/bar/", handler_bar)
+    app.router.add_get("/storage/test-project", handler_home)
+    app.router.add_get("/storage/test-project/", handler_home)
+    app.router.add_get("/storage/test-project/folder", handler_folder)
+    app.router.add_get("/storage/test-project/folder/", handler_folder)
+    app.router.add_get("/storage/test-project/folder/foo", handler_foo)
+    app.router.add_get("/storage/test-project/folder/foo/", handler_foo)
+    app.router.add_get("/storage/test-project/folder/bar", handler_bar)
+    app.router.add_get("/storage/test-project/folder/bar/", handler_bar)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
 
         async def glob(pattern: str) -> List[URL]:
             async with client.storage.glob(URL(pattern)) as it:
@@ -722,189 +731,191 @@
         ]
         assert await glob("storage:**/b*/") == [URL("storage:folder/bar/")]
 
 
 async def test_storage_rm_file(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    remove_listing = {"path": "/user/file", "is_dir": False}
+    remove_listing = {"path": "/test-project/file", "is_dir": False}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(remove_listing).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage/user/file", delete_handler)
+    app.router.add_delete("/storage/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.rm(URL("storage:file"))
 
 
 async def test_storage_rm_file_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    remove_listing = {"path": "/user/file", "is_dir": False}
+    remove_listing = {"path": "/test-project/file", "is_dir": False}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage2/user/file"
+        assert request.path == "/storage2/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(remove_listing).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage2/user/file", delete_handler)
+    app.router.add_delete("/storage2/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        await client.storage.rm(URL("storage://another/user/file"))
+        await client.storage.rm(URL("storage://another/test-project/file"))
 
 
 async def test_storage_rm_file_progress(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    remove_listing = {"path": "/user/file", "is_dir": False}
+    remove_listing = {"path": "/test-project/file", "is_dir": False}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(remove_listing).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage/user/file", delete_handler)
+    app.router.add_delete("/storage/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     progress = mock.Mock()
     async with make_client(srv.make_url("/")) as client:
         await client.storage.rm(URL("storage:file"), progress=progress)
 
     progress.delete.assert_called_with(
         StorageProgressDelete(
-            uri=URL("storage://default/user/file"),
+            uri=URL("storage://default/test-project/file"),
             is_dir=False,
         )
     )
 
 
 async def test_storage_rm_file_progress_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    remove_listing = {"path": "/user/file", "is_dir": False}
+    remove_listing = {"path": "/test-project/file", "is_dir": False}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage2/user/file"
+        assert request.path == "/storage2/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(remove_listing).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage2/user/file", delete_handler)
+    app.router.add_delete("/storage2/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     progress = mock.Mock()
     async with make_client(srv.make_url("/")) as client:
-        await client.storage.rm(URL("storage://another/user/file"), progress=progress)
+        await client.storage.rm(
+            URL("storage://another/test-project/file"), progress=progress
+        )
 
     progress.delete.assert_called_with(
         StorageProgressDelete(
-            uri=URL("storage://another/user/file"),
+            uri=URL("storage://another/test-project/file"),
             is_dir=False,
         )
     )
 
 
 async def test_storage_rm_directory(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def delete_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         return web.json_response(
             {"error": "Target is a directory", "errno": "EISDIR"},
             status=web.HTTPBadRequest.status_code,
         )
 
     app = web.Application()
-    app.router.add_delete("/storage/user/folder", delete_handler)
+    app.router.add_delete("/storage/test-project/folder", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(IsADirectoryError, match="Target is a directory") as cm:
             await client.storage.rm(URL("storage:folder"))
         assert cm.value.errno == errno.EISDIR
 
 
 async def test_storage_rm_recursive(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     remove_listing = {
-        "path": "/user/folder",
+        "path": "/test-project/folder",
         "is_dir": True,
     }
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "DELETE", "recursive": "true"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(remove_listing).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage/user/folder", delete_handler)
+    app.router.add_delete("/storage/test-project/folder", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.rm(URL("storage:folder"), recursive=True)
 
 
 async def test_storage_rm_oserror_in_the_response_stream(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     error_result = {"error": "Server is to busy", "errno": "EBUSY"}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(error_result).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage/user/file", delete_handler)
+    app.router.add_delete("/storage/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(OSError) as err:
             await client.storage.rm(URL("storage:file"))
         assert err.value.strerror == "Server is to busy"
@@ -913,239 +924,242 @@
 
 async def test_storage_rm_generic_error_in_the_response_stream(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     error_result = {"error": "Server failed", "errno": None}
 
     async def delete_handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "DELETE", "recursive": "false"}
         assert request.headers["Accept"] == "application/x-ndjson"
         resp = web.StreamResponse()
         resp.headers["Content-Type"] = "application/x-ndjson"
         await resp.prepare(request)
         await resp.write(json.dumps(error_result).encode() + b"\n")
         return resp
 
     app = web.Application()
-    app.router.add_delete("/storage/user/file", delete_handler)
+    app.router.add_delete("/storage/test-project/file", delete_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(Exception) as err:
             await client.storage.rm(URL("storage:file"))
         assert err.value.args[0] == "Server failed"
 
 
 async def test_storage_mv(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
-        assert request.query == {"op": "RENAME", "destination": "/user/other"}
+        assert request.path == "/storage/test-project/folder"
+        assert request.query == {"op": "RENAME", "destination": "/test-project/other"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_post("/storage/user/folder", handler)
+    app.router.add_post("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mv(URL("storage:folder"), URL("storage:other"))
 
 
 async def test_storage_mv_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage2/user/folder"
-        assert request.query == {"op": "RENAME", "destination": "/user/other"}
+        assert request.path == "/storage2/test-project/folder"
+        assert request.query == {"op": "RENAME", "destination": "/test-project/other"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_post("/storage2/user/folder", handler)
+    app.router.add_post("/storage2/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mv(
-            URL("storage://another/user/folder"), URL("storage://another/user/other")
+            URL("storage://another/test-project/folder"),
+            URL("storage://another/test-project/other"),
         )
 
 
 async def test_storage_mv_different_clusters(make_client: _MakeClient) -> None:
     async with make_client("https://example.com") as client:
         with pytest.raises(ValueError, match="Cannot move cross-cluster"):
             await client.storage.mv(
-                URL("storage:folder"), URL("storage://another/user/other")
+                URL("storage:folder"), URL("storage://another/test-project/other")
             )
         with pytest.raises(ValueError, match="Cannot move cross-cluster"):
             await client.storage.mv(
-                URL("storage://another/user/folder"), URL("storage:other")
+                URL("storage://another/test-project/folder"), URL("storage:other")
             )
 
 
 async def test_storage_mv_unknown_cluster(make_client: _MakeClient) -> None:
     async with make_client("https://example.com") as client:
         with pytest.raises(
             RuntimeError,
             match="Cluster unknown doesn't exist in a list of available clusters",
         ):
             await client.storage.mv(
-                URL("storage://unknown/user/folder"),
-                URL("storage://unknown/user/other"),
+                URL("storage://unknown/test-project/folder"),
+                URL("storage://unknown/test-project/other"),
             )
 
 
 async def test_storage_mkdir_parents_exist_ok(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "MKDIRS"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_put("/storage/user/folder/sub", handler)
+    app.router.add_put("/storage/test-project/folder/sub", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mkdir(
             URL("storage:folder/sub"), parents=True, exist_ok=True
         )
 
 
 async def test_storage_mkdir_parents_exist_ok_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage2/user/folder/sub"
+        assert request.path == "/storage2/test-project/folder/sub"
         assert request.query == {"op": "MKDIRS"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_put("/storage2/user/folder/sub", handler)
+    app.router.add_put("/storage2/test-project/folder/sub", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mkdir(
-            URL("storage://another/user/folder/sub"), parents=True, exist_ok=True
+            URL("storage://another/test-project/folder/sub"),
+            parents=True,
+            exist_ok=True,
         )
 
 
 async def test_storage_mkdir_parents(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def get_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.Response(status=404)
 
     async def put_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "MKDIRS"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder/sub", get_handler)
-    app.router.add_put("/storage/user/folder/sub", put_handler)
+    app.router.add_get("/storage/test-project/folder/sub", get_handler)
+    app.router.add_put("/storage/test-project/folder/sub", put_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mkdir(URL("storage:folder/sub"), parents=True)
 
 
 async def test_storage_mkdir_exist_ok(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def get_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder",
+                    "path": "/test-project/folder",
                     "type": "DIRECTORY",
                     "length": 1234,
                     "modificationTime": 3456,
                     "permission": "read",
                 }
             }
         )
 
     async def put_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "MKDIRS"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", get_handler)
-    app.router.add_put("/storage/user/folder/sub", put_handler)
+    app.router.add_get("/storage/test-project/folder", get_handler)
+    app.router.add_put("/storage/test-project/folder/sub", put_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mkdir(URL("storage:folder/sub"), exist_ok=True)
 
 
 async def test_storage_mkdir(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def get_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.Response(status=404)
 
     async def parent_get_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder",
+                    "path": "/test-project/folder",
                     "type": "DIRECTORY",
                     "length": 1234,
                     "modificationTime": 3456,
                     "permission": "read",
                 }
             }
         )
 
     async def put_handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder/sub"
+        assert request.path == "/storage/test-project/folder/sub"
         assert request.query == {"op": "MKDIRS"}
         return web.Response(status=204)
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder/sub", get_handler)
-    app.router.add_get("/storage/user/folder", parent_get_handler)
-    app.router.add_put("/storage/user/folder/sub", put_handler)
+    app.router.add_get("/storage/test-project/folder/sub", get_handler)
+    app.router.add_get("/storage/test-project/folder", parent_get_handler)
+    app.router.add_put("/storage/test-project/folder/sub", put_handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.mkdir(URL("storage:folder/sub"))
 
 
 async def test_storage_create(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "CREATE"}
         content = await request.read()
         assert content == b"01234"
         return web.Response(status=201)
 
     app = web.Application()
-    app.router.add_put("/storage/user/file", handler)
+    app.router.add_put("/storage/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async def gen() -> AsyncIterator[bytes]:
         for i in range(5):
             yield str(i).encode("ascii")
 
@@ -1153,198 +1167,200 @@
         await client.storage.create(URL("storage:file"), gen())
 
 
 async def test_storage_create_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage2/user/file"
+        assert request.path == "/storage2/test-project/file"
         assert request.query == {"op": "CREATE"}
         content = await request.read()
         assert content == b"01234"
         return web.Response(status=201)
 
     app = web.Application()
-    app.router.add_put("/storage2/user/file", handler)
+    app.router.add_put("/storage2/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async def gen() -> AsyncIterator[bytes]:
         for i in range(5):
             yield str(i).encode("ascii")
 
     async with make_client(srv.make_url("/")) as client:
-        await client.storage.create(URL("storage://another/user/file"), gen())
+        await client.storage.create(URL("storage://another/test-project/file"), gen())
 
 
 async def test_storage_write(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         assert request.query == {"op": "WRITE"}
         rng = _parse_content_range(request.headers.get("Content-Range"))
         assert rng == slice(4, 9)
         content = await request.read()
         assert content == b"01234"
         return web.Response(status=200)
 
     app = web.Application()
-    app.router.add_patch("/storage/user/file", handler)
+    app.router.add_patch("/storage/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         await client.storage.write(URL("storage:file"), b"01234", 4)
 
 
 async def test_storage_write_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage2/user/file"
+        assert request.path == "/storage2/test-project/file"
         assert request.query == {"op": "WRITE"}
         rng = _parse_content_range(request.headers.get("Content-Range"))
         assert rng == slice(4, 9)
         content = await request.read()
         assert content == b"01234"
         return web.Response(status=200)
 
     app = web.Application()
-    app.router.add_patch("/storage2/user/file", handler)
+    app.router.add_patch("/storage2/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        await client.storage.write(URL("storage://another/user/file"), b"01234", 4)
+        await client.storage.write(
+            URL("storage://another/test-project/file"), b"01234", 4
+        )
 
 
 async def test_storage_stats(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder",
+                    "path": "/test-project/folder",
                     "type": "DIRECTORY",
                     "length": 1234,
                     "modificationTime": 3456,
                     "permission": "read",
                 }
             }
         )
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", handler)
+    app.router.add_get("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         stats = await client.storage.stat(URL("storage:folder"))
         assert stats == FileStatus(
-            path="/user/folder",
+            path="/test-project/folder",
             type=FileStatusType.DIRECTORY,
             size=1234,
             modification_time=3456,
             permission=Action.READ,
-            uri=URL("storage://default/user/folder"),
+            uri=URL("storage://default/test-project/folder"),
         )
 
 
 async def test_storage_stats_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage2/user/folder"
+        assert request.path == "/storage2/test-project/folder"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder",
+                    "path": "/test-project/folder",
                     "type": "DIRECTORY",
                     "length": 1234,
                     "modificationTime": 3456,
                     "permission": "read",
                 }
             }
         )
 
     app = web.Application()
-    app.router.add_get("/storage2/user/folder", handler)
+    app.router.add_get("/storage2/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
-        stats = await client.storage.stat(URL("storage://another/user/folder"))
+        stats = await client.storage.stat(URL("storage://another/test-project/folder"))
         assert stats == FileStatus(
-            path="/user/folder",
+            path="/test-project/folder",
             type=FileStatusType.DIRECTORY,
             size=1234,
             modification_time=3456,
             permission=Action.READ,
-            uri=URL("storage://another/user/folder"),
+            uri=URL("storage://another/test-project/folder"),
         )
 
 
 async def test_storage_stats_symlink(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/link"
+        assert request.path == "/storage/test-project/link"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/link",
+                    "path": "/test-project/link",
                     "type": "SYMLINK",
                     "length": 1234,
                     "modificationTime": 3456,
                     "permission": "read",
                     "target": "folder/subfolder/file",
                 }
             }
         )
 
     app = web.Application()
-    app.router.add_get("/storage/user/link", handler)
+    app.router.add_get("/storage/test-project/link", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         stats = await client.storage.stat(URL("storage:link"))
         assert stats == FileStatus(
-            path="/user/link",
+            path="/test-project/link",
             type=FileStatusType.SYMLINK,
             size=1234,
             modification_time=3456,
             permission=Action.READ,
             target="folder/subfolder/file",
-            uri=URL("storage://default/user/link"),
+            uri=URL("storage://default/test-project/link"),
         )
 
 
 async def test_storage_open(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         if request.query["op"] == "OPEN":
             resp = web.StreamResponse()
             await resp.prepare(request)
             for i in range(5):
                 await resp.write(str(i).encode("ascii"))
             return resp
         else:
             raise AssertionError(f"Unknown operation {request.query['op']}")
 
     app = web.Application()
-    app.router.add_get("/storage/user/file", handler)
+    app.router.add_get("/storage/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         buf = bytearray()
         async with client.storage.open(URL("storage:file")) as it:
             async for chunk in it:
@@ -1352,56 +1368,58 @@
         assert buf == b"01234"
 
 
 async def test_storage_open_another_cluster(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage2/user/file"
+        assert request.path == "/storage2/test-project/file"
         if request.query["op"] == "OPEN":
             resp = web.StreamResponse()
             await resp.prepare(request)
             for i in range(5):
                 await resp.write(str(i).encode("ascii"))
             return resp
         else:
             raise AssertionError(f"Unknown operation {request.query['op']}")
 
     app = web.Application()
-    app.router.add_get("/storage2/user/file", handler)
+    app.router.add_get("/storage2/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         buf = bytearray()
-        async with client.storage.open(URL("storage://another/user/file")) as it:
+        async with client.storage.open(
+            URL("storage://another/test-project/file")
+        ) as it:
             async for chunk in it:
                 buf.extend(chunk)
         assert buf == b"01234"
 
 
 async def test_storage_open_partial_read(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         if request.query["op"] == "OPEN":
             rng = request.http_range
             data = b"ababahalamaha"
             start, stop, _ = rng.indices(len(data))
             return web.Response(
                 status=web.HTTPPartialContent.status_code,
                 headers={"Content-Range": f"bytes {start}-{stop-1}/{len(data)}"},
                 body=data[start:stop],
             )
         else:
             raise AssertionError(f"Unknown operation {request.query['op']}")
 
     app = web.Application()
-    app.router.add_get("/storage/user/file", handler)
+    app.router.add_get("/storage/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         buf = bytearray()
         async with client.storage.open(URL("storage:file"), 5) as it:
             async for chunk in it:
@@ -1427,26 +1445,26 @@
         assert buf == b""
 
 
 async def test_storage_open_unsupported_partial_read(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.StreamResponse:
-        assert request.path == "/storage/user/file"
+        assert request.path == "/storage/test-project/file"
         if request.query["op"] == "OPEN":
             resp = web.StreamResponse()
             await resp.prepare(request)
             for i in range(5):
                 await resp.write(str(i).encode("ascii"))
             return resp
         else:
             raise AssertionError(f"Unknown operation {request.query['op']}")
 
     app = web.Application()
-    app.router.add_get("/storage/user/file", handler)
+    app.router.add_get("/storage/test-project/file", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         buf = bytearray()
         async with client.storage.open(URL("storage:file"), 0) as it:
             async for chunk in it:
@@ -1459,30 +1477,30 @@
                     pass
 
 
 async def test_storage_open_directory(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     async def handler(request: web.Request) -> web.Response:
-        assert request.path == "/storage/user/folder"
+        assert request.path == "/storage/test-project/folder"
         assert request.query == {"op": "GETFILESTATUS"}
         return web.json_response(
             {
                 "FileStatus": {
-                    "path": "/user/folder",
+                    "path": "/test-project/folder",
                     "type": "DIRECTORY",
                     "length": 5,
                     "modificationTime": 3456,
                     "permission": "read",
                 }
             }
         )
 
     app = web.Application()
-    app.router.add_get("/storage/user/folder", handler)
+    app.router.add_get("/storage/test-project/folder", handler)
 
     srv = await aiohttp_server(app)
 
     async with make_client(srv.make_url("/")) as client:
         buf = bytearray()
         with pytest.raises((IsADirectoryError, IllegalArgumentError)):
             async with client.storage.open(URL("storage:folder")) as it:
@@ -1528,15 +1546,15 @@
             URL(file_path.as_uri()), URL("storage:file.txt"), progress=progress
         )
 
     uploaded = target_path.read_bytes()
     assert uploaded == b""
 
     src = URL(file_path.as_uri())
-    dst = URL("storage://default/user/file.txt")
+    dst = URL("storage://default/test-project/file.txt")
     progress.start.assert_called_with(StorageProgressStart(src, dst, 0))
     progress.step.assert_not_called()
     progress.complete.assert_called_with(StorageProgressComplete(src, dst, 0))
 
 
 async def test_storage_upload_regular_file_to_existing_file_target(
     storage_server: Any,
@@ -1555,15 +1573,15 @@
         )
 
     expected = file_path.read_bytes()
     uploaded = target_path.read_bytes()
     assert uploaded == expected
 
     src = URL(file_path.as_uri())
-    dst = URL("storage://default/user/file.txt")
+    dst = URL("storage://default/test-project/file.txt")
     progress.start.assert_called_with(StorageProgressStart(src, dst, file_size))
     progress.step.assert_called_with(
         StorageProgressStep(src, dst, file_size, file_size)
     )
     progress.complete.assert_called_with(StorageProgressComplete(src, dst, file_size))
 
 
@@ -1744,15 +1762,15 @@
             URL("storage:file.txt"), URL(local_file.as_uri()), progress=progress
         )
 
     expected = src_file.read_bytes()
     downloaded = local_file.read_bytes()
     assert downloaded == expected
 
-    src = URL("storage://default/user/file.txt")
+    src = URL("storage://default/test-project/file.txt")
     dst = URL(local_file.as_uri())
     file_size = src_file.stat().st_size
     progress.start.assert_called_with(StorageProgressStart(src, dst, file_size))
     progress.step.assert_called_with(
         StorageProgressStep(src, dst, file_size, file_size)
     )
     progress.complete.assert_called_with(StorageProgressComplete(src, dst, file_size))
```

### Comparing `neuro-sdk-23.2.0/tests/test_storage_filestatus.py` & `neuro-sdk-23.7.0/tests/test_storage_filestatus.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_tools.py` & `neuro-sdk-23.7.0/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_url_utils.py` & `neuro-sdk-23.7.0/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_users.py` & `neuro-sdk-23.7.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `neuro-sdk-23.2.0/tests/test_version_check.py` & `neuro-sdk-23.7.0/tests/test_version_check.py`

 * *Files identical despite different names*

