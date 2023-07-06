# Comparing `tmp/neuro-cli-23.2.0.tar.gz` & `tmp/neuro-cli-23.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-cli-23.2.0.tar", last modified: Mon Feb 20 23:18:38 2023, max compression
+gzip compressed data, was "neuro-cli-23.7.0.tar", last modified: Thu Jul  6 19:40:57 2023, max compression
```

## Comparing `neuro-cli-23.2.0.tar` & `neuro-cli-23.7.0.tar`

### file list

```diff
@@ -1,798 +1,813 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.430820 neuro-cli-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89475 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-20 23:18:38.430820 neuro-cli-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-02-20 23:18:38.430820 neuro-cli-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.230818 neuro-cli-23.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.238818 neuro-cli-23.2.0/src/neuro_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56275 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/ael.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/asyncio_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    36988 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/click_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/disks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/docker_credential_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/file_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.242818 neuro-cli-23.2.0/src/neuro_cli/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17863 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/bucket_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/disks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    35512 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29186 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/formatters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    42554 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/share.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    25916 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/src/neuro_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.242818 neuro-cli-23.2.0/src/neuro_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49882 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 23:17:54.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 23:18:38.000000 neuro-cli-23.2.0/src/neuro_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.242818 neuro-cli-23.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.246818 neuro-cli-23.2.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.246818 neuro-cli-23.2.0/tests/e2e/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/assets/echo-tag.tar
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/clear-all-my-permissions.sh
--rw-r--r--   0 runner    (1001) docker     (123)    36166 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    39074 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_share.py
--rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/test_e2e_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/e2e/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.250818 neuro-cli-23.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.382820 neuro-cli-23.2.0/tests/unit/ascii/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_delete_progress[True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_fail[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-False-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[False-True-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-False-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-False-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-False]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_10.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_11.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_12.ref
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_nested[True-True-True-True]_9.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[False-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-False-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-False-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-False]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/ascii/test_progress[True-True-True-True]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)    14497 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.386820 neuro-cli-23.2.0/tests/unit/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 23:18:38.430820 neuro-cli-23.2.0/tests/unit/formatters/ascii/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_zeroes_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestAliasesFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_rounding_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_5.ref
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_6.ref
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_7.ref
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_8.ref
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_cluster_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_finished_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_started_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_save_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter2]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter0]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter2]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_files_and_folders[formatter1]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_with_name_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_end_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_step_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_with_name_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_detach_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_kill_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_restart_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_step_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_detach_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[cancelled]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[failed]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[succeeded]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_kill_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_restart_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[pending]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[running]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[suspended]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestNonePainter.test_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_cpu_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_credits_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_gpu_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_jobs_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_zeroes_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_no_quota_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_spent_more_than_quota_left_zero_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_too_many_hours_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_empty_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_list_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[human]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[iso]_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_org_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/TestUsageFormatter.test_path_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_bucket_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_secrets_formatter_short_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_secrets_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_service_account_formatter_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/ascii/test_service_accounts_formatter_simple_0.ref
--rw-r--r--   0 runner    (1001) docker     (123)    16069 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_admin_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_blob_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_bucket_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_config_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_images_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    97131 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_jobs_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_storage_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/formatters/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_ael.py
--rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_click_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_click_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_docker_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_shell_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_storage_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-02-20 23:17:48.000000 neuro-cli-23.2.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:57.022117 neuro-cli-23.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    92203 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 19:40:57.022117 neuro-cli-23.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-06 19:40:57.022117 neuro-cli-23.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.778116 neuro-cli-23.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.790116 neuro-cli-23.7.0/src/neuro_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56931 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24482 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/ael.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/asyncio_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36757 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/click_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/docker_credential_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/file_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.798116 neuro-cli-23.7.0/src/neuro_cli/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/bucket_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35648 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29186 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/formatters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44170 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25962 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/src/neuro_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.794116 neuro-cli-23.7.0/src/neuro_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    51234 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:39:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 19:40:56.000000 neuro-cli-23.7.0/src/neuro_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.798116 neuro-cli-23.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.802116 neuro-cli-23.7.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.802116 neuro-cli-23.7.0/tests/e2e/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/assets/echo-tag.tar
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/clear-all-my-permissions.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    36492 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11563 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39074 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24817 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/test_e2e_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/e2e/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.810116 neuro-cli-23.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.922116 neuro-cli-23.7.0/tests/unit/ascii/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_delete_progress[True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_fail[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-False-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[False-True-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-False-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-False-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-False]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_10.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_11.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_12.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_nested[True-True-True-True]_9.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[False-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-False-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-False-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-False]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/ascii/test_progress[True-True-True-True]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:56.926116 neuro-cli-23.7.0/tests/unit/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:40:57.022117 neuro-cli-23.7.0/tests/unit/formatters/ascii/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestAdminQuotaFormatter.test_output_zeroes_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestAliasesFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[Eafxcxdxbxegedabagacad]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBSDPainter.test_coloring[exfxcxdxbxegedabagacad]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBalanceFormatter.test_output_rounding_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter0]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_5.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_6.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_7.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_8.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_with_current_project_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_no_user_info_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_without_project_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_quiet_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_finished_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_commit_started_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_pull_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_push_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestDockerImageProgress.test_tty_save_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_all_entities[formatter2]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter0]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_empty_files[formatter2]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestFilesFormatter.test_formatter_with_files_and_folders[formatter1]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.text=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[#star#.txt=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#fi=0;44#colon#no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[di=32;41#colon#no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestGnuPainter.test_coloring[no=0;46]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-test-user]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_begin_with_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_end_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_no_tty_step_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_quiet_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_begin_with_name_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_end[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStartProgress.test_tty_step[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_detach_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_kill_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_restart_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_no_tty_step_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_quiet_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_detach_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[cancelled]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[failed]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_end[succeeded]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_kill_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_restart_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[pending]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[running]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobStopProgress.test_tty_step[suspended]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_finished[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestLifeSpanUpdateFormatter.test_not_finished[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestNonePainter.test_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestOrgClusterFormatter.test_org_cluster_formatter_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_cpu_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_credits_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_gpu_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_only_jobs_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaFormatter.test_output_zeroes_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_no_quota_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_spent_more_than_quota_left_zero_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestQuotaInfoFormatter.test_output_too_many_hours_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_empty_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestSimpleJobsFormatter.test_list_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_custom_columns[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-0-owner-#less#you#more#]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[iso-1-alice-alice]_1.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[human]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_working_dir[iso]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestUsageFormatter.test_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestUsageFormatter.test_org_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/TestUsageFormatter.test_path_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_bucket_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_bucket_formatter_with_org_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disk_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_secrets_formatter_short_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_secrets_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_service_account_formatter[None]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_service_account_formatter[some-org]_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_service_account_formatter_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/ascii/test_service_accounts_formatter_simple_0.ref
+-rw-r--r--   0 runner    (1001) docker     (123)    16644 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_admin_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_blob_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_bucket_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_config_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_images_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100930 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_jobs_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_storage_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/formatters/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21084 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_ael.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_click_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_click_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_docker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58991 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_shell_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_storage_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32211 2023-07-06 19:39:48.000000 neuro-cli-23.7.0/tests/unit/test_utils.py
```

### Comparing `neuro-cli-23.2.0/CHANGELOG.md` & `neuro-cli-23.7.0/CHANGELOG.md`

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

### Comparing `neuro-cli-23.2.0/LICENSE` & `neuro-cli-23.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/PKG-INFO` & `neuro-cli-23.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-cli
-Version: 23.2.0
+Version: 23.7.0
 Summary: Neuro Platform client
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `neuro-cli-23.2.0/README.md` & `neuro-cli-23.7.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/setup.cfg` & `neuro-cli-23.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neuro-cli
-version = 23.2.0
+version = 23.7.0
 description = Neuro Platform client
 url = https://github.com/neuro-inc/platform-client-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Neu.ro Team
 author_email = team@neu.ro
 license = Apache 2
@@ -31,15 +31,15 @@
 packages = find:
 zip_safe = False
 python_requires = >=3.8.0
 include_package_data = True
 install_requires = 
 	python-jose>=3.0.0
 	python-dateutil>=2.7.0
-	neuro-sdk>=23.2.0
+	neuro-sdk>=23.7.0
 	click>=8.0
 	humanize>=3.3
 	typing_extensions>=3.7.4
 	certifi
 	wcwidth>=0.1.7
 	prompt-toolkit>=3.0.13
 	rich>=11.0.0
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/admin.py` & `neuro-cli-23.7.0/src/neuro_cli/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 from .click_types import MEMORY
 from .defaults import JOB_CPU_NUMBER, JOB_MEMORY_AMOUNT, PRESET_PRICE
 from .formatters.admin import (
     CloudProviderOptionsFormatter,
     ClustersFormatter,
     ClusterUserFormatter,
+    ClusterUserWithInfoFormatter,
     OrgClusterFormatter,
     OrgClustersFormatter,
     OrgsFormatter,
     OrgUserFormatter,
     ProjectFormatter,
     ProjectsFormatter,
     ProjectUserFormatter,
@@ -557,34 +558,45 @@
 @option(
     "--org",
     metavar="ORG",
     default=None,
     type=str,
     help="org name for org-cluster users",
 )
+@option(
+    "--details/--no-details",
+    default=False,
+    help="Include detailed user info",
+    is_flag=True,
+)
 @argument("cluster_name", required=False, default=None, type=str)
 async def get_cluster_users(
-    root: Root, org: Optional[str], cluster_name: Optional[str]
+    root: Root,
+    org: Optional[str],
+    details: bool,
+    cluster_name: Optional[str],
 ) -> None:
     """
     List users in specified cluster
     """
-    fmt = ClusterUserFormatter()
     cluster_name = cluster_name or root.client.config.cluster_name
     with root.status(
         f"Fetching the list of cluster users of cluster [b]{cluster_name}[/b]"
     ):
-        users = await root.client._admin.list_cluster_users(
+        users = await root.client._admin.list_cluster_users(  # type: ignore
             cluster_name=cluster_name,
-            with_user_info=True,
+            with_user_info=details,
             org_name=org,
         )
         users = sorted(users, key=lambda user: (user.user_name, user.org_name or ""))
     with root.pager():
-        root.print(fmt(users))
+        if details:
+            root.print(ClusterUserWithInfoFormatter()(users))
+        else:
+            root.print(ClusterUserFormatter()(users))
 
 
 @command()
 @argument("cluster_name", required=True, type=str)
 @argument("user_name", required=True, type=str)
 @argument(
     "role",
@@ -646,14 +658,15 @@
         cluster_name,
         user_name,
         _ClusterUserRoleType(role),
         org_name=org,
         balance=balance,
         quota=quota,
     )
+    assert user.role
     if not root.quiet:
         root.print(
             f"Added [bold]{rich_escape(user.user_name)}[/bold] to cluster "
             f"[bold]{rich_escape(cluster_name)}[/bold] as "
             + (
                 f"member of org [bold]{rich_escape(org)}[/bold] as "
                 if org is not None
@@ -1190,15 +1203,15 @@
 
 
 @command()
 @option("--force", default=False, help="Skip prompt", is_flag=True)
 @argument("org_name", required=True, type=str)
 async def remove_org(root: Root, org_name: str, force: bool) -> None:
     """
-    Drop a org
+    Drop an org
 
     Completely removes org from the system.
     """
     orgs = await root.client._admin.list_orgs()
     if not any(org.name == org_name for org in orgs):
         raise ValueError(f"Organization '{org_name}' is not found.")
 
@@ -1274,15 +1287,15 @@
             f"[bold]{rich_escape(org_name)}[/bold]",
             markup=True,
         )
 
 
 @command()
 @argument("cluster_name", required=True, type=str)
-async def get_org_clusters(root: Root, cluster_name: str) -> None:
+async def get_cluster_orgs(root: Root, cluster_name: str) -> None:
     """
     Print the list of all orgs in the cluster
     """
     fmt = OrgClustersFormatter()
     with root.status(f"Fetching the list of orgs of cluster [b]{cluster_name}[/b]"):
         org_clusters = await root.client._admin.list_org_clusters(
             cluster_name=cluster_name
@@ -1746,14 +1759,24 @@
             f"Added project [bold]{rich_escape(project.name)}[/bold] to cluster "
             f"[bold]{rich_escape(cluster_name)}[/bold]"
             f"{f' to org [bold]{rich_escape(org)}[/bold]' if org else ''}. Info:",
             markup=True,
         )
         fmt = ProjectFormatter()
         root.print(fmt(project, skip_cluster_org=True))
+    await root.client.config.fetch()
+    if (
+        not root.client.config.project_name
+        and root.client.cluster_name == project.cluster_name
+    ):
+        await root.client.config.switch_project(project.name)
+        root.print(
+            f"Selected [bold]{rich_escape(project.name)}[/bold] as current project.",
+            markup=True,
+        )
 
 
 @command()
 @argument("cluster_name", required=True, type=str)
 @argument("name", required=True, type=str)
 @option(
     "--org",
@@ -1804,15 +1827,15 @@
             f"updated. Info:",
             markup=True,
         )
         fmt = ProjectFormatter()
         root.print(fmt(project, skip_cluster_org=True))
 
 
-@command(hidden=True)
+@command()
 @option("--force", default=False, help="Skip prompt", is_flag=True)
 @argument("cluster_name", required=True, type=str)
 @argument("name", required=True, type=str)
 @option(
     "--org",
     metavar="ORG",
     default=None,
@@ -2027,15 +2050,15 @@
 admin.add_command(add_org)
 admin.add_command(remove_org)
 
 admin.add_command(get_org_users)
 admin.add_command(add_org_user)
 admin.add_command(remove_org_user)
 
-admin.add_command(get_org_clusters)
+admin.add_command(get_cluster_orgs)
 admin.add_command(add_org_cluster)
 admin.add_command(update_org_cluster)
 admin.add_command(remove_org_cluster)
 
 admin.add_command(set_org_cluster_defaults)
 admin.add_command(get_org_cluster_quota)
 admin.add_command(set_org_cluster_quota)
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/ael.py` & `neuro-cli-23.7.0/src/neuro_cli/ael.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/alias.py` & `neuro-cli-23.7.0/src/neuro_cli/alias.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/asyncio_utils.py` & `neuro-cli-23.7.0/src/neuro_cli/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/blob_storage.py` & `neuro-cli-23.7.0/src/neuro_cli/blob_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,64 +4,62 @@
 from typing import Awaitable, Callable, List, Optional, Sequence, Tuple
 
 import click
 from rich.text import Text
 from yarl import URL
 
 from neuro_sdk import (
+    ORG_NAME_SENTINEL,
     Bucket,
     Client,
     FileFilter,
     FileStatusType,
     IllegalArgumentError,
     ResourceNotFound,
 )
 
-from neuro_cli.click_types import (
+from .click_types import (
     BUCKET,
     BUCKET_CREDENTIAL,
     BUCKET_NAME,
     CLUSTER,
     ORG,
+    PROJECT,
     PlatformURIType,
 )
-from neuro_cli.formatters.bucket_credentials import (
+from .const import EX_OSFILE
+from .formatters.blob_storage import (
+    BaseBlobFormatter,
+    LongBlobFormatter,
+    SimpleBlobFormatter,
+)
+from .formatters.bucket_credentials import (
     BaseBucketCredentialsFormatter,
     BucketCredentialFormatter,
     BucketCredentialsFormatter,
     SimpleBucketCredentialsFormatter,
 )
-from neuro_cli.formatters.buckets import (
+from .formatters.buckets import (
     BaseBucketsFormatter,
     BucketFormatter,
     BucketsFormatter,
     SimpleBucketsFormatter,
 )
-from neuro_cli.formatters.utils import (
-    URIFormatter,
-    get_datetime_formatter,
-    uri_formatter,
-)
-from neuro_cli.parse_utils import parse_timedelta
-from neuro_cli.utils import format_size, parse_org_name
-
-from .const import EX_OSFILE
-from .formatters.blob_storage import (
-    BaseBlobFormatter,
-    LongBlobFormatter,
-    SimpleBlobFormatter,
-)
 from .formatters.storage import DeleteProgress, create_storage_progress, get_painter
+from .formatters.utils import URIFormatter, get_datetime_formatter, uri_formatter
+from .parse_utils import parse_timedelta
 from .root import Root
 from .storage import calc_filters, calc_ignore_file_names, filter_option
 from .utils import (
     argument,
     command,
+    format_size,
     group,
     option,
+    parse_org_name,
     resolve_bucket,
     resolve_bucket_credential,
 )
 
 log = logging.getLogger(__name__)
 
 
@@ -77,42 +75,77 @@
 
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Look on a specified cluster (the current cluster by default).",
 )
+@option(
+    "--org",
+    type=ORG,
+    help="Look on a specified org (the current org by default).",
+)
+@option("--all-orgs", is_flag=True, default=False, help="Show buckets in all orgs.")
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
+)
+@option(
+    "--all-projects", is_flag=True, default=False, help="Show buckets in all projects."
+)
 @option("--full-uri", is_flag=True, help="Output full bucket URI.")
 @option("--long-format", is_flag=True, help="Output all info about bucket.")
 async def lsbucket(
-    root: Root, full_uri: bool, long_format: bool, cluster: Optional[str]
+    root: Root,
+    full_uri: bool,
+    long_format: bool,
+    cluster: Optional[str],
+    org: Optional[str],
+    all_orgs: bool,
+    project: Optional[str],
+    all_projects: bool,
 ) -> None:
     """
     List buckets.
     """
     if root.quiet:
         buckets_fmtr: BaseBucketsFormatter = SimpleBucketsFormatter()
     else:
         if full_uri:
             uri_fmtr: URIFormatter = str
         else:
             uri_fmtr = uri_formatter(
-                username=root.client.username,
-                cluster_name=cluster or root.client.cluster_name,
+                project_name=root.client.config.project_name_or_raise,
+                cluster_name=root.client.cluster_name,
                 org_name=root.client.config.org_name,
             )
         buckets_fmtr = BucketsFormatter(
             uri_fmtr,
             datetime_formatter=get_datetime_formatter(root.iso_datetime_format),
             long_format=long_format,
         )
 
+    if all_orgs:
+        org_name = ORG_NAME_SENTINEL
+    else:
+        org_name = parse_org_name(org, root)  # type: ignore
+
+    if all_projects:
+        project_name = None
+    else:
+        project_name = project or root.client.config.project_name_or_raise
+
     buckets = []
     with root.status("Fetching buckets") as status:
-        async with root.client.buckets.list(cluster_name=cluster) as it:
+        async with root.client.buckets.list(
+            cluster_name=cluster,
+            org_name=org_name,
+            project_name=project_name,
+        ) as it:
             async for bucket in it:
                 buckets.append(bucket)
                 status.update(f"Fetching buckets ({len(buckets)} loaded)")
 
     with root.pager():
         root.print(buckets_fmtr(buckets))
 
@@ -125,34 +158,41 @@
 )
 @option(
     "--org",
     type=ORG,
     help="Perform in a specified org (the current org by default).",
 )
 @option(
+    "--project",
+    type=PROJECT,
+    help="Perform in a specified project (the current project by default).",
+)
+@option(
     "--name",
     type=BUCKET_NAME,
     metavar="NAME",
     help="Optional bucket name",
     default=None,
 )
 async def mkbucket(
     root: Root,
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     org: Optional[str] = None,
+    project: Optional[str] = None,
 ) -> None:
     """
     Create a new bucket.
     """
     org_name = parse_org_name(org, root)
     bucket = await root.client.buckets.create(
         name=name,
         cluster_name=cluster,
         org_name=org_name,
+        project_name=project,
     )
     bucket_fmtr = BucketFormatter(
         str, datetime_formatter=get_datetime_formatter(root.iso_datetime_format)
     )
     with root.pager():
         root.print(bucket_fmtr(bucket))
 
@@ -165,14 +205,19 @@
 )
 @option(
     "--org",
     type=ORG,
     help="Perform in a specified org (the current org by default).",
 )
 @option(
+    "--project",
+    type=PROJECT,
+    help="Perform in a specified project (the current project by default).",
+)
+@option(
     "--name",
     type=BUCKET_NAME,
     metavar="NAME",
     help="Optional bucket name",
     default=None,
 )
 @option(
@@ -266,14 +311,15 @@
     azure_storage_account_url: Optional[str] = None,
     azure_storage_sas_token: Optional[str] = None,
     azure_storage_credential: Optional[str] = None,
     gcp_sa_credential: Optional[str] = None,
     name: Optional[str] = None,
     cluster: Optional[str] = None,
     org: Optional[str] = None,
+    project: Optional[str] = None,
 ) -> None:
     """
     Import an existing bucket.
     """
     org_name = parse_org_name(org, root)
     provider_type = Bucket.Provider(provider)
     credentials = {}
@@ -316,14 +362,15 @@
     bucket = await root.client.buckets.import_external(
         provider=provider_type,
         provider_bucket_name=provider_bucket_name,
         credentials=credentials,
         name=name,
         cluster_name=cluster,
         org_name=org_name,
+        project_name=project,
     )
     bucket_fmtr = BucketFormatter(
         str, datetime_formatter=get_datetime_formatter(root.iso_datetime_format)
     )
     with root.pager():
         root.print(bucket_fmtr(bucket))
 
@@ -331,45 +378,58 @@
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Look on a specified cluster (the current cluster by default).",
 )
 @option(
-    "--owner",
-    type=str,
-    help="Owner of bucket to assume for named bucket (the current user by default)",
+    "--org",
+    type=ORG,
+    help="Look on a specified org (the current org by default).",
+)
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
 )
 @argument("bucket", type=BUCKET)
 @option("--full-uri", is_flag=True, help="Output full bucket URI.")
 async def statbucket(
     root: Root,
     cluster: Optional[str],
-    owner: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
     bucket: str,
     full_uri: bool,
 ) -> None:
     """
     Get bucket BUCKET.
     """
+    org_name = parse_org_name(org, root)
     bucket_obj = await root.client.buckets.get(
-        bucket, cluster_name=cluster, bucket_owner=owner
+        bucket,
+        cluster_name=cluster,
+        org_name=org_name,
+        project_name=project,
     )
     if bucket_obj.imported:
         bc = await root.client.buckets.request_tmp_credentials(
-            bucket, cluster_name=cluster, bucket_owner=owner
+            bucket,
+            cluster_name=bucket_obj.cluster_name,
+            org_name=bucket_obj.org_name,
+            project_name=bucket_obj.project_name,
         )
         credentials = bc.credentials
     else:
         credentials = None
     if full_uri:
         uri_fmtr: URIFormatter = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=cluster or root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     bucket_fmtr = BucketFormatter(
         uri_fmtr, datetime_formatter=get_datetime_formatter(root.iso_datetime_format)
     )
     with root.pager():
@@ -379,38 +439,54 @@
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Look on a specified cluster (the current cluster by default).",
 )
 @option(
-    "--owner",
-    type=str,
-    help="Owner of bucket to assume for named bucket (the current user by default)",
+    "--org",
+    type=ORG,
+    help="Look on a specified org (the current org by default).",
+)
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
 )
 @argument("bucket", type=BUCKET)
 async def du(
-    root: Root, cluster: Optional[str], owner: Optional[str], bucket: str
+    root: Root,
+    cluster: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
+    bucket: str,
 ) -> None:
     """
     Get storage usage for BUCKET.
     """
+    org_name = parse_org_name(org, root)
     bucket_obj = await root.client.buckets.get(
-        bucket, cluster_name=cluster, bucket_owner=owner
+        bucket,
+        cluster_name=cluster,
+        org_name=org_name,
+        project_name=project,
     )
 
     bucket_str = bucket_obj.name or bucket_obj.id
     if bucket_obj.owner != root.client.config.username:
         bucket_str += f" (owner {bucket_obj.owner})"
 
     base_str = f"Calculating bucket {bucket_str} disk usage"
 
     with root.status(base_str) as status:
         async with root.client.buckets.get_disk_usage(
-            bucket_obj.id, cluster_name=cluster, bucket_owner=bucket_obj.owner
+            bucket_obj.id,
+            cluster_name=bucket_obj.cluster_name,
+            org_name=bucket_obj.org_name,
+            project_name=bucket_obj.project_name,
         ) as usage_it:
             async for usage in usage_it:
                 status.update(
                     f"{base_str}: total size {format_size(usage.total_bytes)}, "
                     f"objects count {usage.object_count}"
                 )
     root.print(
@@ -423,91 +499,104 @@
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Perform on a specified cluster (the current cluster by default).",
 )
 @option(
+    "--org",
+    type=ORG,
+    help="Perform on a specified org (the current org by default).",
+)
+@option(
+    "--project",
+    type=PROJECT,
+    help="Perform on a specified project (the current project by default).",
+)
+@option(
     "-f",
     "--force",
     is_flag=True,
     help="Force removal of all blobs inside bucket",
 )
-@option(
-    "--owner",
-    type=str,
-    help="Owner of bucket to assume for named bucket (the current user by default)",
-)
 @argument("buckets", type=BUCKET, nargs=-1, required=True)
 async def rmbucket(
     root: Root,
     cluster: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
     force: bool,
-    owner: Optional[str],
     buckets: Sequence[str],
 ) -> None:
     """
     Remove bucket BUCKET.
     """
+    org_name = parse_org_name(org, root)
     for bucket in buckets:
         bucket_id = await resolve_bucket(
             bucket,
             client=root.client,
             cluster_name=cluster,
-            bucket_owner=owner,
+            org_name=org_name,
+            project_name=project,
         )
         if force:
-            bucket_obj = await root.client.buckets.get(
-                bucket_id,
-                cluster_name=cluster,
-                bucket_owner=owner,
-            )
+            bucket_obj = await root.client.buckets.get(bucket_id, cluster_name=cluster)
             await root.client.buckets.blob_rm(bucket_obj.uri, recursive=True)
-        await root.client.buckets.rm(
-            bucket_id, cluster_name=cluster, bucket_owner=owner
-        )
+        await root.client.buckets.rm(bucket_id, cluster)
         if root.verbosity >= 0:
             root.print(f"Bucket with id '{bucket_id}' was successfully removed.")
 
 
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Perform on a specified cluster (the current cluster by default).",
 )
 @option(
-    "--owner",
-    type=str,
-    help="Owner of bucket to assume for named bucket (the current user by default)",
+    "--org",
+    type=ORG,
+    help="Perform on a specified org (the current org by default).",
+)
+@option(
+    "--project",
+    type=PROJECT,
+    help="Perform on a specified project (the current project by default).",
 )
 @argument("bucket", type=BUCKET, required=True)
 @argument(
     "public_level",
     type=click.Choice(["public", "private"], case_sensitive=False),
     required=True,
 )
 async def set_bucket_publicity(
     root: Root,
     cluster: Optional[str],
-    owner: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
     bucket: str,
     public_level: str,
 ) -> None:
     """
     Change public access settings for BUCKET
 
     Examples:
 
       neuro blob set-bucket-publicity my-bucket public
       neuro blob set-bucket-publicity my-bucket private
     """
     public = public_level == "public"
+    org_name = parse_org_name(org, root)
     await root.client.buckets.set_public_access(
-        bucket, public, cluster_name=cluster, bucket_owner=owner
+        bucket,
+        public,
+        cluster_name=cluster,
+        org_name=org_name,
+        project_name=project,
     )
     if root.verbosity >= 0:
         root.print(
             f"Bucket '{bucket}' was made {'public' if public else 'non-public'}."
         )
 
 
@@ -546,15 +635,15 @@
     List buckets or bucket contents.
     """
     formatter: BaseBlobFormatter
     if full_uri:
         uri_fmtr: URIFormatter = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     if format_long:
         # Similar to `ls -l`
         formatter = LongBlobFormatter(
             human_readable=human_readable, color=root.color, uri_formatter=uri_fmtr
@@ -602,20 +691,19 @@
     """
     List resources that match PATTERNS.
     """
     if full_uri:
         uri_fmtr: URIFormatter = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     for pattern in patterns:
-
         if root.verbosity > 0:
             painter = get_painter(root.color)
             uri_text = painter.paint(str(pattern), FileStatusType.FILE)
             root.print(Text.assemble("Using pattern ", uri_text, ":"))
 
         async with root.client.buckets.glob_blobs(uri=pattern) as blobs_it:
             async for entry in blobs_it:
@@ -971,15 +1059,15 @@
     Make signed url for blob in bucket.
     """
     expires_delta = parse_timedelta(expires)
     signed_url = await root.client.buckets.make_signed_url(
         path, int(expires_delta.total_seconds())
     )
 
-    root.print(signed_url)
+    root.print(signed_url, soft_wrap=True)
 
 
 # Bucket credentials commands
 
 
 def make_bucket_getter(
     client: Client, cluster_name: Optional[str] = None
@@ -1021,14 +1109,24 @@
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Perform in a specified cluster (the current cluster by default).",
 )
 @option(
+    "--org",
+    type=ORG,
+    help="Perform in a specified org (the current org by default).",
+)
+@option(
+    "--project",
+    type=PROJECT,
+    help="Perform in a specified project (the current project by default).",
+)
+@option(
     "--name",
     type=str,
     metavar="NAME",
     help="Optional bucket credential name",
     default=None,
 )
 @option(
@@ -1038,21 +1136,30 @@
 )
 @argument("buckets", type=BUCKET, nargs=-1, required=True)
 async def mkcredentials(
     root: Root,
     buckets: Sequence[str],
     name: Optional[str] = None,
     cluster: Optional[str] = None,
+    org: Optional[str] = None,
+    project: Optional[str] = None,
     read_only: bool = False,
 ) -> None:
     """
     Create a new bucket credential.
     """
+    org_name = parse_org_name(org, root)
     bucket_ids = [
-        await resolve_bucket(bucket, client=root.client, cluster_name=cluster)
+        await resolve_bucket(
+            bucket,
+            client=root.client,
+            cluster_name=cluster,
+            org_name=org_name,
+            project_name=project,
+        )
         for bucket in buckets
     ]
     credential = await root.client.buckets.persistent_credentials_create(
         name=name, cluster_name=cluster, read_only=read_only, bucket_ids=bucket_ids
     )
 
     fmtr = BucketCredentialFormatter(make_bucket_getter(root.client, cluster))
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/click_types.py` & `neuro-cli-23.7.0/src/neuro_cli/click_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from typing_extensions import Protocol
 from yarl import URL
 
 from neuro_sdk import (
     Client,
     LocalImage,
     Preset,
+    Project,
     RemoteImage,
     ResourceNotFound,
     TagOption,
 )
 
 from .asyncio_utils import asyncgeneratorcontextmanager
 from .parse_utils import (
@@ -159,15 +160,15 @@
         incomplete: str,
     ) -> List[CompletionItem]:
         if cluster_name not in client.config.clusters:
             return []
         names = []
         prefix = f"{path_prefix}{unquote(incomplete)}"
         for image in await client.images.list(cluster_name):
-            path = f"{image.owner}/{image.name}"
+            path = f"{image.project_name}/{image.name}"
             if image.org_name:
                 path = f"{image.org_name}/{path}"
             if path.startswith(prefix):
                 names.append(incomplete + quote(path[len(prefix) :]))
         return [CompletionItem(name, type="uri", prefix=uri_prefix) for name in names]
 
     async def _complete_image_tags(
@@ -189,15 +190,15 @@
     async def async_shell_complete(
         self, root: Root, ctx: click.Context, param: click.Parameter, incomplete: str
     ) -> List[CompletionItem]:
         if "image".startswith(incomplete):
             return [CompletionItem("image:", type="uri", prefix="")]
 
         async with await root.init_client() as client:
-            if incomplete.startswith("image:"):
+            if incomplete.startswith("image:") and client.config.project_name:
                 incomplete = incomplete[len("image:") :]
                 if self.tag_option != TagOption.DENY and ":" in incomplete:
                     prefix, incomplete = incomplete.split(":", 1)
                     return await self._complete_image_tags(
                         client, f"image:{prefix}", incomplete
                     )
 
@@ -215,15 +216,15 @@
 
                 if incomplete.startswith("/"):
                     incomplete = incomplete[1:]
                     return await self._complete_image_names(
                         client, "image:/", "", client.cluster_name, incomplete
                     )
 
-                path_prefix = f"{client.username}/"
+                path_prefix = f"{client.config.project_name}/"
                 if client.config.org_name:
                     path_prefix = f"{client.config.org_name}/{path_prefix}"
                 return await self._complete_image_names(
                     client, "image:", path_prefix, client.cluster_name, incomplete
                 )
 
             return []
@@ -512,69 +513,114 @@
             ]
 
 
 ORG = OrgType()
 ORG_ALLOW_UNKNOWN = OrgType(allow_unknown=True)
 
 
+class ProjectType(AsyncType[str]):
+    name = "project"
+
+    def __init__(self, allow_unknown: bool = False):
+        self._allow_unknown = allow_unknown
+
+    async def async_convert(
+        self,
+        root: Root,
+        value: str,
+        param: Optional[click.Parameter],
+        ctx: Optional[click.Context],
+    ) -> str:
+        if self._allow_unknown:
+            return value
+        client = await root.init_client()
+        cluster_name = root.client.config.cluster_name
+        org_name = root.client.config.org_name
+        project_key = Project.Key(
+            cluster_name=cluster_name, org_name=org_name, project_name=value
+        )
+        if project_key not in client.config.projects:
+            raise click.BadParameter(
+                f"Project {value} is not valid, "
+                "run 'neuro admin get-projects' to get a list of available projects",
+                ctx,
+                param,
+            )
+        return value
+
+    async def async_shell_complete(
+        self, root: Root, ctx: click.Context, param: click.Parameter, incomplete: str
+    ) -> List[CompletionItem]:
+        # async context manager is used to prevent a message about
+        # unclosed session
+        async with await root.init_client() as client:
+            projects = client.config.cluster_org_projects
+            return [
+                CompletionItem(p.name)
+                for p in projects
+                if p.name.startswith(incomplete)
+            ]
+
+
+PROJECT = ProjectType()
+PROJECT_ALLOW_UNKNOWN = ProjectType(allow_unknown=True)
+
+
 class JobType(AsyncType[str]):
     name = "job"
 
     async def async_convert(
         self,
         root: Root,
         value: str,
         param: Optional[click.Parameter],
         ctx: Optional[click.Context],
     ) -> str:
         return value
 
-    async def _complete_job_owners(
+    async def _complete_job_projects(
         self,
         client: Client,
         prefix: str,
         cluster_name: str,
         incomplete: str,
     ) -> List[CompletionItem]:
         if cluster_name not in client.config.clusters:
             return []
-        now = datetime.now()
-        limit = int(os.environ.get(JOB_LIMIT_ENV, 100))
-        names = []
-        async with client.jobs.list(
-            since=now - timedelta(days=7),
-            reverse=True,
-            limit=limit,
-            cluster_name=cluster_name,
-        ) as it:
-            async for job in it:
-                name = job.owner
-                if name.startswith(incomplete) and name not in names:
-                    names.append(name)
-        return [CompletionItem(f"{name}/", type="uri", prefix=prefix) for name in names]
+        completions = []
+        for project_key in client.config.projects.keys():
+            if project_key.cluster_name != cluster_name:
+                continue
+            if project_key.project_name.startswith(incomplete):
+                completions.append(
+                    CompletionItem(
+                        f"{project_key.project_name}/", type="uri", prefix=prefix
+                    )
+                )
+        return completions
 
     async def _complete_job_names(
         self,
         client: Client,
         prefix: str,
         cluster_name: str,
-        username: str,
+        project_name: Optional[str],
         incomplete: str,
     ) -> List[CompletionItem]:
         if cluster_name not in client.config.clusters:
             return []
         now = datetime.now()
         limit = int(os.environ.get(JOB_LIMIT_ENV, 100))
         names = {}
         async with client.jobs.list(
             since=now - timedelta(days=7),
             reverse=True,
             limit=limit,
             cluster_name=cluster_name,
-            owners=[username],
+            project_names=(project_name,) if project_name else (),
         ) as it:
             async for job in it:
                 id = job.id
                 name = job.name
                 if id.startswith(incomplete):
                     names[id] = name
                 if name and name.startswith(incomplete):
@@ -595,45 +641,49 @@
                 return []
 
             if incomplete.startswith("job://"):
                 parts = incomplete[len("job://") :].split("/")
                 if len(parts) == 1:
                     return _complete_clusters(client, "job://", *parts)
                 elif len(parts) == 2:
-                    return await self._complete_job_owners(
+                    return await self._complete_job_projects(
                         client, f"job://{parts[0]}/", *parts
                     )
                 elif len(parts) == 3:
                     return await self._complete_job_names(
                         client, f"job://{parts[0]}/{parts[1]}/", *parts
                     )
                 return []
 
             if incomplete.startswith("job:/"):
                 parts = incomplete[len("job:/") :].split("/")
                 if len(parts) == 1:
-                    return await self._complete_job_owners(
+                    return await self._complete_job_projects(
                         client, "job:/", client.cluster_name, *parts
                     )
                 elif len(parts) == 2:
                     return await self._complete_job_names(
                         client, f"job:/{parts[0]}/", client.cluster_name, *parts
                     )
                 return []
 
             if incomplete.startswith("job:"):
                 parts = incomplete[len("job:") :].split("/")
                 if len(parts) == 1:
                     return await self._complete_job_names(
-                        client, "job:", client.cluster_name, client.username, *parts
+                        client,
+                        "job:",
+                        client.cluster_name,
+                        client.config.project_name,
+                        *parts,
                     )
                 return []
 
             return await self._complete_job_names(
-                client, "", client.cluster_name, client.username, incomplete
+                client, "", client.cluster_name, client.config.project_name, incomplete
             )
 
 
 JOB = JobType()
 
 
 def _complete_id_name(
@@ -826,27 +876,35 @@
     async def get_completions(
         self,
         uri: URL,
         root: Root,
         incomplete: str,
     ) -> AsyncIterator[CompletionItem]:
         full_uri = root.client.parse.normalize_uri(uri)
-        bucket_id_complete = len(full_uri.parts) > 3 or (
-            len(full_uri.parts) == 3 and incomplete.endswith("/")
-        )
-        if not bucket_id_complete:
+        if not self._is_bucket_uri_complete(full_uri, root, incomplete):
+            prefix = uri.parent
+            full_prefix = full_uri.parent if uri.path else full_uri
+            full_prefix_str = str(full_prefix / "")
+            full_uri_str = str(full_uri if uri.path else full_uri / "")
+            completions = set()
             async with root.client.buckets.list(cluster_name=full_uri.host) as it:
                 async for bucket in it:
-                    if uri.host:
-                        prefix = URL(f"blob://{full_uri.host}/{bucket.owner}")
-                    else:
-                        prefix = URL(f"blob:")
-                    names = [bucket.id] + ([bucket.name] if bucket.name else [])
-                    for name in names:
-                        if str(prefix / name).startswith(incomplete):
+                    bucket_uris = [bucket.uri]
+                    if bucket.name:
+                        bucket_uris = [bucket.uri.parent / bucket.id] + bucket_uris
+                    for bucket_uri in bucket_uris:
+                        bucket_uri_str = str(bucket_uri)
+                        if not bucket_uri_str.startswith(full_uri_str):
+                            continue
+                        path_parts = bucket_uri_str[len(full_prefix_str) :].split("/")
+                        if len(path_parts) == 0:
+                            continue
+                        name = path_parts[0]
+                        if name not in completions:
+                            completions.add(name)
                             yield self._make_item(prefix, name, True)
         else:
             # Generic get_completions() is not used here because we can
             # benefit from prefix search in list_blobs().
             if incomplete.endswith("/"):
                 prefix = uri
                 full_uri = full_uri / ""
@@ -865,14 +923,28 @@
                             continue
                     else:
                         if not self._complete_file:
                             continue
 
                     yield self._make_item(prefix, item.name, item.is_dir())
 
+    def _is_bucket_uri_complete(self, uri: URL, root: Root, incomplete: str) -> bool:
+        parts = uri.parts
+        if len(parts) > 4:
+            # Check uri has format blob://cluster/org/project/bucket/
+            return True
+        if len(parts) == 4 or (
+            len(parts) == 3 and parts[-1] and incomplete.endswith("/")
+        ):
+            assert uri.host
+            cluster = root.client.config.clusters.get(uri.host)
+            # Check uri has format blob://cluster/project/bucket/
+            return bool(cluster and parts[1] not in cluster.orgs)
+        return False
+
 
 class PlatformURIType(AsyncType[URL]):
     name = "uri"
 
     def __init__(
         self,
         *,
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/completion.py` & `neuro-cli-23.7.0/src/neuro_cli/completion.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/config.py` & `neuro-cli-23.7.0/src/neuro_cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,25 @@
 from yarl import URL
 
 from neuro_sdk import DEFAULT_API_URL, AuthorizationError, ConfigError
 
 from neuro_cli.formatters.config import ClustersFormatter
 
 from .alias import list_aliases
-from .click_types import CLUSTER_ALLOW_UNKNOWN, ORG, ORG_ALLOW_UNKNOWN
-from .formatters.config import AliasesFormatter, ConfigFormatter
+from .click_types import (
+    CLUSTER_ALLOW_UNKNOWN,
+    ORG,
+    ORG_ALLOW_UNKNOWN,
+    PROJECT_ALLOW_UNKNOWN,
+)
+from .formatters.config import (
+    AliasesFormatter,
+    ClusterOrgProjectsFormatter,
+    ConfigFormatter,
+)
 from .root import Root
 from .utils import argument, command, group, option
 
 
 @group()
 def config() -> None:
     """Client configuration."""
@@ -71,14 +80,15 @@
 
 def _print_welcome(root: Root, url: URL) -> None:
     if root.client.config.clusters:
         root.print(
             f"Logged into {url} as [u]{root.client.config.username}[/u]"
             f", current cluster is [b]{root.client.config.cluster_name}[/b], "
             f"org is [b]{root.client.config.org_name or ORG.NO_ORG_STR}[/b]",
+            f"project is [b]{root.client.config.project_name}[/b]",
             markup=True,
         )
     else:
         root.print(
             f"Logged into {url} as [u]{root.client.config.username}[/u]", markup=True
         )
     root.print(
@@ -298,14 +308,41 @@
     await root.client.config.switch_org(org_name)
     root.print(
         f"The current org_name is [u]{rich_escape(org_name or '<no-org>')}[/u]",
         markup=True,
     )
 
 
+@command()
+@argument("project_name", required=False, default=None, type=PROJECT_ALLOW_UNKNOWN)
+async def switch_project(root: Root, project_name: Optional[str]) -> None:
+    """
+    Switch the active project.
+
+    PROJECT_NAME is the project name to select. The interactive prompt is used if the
+    name is omitted (default).
+
+    """
+    with root.status("Fetching the list of available projects"):
+        await root.client.config.fetch()
+    if project_name is None:
+        if not root.tty:
+            raise click.BadArgumentUsage(
+                "Interactive mode is disabled for non-TTY mode, "
+                "please specify the PROJECT_NAME"
+            )
+        real_project_name = await prompt_project(root)
+    else:
+        real_project_name = project_name
+    await root.client.config.switch_project(real_project_name)
+    root.print(
+        f"The current project is [u]{rich_escape(real_project_name)}[/u]", markup=True
+    )
+
+
 async def prompt_cluster(
     root: Root, *, session: Optional[PromptSession[str]] = None
 ) -> str:
     if session is None:
         session = PromptSession()
     clusters = root.client.config.clusters
     while True:
@@ -330,20 +367,49 @@
                 f"doesn't exist, please try again.",
                 markup=True,
             )
         else:
             return answer
 
 
+async def prompt_project(
+    root: Root, *, session: Optional[PromptSession[str]] = None
+) -> str:
+    if session is None:
+        session = PromptSession()
+    projects = sorted(p.name for p in root.client.config.cluster_org_projects)
+    while True:
+        fmt = ClusterOrgProjectsFormatter()
+        root.print(fmt(projects, root.client.config.project_name))
+        with patch_stdout():
+            answer = await session.prompt_async(
+                f"Select project to switch [{root.client.config.project_name}]: "
+            )
+        answer = answer.strip()
+        if not answer:
+            if not root.client.config.project_name:
+                continue
+            answer = root.client.config.project_name
+        if answer not in projects:
+            root.print(
+                f"Selected project [u]{rich_escape(answer)}[/u] "
+                f"doesn't exist, please try again.",
+                markup=True,
+            )
+        else:
+            return answer
+
+
 config.add_command(login)
 config.add_command(login_with_token)
 config.add_command(login_headless)
 config.add_command(show)
 config.add_command(show_token)
 config.add_command(aliases)
 config.add_command(get_clusters)
+config.add_command(switch_project)
 config.add_command(switch_cluster)
 config.add_command(switch_org)
 
 config.add_command(docker)
 
 config.add_command(logout)
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/docker_credential_helper.py` & `neuro-cli-23.7.0/src/neuro_cli/docker_credential_helper.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/file_logging.py` & `neuro-cli-23.7.0/src/neuro_cli/file_logging.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/admin.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from neuro_sdk import (
     _AWSStorageOptions,
     _AzureStorageOptions,
     _CloudProviderOptions,
     _CloudProviderType,
     _Cluster,
+    _ClusterUser,
     _ClusterUserWithInfo,
     _ConfigCluster,
     _GoogleStorageOptions,
     _NodePool,
     _NodePoolOptions,
     _Org,
     _OrgCluster,
@@ -29,15 +30,15 @@
 )
 
 from neuro_cli.formatters.config import format_quota_details
 from neuro_cli.formatters.utils import format_datetime_iso
 from neuro_cli.utils import format_size
 
 
-class ClusterUserFormatter:
+class ClusterUserWithInfoFormatter:
     def __call__(
         self, clusters_users: Iterable[_ClusterUserWithInfo]
     ) -> RenderableType:
         table = Table(box=box.MINIMAL_HEAVY_HEAD)
         table.add_column("Name", style="bold")
         table.add_column("Org")
         table.add_column("Role")
@@ -50,15 +51,15 @@
         rows = []
 
         for user in clusters_users:
             rows.append(
                 (
                     user.user_name,
                     user.org_name or "",
-                    user.role.value,
+                    user.role.value if user.role else "",
                     user.user_info.email,
                     user.user_info.full_name,
                     format_datetime_iso(user.user_info.created_at),
                     format_quota_details(user.balance.credits),
                     format_quota_details(user.balance.spent_credits),
                     format_quota_details(user.quota.total_running_jobs),
                 )
@@ -66,14 +67,30 @@
         rows.sort(key=operator.itemgetter(0))
 
         for row in rows:
             table.add_row(*row)
         return table
 
 
+class ClusterUserFormatter:
+    def __call__(self, clusters_users: Iterable[_ClusterUser]) -> RenderableType:
+        table = Table(box=box.MINIMAL_HEAVY_HEAD)
+        table.add_column("Name", style="bold")
+        table.add_column("Org")
+        rows = []
+
+        for user in clusters_users:
+            rows.append((user.user_name, user.org_name or ""))
+        rows.sort(key=operator.itemgetter(0))
+
+        for row in rows:
+            table.add_row(*row)
+        return table
+
+
 class OrgUserFormatter:
     def __call__(self, org_users: Iterable[_OrgUserWithInfo]) -> RenderableType:
         table = Table(box=box.MINIMAL_HEAVY_HEAD)
         table.add_column("Name", style="bold")
         table.add_column("Role")
         table.add_column("Email")
         table.add_column("Full name")
@@ -444,15 +461,15 @@
                 f"{min_capacity} - {max_capacity}",
             )
         return table
 
 
 class ProjectsFormatter:
     def __call__(self, projects: Iterable[_Project]) -> RenderableType:
-        table = Table(box=box.MINIMAL_HEAVY_HEAD)
+        table = Table(box=box.SIMPLE_HEAVY)
         table.add_column("Project name", style="bold")
         table.add_column("Cluster name")
         table.add_column("Org name")
         table.add_column("Default role")
         table.add_column("Is default project")
         rows = []
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/blob_storage.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/bucket_credentials.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/bucket_credentials.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/buckets.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/buckets.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             bucket.name or "",
             bucket.provider + (" (imported)" if bucket.imported else ""),
             self._uri_formatter(bucket.uri),
         ]
         if self._long_format:
             line += [
                 bucket.org_name or ORG.NO_ORG_STR,
+                bucket.project_name,
                 self._datetime_formatter(bucket.created_at),
                 "√" if bucket.public else "×",
             ]
         return line
 
     def __call__(self, buckets: Sequence[Bucket]) -> RenderableType:
         buckets = sorted(buckets, key=operator.attrgetter("id"))
@@ -59,14 +60,15 @@
         width = len("bucket-06bed296-8b27-4aa8-9e2a-f3c47b41c807")
         table.add_column("Id", style="bold", width=width)
         table.add_column("Name")
         table.add_column("Provider")
         table.add_column("Uri")
         if self._long_format:
             table.add_column("Org name")
+            table.add_column("Project name")
             table.add_column("Created at")
             table.add_column("Public")
         for bucket in buckets:
             table.add_row(*self._bucket_to_table_row(bucket))
         return table
 
 
@@ -88,14 +90,15 @@
         table.add_column()
         table.add_column(style="bold")
         table.add_row("Id", bucket.id)
         table.add_row("Uri", self._uri_formatter(bucket.uri))
         if bucket.name:
             table.add_row("Name", bucket.name)
         table.add_row("Org name", bucket.org_name or ORG.NO_ORG_STR)
+        table.add_row("Project name", bucket.project_name)
         table.add_row("Created at", self._datetime_formatter(bucket.created_at))
         table.add_row("Provider", bucket.provider)
         table.add_row("Imported", str(bucket.imported))
         table.add_row("Public", str(bucket.public))
         if credentials is not None:
             for key, title in [
                 ("bucket_name", "External name"),
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/config.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             show_edge=False,
         )
         table.add_column()
         table.add_column(style="bold")
         table.add_row("User Name", config.username)
         table.add_row("Current Cluster", config.cluster_name)
         table.add_row("Current Org", config.org_name or "<no-org>")
+        table.add_row("Current Project", config.project_name or "<no-project>")
         table.add_row("Credits Quota", format_quota_details(quota.credits))
         table.add_row("Jobs Quota", format_quota_details(quota.total_running_jobs))
         if org_quota:
             table.add_row("Org Credits Quota", format_quota_details(org_quota.credits))
             table.add_row(
                 "Org Jobs Quota", format_quota_details(org_quota.total_running_jobs)
             )
@@ -202,14 +203,27 @@
                 timeslot[0].strftime("%H:%M"),
                 timeslot[1].strftime("%H:%M"),
                 ", ".join([calendar.day_abbr[x - 1] for x in sorted(days)]),
             )
     return summary_tbl, schedules_tbl
 
 
+class ClusterOrgProjectsFormatter:
+    def __call__(
+        self, projects: Iterable[str], current_project: Optional[str]
+    ) -> RenderableType:
+        out: List[RenderableType] = [Text("Available projects:", style="i")]
+        for project in projects:
+            if project == current_project:
+                out.append(Text(f"* {project}", style="bold"))
+            else:
+                out.append(Text(f"  {project}"))
+        return RichGroup(*out)
+
+
 class AliasesFormatter:
     def __call__(self, aliases: Iterable[click.Command]) -> Table:
         table = Table(box=box.MINIMAL_HEAVY_HEAD)
         table.add_column("Alias", style="bold")
         table.add_column("Description")
         for alias in sorted(aliases, key=operator.attrgetter("name")):
             table.add_row(alias.name, alias.get_short_help_str())
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/disks.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/disks.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             used_str,
             self._uri_formatter(disk.uri),
             disk.status.value,
         ]
         if self._long_format:
             line += [
                 disk.org_name or ORG.NO_ORG_STR,
+                disk.project_name,
                 self._datetime_formatter(disk.created_at),
                 self._datetime_formatter(disk.last_usage),
                 format_disk_timeout_unused(disk.timeout_unused),
             ]
         return line
 
     def __call__(self, disks: Sequence[Disk]) -> RenderableType:
@@ -69,14 +70,15 @@
         table.add_column("Name")
         table.add_column("Storage")
         table.add_column("Used")
         table.add_column("Uri")
         table.add_column("Status")
         if self._long_format:
             table.add_column("Org name")
+            table.add_column("Project name")
             table.add_column("Created at")
             table.add_column("Last used")
             table.add_column("Timeout unused")
         for disk in disks:
             table.add_row(*self._disk_to_table_row(disk))
         return table
 
@@ -99,14 +101,16 @@
         table.add_row("Id", disk.id)
         table.add_row("Storage", utils.format_size(disk.storage))
         table.add_row("Used", utils.format_size(disk.used_bytes))
         table.add_row("Uri", self._uri_formatter(disk.uri))
         if disk.name:
             table.add_row("Name", disk.name)
         table.add_row("Org name", disk.org_name or ORG.NO_ORG_STR)
+        table.add_row("Project name", disk.project_name)
+        table.add_row("Owner", disk.owner)
         table.add_row("Status", disk.status.value)
         table.add_row("Created at", self._datetime_formatter(disk.created_at))
         table.add_row("Last used", self._datetime_formatter(disk.last_usage))
         table.add_row("Timeout unused", format_disk_timeout_unused(disk.timeout_unused))
         return table
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/images.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/images.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/jobs.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         table.add_row("Job", job_status.id)
         if job_status.name:
             table.add_row("Name", job_status.name)
         if job_status.tags:
             text = ", ".join(job_status.tags)
             table.add_row("Tags", text)
         table.add_row("Owner", job_status.owner or "")
+        table.add_row("Project", job_status.project_name or "")
         table.add_row("Cluster", job_status.cluster_name)
         if job_status.org_name:
             table.add_row("Organization", job_status.org_name)
         if job_status.description:
             table.add_row("Description", job_status.description)
         status_text = fmt_status(job_status.status)
         if job_status.history.reason:
@@ -132,15 +133,15 @@
                 f"{job_status.container.resources.gpu_model}",
             )
 
         if job_status.container.resources.tpu_type:
             resources.add_row(
                 "TPU",
                 f"{job_status.container.resources.tpu_type}/"
-                "{job_status.container.resources.tpu_software_version}",
+                f"{job_status.container.resources.tpu_software_version}",
             )
 
         if job_status.container.resources.shm:
             resources.add_row("Extended SHM space", "True")
 
         table.add_row("Resources", Styled(resources, style="reset"))
 
@@ -427,14 +428,15 @@
     description: str
     cluster_name: str
     org_name: str
     command: str
     life_span: str
     workdir: str
     preset: str
+    project_name: str
 
     @classmethod
     def from_job(
         cls,
         job: JobDescription,
         username: str,
         image_formatter: ImageFormatter,
@@ -454,14 +456,15 @@
             description=job.description if job.description else "",
             cluster_name=job.cluster_name,
             org_name=job.org_name or "",
             command=job.container.command if job.container.command else "",
             life_span=format_life_span(job.life_span),
             workdir=job.container.working_dir or "",
             preset=job.preset_name or "",
+            project_name=job.project_name or "",
         )
 
     def to_list(self, columns: JobTableFormat) -> List[TextType]:
         return _format_row(columns, lambda id: getattr(self, id))
 
 
 def _format_row(
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/secrets.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/secrets.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,19 +32,21 @@
     ) -> None:
         self._uri_formatter = uri_formatter
 
     def _secret_to_table_row(self, secret: Secret) -> Sequence[str]:
         line = [
             self._uri_formatter(secret.uri),
             secret.org_name or ORG.NO_ORG_STR,
+            secret.project_name,
         ]
         return line
 
     def __call__(self, secrets: Sequence[Secret]) -> RenderableType:
         secrets = sorted(secrets, key=operator.attrgetter("key"))
         table = Table(box=box.SIMPLE_HEAVY)
         table.add_column("Key", style="bold")
         table.add_column("Org")
+        table.add_column("Project")
 
         for secret in secrets:
             table.add_row(*self._secret_to_table_row(secret))
         return table
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/service_accounts.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/service_accounts.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from rich.console import Group as RichGroup
 from rich.console import RenderableType
 from rich.table import Table
 from rich.text import Text
 
 from neuro_sdk import ServiceAccount
 
+from neuro_cli.click_types import ORG
 from neuro_cli.formatters.utils import DatetimeFormatter
 
 
 class BaseServiceAccountsFormatter:
     @abc.abstractmethod
     def __call__(self, accounts: Sequence[ServiceAccount]) -> RenderableType:
         pass
@@ -71,29 +72,40 @@
         table.add_column()
         table.add_column(style="bold")
         table.add_row("Id", account.id)
         table.add_row("Name", account.name or "")
         table.add_row("Role", account.role)
         table.add_row("Owner", account.owner)
         table.add_row("Default cluster", account.default_cluster)
+        table.add_row("Default org", account.default_org or ORG.NO_ORG_STR)
+        table.add_row("Default project", account.default_project)
         table.add_row("Created at", self._datetime_formatter(account.created_at))
         return table
 
 
-def service_account_token_fmtr(token: str) -> RenderableType:
-    token_data = json.loads(base64.b64decode(token.encode()).decode())
+def service_account_token_fmtr(token: str, account: ServiceAccount) -> RenderableType:
+    token_data: dict[str, str] = json.loads(base64.b64decode(token.encode()).decode())
     auth_token = token_data["token"]
 
-    return Text.from_markup(
-        "\n".join(
-            [
-                "Full token with cluster and API url embedded (this value can "
-                "be used as [b]NEURO_PASSED_CONFIG[/b] environment variable):\n",
-                token,
-                "\nJust auth token (this value can be passed to [b]neuro config"
-                " login-with-token[/b]):\n",
-                auth_token,
-                "\n[b red]Save it to some secure place, you will be unable to "
-                "retrieve it later![/b red]",
-            ]
-        )
+    org = "/" + token_data.get("org_name", "") if token_data.get("org_name") else ""
+
+    res_example = f"scheme://{token_data['cluster']}{org}/{token_data['project_name']}"
+    share_resource_cmd_hint = (
+        f"[b]neuro acl grant {res_example} {account.role} {{read|write|manage}}[/b]\n"
     )
+
+    lines = [
+        "Full token with cluster and API url embedded (this value can "
+        "be used as [b]NEURO_PASSED_CONFIG[/b] environment variable):\n",
+        token,
+        "\nJust auth token (this value can be passed to [b]neuro config"
+        " login-with-token[/b]):\n",
+        auth_token,
+        "\n[b red]Save it to some secure place, you will be unable to "
+        "retrieve it later![/b red]",
+        "\nTo allow access to your project resources for this service account, "
+        "perform:\n",
+        share_resource_cmd_hint,
+        "",
+    ]
+
+    return Text.from_markup("\n".join(lines))
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/storage.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/formatters/utils.py` & `neuro-cli-23.7.0/src/neuro_cli/formatters/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 from neuro_sdk import SCHEMES, RemoteImage
 
 URIFormatter = Callable[[URL], str]
 ImageFormatter = Callable[[RemoteImage], str]
 
 
 def uri_formatter(
-    username: str, cluster_name: str, org_name: Optional[str]
+    project_name: str, cluster_name: str, org_name: Optional[str]
 ) -> URIFormatter:
     def formatter(uri: URL) -> str:
         if uri.scheme in SCHEMES:
             if uri.host == cluster_name:
                 assert uri.path[0] == "/"
                 path = uri.path.lstrip("/")
-                owner_or_org, _, rest = path.partition("/")
+                project_or_org, _, rest = path.partition("/")
                 if org_name:
-                    if owner_or_org != org_name:
+                    if project_or_org != org_name:
                         return str(uri)
                     path = rest
-                    owner, _, rest = path.partition("/")
+                    project, _, rest = path.partition("/")
                 else:
-                    owner = owner_or_org
-                if owner == username:
+                    project = project_or_org
+                if project == project_name:
                     path = rest.lstrip("/")
                 else:
                     path = "/" + path
                 uri = URL.build(scheme=uri.scheme, path=path)
         return str(uri)
 
     return formatter
@@ -103,23 +103,29 @@
     "Jan 1 at 00:01"
     """
     if when is None:
         return ""
     assert when.tzinfo is not None
     delta = datetime.datetime.now(datetime.timezone.utc) - when
     if delta < datetime.timedelta(days=1):
+        prefix = ""
+        suffix = " ago"
+        if delta != abs(delta):  # negative delta means lifespan ends in future
+            prefix = "in "
+            suffix = ""
         if precise:
             min_unit = "seconds"
-            if delta > datetime.timedelta(hours=1):
+            if abs(delta) > datetime.timedelta(hours=1):
                 min_unit = "minutes"
             return (
-                humanize.precisedelta(delta, minimum_unit=min_unit, format="%0.0f")
-                + " ago"
+                prefix
+                + humanize.precisedelta(delta, minimum_unit=min_unit, format="%0.0f")
+                + suffix
             )
-        return humanize.naturaldelta(delta) + " ago"
+        return prefix + humanize.naturaldelta(delta) + suffix
     else:
         when_local = when.astimezone(timezone)
         result = humanize.naturaldate(when_local)
         if precise:
             result = f"{result} at {when_local.strftime('%H:%M')} "
         return result
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/image.py` & `neuro-cli-23.7.0/src/neuro_cli/image.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,28 @@
 from typing import Optional, Sequence
 
 from rich.markup import escape as rich_escape
 from rich.progress import Progress
 
 from neuro_sdk import LocalImage, RemoteImage, Tag, TagOption
 
-from neuro_cli.formatters.images import (
+from .click_types import CLUSTER, ORG, PROJECT, RemoteImageType
+from .formatters.images import (
     BaseImagesFormatter,
     BaseTagsFormatter,
     DockerImageProgress,
     LongImagesFormatter,
     LongTagsFormatter,
     QuietImagesFormatter,
     ShortImagesFormatter,
     ShortTagsFormatter,
 )
-from neuro_cli.formatters.utils import ImageFormatter, image_formatter, uri_formatter
-
-from .click_types import CLUSTER, RemoteImageType
+from .formatters.utils import ImageFormatter, image_formatter, uri_formatter
 from .root import Root
-from .utils import argument, command, format_size, group, option
+from .utils import argument, command, format_size, group, option, parse_org_name
 
 log = logging.getLogger(__name__)
 
 
 @group()
 def image() -> None:
     """
@@ -46,15 +45,15 @@
     Image names can contain tag. If tags not specified 'latest' will
     be used as value.
 
     Examples:
 
     neuro push myimage
     neuro push alpine:latest image:my-alpine:production
-    neuro push alpine image://myfriend/alpine:shared
+    neuro push alpine image:/other-project/alpine:shared
 
     """
 
     progress = DockerImageProgress.create(console=root.console, quiet=root.quiet)
     local_obj = root.client.parse.local_image(local_image)
     if remote_image is not None:
         remote_obj: Optional[RemoteImage] = root.client.parse.remote_image(remote_image)
@@ -76,16 +75,16 @@
 
     Remote image name must be URL with image:// scheme.
     Image names can contain tag.
 
     Examples:
 
     neuro pull image:myimage
-    neuro pull image://myfriend/alpine:shared
-    neuro pull image://username/my-alpine:production alpine:from-registry
+    neuro pull image:/other-project/alpine:shared
+    neuro pull image:/project/my-alpine:production alpine:from-registry
 
     """
 
     progress = DockerImageProgress.create(console=root.console, quiet=root.quiet)
     remote_obj = root.client.parse.remote_image(remote_image)
     if local_image is not None:
         local_obj: Optional[LocalImage] = root.client.parse.local_image(local_image)
@@ -100,65 +99,86 @@
 
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Show images on a specified cluster (the current cluster by default).",
 )
-@option("-l", "format_long", is_flag=True, help="List in long format.")
-@option("--full-uri", is_flag=True, help="Output full image URI.")
 @option(
-    "-o",
-    "--owner",
+    "--org",
+    type=ORG,
     multiple=True,
-    help="Filter out images by owner (multiple option). "
-    "Supports `ME` option to filter by the current user.",
-    secure=True,
+    help="Filter out images by org (multiple option, the current org by default).",
+)
+@option("--all-orgs", is_flag=True, default=False, help="Show images in all orgs.")
+@option(
+    "--project",
+    type=PROJECT,
+    multiple=True,
+    help="Filter out images by project "
+    "(multiple option, the current project by default).",
 )
 @option(
+    "--all-projects", is_flag=True, default=False, help="Show images in all projects."
+)
+@option("-l", "format_long", is_flag=True, help="List in long format.")
+@option("--full-uri", is_flag=True, help="Output full image URI.")
+@option(
     "-n",
     "--name",
     metavar="PATTERN",
     help="Filter out images by name regex.",
     secure=True,
 )
 async def ls(
     root: Root,
     cluster: str,
+    org: Sequence[str],
+    all_orgs: bool,
+    project: Sequence[str],
+    all_projects: bool,
     format_long: bool,
     full_uri: bool,
-    owner: Sequence[str],
     name: Optional[str],
 ) -> None:
     """
     List images.
     """
 
     if not cluster:
         cluster = root.client.config.cluster_name
     with root.status("Fetching images"):
         images = await root.client.images.list(cluster_name=cluster)
 
-    if owner:
-        owners = set(owner)
-        if "ME" in owners:
-            owners.remove("ME")
-            owners.add(root.client.config.username)
-        images = [image for image in images if image.owner in owners]
+    if all_orgs:
+        org_names = None
+    elif org:
+        org_names = {parse_org_name(o, root) for o in org}
+    else:
+        org_names = {root.client.config.org_name}
+    if org_names:
+        images = [image for image in images if image.org_name in org_names]
+
+    if all_projects:
+        project_names = None
+    else:
+        project_names = set(project or [root.client.config.project_name_or_raise])
+    if project_names:
+        images = [image for image in images if image.project_name in project_names]
 
     if name:
         name_re = re.compile(name)
         images = [image for image in images if name_re.fullmatch(image.name)]
 
     image_fmtr: ImageFormatter
     if full_uri:
         image_fmtr = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
         image_fmtr = image_formatter(uri_formatter=uri_fmtr)
     formatter: BaseImagesFormatter
     if root.quiet:
         formatter = QuietImagesFormatter(image_formatter=image_fmtr)
@@ -179,15 +199,15 @@
     """
     List tags for image in platform registry.
 
     Image name must be URL with image:// scheme.
 
     Examples:
 
-    neuro image tags image://myfriend/alpine
+    neuro image tags image:/other-project/alpine
     neuro image tags -l image:myimage
     """
 
     with root.status(f"Fetching tags for image [b]{image}[/b]"):
         tags_list = [
             Tag(name=str(img.tag)) for img in await root.client.images.tags(image)
         ]
@@ -227,15 +247,15 @@
     Remove image from platform registry.
 
     Image name must be URL with image:// scheme.
     Image name must contain tag.
 
     Examples:
 
-    neuro image rm image://myfriend/alpine:shared
+    neuro image rm image:/other-project/alpine:shared
     neuro image rm image:myimage:latest
     """
     for image in images:
         if image.tag is None:
             await remove_image(root, image)
         else:
             await remove_tag(root, image, force=force)
@@ -248,15 +268,15 @@
     Get image size
 
     Image name must be URL with image:// scheme.
     Image name must contain tag.
 
     Examples:
 
-    neuro image size image://myfriend/alpine:shared
+    neuro image size image:/other-project/alpine:shared
     neuro image size image:myimage:latest
     """
     size = await root.client.images.size(image)
     root.print(format_size(size))
 
 
 @command()
@@ -266,15 +286,15 @@
     Get digest of an image from remote registry
 
     Image name must be URL with image:// scheme.
     Image name must contain tag.
 
     Examples:
 
-    neuro image digest image://myfriend/alpine:shared
+    neuro image digest image:/other-project/alpine:shared
     neuro image digest image:myimage:latest
     """
     res = await root.client.images.digest(image)
     root.print(res)
 
 
 image.add_command(ls)
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/job.py` & `neuro-cli-23.7.0/src/neuro_cli/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,62 +24,63 @@
     JobPriority,
     JobRestartPolicy,
     JobStatus,
     Permission,
     RemoteImage,
 )
 
-from neuro_cli.formatters.images import DockerImageProgress
-from neuro_cli.formatters.utils import (
-    URIFormatter,
-    get_datetime_formatter,
-    image_formatter,
-    uri_formatter,
-)
-from neuro_cli.parse_utils import parse_sort_keys
-from neuro_cli.utils import parse_org_name, resolve_disk
-
 from .ael import print_job_result, process_attach, process_exec, process_logs
 from .click_types import (
     CLUSTER,
     JOB,
     JOB_COLUMNS,
     JOB_NAME,
     LOCAL_REMOTE_PORT,
     ORG,
     PRESET,
+    PROJECT,
     TOP_COLUMNS,
     RemoteImageType,
 )
 from .const import EX_PLATFORMERROR
+from .formatters.images import DockerImageProgress
 from .formatters.jobs import (
     BaseJobsFormatter,
     JobStartProgress,
     JobStatusFormatter,
     JobTelemetryFormatter,
     LifeSpanUpdateFormatter,
     SimpleJobsFormatter,
     TabularJobsFormatter,
 )
+from .formatters.utils import (
+    URIFormatter,
+    get_datetime_formatter,
+    image_formatter,
+    uri_formatter,
+)
 from .parse_utils import (
     JobTableFormat,
     get_default_ps_columns,
     get_default_top_columns,
     parse_ps_columns,
+    parse_sort_keys,
     parse_timedelta,
     parse_top_columns,
     serialize_timedelta,
 )
 from .root import Root
 from .utils import (
     argument,
     calc_life_span,
     command,
     group,
     option,
+    parse_org_name,
+    resolve_disk,
     resolve_job,
     resolve_job_ex,
     volume_to_verbose_str,
 )
 
 log = logging.getLogger(__name__)
 
@@ -291,14 +292,33 @@
 )
 @option(
     "--cluster",
     type=CLUSTER,
     help="Show jobs on a specified cluster (the current cluster by default).",
 )
 @option(
+    "--org",
+    type=ORG,
+    help="Filter out jobs by org name "
+    "(multiple option, the current org by default).",
+    multiple=True,
+)
+@option("--all-orgs", is_flag=True, default=False, help="Show jobs in all orgs.")
+@option(
+    "-p",
+    "--project",
+    type=PROJECT,
+    help="Filter out jobs by project name "
+    "(multiple option, the current project by default).",
+    multiple=True,
+)
+@option(
+    "--all-projects", is_flag=True, default=False, help="Show jobs in all projects."
+)
+@option(
     "-o",
     "--owner",
     multiple=True,
     help="Filter out jobs by owner (multiple option). "
     "Supports `ME` option to filter by the current user.",
     secure=True,
 )
@@ -366,14 +386,18 @@
 )
 @option("--full-uri", is_flag=True, help="Output full image URI.")
 async def ls(
     root: Root,
     status: Sequence[str],
     all: bool,
     cluster: str,
+    org: Sequence[str],
+    all_orgs: bool,
+    project: Sequence[str],
+    all_projects: bool,
     name: str,
     distinct: bool,
     recent_first: bool,
     tag: Sequence[str],
     owner: Sequence[str],
     since: str,
     until: str,
@@ -402,20 +426,32 @@
     if "ME" in owners:
         owners.remove("ME")
         owners.add(root.client.config.username)
     tags = set(tag)
     if not cluster:
         cluster = root.client.config.cluster_name
 
+    if all_orgs:
+        org_names = []
+    elif org:
+        org_names = [parse_org_name(o, root) for o in org]
+    else:
+        org_names = [root.client.config.org_name]
+
+    if all_projects:
+        project_names: Sequence[str] = []
+    else:
+        project_names = project or [root.client.config.project_name_or_raise]
+
     uri_fmtr: URIFormatter
     if full_uri:
         uri_fmtr = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     if root.quiet:
         formatter: BaseJobsFormatter = SimpleJobsFormatter()
     else:
         image_fmtr = image_formatter(uri_formatter=uri_fmtr)
@@ -431,14 +467,16 @@
         name=name,
         owners=owners,
         tags=tags,
         since=_parse_date(since),
         until=_parse_date(until),
         reverse=recent_first,
         cluster_name=cluster,
+        org_names=org_names,
+        project_names=project_names,
     ) as jobs:
         # client-side filtering
         if description:
             jobs = (job async for job in jobs if job.description == description)
 
         if distinct:
 
@@ -479,15 +517,15 @@
     )
     res = await root.client.jobs.status(id)
     uri_fmtr: URIFormatter
     if full_uri:
         uri_fmtr = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     root.print(
         JobStatusFormatter(
             uri_formatter=uri_fmtr,
             datetime_formatter=get_datetime_formatter(root.iso_datetime_format),
@@ -606,28 +644,36 @@
 @option(
     "--timeout",
     default=0,
     type=float,
     show_default=True,
     help="Maximum allowed time for executing the command, 0 for no timeout",
 )
+@option(
+    "-p",
+    "--project",
+    type=PROJECT,
+    help="Filter out jobs by project name (multiple option).",
+    multiple=True,
+)
 async def top(
     root: Root,
     jobs: Sequence[str],
     cluster: str,
     name: str,
     tag: Sequence[str],
     owner: Sequence[str],
     since: str,
     until: str,
     description: str,
     sort: str,
     format: Optional[JobTableFormat],
     full_uri: bool,
     timeout: float,
+    project: Sequence[str],
 ) -> None:
     """
     Display GPU/CPU/Memory usage.
 
     Examples:
 
     neuro top
@@ -648,14 +694,15 @@
     if jobs:
         for opt, val in [
             ("name", name),
             ("owner", owner),
             ("since", since),
             ("until", until),
             ("description", description),
+            ("project", project),
         ]:
             if val:
                 raise click.UsageError(
                     f"Option --{opt} is mutually exclusive with job arguments"
                 )
 
         async def create_pollers() -> None:
@@ -693,14 +740,15 @@
                     statuses=JobStatus.active_items(),
                     name=name,
                     owners=owners,
                     tags=tags,
                     since=since_dt,
                     until=until_dt,
                     cluster_name=cluster,
+                    project_names=project,
                 ) as jobs:
                     # client-side filtering
                     if description:
                         jobs = (
                             job async for job in jobs if job.description == description
                         )
 
@@ -741,15 +789,15 @@
                 await asyncio.sleep(TOP_REFRESH_DELAY)
 
     uri_fmtr: URIFormatter
     if full_uri:
         uri_fmtr = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
     image_fmtr = image_formatter(uri_formatter=uri_fmtr)
     datetime_fmtr = get_datetime_formatter(root.iso_datetime_format)
 
     with JobTelemetryFormatter(
@@ -1026,14 +1074,21 @@
     "--energy-schedule",
     metavar="NAME",
     help=(
         "Run job only within a selected energy schedule. "
         "Selected preset should have scheduler enabled."
     ),
 )
+@option(
+    "-p",
+    "--project",
+    type=PROJECT,
+    help="Run job in a specified project.",
+    default=None,
+)
 @TTY_OPT
 async def run(
     root: Root,
     image: RemoteImage,
     preset: str,
     cluster: Optional[str],
     org: Optional[str],
@@ -1060,14 +1115,15 @@
     detach: bool,
     tty: Optional[bool],
     schedule_timeout: Optional[str],
     privileged: bool,
     share: Sequence[str],
     priority: Optional[str],
     energy_schedule: Optional[str],
+    project: Optional[str],
 ) -> None:
     """
     Run a job
 
     IMAGE docker image name to run in a job.
 
     CMD list will be passed as arguments to the executed job's image.
@@ -1129,14 +1185,15 @@
         schedule_timeout=schedule_timeout,
         privileged=privileged,
         share=share,
         cluster_name=cluster_name,
         org_name=org_name,
         priority=priority,
         energy_schedule_name=energy_schedule,
+        project_name=project,
     )
 
 
 @command()
 @argument("job", type=JOB)
 async def generate_run_command(root: Root, job: str) -> None:
     """
@@ -1150,15 +1207,15 @@
     id = await resolve_job(
         job,
         client=root.client,
         status=JobStatus.items(),
     )
     job_description = await root.client.jobs.status(id)
     args = _job_to_cli_args(job_description)
-    root.print(f"neuro run " + " ".join(args), soft_wrap=True)
+    root.print("neuro run " + " ".join(args), soft_wrap=True)
 
 
 job.add_command(run)
 job.add_command(generate_run_command)
 job.add_command(ls)
 job.add_command(status)
 job.add_command(exec)
@@ -1201,14 +1258,15 @@
     schedule_timeout: Optional[str],
     privileged: bool,
     share: Sequence[str],
     cluster_name: str,
     org_name: Optional[str],
     priority: Optional[str],
     energy_schedule_name: Optional[str],
+    project_name: Optional[str],
 ) -> JobDescription:
     if http_auth is None:
         http_auth = True
     elif not http_port:
         if http_auth:
             raise click.UsageError("--http-auth requires --http-port")
         else:
@@ -1272,14 +1330,17 @@
         log.info(
             "Using volumes: \n"
             + "\n".join(f"  {volume_to_verbose_str(v)}" for v in volumes)
         )
 
     job_priority = JobPriority[priority.upper()] if priority else None
 
+    if not project_name:
+        project_name = root.client.config.project_name
+
     job = await root.client.jobs.start(
         image=image,
         preset_name=preset,
         cluster_name=cluster_name,
         org_name=org_name,
         entrypoint=entrypoint,
         command=real_cmd,
@@ -1299,14 +1360,15 @@
         description=description,
         restart_policy=job_restart_policy,
         life_span=job_life_span,
         schedule_timeout=job_schedule_timeout,
         privileged=privileged,
         priority=job_priority,
         energy_schedule_name=energy_schedule_name,
+        project_name=project_name,
     )
     permission = Permission(job.uri, Action.WRITE)
     for user in share:
         await root.client.users.share(user, permission)
     with JobStartProgress.create(console=root.console, quiet=root.quiet) as progress:
         progress.begin(job)
         while wait_start and job.status.is_pending:
@@ -1477,17 +1539,17 @@
         res += ["--pass-config"]
     if job.privileged:
         res += ["--privileged"]
     if job.priority != JobPriority.NORMAL:
         res += ["--priority", job.priority.name.lower()]
     if job.energy_schedule_name:
         res += ["--energy-schedule", job.energy_schedule_name]
-    res += [str(job.container.image)]
+    res += ["--project", job.project_name, str(job.container.image)]
     if job.container.command:
-        res += [job.container.command]
+        res += ["--", job.container.command]
     return res
 
 
 def _fix_cmd(cmd_name: str, tmpl: str, cmd: Sequence[str]) -> Sequence[str]:
     if cmd:
         if cmd[0] != "--":
             old_pre, sep, old_suff = tmpl.partition("--")
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/log_formatter.py` & `neuro-cli-23.7.0/src/neuro_cli/log_formatter.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/main.py` & `neuro-cli-23.7.0/src/neuro_cli/main.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/parse_utils.py` & `neuro-cli-23.7.0/src/neuro_cli/parse_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,17 +101,18 @@
     JobColumnInfo("cluster_name", "CLUSTER", "left", max_width=15),
     JobColumnInfo("org_name", "ORG", "left", max_width=15),
     JobColumnInfo("description", "DESCRIPTION", "left", max_width=50),
     JobColumnInfo("command", "COMMAND", "left", max_width=100),
     JobColumnInfo("life_span", "LIFE-SPAN", "left"),
     JobColumnInfo("workdir", "WORKDIR", "left"),
     JobColumnInfo("preset", "PRESET", "left"),
+    JobColumnInfo("project_name", "PROJECT", "left", max_width=25),
 ]
 
-PS_COLUMNS_DEFAULT_FORMAT = "id/name status/when image org_name/owner command"
+PS_COLUMNS_DEFAULT_FORMAT = "id/name status/when image org_name/project_name command"
 
 TOP_COLUMNS = PS_COLUMNS + [
     JobColumnInfo("cpu", "CPU", "right", width=15),
     JobColumnInfo("memory", "MEMORY (MB)", "right", width=15),
     JobColumnInfo("gpu", "GPU (%)", "right", width=15),
     JobColumnInfo("gpu_memory", "GPU_MEMORY (MB)", "right", width=15),
 ]
@@ -322,14 +323,15 @@
     "owner": lambda item: item[0].owner,
     "description": lambda item: item[0].description or "",
     "cluster_name": lambda item: item[0].cluster_name,
     "command": lambda item: item[0].container.command,
     "life_span": lambda item: item[0].life_span or INF,
     "workdir": lambda item: item[0].container.working_dir or "",
     "preset": lambda item: item[0].preset_name or "",
+    "project_name": lambda item: item[0].project_name or "",
     # JobTelemetry attibutes
     "cpu": lambda item: -item[1].cpu,
     "memory": lambda item: -item[1].memory,
     "gpu": lambda item: -(item[1].gpu_duty_cycle or 0),
     "gpu_memory": lambda item: -(item[1].gpu_memory or 0),
 }
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/plugin.py` & `neuro-cli-23.7.0/src/neuro_cli/plugin.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/root.py` & `neuro-cli-23.7.0/src/neuro_cli/root.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/secrets.py` & `neuro-cli-23.7.0/src/neuro_cli/secrets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pathlib
 from typing import Optional
 
-from neuro_cli.click_types import CLUSTER, ORG
-from neuro_cli.formatters.secrets import (
+from neuro_sdk import ORG_NAME_SENTINEL
+
+from .click_types import CLUSTER, ORG, PROJECT
+from .formatters.secrets import (
     BaseSecretsFormatter,
     SecretsFormatter,
     SimpleSecretsFormatter,
 )
-from neuro_cli.formatters.utils import URIFormatter, uri_formatter
-
+from .formatters.utils import URIFormatter, uri_formatter
 from .root import Root
 from .utils import argument, command, group, option, parse_org_name
 
 
 @group()
 def secret() -> None:
     """
@@ -22,37 +23,71 @@
 
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Look on a specified cluster (the current cluster by default).",
 )
-@option("--full-uri", is_flag=True, help="Output full disk URI.")
-async def ls(root: Root, full_uri: bool, cluster: Optional[str]) -> None:
+@option(
+    "--org",
+    type=ORG,
+    help="Look on a specified org (the current org by default).",
+)
+@option("--all-orgs", is_flag=True, default=False, help="Show secrets in all orgs.")
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
+)
+@option(
+    "--all-projects", is_flag=True, default=False, help="Show secrets in all projects."
+)
+@option("--full-uri", is_flag=True, help="Output full secret URI.")
+async def ls(
+    root: Root,
+    full_uri: bool,
+    cluster: Optional[str],
+    org: Optional[str],
+    all_orgs: bool,
+    project: Optional[str],
+    all_projects: bool,
+) -> None:
     """
     List secrets.
     """
     if root.quiet:
         secrets_fmtr: BaseSecretsFormatter = SimpleSecretsFormatter()
     else:
         if full_uri:
             uri_fmtr: URIFormatter = str
         else:
             uri_fmtr = uri_formatter(
-                username=root.client.username,
-                cluster_name=cluster or root.client.cluster_name,
+                cluster_name=root.client.cluster_name,
                 org_name=root.client.config.org_name,
+                project_name=root.client.config.project_name_or_raise,
             )
         secrets_fmtr = SecretsFormatter(
             uri_fmtr,
         )
 
+    if all_orgs:
+        org_name = ORG_NAME_SENTINEL
+    else:
+        org_name = parse_org_name(org, root)  # type: ignore
+
+    if all_projects:
+        project_name = None
+    else:
+        project_name = project or root.client.config.project_name_or_raise
+
     secrets = []
     with root.status("Fetching secrets") as status:
-        async with root.client.secrets.list(cluster_name=cluster) as it:
+        async with root.client.secrets.list(
+            cluster_name=cluster, org_name=org_name, project_name=project_name
+        ) as it:
             async for secret in it:
                 secrets.append(secret)
                 status.update(f"Fetching secrets ({len(secrets)} loaded)")
 
     with root.pager():
         root.print(secrets_fmtr(secrets))
 
@@ -64,54 +99,81 @@
     help="Perform on a specified cluster (the current cluster by default).",
 )
 @option(
     "--org",
     type=ORG,
     help="Look on a specified org (the current org by default).",
 )
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
+)
 @argument("key")
 @argument("value")
 async def add(
-    root: Root, key: str, value: str, cluster: Optional[str], org: Optional[str]
+    root: Root,
+    key: str,
+    value: str,
+    cluster: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
 ) -> None:
     """
     Add secret KEY with data VALUE.
 
     If VALUE starts with @ it points to a file with secrets content.
 
     Examples:
 
       neuro secret add KEY_NAME VALUE
       neuro secret add KEY_NAME @path/to/file.txt
     """
     org_name = parse_org_name(org, root)
     await root.client.secrets.add(
-        key, read_data(value), cluster_name=cluster, org_name=org_name
+        key,
+        read_data(value),
+        cluster_name=cluster,
+        org_name=org_name,
+        project_name=project,
     )
 
 
 @command()
 @option(
     "--cluster",
     type=CLUSTER,
     help="Perform on a specified cluster (the current cluster by default).",
 )
 @option(
     "--org",
     type=ORG,
     help="Look on a specified org (the current org by default).",
 )
+@option(
+    "--project",
+    type=PROJECT,
+    help="Look on a specified project (the current project by default).",
+)
 @argument("key")
-async def rm(root: Root, key: str, cluster: Optional[str], org: Optional[str]) -> None:
+async def rm(
+    root: Root,
+    key: str,
+    cluster: Optional[str],
+    org: Optional[str],
+    project: Optional[str],
+) -> None:
     """
     Remove secret KEY.
     """
 
     org_name = parse_org_name(org, root)
-    await root.client.secrets.rm(key, cluster_name=cluster, org_name=org_name)
+    await root.client.secrets.rm(
+        key, cluster_name=cluster, org_name=org_name, project_name=project
+    )
     if root.verbosity > 0:
         root.print(f"Secret with key '{key}' was successfully removed")
 
 
 secret.add_command(ls)
 secret.add_command(add)
 secret.add_command(rm)
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/service_accounts.py` & `neuro-cli-23.7.0/src/neuro_cli/service_accounts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Sequence
 
-from neuro_cli.click_types import SERVICE_ACCOUNT
+from neuro_cli.click_types import CLUSTER, ORG, PROJECT, SERVICE_ACCOUNT
 from neuro_cli.formatters.service_accounts import (
     BaseServiceAccountsFormatter,
     ServiceAccountFormatter,
     ServiceAccountsFormatter,
     SimpleServiceAccountsFormatter,
     service_account_token_fmtr,
 )
@@ -50,42 +50,60 @@
     "--name",
     metavar="NAME",
     help="Optional service account name",
     default=None,
 )
 @option(
     "--default-cluster",
-    metavar="CLUSTER_NAME",
+    type=CLUSTER,
     help="Service account default cluster. Current cluster will"
     " be used if not specified",
     default=None,
 )
+@option(
+    "--default-org",
+    type=ORG,
+    help="Service account default organization. Current org will"
+    " be used if not specified",
+    default=None,
+)
+@option(
+    "--default-project",
+    type=PROJECT,
+    help="Service account default project. Current project will"
+    " be used if not specified",
+    default=None,
+)
 async def create(
     root: Root,
     name: Optional[str],
     default_cluster: Optional[str],
+    default_org: Optional[str],
+    default_project: Optional[str],
 ) -> None:
     """
     Create a service account.
     """
 
     account, token = await root.client.service_accounts.create(
         name=name,
         default_cluster=default_cluster,
+        default_org=default_org,
+        default_project=default_project,
     )
     fmtr = ServiceAccountFormatter(
         datetime_formatter=get_datetime_formatter(root.iso_datetime_format)
     )
     if root.quiet:
         root.print(token)
     else:
         # No pager here as it can make it harder to copy generated token
         root.print(fmtr(account))
         root.print("")
-        root.print(service_account_token_fmtr(token), soft_wrap=True)
+        root.print(service_account_token_fmtr(token, account), soft_wrap=True)
 
 
 @command()
 @argument("service_account", type=SERVICE_ACCOUNT)
 async def get(root: Root, service_account: str) -> None:
     """
     Get service account SERVICE_ACCOUNT.
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/share.py` & `neuro-cli-23.7.0/src/neuro_cli/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         username = root.client.username
 
     uri_fmtr: URIFormatter
     if full_uri:
         uri_fmtr = str
     else:
         uri_fmtr = uri_formatter(
-            username=root.client.username,
+            project_name=root.client.config.project_name_or_raise,
             cluster_name=root.client.cluster_name,
             org_name=root.client.config.org_name,
         )
 
     uri_obj = URL(uri) if uri else None
 
     if not shared:
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/stats.py` & `neuro-cli-23.7.0/src/neuro_cli/stats.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/storage.py` & `neuro-cli-23.7.0/src/neuro_cli/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,17 @@
 ) -> None:
     """
     Remove files or directories.
 
     Examples:
 
     neuro rm storage:foo/bar
-    neuro rm storage://{username}/foo/bar
-    neuro rm --recursive storage://{username}/foo/
+    neuro rm storage:/{project}/foo/bar
+    neuro rm storage://{cluster}/{project}/foo/bar
+    neuro rm --recursive storage:/{project}/foo/
     neuro rm 'storage:foo/**/*.tmp'
     """
     errors = False
     show_progress = root.tty if progress is None else progress
 
     for uri in await _expand(paths, root, glob):
         try:
@@ -153,15 +154,15 @@
     sort: str,
     directory: bool,
     show_all: bool,
 ) -> None:
     """
     List directory contents.
 
-    By default PATH is equal user's home dir (storage:)
+    By default PATH is equal project's dir (storage:)
     """
     if not paths:
         paths = [URL("storage:")]
     errors = False
     for uri in paths:
         try:
             if directory:
@@ -402,16 +403,16 @@
     # download remote file `foo.txt` into local file `/tmp/foo.txt` with
     # explicit file:// scheme set
     neuro cp storage:foo.txt file:///tmp/foo.txt
     neuro cp -T storage:foo.txt file:///tmp/foo.txt
     neuro cp storage:foo.txt file:///tmp
     neuro cp storage:foo.txt -t file:///tmp
 
-    # download other user's remote file into the current directory
-    neuro cp storage://{username}/foo.txt .
+    # download other project's remote file into the current directory
+    neuro cp storage:/{project}/foo.txt .
 
     # download only files with extension `.out` into the current directory
     neuro cp storage:results/*.out .
     """
     if target_directory:
         if no_target_directory:
             raise click.UsageError(
@@ -606,19 +607,19 @@
     neuro mv storage:foo.txt storage:bar/baz.dat storage:dst
     neuro mv storage:foo.txt storage:bar/baz.dat -t storage:dst
 
     # move the content of remote directory into other existing
     # remote directory
     neuro mv -T storage:foo storage:bar
 
-    # move remote file into other user's directory
-    neuro mv storage:foo.txt storage://{username}/bar.dat
+    # move remote file into other project's directory
+    neuro mv storage:foo.txt storage:/{project}/bar.dat
 
-    # move remote file from other user's directory
-    neuro mv storage://{username}/foo.txt storage:bar.dat
+    # move remote file from other project's directory
+    neuro mv storage:/{project}/foo.txt storage:bar.dat
     """
     if target_directory:
         if no_target_directory:
             raise click.UsageError(
                 "Cannot combine --target-directory (-t) and --no-target-directory (-T)"
             )
         if destination is None:
@@ -710,15 +711,15 @@
     of files, which is colorized ala dircolors if the LS_COLORS environment variable is
     set and output is to tty.  With no arguments, tree lists the files in the storage:
     directory.  When directory arguments are given, tree lists all the files and/or
     directories found in the given directories each in turn.  Upon completion of listing
     all files/directories found, tree returns the total number of files and/or
     directories listed.
 
-    By default PATH is equal user's home dir (storage:)
+    By default PATH is equal project's dir (storage:)
 
     """
     if not path:
         path = URL("storage:")
 
     errors = False
     try:
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli/topics.py` & `neuro-cli-23.7.0/src/neuro_cli/topics.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/src/neuro_cli/utils.py` & `neuro-cli-23.7.0/src/neuro_cli/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,15 +28,23 @@
 )
 
 import click
 import humanize
 from aiohttp import ClientResponseError
 from yarl import URL
 
-from neuro_sdk import Action, Client, JobStatus, ResourceNotFound, Volume
+from neuro_sdk import (
+    ORG_NAME_SENTINEL,
+    Action,
+    Client,
+    JobStatus,
+    OrgNameSentinel,
+    ResourceNotFound,
+    Volume,
+)
 
 from .parse_utils import parse_timedelta
 from .root import Root
 from .stats import upload_gmp_stats
 
 log = logging.getLogger(__name__)
 
@@ -428,129 +436,151 @@
     id, _ = await resolve_job_ex(id_or_name_or_uri, client=client, status=status)
     return id
 
 
 async def resolve_job_ex(
     id_or_name_or_uri: str, *, client: Client, status: Set[JobStatus]
 ) -> Tuple[str, str]:
-    default_user = client.username
     default_cluster = client.cluster_name
     default_org = client.config.org_name
+    default_project = client.config.project_name_or_raise
     if id_or_name_or_uri.startswith("job:"):
         uri = client.parse.str_to_uri(
             id_or_name_or_uri,
             allowed_schemes=("job",),
         )
         assert uri.host
         cluster_name = uri.host
-        owner, _, id_or_name = uri.path.lstrip("/").rpartition("/")
-        owners: Dict[str, Optional[str]] = {}
-        if "/" not in owner:
-            owners[owner] = None
-        elif default_org and owner.startswith(default_org + "/"):
-            org_name, _, owner = owner.partition("/")
-            owners[owner] = org_name
-        elif owner == default_user or owner.startswith(default_user + "/"):
-            owners[owner] = None
+        project, _, id_or_name = uri.path.lstrip("/").rpartition("/")
+        project_names: Dict[str, Optional[str]] = {}
+        if "/" not in project:
+            project_names[project] = None
+        elif default_org and project.startswith(default_org + "/"):
+            org_name, _, project = project.partition("/")
+            project_names[project] = org_name
+        elif project == default_project or project.startswith(default_project + "/"):
+            project_names[project] = None
         else:
-            owners[owner] = None
-            org_name, _, owner = owner.partition("/")
-            owners[owner] = org_name
+            project_names[project] = None
+            org_name, _, project = project.partition("/")
+            project_names[project] = org_name
 
-        if not id_or_name or not owner:
+        if not id_or_name or not project:
             raise ValueError(f"Invalid job URI: {uri!s}")
     else:
         id_or_name = id_or_name_or_uri
-        owner = default_user
-        owners = {default_user: default_org}
+        project = default_project
+        project_names = {default_project: default_org}
         cluster_name = default_cluster
 
     # Temporary fast path.
     if re.fullmatch(JOB_ID_PATTERN, id_or_name):
         return id_or_name, cluster_name
 
     try:
         async with client.jobs.list(
             name=id_or_name,
-            owners=owners.keys(),
+            project_names=project_names.keys(),
             reverse=True,
             cluster_name=cluster_name,
         ) as it:
             async for job in it:
-                if job.owner in owners and job.org_name == owners[job.owner]:
+                if (
+                    job.project_name in project_names
+                    and job.org_name == project_names[job.project_name]
+                ):
                     log.debug(f"Job name '{id_or_name}' resolved to job ID '{job.id}'")
                     return job.id, cluster_name
     except asyncio.CancelledError:
         raise
     except ClientResponseError as e:
         log.error(
             f"Failed to resolve job-name {id_or_name_or_uri} resolved as "
-            f"name={id_or_name}, owners={owners} to a job-ID: {e}"
+            f"name={id_or_name}, project_names={project_names} to a job-ID: {e}"
         )
 
-    if owner != default_user:
+    if project != default_project:
         raise ValueError(f"Failed to resolve job {id_or_name_or_uri}")
     return id_or_name, cluster_name
 
 
 DISK_ID_PATTERN = r"disk-[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}"
 
 
 async def resolve_disk(
     id_or_name_or_uri: Union[str, URL],
     *,
     client: Client,
     cluster_name: Optional[str] = None,
+    org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+    project_name: Optional[str] = None,
 ) -> str:
     if isinstance(id_or_name_or_uri, URL):
         id_or_name = id_or_name_or_uri.parts[-1]
     else:
         id_or_name = id_or_name_or_uri
     # Temporary fast path.
     if re.fullmatch(DISK_ID_PATTERN, id_or_name):
         return id_or_name
 
     if isinstance(id_or_name_or_uri, URL):
         cluster_name = id_or_name_or_uri.host
-        possible_owners = [
-            "/".join(id_or_name_or_uri.parts[1:-1]),
-            "/".join(id_or_name_or_uri.parts[2:-1]),
-        ]
-        for owner in possible_owners:
-            try:
-                disk = await client.disks.get(id_or_name, cluster_name, owner=owner)
-                return disk.id
-            except ResourceNotFound:
-                pass
-        raise ValueError(f"Failed to resolve job {id_or_name_or_uri}")
+        if cluster_name:
+            possible_org = id_or_name_or_uri.parts[1]
+            cluster = client.config.clusters[cluster_name]
+            org_name = possible_org if possible_org in cluster.orgs else None
+        else:
+            org_name = ORG_NAME_SENTINEL
+        if cluster_name and org_name:
+            project_name = "/".join(id_or_name_or_uri.parts[2:-1])
+        else:
+            project_name = "/".join(id_or_name_or_uri.parts[1:-1])
+        try:
+            disk = await client.disks.get(
+                id_or_name,
+                cluster_name=cluster_name,
+                org_name=org_name,
+                project_name=project_name,
+            )
+            return disk.id
+        except ResourceNotFound:
+            pass
+        raise ValueError(f"Failed to resolve disk {id_or_name_or_uri}")
     else:
-        disk = await client.disks.get(id_or_name, cluster_name)
+        disk = await client.disks.get(
+            id_or_name,
+            cluster_name=cluster_name,
+            org_name=org_name,
+            project_name=project_name,
+        )
     return disk.id
 
 
 BUCKET_ID_PATTERN = (
     r"bucket-[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}"
 )
 
 
 async def resolve_bucket(
     id_or_name: str,
     *,
     client: Client,
     cluster_name: Optional[str] = None,
-    bucket_owner: Optional[str] = None,
+    org_name: Union[Optional[str], OrgNameSentinel] = ORG_NAME_SENTINEL,
+    project_name: Optional[str] = None,
 ) -> str:
     # Temporary fast path.
     if re.fullmatch(BUCKET_ID_PATTERN, id_or_name):
         return id_or_name
 
     bucket = await client.buckets.get(
         id_or_name,
         cluster_name=cluster_name,
-        bucket_owner=bucket_owner,
+        org_name=org_name,
+        project_name=project_name,
     )
     return bucket.id
 
 
 BUCKET_CREDENTIAL_ID_PATTERN = (
     r"bucket-credentials-[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}"
 )
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli.egg-info/PKG-INFO` & `neuro-cli-23.7.0/src/neuro_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuro-cli
-Version: 23.2.0
+Version: 23.7.0
 Summary: Neuro Platform client
 Home-page: https://github.com/neuro-inc/platform-client-python
 Author: Neu.ro Team
 Author-email: team@neu.ro
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `neuro-cli-23.2.0/src/neuro_cli.egg-info/SOURCES.txt` & `neuro-cli-23.7.0/src/neuro_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -535,26 +535,31 @@
 tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_5.ref
 tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_6.ref
 tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_7.ref
 tests/unit/formatters/ascii/TestBlobFormatter.test_long_formatter[formatter1]_8.ref
 tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref
 tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref
 tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref
-tests/unit/formatters/ascii/TestClusterUserFormatter.test_cluster_list_0.ref
+tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_0.ref
+tests/unit/formatters/ascii/TestClusterOrgProjectsFormatter.test_output_with_current_project_0.ref
+tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_no_user_info_0.ref
+tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref
 tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref
 tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref
 tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref
 tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref
 tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref
 tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref
+tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref
+tests/unit/formatters/ascii/TestConfigFormatter.test_output_without_project_0.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_finished_0.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_commit_started_0.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_0.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_1.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_pull_2.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_0.ref
 tests/unit/formatters/ascii/TestDockerImageProgress.test_no_tty_push_1.ref
@@ -623,14 +628,20 @@
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-test-user]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref
+tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-test-user]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref
 tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref
@@ -746,14 +757,16 @@
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_empty[iso]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[human]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_life_span[iso]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[human]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_org_name[iso]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[human]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_preset[iso]_0.ref
+tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[human]_0.ref
+tests/unit/formatters/ascii/TestTabularJobsFormatter.test_project_name[iso]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[0-owner-#less#you#more#]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[1-alice-alice]_1.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-0-owner-#less#you#more#]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[human-1-alice-alice]_1.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref
 tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref
@@ -777,9 +790,11 @@
 tests/unit/formatters/ascii/test_disk_formatter_0.ref
 tests/unit/formatters/ascii/test_disks_formatter_0.ref
 tests/unit/formatters/ascii/test_disks_formatter_long_0.ref
 tests/unit/formatters/ascii/test_disks_formatter_short_0.ref
 tests/unit/formatters/ascii/test_disks_formatter_simple_0.ref
 tests/unit/formatters/ascii/test_secrets_formatter_short_0.ref
 tests/unit/formatters/ascii/test_secrets_formatter_simple_0.ref
+tests/unit/formatters/ascii/test_service_account_formatter[None]_0.ref
+tests/unit/formatters/ascii/test_service_account_formatter[some-org]_0.ref
 tests/unit/formatters/ascii/test_service_account_formatter_0.ref
 tests/unit/formatters/ascii/test_service_accounts_formatter_simple_0.ref
```

### Comparing `neuro-cli-23.2.0/tests/__init__.py` & `neuro-cli-23.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/conftest.py` & `neuro-cli-23.7.0/tests/conftest.py`

 * *Files 8% similar despite different names*

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
 
 from neuro_cli.asyncio_utils import setup_child_watcher
 
 
 def pytest_addoption(parser: Any, pluginmanager: Any) -> None:
@@ -100,17 +100,19 @@
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
     ) -> Client:
         url = URL(url_str)
         if clusters is None:
             cluster_config = Cluster(
                 registry_url=URL(registry_url),
                 monitoring_url=(url / "jobs"),
                 storage_url=(url / "storage"),
@@ -140,14 +142,25 @@
                         credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
                     ),
                 },
                 name="default",
                 orgs=[org_name],
             )
             clusters = {cluster_config.name: cluster_config}
+        if projects is None:
+            projects = {}
+            for cluster in clusters.values():
+                project = Project(
+                    cluster_name=cluster.name,
+                    org_name=cluster.orgs[0],
+                    name="test-project",
+                    role="owner",
+                )
+                projects[project.key] = project
+            project_name = "test-project"
         if token_url is not None:
             real_auth_config = replace(auth_config, token_url=token_url)
         else:
             real_auth_config = auth_config
         if plugin_manager is None:
             plugin_manager = PluginManager()
         cluster_name = next(iter(clusters))
@@ -155,15 +168,17 @@
             auth_config=real_auth_config,
             auth_token=_AuthToken.create_non_expiring(token),
             url=URL(url),
             admin_url=URL(url) / ".." / ".." / "apis" / "admin" / "v1",
             version=__version__,
             cluster_name=cluster_name,
             org_name=clusters[cluster_name].orgs[0],
+            project_name=project_name,
             clusters=clusters,
+            projects=projects or {},
         )
         config_dir = tmp_path / ".neuro"
         _save(config, config_dir)
         session = aiohttp.ClientSession(trace_configs=[_make_trace_config()])
         return Client._create(
             session,
             config_dir,
```

### Comparing `neuro-cli-23.2.0/tests/e2e/assets/echo-tag.tar` & `neuro-cli-23.7.0/tests/e2e/assets/echo-tag.tar`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/conftest.py` & `neuro-cli-23.7.0/tests/e2e/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,15 +700,20 @@
             return bucket
 
     create_bucket = run_async(acreate_bucket)
 
     async def adelete_bucket(self, bucket: Bucket) -> None:
         __tracebackhide__ = True
         async with api_get(timeout=CLIENT_TIMEOUT, path=self._nmrc_path) as client:
-            await client.buckets.rm(bucket.id, bucket_owner=bucket.owner)
+            await client.buckets.rm(
+                bucket.id,
+                cluster_name=bucket.cluster_name,
+                org_name=bucket.org_name,
+                project_name=bucket.project_name,
+            )
 
     delete_bucket = run_async(adelete_bucket)
 
     async def acleanup_bucket(self, bucket: Bucket) -> None:
         __tracebackhide__ = True
         # Each test needs a clean bucket state and we can't delete bucket until it's
         # cleaned
@@ -720,15 +725,19 @@
                 # 10000 of objects.
                 # If we do, please add a semaphore here.
                 tasks = []
                 async for blob in blobs_it:
                     log.info("Removing %s", blob.uri)
                     tasks.append(
                         client.buckets.delete_blob(
-                            bucket.id, key=blob.key, bucket_owner=bucket.owner
+                            bucket.id,
+                            key=blob.key,
+                            cluster_name=bucket.cluster_name,
+                            org_name=bucket.org_name,
+                            project_name=bucket.project_name,
                         )
                     )
             await asyncio.gather(*tasks)
 
     cleanup_bucket = run_async(acleanup_bucket)
 
     @run_async
```

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_admin.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
 @pytest.mark.e2e
 @pytest.mark.skip
 def test_list_org_clusters(
     helper: Helper, tmp_test_org: str, tmp_test_cluster: str
 ) -> None:
     helper.run_cli(["admin", "add-org-cluster", tmp_test_cluster, tmp_test_org])
-    captured = helper.run_cli(["admin", "get-org-clusters", tmp_test_cluster])
+    captured = helper.run_cli(["admin", "get-cluster-orgs", tmp_test_cluster])
     org_cluster_lines = captured.out.split("\n")[3:]
     assert any(
         tmp_test_org in line and tmp_test_cluster in line for line in org_cluster_lines
     )
 
 
 @pytest.mark.e2e
@@ -393,15 +393,15 @@
 def test_remove_org_cluster(
     helper: Helper, tmp_test_org: str, tmp_test_cluster: str
 ) -> None:
     helper.run_cli(["admin", "add-org-cluster", tmp_test_cluster, tmp_test_org])
     helper.run_cli(
         ["admin", "remove-org-cluster", "--force", tmp_test_cluster, tmp_test_org]
     )
-    captured = helper.run_cli(["admin", "get-org-clusters", tmp_test_cluster])
+    captured = helper.run_cli(["admin", "get-cluster-orgs", tmp_test_cluster])
     assert tmp_test_org not in captured.out
 
 
 @pytest.fixture
 def tmp_test_org_cluster(
     helper: Helper, tmp_test_cluster: str, tmp_test_org: str
 ) -> Iterator[Tuple[str, str]]:
```

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_blob_storage.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_blob_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_disks.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_disks.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_images.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_images.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_jobs.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_jobs.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_secrets.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_secrets.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_share.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_share.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/test_e2e_storage.py` & `neuro-cli-23.7.0/tests/e2e/test_e2e_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/e2e/utils.py` & `neuro-cli-23.7.0/tests/e2e/utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/conftest.py` & `neuro-cli-23.7.0/tests/unit/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, Callable, DefaultDict, Iterator, List, Optional, Set, Union
 
 import click
 import pytest
 from rich.console import Console, RenderableType
 from yarl import URL
 
-from neuro_sdk import Cluster, Factory, Preset
+from neuro_sdk import Cluster, Factory, Preset, Project
 from neuro_sdk._config import _AuthConfig, _AuthToken, _ConfigData
 
 from neuro_cli import __version__
 from neuro_cli.const import EX_OK
 from neuro_cli.main import main
 from neuro_cli.root import Root
 from neuro_cli.utils import Command, Context
@@ -55,15 +55,15 @@
                 credits_per_hour=Decimal("10"), cpu=7, memory=2 * 2**30
             ),
             "cpu-large": Preset(
                 credits_per_hour=Decimal("10"), cpu=7, memory=14 * 2**30
             ),
         },
         name="default",
-        orgs=[None],
+        orgs=[None, "org"],
     )
     cluster2_config = Cluster(
         registry_url=URL("https://registry2-dev.neu.ro"),
         storage_url=URL("https://storage2-dev.neu.ro"),
         users_url=URL("https://users2-dev.neu.ro"),
         monitoring_url=URL("https://monitoring2-dev.neu.ro"),
         secrets_url=URL("https://secrets2-dev.neu.ro"),
@@ -85,14 +85,57 @@
         version=__version__,
         cluster_name=cluster_config.name,
         org_name=cluster_config.orgs[0],
         clusters={
             cluster_config.name: cluster_config,
             cluster2_config.name: cluster2_config,
         },
+        projects={
+            Project.Key(
+                cluster_name=cluster_config.name,
+                org_name=cluster_config.orgs[0],
+                project_name="project",
+            ): Project(
+                cluster_name=cluster_config.name,
+                org_name=cluster_config.orgs[0],
+                name="project",
+                role="owner",
+            ),
+            Project.Key(
+                cluster_name=cluster_config.name,
+                org_name=None,
+                project_name="user",
+            ): Project(
+                cluster_name=cluster_config.name,
+                org_name=None,
+                name="user",
+                role="admin",
+            ),
+            Project.Key(
+                cluster_name=cluster_config.name,
+                org_name=None,
+                project_name="otherproject",
+            ): Project(
+                cluster_name=cluster_config.name,
+                org_name=None,
+                name="otherproject",
+                role="admin",
+            ),
+            Project.Key(
+                cluster_name=cluster2_config.name,
+                org_name=None,
+                project_name="user",
+            ): Project(
+                cluster_name=cluster2_config.name,
+                org_name=None,
+                name="user",
+                role="admin",
+            ),
+        },
+        project_name="project",
     )
     Factory(nmrc_path)._save(config)
     return nmrc_path
 
 
 def create_root(config_path: Path) -> Root:
     async def cmd() -> None:
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_aws_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_azure_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestCloudProviderOptionsFormatter.test_formatter_gcp_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_cluster_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClusterUserFormatter.test_list_users_with_user_info_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_storage_without_size_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_maximum_node_pool_properties_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_cloud_provider_with_minimum_node_pool_properties_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestClustersFormatter.test_cluster_with_on_prem_cloud_provider_list_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_project_name_0.ref`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
+ Current Project      main                        
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
-Resource Presets:                                                                                       
- Name        #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
-━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
- gpu-small      7   32.2 GB        ×               ×           1 x nvidia-tesla-k80    10               
- gpu-large      7   64.4 GB        ×               ×           1 x nvidia-tesla-v100   10               
- cpu-small      7    2.1 GB        ×               ×                                   10               
- cpu-large      7   15.0 GB        ×               ×                                   10
+Resource Presets:                                                                                         
+ Name          #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ gpu-small        7   32.2 GB        ×               ×           1 x nvidia-tesla-k80    10               
+ gpu-large        7   64.4 GB        ×               ×           1 x nvidia-tesla-v100   10               
+ cpu-small        7    2.1 GB        ×               ×                                   10               
+ cpu-large        7   15.0 GB        ×               ×                                   10               
+ cpu-large-p      7   15.0 GB        √               √                                   10
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_energy_schedules_0.ref`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
+ Current Project      project                     
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
 Resource Presets:                                                                                       
  Name        #CPU    Memory   Round Robin   Preemptible Node   GPU                     Credits per hour 
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_for_tpu_presets_0.ref`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
+ Current Project      test-project                
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
 Resource Presets:                                                                                                      
  Name          #CPU    Memory   Round Robin   Preemptible Node   GPU                     TPU          Credits per hour 
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_jobs_available_0.ref`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
+ Current Project      project                     
  Credits Quota        500.00                      
  Jobs Quota           10                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
 Resource Presets:                                                                                                    
  Name        #CPU    Memory   Round Robin   Preemptible Node   GPU                     Jobs Avail   Credits per hour 
 ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestConfigFormatter.test_output_with_org_quota_0.ref`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 User Configuration:                               
  User Name            user                        
  Current Cluster      default                     
  Current Org          <no-org>                    
+ Current Project      project                     
  Credits Quota        500.00                      
  Jobs Quota           10                          
  Org Credits Quota    1000.00                     
  Org Jobs Quota       50                          
  API URL              https://dev.neu.ro/api/v1   
  Docker Registry URL  https://registry-dev.neu.ro 
 Resource Presets:
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Job                     test-job              
  Owner                   owner                 
+ Project                 myproject             
  Cluster                 default               
  Description             test job description  
  Status                  pending               
  Image                   test-image            
  Command                 test-command          
  Priority                Normal                
  Price (credits / hour)  15.0000               
  Current cost            150.0000              
  Resources                Memory  16.8 MB      
                           CPU         0.1      
  Round Robin             True                  
- Preemptible Node        True                  
  TTY                     False                 
  Created                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Job                     test-job                         
  Owner                   owner                            
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  pending                          
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  Round Robin             True                             
- Preemptible Node        True                             
  TTY                     False                            
  Created                 2018-09-25T12:28:21.298672+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[human]_0.ref`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Job                     test-job                                                    
- Name                    test-job-name                                               
- Owner                   test-user                                                   
- Cluster                 default                                                     
- Description             test job description                                        
- Status                  failed (ErrorReason)                                        
- Image                   image:test-image:sometag                                    
- Command                 test-command                                                
- Priority                Normal                                                      
- Price (credits / hour)  15.0000                                                     
- Current cost            150.0000                                                    
- Resources                Memory  16.8 MB                                            
-                          CPU         0.1                                            
- TTY                     False                                                       
- Disk volumes             /mnt/disk1  disk:disk1                           READONLY  
-                          /mnt/disk2  disk:/otheruser/disk2                          
-                          /mnt/disk3  disk://othercluster/otheruser/disk3            
- Http URL                http://local.host.test/                                     
- Http port               80                                                          
- Http authentication     True                                                        
- Created                 Sep 25 2018 at 12:28                                        
- Started                 Sep 25 2018 at 12:28                                        
- Finished                Sep 25 2018 at 12:28                                        
- Exit code               123                                                         
+Job                     test-job                                                       
+ Name                    test-job-name                                                  
+ Owner                   test-user                                                      
+ Project                 myproject                                                      
+ Cluster                 default                                                        
+ Description             test job description                                           
+ Status                  failed (ErrorReason)                                           
+ Image                   image:test-image:sometag                                       
+ Command                 test-command                                                   
+ Priority                Normal                                                         
+ Price (credits / hour)  15.0000                                                        
+ Current cost            150.0000                                                       
+ Resources                Memory  16.8 MB                                               
+                          CPU         0.1                                               
+ TTY                     False                                                          
+ Disk volumes             /mnt/disk1  disk:disk1                              READONLY  
+                          /mnt/disk2  disk:/otherproject/disk2                          
+                          /mnt/disk3  disk://othercluster/otherproject/disk3            
+ Http URL                http://local.host.test/                                        
+ Http port               80                                                             
+ Http authentication     True                                                           
+ Created                 Sep 25 2018 at 12:28                                           
+ Started                 Sep 25 2018 at 12:28                                           
+ Finished                Sep 25 2018 at 12:28                                           
+ Exit code               123                                                            
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_disk_volumes_short[iso]_0.ref`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Job                     test-job                                                    
- Name                    test-job-name                                               
- Owner                   test-user                                                   
- Cluster                 default                                                     
- Description             test job description                                        
- Status                  failed (ErrorReason)                                        
- Image                   image:test-image:sometag                                    
- Command                 test-command                                                
- Priority                Normal                                                      
- Price (credits / hour)  15.0000                                                     
- Current cost            150.0000                                                    
- Resources                Memory  16.8 MB                                            
-                          CPU         0.1                                            
- TTY                     False                                                       
- Disk volumes             /mnt/disk1  disk:disk1                           READONLY  
-                          /mnt/disk2  disk:/otheruser/disk2                          
-                          /mnt/disk3  disk://othercluster/otheruser/disk3            
- Http URL                http://local.host.test/                                     
- Http port               80                                                          
- Http authentication     True                                                        
- Created                 2018-09-25T12:28:21.298672+00:00                            
- Started                 2018-09-25T12:28:59.759433+00:00                            
- Finished                2018-09-25T12:28:59.759433+00:00                            
- Exit code               123                                                         
+Job                     test-job                                                       
+ Name                    test-job-name                                                  
+ Owner                   test-user                                                      
+ Project                 myproject                                                      
+ Cluster                 default                                                        
+ Description             test job description                                           
+ Status                  failed (ErrorReason)                                           
+ Image                   image:test-image:sometag                                       
+ Command                 test-command                                                   
+ Priority                Normal                                                         
+ Price (credits / hour)  15.0000                                                        
+ Current cost            150.0000                                                       
+ Resources                Memory  16.8 MB                                               
+                          CPU         0.1                                               
+ TTY                     False                                                          
+ Disk volumes             /mnt/disk1  disk:disk1                              READONLY  
+                          /mnt/disk2  disk:/otherproject/disk2                          
+                          /mnt/disk3  disk://othercluster/otherproject/disk3            
+ Http URL                http://local.host.test/                                        
+ Http port               80                                                             
+ Http authentication     True                                                           
+ Created                 2018-09-25T12:28:21.298672+00:00                               
+ Started                 2018-09-25T12:28:59.759433+00:00                               
+ Finished                2018-09-25T12:28:59.759433+00:00                               
+ Exit code               123                                                            
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Job                     test-job              
- Owner                   owner                 
- Cluster                 default               
- Description             test job description  
- Status                  pending               
- Image                   test-image            
- Command                 test-command          
- Preset                  cpu-small             
- Energy schedule         some-schedule         
- Priority                Normal                
- Price (credits / hour)  15.0000               
- Current cost            150.0000              
- Resources                Memory  16.8 MB      
-                          CPU         0.1      
- Round Robin             True                  
- TTY                     False                 
- Created                 Sep 25 2018 at 12:28
+Job                     test-job                         
+ Owner                   owner                            
+ Project                 myproject                        
+ Cluster                 default                          
+ Description             test job description             
+ Status                  pending                          
+ Image                   test-image                       
+ Command                 test-command                     
+ Preset                  cpu-small                        
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory  16.8 MB                 
+                          CPU         0.1                 
+ TTY                     False                            
+ Created                 2018-09-25T12:28:21.298672+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_on_preemptible_node[iso]_0.ref`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Job                     test-job                         
  Owner                   owner                            
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  pending                          
  Image                   test-image                       
  Command                 test-command                     
- Preset                  cpu-small                        
- Energy schedule         some-schedule                    
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  Round Robin             True                             
+ Preemptible Node        True                             
  TTY                     False                            
  Created                 2018-09-25T12:28:21.298672+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-Job                     test-job                   
- Owner                   test-user                  
- Cluster                 default                    
- Description             test job description       
- Status                  running (ContainerRunning) 
- Image                   test-image                 
- Entrypoint              /usr/bin/make              
- Command                 test                       
- Priority                Normal                     
- Price (credits / hour)  15.0000                    
- Current cost            150.0000                   
- Resources                Memory  16.8 MB           
-                          CPU         0.1           
- TTY                     False                      
- Internal Hostname       host.local                 
- Http URL                http://local.host.test/    
- Created                 Sep 25 2018 at 12:28       
- Started                 Sep 25 2018 at 12:28
+Job                     test-job                         
+ Tags                    tag1, tag2, tag3                 
+ Owner                   test-user                        
+ Project                 myproject                        
+ Cluster                 default                          
+ Description             test job description             
+ Status                  failed (ErrorReason)             
+ Image                   test-image                       
+ Command                 test-command                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory  16.8 MB                 
+                          CPU         0.1                 
+ TTY                     False                            
+ Http URL                http://local.host.test/          
+ Http port               80                               
+ Http authentication     True                             
+ Created                 2018-09-25T12:28:21.298672+00:00 
+ Started                 2018-09-25T12:28:59.759433+00:00 
+ Finished                2018-09-25T12:28:59.759433+00:00 
+ Exit code               123                              
+ Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Job                     test-job                         
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  running (ContainerRunning)       
  Image                   test-image                       
- Entrypoint              /usr/bin/make                    
- Command                 test                             
+ Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  TTY                     False                            
  Internal Hostname       host.local
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[human]_0.ref`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Job                     test-job                 
  Name                    test-job-name            
  Owner                   test-user                
+ Project                 myproject                
  Cluster                 default                  
  Description             test job description     
  Status                  failed (ErrorReason)     
  Image                   image:test-image:sometag 
  Command                 test-command             
  Priority                Normal                   
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Job                     test-job                         
  Name                    test-job-name                    
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
  Image                   image:test-image:sometag         
  Command                 test-command                     
+ Working dir             /working/dir                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  TTY                     False                            
  Http URL                http://local.host.test/          
  Http port               80                               
  Http authentication     True                             
- Environment              ENV_NAME_1  __value1__          
-                          ENV_NAME_2  **value2**          
  Created                 2018-09-25T12:28:21.298672+00:00 
  Started                 2018-09-25T12:28:59.759433+00:00 
  Finished                2018-09-25T12:28:59.759433+00:00 
  Exit code               123                              
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-Job                     test-job                
- Owner                   test-user               
- Cluster                 default                 
- Description             test job description    
- Status                  failed (ErrorReason)    
- Image                   test-image              
- Command                 test-command            
- Priority                Normal                  
- Price (credits / hour)  15.0000                 
- Current cost            150.0000                
- Resources                Memory  16.8 MB        
-                          CPU         0.1        
- Life span               1d2h3m4s                
- TTY                     False                   
- Http URL                http://local.host.test/ 
- Http port               80                      
- Http authentication     True                    
- Created                 Sep 25 2018 at 12:28    
- Started                 Sep 25 2018 at 12:28    
- Finished                Sep 25 2018 at 12:28    
- Exit code               123                     
+Job                     test-job                 
+ Name                    test-job-name            
+ Owner                   test-user                
+ Project                 myproject                
+ Cluster                 default                  
+ Description             test job description     
+ Status                  failed (ErrorReason)     
+ Image                   image:test-image:sometag 
+ Command                 test-command             
+ Working dir             /working/dir             
+ Priority                Normal                   
+ Price (credits / hour)  15.0000                  
+ Current cost            150.0000                 
+ Resources                Memory  16.8 MB         
+                          CPU         0.1         
+ TTY                     False                    
+ Http URL                http://local.host.test/  
+ Http port               80                       
+ Http authentication     True                     
+ Created                 Sep 25 2018 at 12:28     
+ Started                 Sep 25 2018 at 12:28     
+ Finished                Sep 25 2018 at 12:28     
+ Exit code               123                      
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[iso]_0.ref`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                         
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[human]_0.ref`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                
  Owner                   test-user               
+ Project                 myproject               
  Cluster                 default                 
  Description             test job description    
  Status                  failed (ErrorReason)    
  Image                   test-image              
  Command                 test-command            
  Priority                Normal                  
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_without_value[iso]_0.ref`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                         
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Job                     test-job                
- Name                    test-job-name           
  Owner                   test-user               
+ Project                 myproject               
  Cluster                 default                 
  Description             test job description    
  Status                  failed (ErrorReason)    
  Image                   test-image              
  Command                 test-command            
  Priority                Normal                  
  Price (credits / hour)  15.0000                 
  Current cost            150.0000                
  Resources                Memory  16.8 MB        
                           CPU         0.1        
+ Restart policy          always                  
+ Restarts                4                       
  TTY                     False                   
  Http URL                http://local.host.test/ 
  Http port               80                      
  Http authentication     True                    
  Created                 Sep 25 2018 at 12:28    
  Started                 Sep 25 2018 at 12:28    
  Finished                Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[iso]_0.ref`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Job                     test-job                         
  Name                    test-job-name                    
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[human]_0.ref`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Job                     test-job                   
  Name                    test-job                   
  Owner                   test-user                  
+ Project                 myproject                  
  Cluster                 default                    
  Organization            test-job-org-name          
  Status                  running (ContainerRunning) 
  Image                   test-image                 
  Command                 test-command               
  Priority                Normal                     
- Price (credits / hour)  15.0000                    
- Current cost            150.0000                   
+ Price (credits / hour)  0.0010                     
+ Current cost            0.0100                     
  Resources                Memory  16.8 MB           
                           CPU         0.1           
  TTY                     False                      
  Http URL                http://local.host.test/    
  Created                 Sep 25 2018 at 12:28       
  Started                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[iso]_0.ref`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Job                     test-job                         
- Name                    test-job                         
- Owner                   test-user                        
+ Owner                   owner                            
+ Project                 myproject                        
  Cluster                 default                          
- Organization            test-job-org-name                
- Status                  running (ContainerRunning)       
+ Description             test job description             
+ Status                  pending (ContainerCreating)      
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
- TTY                     False                            
- Http URL                http://local.host.test/          
- Created                 2018-09-25T12:28:21.298672+00:00 
- Started                 2018-09-25T12:28:24.759433+00:00
+ Round Robin             True                             
+ TTY                     True                             
+ Created                 2018-09-25T12:28:21.298672+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_name[human]_0.ref`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Job                     test-job                          
- Name                    test-job-name                     
- Owner                   test-user                         
- Cluster                 default                           
- Organization            test-org                          
- Description             test job description              
- Status                  failed (ErrorReason)              
- Image                   test-image                        
- Command                 test-command                      
- Priority                Normal                            
- Price (credits / hour)  15.0000                           
- Current cost            150.0000                          
- Resources                Memory  16.8 MB                  
-                          CPU         0.1                  
- TTY                     False                             
- Volumes                  /mnt/storage  storage:folder     
- Http URL                http://local.host.test/           
- Http port               80                                
- Http authentication     True                              
- Created                 Sep 25 2018 at 12:28              
- Started                 Sep 25 2018 at 12:28              
- Finished                Sep 25 2018 at 12:28              
- Exit code               123                               
+Job                     test-job                
+ Name                    test-job-name           
+ Owner                   test-user               
+ Project                 myproject               
+ Cluster                 default                 
+ Description             test job description    
+ Status                  failed (ErrorReason)    
+ Image                   test-image              
+ Command                 test-command            
+ Priority                Normal                  
+ Price (credits / hour)  15.0000                 
+ Current cost            150.0000                
+ Resources                Memory  16.8 MB        
+                          CPU         0.1        
+ TTY                     False                   
+ Http URL                http://local.host.test/ 
+ Http port               80                      
+ Http authentication     True                    
+ Created                 Sep 25 2018 at 12:28    
+ Started                 Sep 25 2018 at 12:28    
+ Finished                Sep 25 2018 at 12:28    
+ Exit code               123                     
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Job                     test-job                          
- Name                    test-job-name                     
- Owner                   test-user                         
- Cluster                 default                           
- Organization            test-org                          
- Description             test job description              
- Status                  failed (ErrorReason)              
- Image                   test-image                        
- Command                 test-command                      
- Priority                Normal                            
- Price (credits / hour)  15.0000                           
- Current cost            150.0000                          
- Resources                Memory  16.8 MB                  
-                          CPU         0.1                  
- TTY                     False                             
- Volumes                  /mnt/storage  storage:folder     
- Http URL                http://local.host.test/           
- Http port               80                                
- Http authentication     True                              
- Created                 2018-09-25T12:28:21.298672+00:00  
- Started                 2018-09-25T12:28:59.759433+00:00  
- Finished                2018-09-25T12:28:59.759433+00:00  
- Exit code               123                               
+Job                     test-job                                       
+ Tags                    long-tag-1, long-tag-2, long-tag-3, long-tag-4 
+ Owner                   test-user                                      
+ Project                 myproject                                      
+ Cluster                 default                                        
+ Description             test job description                           
+ Status                  failed (ErrorReason)                           
+ Image                   test-image                                     
+ Command                 test-command                                   
+ Priority                Normal                                         
+ Price (credits / hour)  15.0000                                        
+ Current cost            150.0000                                       
+ Resources                Memory  16.8 MB                               
+                          CPU         0.1                               
+ TTY                     False                                          
+ Http URL                http://local.host.test/                        
+ Http port               80                                             
+ Http authentication     True                                           
+ Created                 2018-09-25T12:28:21.298672+00:00               
+ Started                 2018-09-25T12:28:59.759433+00:00               
+ Finished                2018-09-25T12:28:59.759433+00:00               
+ Exit code               123                                            
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_partial_credits[iso]_0.ref`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Job                     test-job                         
  Name                    test-job                         
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Organization            test-job-org-name                
  Status                  running (ContainerRunning)       
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  0.0010
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Job                     test-job              
- Owner                   owner                 
- Cluster                 default               
- Description             test job description  
- Status                  pending               
- Image                   test-image            
- Command                 test-command          
- Preset                  cpu-small             
- Priority                Normal                
- Price (credits / hour)  15.0000               
- Current cost            150.0000              
- Resources                Memory  16.8 MB      
-                          CPU         0.1      
- TTY                     False                 
+Job                     test-job                    
+ Owner                   owner                       
+ Project                 myproject                   
+ Cluster                 default                     
+ Status                  pending (ContainerCreating) 
+ Image                   test-image                  
+ Command                 test-command                
+ Priority                Normal                      
+ Price (credits / hour)  15.0000                     
+ Current cost            150.0000                    
+ Resources                Memory  16.8 MB            
+                          CPU         0.1            
+ Round Robin             True                        
+ TTY                     False                       
  Created                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_preset_name[human]_0.ref`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-Job                     test-job                         
- Owner                   owner                            
- Cluster                 default                          
- Description             test job description             
- Status                  pending                          
- Image                   test-image                       
- Command                 test-command                     
- Preset                  cpu-small                        
- Priority                Normal                           
- Price (credits / hour)  15.0000                          
- Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
- TTY                     False                            
- Created                 2018-09-25T12:28:21.298672+00:00
+Job                     test-job              
+ Owner                   owner                 
+ Project                 myproject             
+ Cluster                 default               
+ Description             test job description  
+ Status                  pending               
+ Image                   test-image            
+ Command                 test-command          
+ Preset                  cpu-small             
+ Priority                Normal                
+ Price (credits / hour)  15.0000               
+ Current cost            150.0000              
+ Resources                Memory  16.8 MB      
+                          CPU         0.1      
+ TTY                     False                 
+ Created                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_urls[human]_0.ref`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-Job                     test-job                
- Owner                   test-user               
- Cluster                 default                 
- Description             test job description    
- Status                  failed (ErrorReason)    
- Image                   test-image              
- Command                 test-command            
- Priority                Normal                  
- Price (credits / hour)  15.0000                 
- Current cost            150.0000                
- Resources                Memory  16.8 MB        
-                          CPU         0.1        
- Restart policy          always                  
- Restarts                4                       
- TTY                     False                   
- Http URL                http://local.host.test/ 
- Http port               80                      
- Http authentication     True                    
- Created                 Sep 25 2018 at 12:28    
- Started                 Sep 25 2018 at 12:28    
- Finished                Sep 25 2018 at 12:28    
- Exit code               123                     
+Job                     test-job                                     
+ Name                    test-job-name                                
+ Owner                   test-user                                    
+ Project                 myproject                                    
+ Cluster                 default                                      
+ Organization            test-org                                     
+ Description             test job description                         
+ Status                  failed (ErrorReason)                         
+ Image                   test-image                                   
+ Command                 test-command                                 
+ Priority                Normal                                       
+ Price (credits / hour)  15.0000                                      
+ Current cost            150.0000                                     
+ Resources                Memory  16.8 MB                             
+                          CPU         0.1                             
+ TTY                     False                                        
+ Volumes                  /mnt/storage  storage:/test-user/folder     
+ Http URL                http://local.host.test/                      
+ Http port               80                                           
+ Http authentication     True                                         
+ Created                 Sep 25 2018 at 12:28                         
+ Started                 Sep 25 2018 at 12:28                         
+ Finished                Sep 25 2018 at 12:28                         
+ Exit code               123                                          
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_restart_policy[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_environment[iso]_0.ref`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Job                     test-job                         
+ Name                    test-job-name                    
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
- Image                   test-image                       
+ Image                   image:test-image:sometag         
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
- Restart policy          always                           
- Restarts                4                                
  TTY                     False                            
  Http URL                http://local.host.test/          
  Http port               80                               
  Http authentication     True                             
+ Environment              ENV_NAME_1  __value1__          
+                          ENV_NAME_2  **value2**          
  Created                 2018-09-25T12:28:21.298672+00:00 
  Started                 2018-09-25T12:28:59.759433+00:00 
  Finished                2018-09-25T12:28:59.759433+00:00 
  Exit code               123                              
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_secrets_short[human]_0.ref`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-Job                     test-job                                                    
- Name                    test-job-name                                               
- Owner                   test-user                                                   
- Cluster                 default                                                     
- Description             test job description                                        
- Status                  failed (ErrorReason)                                        
- Image                   image:test-image:sometag                                    
- Command                 test-command                                                
- Priority                Normal                                                      
- Price (credits / hour)  15.0000                                                     
- Current cost            150.0000                                                    
- Resources                Memory  16.8 MB                                            
-                          CPU         0.1                                            
- TTY                     False                                                       
- Volumes                  /mnt/rw  storage:rw                                        
- Secret files             /var/run/secret1  secret:secret1                           
-                          /var/run/secret2  secret:/otheruser/secret2                
-                          /var/run/secret3  secret://othercluster/otheruser/secret3  
- Http URL                http://local.host.test/                                     
- Http port               80                                                          
- Http authentication     True                                                        
- Environment              ENV_NAME_0  somevalue                                      
- Secret environment       ENV_NAME_1  secret:secret4                                 
-                          ENV_NAME_2  secret:/otheruser/secret5                      
-                          ENV_NAME_3  secret://othercluster/otheruser/secret6        
- Created                 Sep 25 2018 at 12:28                                        
- Started                 Sep 25 2018 at 12:28                                        
- Finished                Sep 25 2018 at 12:28                                        
- Exit code               123                                                         
+Job                     test-job                                                       
+ Name                    test-job-name                                                  
+ Owner                   test-user                                                      
+ Project                 myproject                                                      
+ Cluster                 default                                                        
+ Description             test job description                                           
+ Status                  failed (ErrorReason)                                           
+ Image                   image:test-image:sometag                                       
+ Command                 test-command                                                   
+ Priority                Normal                                                         
+ Price (credits / hour)  15.0000                                                        
+ Current cost            150.0000                                                       
+ Resources                Memory  16.8 MB                                               
+                          CPU         0.1                                               
+ TTY                     False                                                          
+ Volumes                  /mnt/rw  storage:rw                                           
+ Secret files             /var/run/secret1  secret:secret1                              
+                          /var/run/secret2  secret:/otherproject/secret2                
+                          /var/run/secret3  secret://othercluster/otherproject/secret3  
+ Http URL                http://local.host.test/                                        
+ Http port               80                                                             
+ Http authentication     True                                                           
+ Environment              ENV_NAME_0  somevalue                                         
+ Secret environment       ENV_NAME_1  secret:secret4                                    
+                          ENV_NAME_2  secret:/otherproject/secret5                      
+                          ENV_NAME_3  secret://othercluster/otherproject/secret6        
+ Created                 Sep 25 2018 at 12:28                                           
+ Started                 Sep 25 2018 at 12:28                                           
+ Finished                Sep 25 2018 at 12:28                                           
+ Exit code               123                                                            
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[human]_0.ref`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Job                     test-job                
  Tags                    tag1, tag2, tag3        
  Owner                   test-user               
+ Project                 myproject               
  Cluster                 default                 
  Description             test job description    
  Status                  failed (ErrorReason)    
  Image                   test-image              
  Command                 test-command            
  Priority                Normal                  
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Job                     test-job                         
- Tags                    tag1, tag2, tag3                 
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  failed (ErrorReason)             
  Image                   test-image                       
  Command                 test-command                     
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
@@ -14,9 +14,9 @@
  TTY                     False                            
  Http URL                http://local.host.test/          
  Http port               80                               
  Http authentication     True                             
  Created                 2018-09-25T12:28:21.298672+00:00 
  Started                 2018-09-25T12:28:59.759433+00:00 
  Finished                2018-09-25T12:28:59.759433+00:00 
- Exit code               123                              
+ Exit code               321                              
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-]_0.ref`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Job                     test-job                                       
- Tags                    long-tag-1, long-tag-2, long-tag-3, long-tag-4 
- Owner                   test-user                                      
- Cluster                 default                                        
- Description             test job description                           
- Status                  failed (ErrorReason)                           
- Image                   test-image                                     
- Command                 test-command                                   
- Priority                Normal                                         
- Price (credits / hour)  15.0000                                        
- Current cost            150.0000                                       
- Resources                Memory  16.8 MB                               
-                          CPU         0.1                               
- TTY                     False                                          
- Http URL                http://local.host.test/                        
- Http port               80                                             
- Http authentication     True                                           
- Created                 Sep 25 2018 at 12:28                           
- Started                 Sep 25 2018 at 12:28                           
- Finished                Sep 25 2018 at 12:28                           
- Exit code               123                                            
- Description             ErrorDesc
+Job                     test-job                                    
+ Owner                   test-user                                   
+ Project                                                             
+ Cluster                 default                                     
+ Description             test job description                        
+ Status                  succeeded                                   
+ Image                   test-image                                  
+ Command                 test-command                                
+ Priority                Normal                                      
+ Price (credits / hour)  15.0000                                     
+ Current cost            150.0000                                    
+ Resources                Memory                           16 Bytes  
+                          CPU                                   0.1  
+                          GPU                 4.0 x nvidia-tesla-p4  
+                          TPU                             v2-8/1.14  
+                          Extended SHM space                   True  
+ TTY                     False                                       
+ Http URL                http://local.host.test/                     
+ Created                 2018-09-25T12:28:21.298672+00:00            
+ Started                 2018-09-25T12:28:59.759433+00:00            
+ Finished                2018-09-25T12:28:59.759433+00:00            
+ Exit code               None
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_tags_wrap_tags[human]_0.ref`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Job                     test-job                                       
  Tags                    long-tag-1, long-tag-2, long-tag-3, long-tag-4 
  Owner                   test-user                                      
+ Project                 myproject                                      
  Cluster                 default                                        
  Description             test job description                           
  Status                  failed (ErrorReason)                           
  Image                   test-image                                     
  Command                 test-command                                   
  Priority                Normal                                         
  Price (credits / hour)  15.0000                                        
  Current cost            150.0000                                       
  Resources                Memory  16.8 MB                               
                           CPU         0.1                               
  TTY                     False                                          
  Http URL                http://local.host.test/                        
  Http port               80                                             
  Http authentication     True                                           
- Created                 2018-09-25T12:28:21.298672+00:00               
- Started                 2018-09-25T12:28:59.759433+00:00               
- Finished                2018-09-25T12:28:59.759433+00:00               
+ Created                 Sep 25 2018 at 12:28                           
+ Started                 Sep 25 2018 at 12:28                           
+ Finished                Sep 25 2018 at 12:28                           
  Exit code               123                                            
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[human]_0.ref`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Job                     test-job                                                 
- Name                    test-job-name                                            
- Owner                   test-user                                                
- Cluster                 default                                                  
- Description             test job description                                     
- Status                  failed (ErrorReason)                                     
- Image                   image://test-cluster/test-user/test-image:sometag        
- Command                 test-command                                             
- Priority                Normal                                                   
- Price (credits / hour)  15.0000                                                  
- Current cost            150.0000                                                 
- Resources                Memory  16.8 MB                                         
-                          CPU         0.1                                         
- TTY                     False                                                    
- Volumes                  /mnt/ro  storage://test-cluster/otheruser/ro  READONLY  
-                          /mnt/rw  storage://test-cluster/test-user/rw            
- Http URL                http://local.host.test/                                  
- Http port               80                                                       
- Http authentication     True                                                     
- Created                 Sep 25 2018 at 12:28                                     
- Started                 Sep 25 2018 at 12:28                                     
- Finished                Sep 25 2018 at 12:28                                     
- Exit code               123                                                      
+Job                     test-job                                                    
+ Name                    test-job-name                                               
+ Owner                   test-user                                                   
+ Project                 myproject                                                   
+ Cluster                 default                                                     
+ Description             test job description                                        
+ Status                  failed (ErrorReason)                                        
+ Image                   image://test-cluster/test-project/test-image:sometag        
+ Command                 test-command                                                
+ Priority                Normal                                                      
+ Price (credits / hour)  15.0000                                                     
+ Current cost            150.0000                                                    
+ Resources                Memory  16.8 MB                                            
+                          CPU         0.1                                            
+ TTY                     False                                                       
+ Volumes                  /mnt/ro  storage://test-cluster/otherproject/ro  READONLY  
+                          /mnt/rw  storage://test-cluster/test-project/rw            
+ Http URL                http://local.host.test/                                     
+ Http port               80                                                          
+ Http authentication     True                                                        
+ Created                 Sep 25 2018 at 12:28                                        
+ Started                 Sep 25 2018 at 12:28                                        
+ Finished                Sep 25 2018 at 12:28                                        
+ Exit code               123                                                         
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_long[iso]_0.ref`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Job                     test-job                                                 
- Name                    test-job-name                                            
- Owner                   test-user                                                
- Cluster                 default                                                  
- Description             test job description                                     
- Status                  failed (ErrorReason)                                     
- Image                   image://test-cluster/test-user/test-image:sometag        
- Command                 test-command                                             
- Priority                Normal                                                   
- Price (credits / hour)  15.0000                                                  
- Current cost            150.0000                                                 
- Resources                Memory  16.8 MB                                         
-                          CPU         0.1                                         
- TTY                     False                                                    
- Volumes                  /mnt/ro  storage://test-cluster/otheruser/ro  READONLY  
-                          /mnt/rw  storage://test-cluster/test-user/rw            
- Http URL                http://local.host.test/                                  
- Http port               80                                                       
- Http authentication     True                                                     
- Created                 2018-09-25T12:28:21.298672+00:00                         
- Started                 2018-09-25T12:28:59.759433+00:00                         
- Finished                2018-09-25T12:28:59.759433+00:00                         
- Exit code               123                                                      
+Job                     test-job                                                    
+ Name                    test-job-name                                               
+ Owner                   test-user                                                   
+ Project                 myproject                                                   
+ Cluster                 default                                                     
+ Description             test job description                                        
+ Status                  failed (ErrorReason)                                        
+ Image                   image://test-cluster/test-project/test-image:sometag        
+ Command                 test-command                                                
+ Priority                Normal                                                      
+ Price (credits / hour)  15.0000                                                     
+ Current cost            150.0000                                                    
+ Resources                Memory  16.8 MB                                            
+                          CPU         0.1                                            
+ TTY                     False                                                       
+ Volumes                  /mnt/ro  storage://test-cluster/otherproject/ro  READONLY  
+                          /mnt/rw  storage://test-cluster/test-project/rw            
+ Http URL                http://local.host.test/                                     
+ Http port               80                                                          
+ Http authentication     True                                                        
+ Created                 2018-09-25T12:28:21.298672+00:00                            
+ Started                 2018-09-25T12:28:59.759433+00:00                            
+ Finished                2018-09-25T12:28:59.759433+00:00                            
+ Exit code               123                                                         
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_volumes_short[human]_0.ref`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Job                     test-job                                                   
- Name                    test-job-name                                              
- Owner                   test-user                                                  
- Cluster                 default                                                    
- Description             test job description                                       
- Status                  failed (ErrorReason)                                       
- Image                   image:test-image:sometag                                   
- Command                 test-command                                               
- Priority                Normal                                                     
- Price (credits / hour)  15.0000                                                    
- Current cost            150.0000                                                   
- Resources                Memory  16.8 MB                                           
-                          CPU         0.1                                           
- TTY                     False                                                      
- Volumes                  /mnt/_ro_  storage:/otheruser/_ro_              READONLY  
-                          /mnt/rw    storage:rw                                     
-                          /mnt/ro    storage://othercluster/otheruser/ro  READONLY  
- Http URL                http://local.host.test/                                    
- Http port               80                                                         
- Http authentication     True                                                       
- Created                 Sep 25 2018 at 12:28                                       
- Started                 Sep 25 2018 at 12:28                                       
- Finished                Sep 25 2018 at 12:28                                       
- Exit code               123                                                        
+Job                     test-job                                                      
+ Name                    test-job-name                                                 
+ Owner                   test-user                                                     
+ Project                 myproject                                                     
+ Cluster                 default                                                       
+ Description             test job description                                          
+ Status                  failed (ErrorReason)                                          
+ Image                   image:test-image:sometag                                      
+ Command                 test-command                                                  
+ Priority                Normal                                                        
+ Price (credits / hour)  15.0000                                                       
+ Current cost            150.0000                                                      
+ Resources                Memory  16.8 MB                                              
+                          CPU         0.1                                              
+ TTY                     False                                                         
+ Volumes                  /mnt/_ro_  storage:/otherproject/_ro_              READONLY  
+                          /mnt/rw    storage:rw                                        
+                          /mnt/ro    storage://othercluster/otherproject/ro  READONLY  
+ Http URL                http://local.host.test/                                       
+ Http port               80                                                            
+ Http authentication     True                                                          
+ Created                 Sep 25 2018 at 12:28                                          
+ Started                 Sep 25 2018 at 12:28                                          
+ Finished                Sep 25 2018 at 12:28                                          
+ Exit code               123                                                           
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-Job                     test-job                 
- Name                    test-job-name            
- Owner                   test-user                
- Cluster                 default                  
- Description             test job description     
- Status                  failed (ErrorReason)     
- Image                   image:test-image:sometag 
- Command                 test-command             
- Working dir             /working/dir             
- Priority                Normal                   
- Price (credits / hour)  15.0000                  
- Current cost            150.0000                 
- Resources                Memory  16.8 MB         
-                          CPU         0.1         
- TTY                     False                    
- Http URL                http://local.host.test/  
- Http port               80                       
- Http authentication     True                     
- Created                 Sep 25 2018 at 12:28     
- Started                 Sep 25 2018 at 12:28     
- Finished                Sep 25 2018 at 12:28     
- Exit code               123                      
- Description             ErrorDesc
+Job                     test-job                   
+ Owner                   test-user                  
+ Project                 myproject                  
+ Cluster                 default                    
+ Description             test job description       
+ Status                  running (ContainerRunning) 
+ Image                   test-image                 
+ Command                 test-command               
+ Priority                Normal                     
+ Price (credits / hour)  15.0000                    
+ Current cost            150.0000                   
+ Resources                Memory  16.8 MB           
+                          CPU         0.1           
+ TTY                     False                      
+ Internal Hostname       host.local                 
+ Http URL                http://local.host.test/    
+ Created                 Sep 25 2018 at 12:28       
+ Started                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_working_dir[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[iso-someotherproject]_0.ref`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-Job                     test-job                         
- Name                    test-job-name                    
- Owner                   test-user                        
- Cluster                 default                          
- Description             test job description             
- Status                  failed (ErrorReason)             
- Image                   image:test-image:sometag         
- Command                 test-command                     
- Working dir             /working/dir                     
- Priority                Normal                           
- Price (credits / hour)  15.0000                          
- Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
- TTY                     False                            
- Http URL                http://local.host.test/          
- Http port               80                               
- Http authentication     True                             
- Created                 2018-09-25T12:28:21.298672+00:00 
- Started                 2018-09-25T12:28:59.759433+00:00 
- Finished                2018-09-25T12:28:59.759433+00:00 
- Exit code               123                              
- Description             ErrorDesc
+Job                     test-job                                    
+ Owner                   test-user                                   
+ Project                 someotherproject                            
+ Cluster                 default                                     
+ Description             test job description                        
+ Status                  succeeded                                   
+ Image                   test-image                                  
+ Command                 test-command                                
+ Priority                Normal                                      
+ Price (credits / hour)  15.0000                                     
+ Current cost            150.0000                                    
+ Resources                Memory                           16 Bytes  
+                          CPU                                   0.1  
+                          GPU                 4.0 x nvidia-tesla-p4  
+                          TPU                             v2-8/1.14  
+                          Extended SHM space                   True  
+ TTY                     False                                       
+ Http URL                http://local.host.test/                     
+ Created                 2018-09-25T12:28:21.298672+00:00            
+ Started                 2018-09-25T12:28:59.759433+00:00            
+ Finished                2018-09-25T12:28:59.759433+00:00            
+ Exit code               None
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_life_span_with_value[human]_0.ref`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Job                     test-job                
  Owner                   test-user               
+ Project                 myproject               
  Cluster                 default                 
  Description             test job description    
  Status                  failed (ErrorReason)    
  Image                   test-image              
  Command                 test-command            
  Priority                Normal                  
  Price (credits / hour)  15.0000                 
  Current cost            150.0000                
  Resources                Memory  16.8 MB        
                           CPU         0.1        
+ Life span               1d2h3m4s                
  TTY                     False                   
  Http URL                http://local.host.test/ 
  Http port               80                      
  Http authentication     True                    
  Created                 Sep 25 2018 at 12:28    
  Started                 Sep 25 2018 at 12:28    
  Finished                Sep 25 2018 at 12:28    
- Exit code               321                     
+ Exit code               123                     
  Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Job                     test-job                         
- Owner                   test-user                        
- Cluster                 default                          
- Description             test job description             
- Status                  failed (ErrorReason)             
- Image                   test-image                       
- Command                 test-command                     
- Priority                Normal                           
- Price (credits / hour)  15.0000                          
- Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
- TTY                     False                            
- Http URL                http://local.host.test/          
- Http port               80                               
- Http authentication     True                             
- Created                 2018-09-25T12:28:21.298672+00:00 
- Started                 2018-09-25T12:28:59.759433+00:00 
- Finished                2018-09-25T12:28:59.759433+00:00 
- Exit code               321                              
- Description             ErrorDesc
+Job                      test-job                         
+ Name                     test-job                         
+ Owner                    test-user                        
+ Project                  myproject                        
+ Cluster                  default                          
+ Description              test job description             
+ Status                   running (ContainerRunning)       
+ Image                    test-image                       
+ Command                  test-command                     
+ Priority                 Normal                           
+ Price (credits / hour)   15.0000                          
+ Current cost             150.0000                         
+ Resources                 Memory  16.8 MB                 
+                           CPU         0.1                 
+ TTY                      False                            
+ Internal Hostname        host.local                       
+ Internal Hostname Named  test-job--test-owner.local       
+ Http URL                 http://local.host.test/          
+ Created                  2018-09-25T12:28:21.298672+00:00 
+ Started                  2018-09-25T12:28:24.759433+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Job                     test-job                    
- Owner                   owner                       
- Cluster                 default                     
- Status                  pending (ContainerCreating) 
- Image                   test-image                  
- Command                 test-command                
- Priority                Normal                      
- Price (credits / hour)  15.0000                     
- Current cost            150.0000                    
- Resources                Memory  16.8 MB            
-                          CPU         0.1            
- Round Robin             True                        
- TTY                     False                       
- Created                 Sep 25 2018 at 12:28
+Job                     test-job                         
+ Owner                   owner                            
+ Project                 myproject                        
+ Cluster                 default                          
+ Status                  pending (ContainerCreating)      
+ Image                   test-image                       
+ Command                 test-command                     
+ Priority                Normal                           
+ Price (credits / hour)  15.0000                          
+ Current cost            150.0000                         
+ Resources                Memory  16.8 MB                 
+                          CPU         0.1                 
+ Round Robin             True                             
+ TTY                     False                            
+ Created                 2018-09-25T12:28:21.298672+00:00
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_description[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[iso]_0.ref`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Job                     test-job                         
  Owner                   owner                            
+ Project                 myproject                        
  Cluster                 default                          
- Status                  pending (ContainerCreating)      
+ Description             test job description             
+ Status                  pending                          
  Image                   test-image                       
  Command                 test-command                     
+ Preset                  cpu-small                        
+ Energy schedule         some-schedule                    
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  Round Robin             True                             
  TTY                     False
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_energy_schedule[human]_0.ref`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Job                     test-job              
  Owner                   owner                 
+ Project                 myproject             
  Cluster                 default               
  Description             test job description  
  Status                  pending               
  Image                   test-image            
  Command                 test-command          
+ Preset                  cpu-small             
+ Energy schedule         some-schedule         
  Priority                Normal                
  Price (credits / hour)  15.0000               
  Current cost            150.0000              
  Resources                Memory  16.8 MB      
                           CPU         0.1      
  Round Robin             True                  
  TTY                     False
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_no_reason[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job[human]_0.ref`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-Job                     test-job                         
- Owner                   owner                            
- Cluster                 default                          
- Description             test job description             
- Status                  pending                          
- Image                   test-image                       
- Command                 test-command                     
- Priority                Normal                           
- Price (credits / hour)  15.0000                          
- Current cost            150.0000                         
- Resources                Memory  16.8 MB                 
-                          CPU         0.1                 
- Round Robin             True                             
- TTY                     False                            
- Created                 2018-09-25T12:28:21.298672+00:00
+Job                     test-job                
+ Owner                   test-user               
+ Project                 myproject               
+ Cluster                 default                 
+ Description             test job description    
+ Status                  failed (ErrorReason)    
+ Image                   test-image              
+ Command                 test-command            
+ Priority                Normal                  
+ Price (credits / hour)  15.0000                 
+ Current cost            150.0000                
+ Resources                Memory  16.8 MB        
+                          CPU         0.1        
+ TTY                     False                   
+ Http URL                http://local.host.test/ 
+ Http port               80                      
+ Http authentication     True                    
+ Created                 Sep 25 2018 at 12:28    
+ Started                 Sep 25 2018 at 12:28    
+ Finished                Sep 25 2018 at 12:28    
+ Exit code               321                     
+ Description             ErrorDesc
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_pending_job_with_reason[human]_0.ref`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                    
  Owner                   owner                       
+ Project                 myproject                   
  Cluster                 default                     
  Description             test job description        
  Status                  pending (ContainerCreating) 
  Image                   test-image                  
  Command                 test-command                
  Priority                Normal                      
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_org_name[human]_0.ref`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Job                     test-job                   
+ Name                    test-job                   
  Owner                   test-user                  
+ Project                 myproject                  
  Cluster                 default                    
- Description             test job description       
+ Organization            test-job-org-name          
  Status                  running (ContainerRunning) 
  Image                   test-image                 
  Command                 test-command               
  Priority                Normal                     
  Price (credits / hour)  15.0000                    
  Current cost            150.0000                   
  Resources                Memory  16.8 MB           
                           CPU         0.1           
  TTY                     False                      
- Internal Hostname       host.local                 
  Http URL                http://local.host.test/    
  Created                 Sep 25 2018 at 12:28       
  Started                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[iso]_0.ref`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Job                     test-job                         
  Owner                   test-user                        
+ Project                 myproject                        
  Cluster                 default                          
  Description             test job description             
  Status                  running (ContainerRunning)       
  Image                   test-image                       
- Command                 test-command                     
+ Entrypoint              /usr/bin/make                    
+ Command                 test                             
  Priority                Normal                           
  Price (credits / hour)  15.0000                          
  Current cost            150.0000                         
  Resources                Memory  16.8 MB                 
                           CPU         0.1                 
  TTY                     False                            
  Internal Hostname       host.local
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[human]_0.ref`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                                             
  Owner                   test-user                                            
+ Project                 myproject                                            
  Cluster                 default                                              
  Description             test job description                                 
  Status                  running (ContainerRunning)                           
  Image                   test-image                                           
  Command                 test-command                                         
  Priority                Normal                                               
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_job_with_status_items[iso]_0.ref`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Job                     test-job                                                        
  Owner                   test-user                                                       
+ Project                 myproject                                                       
  Cluster                 default                                                         
  Description             test job description                                            
  Status                  running (ContainerRunning)                                      
  Image                   test-image                                                      
  Command                 test-command                                                    
  Priority                Normal                                                          
  Price (credits / hour)  15.0000
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_entrypoint[human]_0.ref`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Job                      test-job                   
- Name                     test-job                   
- Owner                    test-user                  
- Cluster                  default                    
- Description              test job description       
- Status                   running (ContainerRunning) 
- Image                    test-image                 
- Command                  test-command               
- Priority                 Normal                     
- Price (credits / hour)   15.0000                    
- Current cost             150.0000                   
- Resources                 Memory  16.8 MB           
-                           CPU         0.1           
- TTY                      False                      
- Internal Hostname        host.local                 
- Internal Hostname Named  test-job--test-owner.local 
- Http URL                 http://local.host.test/    
- Created                  Sep 25 2018 at 12:28       
- Started                  Sep 25 2018 at 12:28
+Job                     test-job                   
+ Owner                   test-user                  
+ Project                 myproject                  
+ Cluster                 default                    
+ Description             test job description       
+ Status                  running (ContainerRunning) 
+ Image                   test-image                 
+ Entrypoint              /usr/bin/make              
+ Command                 test                       
+ Priority                Normal                     
+ Price (credits / hour)  15.0000                    
+ Current cost            150.0000                   
+ Resources                Memory  16.8 MB           
+                          CPU         0.1           
+ TTY                     False                      
+ Internal Hostname       host.local                 
+ Http URL                http://local.host.test/    
+ Created                 Sep 25 2018 at 12:28       
+ Started                 Sep 25 2018 at 12:28
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_running_named_job[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobOutputFormatter.test_job_with_project_name[human-someotherproject]_0.ref`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-Job                      test-job                         
- Name                     test-job                         
- Owner                    test-user                        
- Cluster                  default                          
- Description              test job description             
- Status                   running (ContainerRunning)       
- Image                    test-image                       
- Command                  test-command                     
- Priority                 Normal                           
- Price (credits / hour)   15.0000                          
- Current cost             150.0000                         
- Resources                 Memory  16.8 MB                 
-                           CPU         0.1                 
- TTY                      False                            
- Internal Hostname        host.local                       
- Internal Hostname Named  test-job--test-owner.local       
- Http URL                 http://local.host.test/          
- Created                  2018-09-25T12:28:21.298672+00:00 
- Started                  2018-09-25T12:28:24.759433+00:00
+Job                     test-job                                    
+ Owner                   test-user                                   
+ Project                 someotherproject                            
+ Cluster                 default                                     
+ Description             test job description                        
+ Status                  succeeded                                   
+ Image                   test-image                                  
+ Command                 test-command                                
+ Priority                Normal                                      
+ Price (credits / hour)  15.0000                                     
+ Current cost            150.0000                                    
+ Resources                Memory                           16 Bytes  
+                          CPU                                   0.1  
+                          GPU                 4.0 x nvidia-tesla-p4  
+                          TPU                             v2-8/1.14  
+                          Extended SHM space                   True  
+ TTY                     False                                       
+ Http URL                http://local.host.test/                     
+ Created                 Sep 25 2018 at 12:28                        
+ Started                 Sep 25 2018 at 12:28                        
+ Finished                Sep 25 2018 at 12:28                        
+ Exit code               None
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_limited_height[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_2.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_3.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[human]_4.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_2.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_3.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_multiple_jobs[iso]_4.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_no_gpu[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[human]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_seq[iso]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestJobTelemetryFormatter.test_format_telemetry_with_gpu[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[human]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates[iso]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_dates_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-0-owner-#less#you#more#]_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_short_cells[iso-1-alice-alice]_1.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/TestTabularJobsFormatter.test_wide_cells[human-0-owner-#less#you#more#]_0.ref`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-ID/NAME                                    STATUS/WHEN    IMAGE                                      ORG/OWNER   COMMAND            
- ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
-  job-7ee153a7-249c-4be9-965a-ba3eafb67c82   failed         some-image-name:with-long-tag                          ls -la /some/path  
-   name1                                      Sep 25 2017                                               YOU                           
-  job-7ee153a7-249c-4be9-965a-ba3eafb67c84   pending        image://test-cluster/bob/some-image-nam…               ls -la /some/path  
-   name2                                      Sep 25 2017                                               YOU
+ID/NAME                                    STATUS/WHEN    IMAGE                                      ORG/PROJECT   COMMAND            
+ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
+  job-7ee153a7-249c-4be9-965a-ba3eafb67c82   failed         some-image-name:with-long-tag                            ls -la /some/path  
+   name1                                      Sep 25 2017                                               myproject                       
+  job-7ee153a7-249c-4be9-965a-ba3eafb67c84   pending        image://test-cluster/test-project/some-…                 ls -la /some/path  
+   name2                                      Sep 25 2017                                               myproject
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_bucket_credentials_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_credentials_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_buckets_formatter_long_0.ref`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-Id                                            Name            Provider   Uri                                       Org name   Created at    Public  
- ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
-  bucket-1                                      test-bucket     aws        blob://cluster/user/test-bucket           NO_ORG     Mar 04 2017   ×       
-  bucket-2                                      test-bucket-2   aws        blob://cluster/user/test-bucket-2         NO_ORG     Mar 04 2016   ×       
-  bucket-3                                                      aws        blob://cluster/test-org/user-2/bucket-3   test-org   Mar 04 2018   ×       
-  bucket-4                                                      aws        blob://cluster/test-org/user/bucket-4     test-org   Mar 04 2019   √
+Id                                            Name            Provider   Uri                                  Org name   Project name   Created at    Public  
+ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
+  bucket-1                                      test-bucket     aws        blob://cluster/test-project/test-…   NO_ORG     test-project   Mar 04 2017   ×       
+  bucket-2                                      test-bucket-2   aws        blob://cluster/test-project/test-…   NO_ORG     test-project   Mar 04 2016   ×       
+  bucket-3                                                      aws        blob://cluster/test-org/test-proj…   test-org   test-project   Mar 04 2018   ×       
+  bucket-4                                                      aws        blob://cluster/test-org/test-proj…   test-org   test-project   Mar 04 2019   √
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_0.ref`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_long_0.ref`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,7 @@
-Id                                          Name   Storage    Used   Uri                     Status    Org name   Created at    Last used     Timeout unused  
+Project                                   Timeout     
+  Id                                          Name   Storage    Used   Uri           Status    Org name   name          Created at    Last used     unused      
  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
-  disk-1                                             53.7 GB           disk://cluster/user/…   Pending   NO_ORG     Mar 04 2017   Mar 08 2017   no limit        
-  disk-2                                             52.4 MB           disk://cluster/user/…   Ready     NO_ORG     Apr 04 2017                 2d3h4m5s        
-  disk-3                                             51.2 kB           disk://cluster/test-…   Ready     test-org   May 04 2017                 no limit        
-  disk-4                                             50 Bytes          disk://cluster/user/…   Broken    NO_ORG     Jun 04 2017                 no limit
+  disk-1                                             53.7 GB           disk://clu…   Pending   NO_ORG     test-proje…   Mar 04 2017   Mar 08 2017   no limit    
+  disk-2                                             52.4 MB           disk://clu…   Ready     NO_ORG     another-pr…   Apr 04 2017                 2d3h4m5s    
+  disk-3                                             51.2 kB           disk://clu…   Ready     test-org   another-pr…   May 04 2017                 no limit    
+  disk-4                                             50 Bytes          disk://clu…   Broken    NO_ORG     test-proje…   Jun 04 2017                 no limit
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref` & `neuro-cli-23.7.0/tests/unit/formatters/ascii/test_disks_formatter_short_0.ref`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-Id                                          Name   Storage    Used   Uri                                   Status   
- ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
-  disk-1                                             53.7 GB           disk://cluster/user/disk-1            Pending  
-  disk-2                                             52.4 MB           disk://cluster/user/disk-2            Ready    
-  disk-3                                             51.2 kB           disk://cluster/test-org/user/disk-3   Ready    
-  disk-4                                             50 Bytes          disk://cluster/user/disk-4            Broken
+Id                                          Name   Storage    Used   Uri                                              Status   
+ ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 
+  disk-1                                             53.7 GB           disk://cluster/test-project/disk-1               Pending  
+  disk-2                                             52.4 MB           disk://cluster/another-project/disk-2            Ready    
+  disk-3                                             51.2 kB           disk://cluster/test-org/another-project/disk-3   Ready    
+  disk-4                                             50 Bytes          disk://cluster/test-project/disk-4               Broken
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_admin_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_admin_formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     _AzureStorageOptions,
     _AzureStorageTier,
     _Balance,
     _CloudProviderOptions,
     _CloudProviderType,
     _Cluster,
     _ClusterStatus,
+    _ClusterUser,
     _ClusterUserRoleType,
     _ClusterUserWithInfo,
     _ConfigCluster,
     _EFSPerformanceMode,
     _EFSThroughputMode,
     _GoogleCloudProvider,
     _GoogleFilestoreTier,
@@ -33,23 +34,24 @@
     _UserInfo,
 )
 
 from neuro_cli.formatters.admin import (
     CloudProviderOptionsFormatter,
     ClustersFormatter,
     ClusterUserFormatter,
+    ClusterUserWithInfoFormatter,
     OrgClusterFormatter,
 )
 
 RichCmp = Callable[[RenderableType], None]
 
 
 class TestClusterUserFormatter:
-    def test_cluster_list(self, rich_cmp: RichCmp) -> None:
-        formatter = ClusterUserFormatter()
+    def test_list_users_with_user_info(self, rich_cmp: RichCmp) -> None:
+        formatter = ClusterUserWithInfoFormatter()
         users = [
             _ClusterUserWithInfo(
                 user_name="denis",
                 cluster_name="default",
                 org_name=None,
                 role=_ClusterUserRoleType("admin"),
                 quota=_Quota(),
@@ -116,14 +118,24 @@
                     email="alex@domain.name",
                     created_at=None,
                 ),
             ),
         ]
         rich_cmp(formatter(users))
 
+    def test_list_users_no_user_info(self, rich_cmp: RichCmp) -> None:
+        formatter = ClusterUserFormatter()
+        users = [
+            _ClusterUser("default", "denis", None, _Quota(), _Balance(), None),
+            _ClusterUser("default", "denis", None, _Quota(), _Balance(), "Org"),
+            _ClusterUser("default", "andrew", None, _Quota(), _Balance(), None),
+            _ClusterUser("default", "andrew", None, _Quota(), _Balance(), "Org"),
+        ]
+        rich_cmp(formatter(users))
+
 
 class TestClustersFormatter:
     def _create_node_pool(
         self,
         name: str,
         disk_type: str = "",
         is_scalable: bool = True,
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_blob_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_buckets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,113 @@
-from datetime import datetime
-from typing import Any, List, Union
+from typing import Any, List
 
 import pytest
+from dateutil.parser import isoparse
 
-from neuro_sdk import BlobCommonPrefix, BlobObject, Bucket, BucketEntry
+from neuro_sdk import Bucket
 
-from neuro_cli.formatters.blob_storage import (
-    BaseBlobFormatter,
-    LongBlobFormatter,
-    SimpleBlobFormatter,
+from neuro_cli.formatters.buckets import (
+    BucketFormatter,
+    BucketsFormatter,
+    SimpleBucketsFormatter,
 )
+from neuro_cli.formatters.utils import format_datetime_human
 
 
-class TestBlobFormatter:
+def test_bucket_formatter(rich_cmp: Any) -> None:
+    bucket = Bucket(
+        id="bucket",
+        name="test-bucket",
+        owner="user",
+        cluster_name="cluster",
+        provider=Bucket.Provider.AWS,
+        created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
+        imported=False,
+        org_name=None,
+        project_name="test-project",
+    )
+    fmtr = BucketFormatter(str, datetime_formatter=format_datetime_human)
+    rich_cmp(fmtr(bucket))
+
+
+def test_bucket_formatter_with_org(rich_cmp: Any) -> None:
+    bucket = Bucket(
+        id="bucket",
+        name="test-bucket",
+        owner="user",
+        cluster_name="cluster",
+        provider=Bucket.Provider.AWS,
+        created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
+        imported=False,
+        org_name="test-org",
+        project_name="test-project",
+    )
+    fmtr = BucketFormatter(str, datetime_formatter=format_datetime_human)
+    rich_cmp(fmtr(bucket))
+
 
-    buckets: List[Bucket] = [
+@pytest.fixture
+def buckets_list() -> List[Bucket]:
+    return [
         Bucket(
             id="bucket-1",
-            name="neuro-my-bucket",
-            created_at=datetime(2018, 1, 1, 3),
-            cluster_name="test-cluster",
-            owner="test-user",
+            name="test-bucket",
+            owner="user",
+            cluster_name="cluster",
+            created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-2",
-            name="neuro-public-bucket",
-            created_at=datetime(2018, 1, 1, 17, 2, 4),
-            cluster_name="test-cluster",
-            owner="public",
+            name="test-bucket-2",
+            owner="user",
+            cluster_name="cluster",
+            created_at=isoparse("2016-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-3",
-            name="neuro-shared-bucket",
-            created_at=datetime(2018, 1, 1, 13, 1, 5),
-            cluster_name="test-cluster",
-            owner="another-user",
+            name=None,
+            owner="user-2",
+            cluster_name="cluster",
+            created_at=isoparse("2018-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name="test-org",
+            project_name="test-project",
         ),
-    ]
-
-    blobs: List[BucketEntry] = [
-        BlobObject(
-            key="file1024.txt",
-            modified_at=datetime(2018, 1, 1, 14, 0, 0),
-            bucket=buckets[0],
-            size=1024,
-        ),
-        BlobObject(
-            key="file_bigger.txt",
-            modified_at=datetime(2018, 1, 1, 14, 0, 0),
-            bucket=buckets[1],
-            size=1_024_001,
-        ),
-        BlobObject(
-            key="folder2/info.txt",
-            modified_at=datetime(2018, 1, 1, 14, 0, 0),
-            bucket=buckets[2],
-            size=240,
-        ),
-        BlobObject(
-            key="folder2/",
-            modified_at=datetime(2018, 1, 1, 14, 0, 0),
-            bucket=buckets[2],
-            size=0,
+        Bucket(
+            id="bucket-4",
+            name=None,
+            owner="user",
+            cluster_name="cluster",
+            created_at=isoparse("2019-03-04T12:28:59.759433+00:00"),
+            provider=Bucket.Provider.AWS,
+            imported=False,
+            public=True,
+            org_name="test-org",
+            project_name="test-project",
         ),
     ]
-    folders: List[BucketEntry] = [
-        BlobCommonPrefix(bucket=buckets[0], key="folder1/", size=0),
-        BlobCommonPrefix(bucket=buckets[1], key="folder2/", size=0),
-    ]
 
-    all: List[Union[Bucket, BucketEntry]] = [*buckets, *blobs, *folders]
 
-    @pytest.mark.parametrize(
-        "formatter",
-        [
-            (SimpleBlobFormatter(color=False, uri_formatter=str)),
-            (LongBlobFormatter(human_readable=False, color=False, uri_formatter=str)),
-        ],
+def test_buckets_formatter_simple(buckets_list: List[Bucket], rich_cmp: Any) -> None:
+    fmtr = SimpleBucketsFormatter()
+    rich_cmp(fmtr(buckets_list))
+
+
+def test_buckets_formatter_short(buckets_list: List[Bucket], rich_cmp: Any) -> None:
+    fmtr = BucketsFormatter(str, datetime_formatter=format_datetime_human)
+    rich_cmp(fmtr(buckets_list))
+
+
+def test_buckets_formatter_long(buckets_list: List[Bucket], rich_cmp: Any) -> None:
+    fmtr = BucketsFormatter(
+        str, long_format=True, datetime_formatter=format_datetime_human
     )
-    def test_long_formatter(self, rich_cmp: Any, formatter: BaseBlobFormatter) -> None:
-        for index, item in enumerate(self.all):
-            rich_cmp(formatter(item), index=index)
+    rich_cmp(fmtr(buckets_list))
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_bucket_credentials.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_bucket_credentials.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         name="test-bucket",
         owner="user",
         cluster_name="cluster",
         provider=Bucket.Provider.AWS,
         created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         imported=False,
         org_name=None,
+        project_name="test-project",
     )
     credentials = PersistentBucketCredentials(
         id="bucket-credentials",
         name="test-credentials",
         owner="user",
         cluster_name="cluster",
         read_only=False,
@@ -62,44 +63,48 @@
             name="test-bucket",
             owner="user",
             cluster_name="cluster",
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-2",
             name="test-bucket-2",
             owner="user",
             cluster_name="cluster",
             created_at=isoparse("2016-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-3",
             name=None,
             owner="user-2",
             cluster_name="cluster",
             created_at=isoparse("2018-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
         Bucket(
             id="bucket-4",
             name=None,
             owner="user",
             cluster_name="cluster",
             created_at=isoparse("2019-03-04T12:28:59.759433+00:00"),
             provider=Bucket.Provider.AWS,
             imported=False,
             org_name=None,
+            project_name="test-project",
         ),
     ]
 
     async def _get_bucket(bucket_id: str) -> Bucket:
         return next(bucket for bucket in buckets if bucket.id == bucket_id)
 
     credentials = [
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_config_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_config_formatters.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 )
 
 from neuro_cli.alias import list_aliases
 from neuro_cli.formatters.config import (
     AdminQuotaFormatter,
     AliasesFormatter,
     BalanceFormatter,
+    ClusterOrgProjectsFormatter,
     ConfigFormatter,
     format_quota_details,
 )
 from neuro_cli.root import Root
 
 RichCmp = Callable[[RenderableType], None]
 
@@ -122,14 +123,34 @@
             root.client.config,
             available_jobs_counts,
             Quota(credits=Decimal("500"), total_running_jobs=10),
             Quota(credits=Decimal("1000"), total_running_jobs=50),
         )
         rich_cmp(out)
 
+    async def test_output_without_project(
+        self,
+        make_client: Callable[..., Client],
+        cluster_config: Cluster,
+        rich_cmp: RichCmp,
+    ) -> None:
+        client = make_client(
+            "https://dev.neu.ro/api/v1",
+            clusters={cluster_config.name: cluster_config},
+            projects={},
+            project_name=None,
+        )
+        out = ConfigFormatter()(
+            client.config,
+            {},
+            Quota(credits=Decimal("500"), total_running_jobs=10),
+            None,
+        )
+        rich_cmp(out)
+
     @pytest.fixture
     def _config_cluster_with_energy(self) -> _ConfigCluster:
         return _ConfigCluster(
             name="default",
             status=_ClusterStatus.DEPLOYED,
             created_at=datetime.now(),
             energy=_EnergyConfig(
@@ -259,7 +280,19 @@
                     }
                 }
             )
         )
         lst = await list_aliases(root)
         out = AliasesFormatter()(lst)
         rich_cmp(out)
+
+
+class TestClusterOrgProjectsFormatter:
+    async def test_output(self, rich_cmp: RichCmp) -> None:
+        projects = ["project1", "project2"]
+        out = ClusterOrgProjectsFormatter()(projects, None)
+        rich_cmp(out)
+
+    async def test_output_with_current_project(self, rich_cmp: RichCmp) -> None:
+        projects = ["project1", "project2"]
+        out = ClusterOrgProjectsFormatter()(projects, "project1")
+        rich_cmp(out)
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_disks.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_disks.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def test_disk_formatter(rich_cmp: Any) -> None:
     disk = Disk(
         id="disk",
         name="test-disk",
         storage=int(11.93 * (1024**3)),
         owner="user",
+        project_name="test-project",
         status=Disk.Status.READY,
         cluster_name="cluster",
         org_name=None,
         created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         last_usage=isoparse("2017-04-04T12:28:59.759433+00:00"),
         timeout_unused=timedelta(days=1, hours=2, minutes=3, seconds=4),
     )
@@ -34,43 +35,47 @@
 @pytest.fixture
 def disks_list() -> List[Disk]:
     return [
         Disk(
             id="disk-1",
             storage=50 * (1024**3),
             owner="user",
+            project_name="test-project",
             status=Disk.Status.PENDING,
             cluster_name="cluster",
             org_name=None,
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
             last_usage=isoparse("2017-03-08T12:28:59.759433+00:00"),
         ),
         Disk(
             id="disk-2",
             storage=50 * (1024**2),
             owner="user",
+            project_name="another-project",
             status=Disk.Status.READY,
             cluster_name="cluster",
             org_name=None,
             created_at=isoparse("2017-04-04T12:28:59.759433+00:00"),
             timeout_unused=timedelta(days=2, hours=3, minutes=4, seconds=5),
         ),
         Disk(
             id="disk-3",
             storage=50 * (1024**1),
             owner="user",
+            project_name="another-project",
             status=Disk.Status.READY,
             cluster_name="cluster",
             org_name="test-org",
             created_at=isoparse("2017-05-04T12:28:59.759433+00:00"),
         ),
         Disk(
             id="disk-4",
             storage=50,
             owner="user",
+            project_name="test-project",
             status=Disk.Status.BROKEN,
             cluster_name="cluster",
             org_name=None,
             created_at=isoparse("2017-06-04T12:28:59.759433+00:00"),
         ),
     ]
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_images_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_images_formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
         console = new_console(tty=False)
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.pull(
                 ImageProgressPull(
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                     LocalImage("input", "latest"),
                 )
             )
             rich_cmp(console, index=0)
             formatter.step(ImageProgressStep("message1", "layer1", "status1", 1, 100))
             rich_cmp(console, index=1)
@@ -97,18 +97,18 @@
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.push(
                 ImageProgressPush(
                     LocalImage("input", "latest"),
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                 )
             )
             rich_cmp(console, index=0)
             formatter.step(ImageProgressStep("message1", "layer1", "status1", 1, 100))
             rich_cmp(console, index=1)
             formatter.step(ImageProgressStep("message2", "layer1", "status2", 30, 100))
@@ -119,18 +119,18 @@
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.save(
                 ImageProgressSave(
                     "job-id",
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                 )
             )
             rich_cmp(console)
 
     def test_no_tty_commit_started(
         self, rich_cmp: Any, new_console: NewConsole
@@ -139,18 +139,18 @@
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.commit_started(
                 ImageCommitStarted(
                     job_id="job-id",
                     target_image=RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                 )
             )
             rich_cmp(console)
 
     def test_no_tty_commit_finished(
         self, rich_cmp: Any, new_console: NewConsole
@@ -164,18 +164,18 @@
         console = new_console(tty=True)
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.pull(
                 ImageProgressPull(
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                     LocalImage("input", "latest"),
                 )
             )
             rich_cmp(console, index=0)
             formatter.step(ImageProgressStep("message1", "layer1", "status1", 1, 100))
             time.sleep(0.3)
@@ -189,18 +189,18 @@
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.push(
                 ImageProgressPush(
                     LocalImage("input", "latest"),
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                 )
             )
             rich_cmp(console, index=0)
             formatter.step(ImageProgressStep("message1", "layer1", "status1", 1, 100))
             time.sleep(0.3)
             rich_cmp(console, index=1)
@@ -213,18 +213,18 @@
         with DockerImageProgress.create(console, quiet=False) as formatter:
             formatter.save(
                 ImageProgressSave(
                     "job-id",
                     RemoteImage.new_neuro_image(
                         name="output",
                         tag="stream",
-                        owner="bob",
                         registry="https://registry-dev.neu.ro",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                 )
             )
             rich_cmp(console)
 
     def test_tty_commit_started(self, rich_cmp: Any, new_console: NewConsole) -> None:
         console = new_console(tty=True)
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_jobs_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_jobs_formatters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime as dt_module
 import io
 import itertools
 from dataclasses import replace
 from datetime import datetime, timedelta, timezone
 from decimal import Decimal
 from typing import Any, Callable, Optional
 
@@ -94,14 +95,15 @@
 @pytest.fixture
 def job_descr_no_name() -> JobDescription:
     return JobDescription(
         status=JobStatus.PENDING,
         id=TEST_JOB_ID,
         owner="owner",
         cluster_name="default",
+        project_name="myproject",
         uri=URL(f"job://default/owner/{TEST_JOB_ID}"),
         history=JobStatusHistory(
             status=JobStatus.PENDING,
             reason="ErrorReason",
             description="ErrorDesc",
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
             started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
@@ -121,14 +123,15 @@
 @pytest.fixture
 def job_descr() -> JobDescription:
     return JobDescription(
         status=JobStatus.PENDING,
         id=TEST_JOB_ID,
         name=TEST_JOB_NAME,
         owner="owner",
+        project_name="myproject",
         cluster_name="default",
         uri=URL(f"job://default/owner/{TEST_JOB_ID}"),
         history=JobStatusHistory(
             status=JobStatus.PENDING,
             reason="ErrorReason",
             description="ErrorDesc",
             created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
@@ -152,19 +155,22 @@
     *,
     name: Optional[str] = None,
     life_span: Optional[float] = None,
     description: str = "ErrorDesc",
     total_price_credits: Decimal = Decimal("150"),
     price_credits_per_hour: Decimal = Decimal("15"),
     restarts: int = 0,
+    owner: str = "test-user",
+    project_name: str = "myproject",
 ) -> JobDescription:
     return JobDescription(
         name=name,
         status=status,
-        owner="test-user",
+        owner=owner,
+        project_name=project_name,
         cluster_name="default",
         id="test-job",
         uri=URL("job://default/test-user/test-job"),
         description="test job description",
         http_url=URL("http://local.host.test/"),
         history=JobStatusHistory(
             status=status,
@@ -401,14 +407,15 @@
 class TestJobOutputFormatter:
     def test_job_with_name(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -429,29 +436,30 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_org_urls(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
             cluster_name="default",
+            project_name="myproject",
             org_name="test-org",
             id="test-job",
             uri=URL("job://default/test-org/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -478,28 +486,29 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="default", org_name="test-org"
+            project_name="test-project", cluster_name="default", org_name="test-org"
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_tags(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             tags=["tag1", "tag2", "tag3"],
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -520,28 +529,29 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_tags_wrap_tags(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             tags=["long-tag-1", "long-tag-2", "long-tag-3", "long-tag-4"],
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -562,28 +572,29 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_life_span_with_value(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
                 status=JobStatus.PENDING,
@@ -604,28 +615,29 @@
             pass_config=True,
             life_span=1.0 * ((60 * 60 * 24 * 1) + (60 * 60 * 2) + (60 * 3) + 4),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_life_span_without_value(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
                 status=JobStatus.PENDING,
@@ -646,28 +658,29 @@
             pass_config=True,
             life_span=0.0,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_restart_policy(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
                 status=JobStatus.PENDING,
@@ -689,28 +702,29 @@
             pass_config=True,
             restart_policy=JobRestartPolicy.ALWAYS,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_pending_job(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
                 status=JobStatus.PENDING,
@@ -730,15 +744,15 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -760,23 +774,24 @@
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=True,
             pass_config=True,
+            project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -800,22 +815,23 @@
                 command="test-command",
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 tty=True,
             ),
             scheduler_enabled=True,
             pass_config=True,
             owner="owner",
+            project_name="myproject",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -838,34 +854,36 @@
                 image=RemoteImage.new_external_image(name="test-image"),
                 command="test-command",
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=True,
             pass_config=True,
             owner="owner",
+            project_name="myproject",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_running_job(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
+            project_name="myproject",
             owner="test-user",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
@@ -885,28 +903,29 @@
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_running_job_with_status_items(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
                 reason="ContainerRunning",
@@ -946,28 +965,29 @@
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_running_named_job(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             name="test-job",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
@@ -988,28 +1008,29 @@
             internal_hostname="host.local",
             internal_hostname_named="test-job--test-owner.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_entrypoint(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             description="test job description",
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
                 reason="ContainerRunning",
@@ -1029,28 +1050,29 @@
             pass_config=True,
             internal_hostname="host.local",
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_environment(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1064,43 +1086,44 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
                 env={"ENV_NAME_1": "__value1__", "ENV_NAME_2": "**value2**"},
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_volumes_short(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1114,59 +1137,60 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
-                        storage_uri=URL("storage://test-cluster/otheruser/_ro_"),
+                        storage_uri=URL("storage://test-cluster/otherproject/_ro_"),
                         container_path="/mnt/_ro_",
                         read_only=True,
                     ),
                     Volume(
-                        storage_uri=URL("storage://test-cluster/test-user/rw"),
+                        storage_uri=URL("storage://test-cluster/test-project/rw"),
                         container_path="/mnt/rw",
                         read_only=False,
                     ),
                     Volume(
-                        storage_uri=URL("storage://othercluster/otheruser/ro"),
+                        storage_uri=URL("storage://othercluster/otherproject/ro"),
                         container_path="/mnt/ro",
                         read_only=True,
                     ),
                 ],
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_volumes_long(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1180,28 +1204,28 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
-                        storage_uri=URL("storage://test-cluster/otheruser/ro"),
+                        storage_uri=URL("storage://test-cluster/otherproject/ro"),
                         container_path="/mnt/ro",
                         read_only=True,
                     ),
                     Volume(
-                        storage_uri=URL("storage://test-cluster/test-user/rw"),
+                        storage_uri=URL("storage://test-cluster/test-project/rw"),
                         container_path="/mnt/rw",
                         read_only=False,
                     ),
                 ],
             ),
             scheduler_enabled=False,
             pass_config=True,
@@ -1217,14 +1241,15 @@
 
     def test_job_with_secrets_short(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1238,69 +1263,70 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
                 volumes=[
                     Volume(
-                        storage_uri=URL("storage://test-cluster/test-user/rw"),
+                        storage_uri=URL("storage://test-cluster/test-project/rw"),
                         container_path="/mnt/rw",
                         read_only=False,
                     ),
                 ],
                 secret_files=[
                     SecretFile(
-                        URL("secret://test-cluster/test-user/secret1"),
+                        URL("secret://test-cluster/test-project/secret1"),
                         "/var/run/secret1",
                     ),
                     SecretFile(
-                        URL("secret://test-cluster/otheruser/secret2"),
+                        URL("secret://test-cluster/otherproject/secret2"),
                         "/var/run/secret2",
                     ),
                     SecretFile(
-                        URL("secret://othercluster/otheruser/secret3"),
+                        URL("secret://othercluster/otherproject/secret3"),
                         "/var/run/secret3",
                     ),
                 ],
                 env={"ENV_NAME_0": "somevalue"},
                 secret_env={
-                    "ENV_NAME_1": URL("secret://test-cluster/test-user/secret4"),
-                    "ENV_NAME_2": URL("secret://test-cluster/otheruser/secret5"),
-                    "ENV_NAME_3": URL("secret://othercluster/otheruser/secret6"),
+                    "ENV_NAME_1": URL("secret://test-cluster/test-project/secret4"),
+                    "ENV_NAME_2": URL("secret://test-cluster/otherproject/secret5"),
+                    "ENV_NAME_3": URL("secret://othercluster/otherproject/secret6"),
                 },
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_disk_volumes_short(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1314,59 +1340,60 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
                 disk_volumes=[
                     DiskVolume(
-                        URL("disk://test-cluster/test-user/disk1"),
+                        URL("disk://test-cluster/test-project/disk1"),
                         "/mnt/disk1",
                         read_only=True,
                     ),
                     DiskVolume(
-                        URL("disk://test-cluster/otheruser/disk2"),
+                        URL("disk://test-cluster/otherproject/disk2"),
                         "/mnt/disk2",
                         read_only=False,
                     ),
                     DiskVolume(
-                        URL("disk://othercluster/otheruser/disk3"),
+                        URL("disk://othercluster/otherproject/disk3"),
                         "/mnt/disk3",
                         read_only=False,
                     ),
                 ],
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_working_dir(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.FAILED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             name="test-job-name",
             description="test job description",
             http_url=URL("http://local.host.test/"),
             history=JobStatusHistory(
@@ -1380,30 +1407,30 @@
             ),
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_neuro_image(
                     name="test-image",
                     tag="sometag",
                     registry="https://registry.neu.ro",
-                    owner="test-user",
                     cluster_name="test-cluster",
                     org_name=None,
+                    project_name="test-project",
                 ),
                 working_dir="/working/dir",
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                 http=HTTPPort(port=80, requires_auth=True),
             ),
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -1426,23 +1453,24 @@
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=False,
             pass_config=True,
+            project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -1465,36 +1493,38 @@
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=True,
             preemptible_node=True,
             pass_config=True,
+            project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_org_name(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             name="test-job",
             cluster_name="default",
             org_name="test-job-org-name",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
@@ -1513,28 +1543,29 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
     def test_job_with_partial_credits(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         description = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             name="test-job",
             cluster_name="default",
             org_name="test-job-org-name",
             id="test-job",
             uri=URL("job://default/test-user/test-job"),
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
@@ -1553,15 +1584,15 @@
             scheduler_enabled=False,
             pass_config=True,
             total_price_credits=Decimal(150 / 15000),
             price_credits_per_hour=Decimal(15 / 15000),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -1585,23 +1616,42 @@
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=True,
             energy_schedule_name="some-schedule",
             pass_config=True,
+            project_name="myproject",
             owner="owner",
             cluster_name="default",
             uri=URL("job://default/owner/test-job"),
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         uri_fmtr = uri_formatter(
-            username="test-user", cluster_name="test-cluster", org_name=None
+            project_name="test-project", cluster_name="test-cluster", org_name=None
+        )
+        rich_cmp(
+            JobStatusFormatter(
+                uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
+            )(description)
+        )
+
+    @pytest.mark.parametrize("project", ["", "test-user", "someotherproject"])
+    def test_job_with_project_name(
+        self,
+        rich_cmp: Any,
+        datetime_formatter: DatetimeFormatter,
+        project: str,
+    ) -> None:
+        description = make_job(JobStatus.SUCCEEDED, "", project_name=project)
+
+        uri_fmtr = uri_formatter(
+            project_name=project, cluster_name="test-cluster", org_name=None
         )
         rich_cmp(
             JobStatusFormatter(
                 uri_formatter=uri_fmtr, datetime_formatter=datetime_formatter
             )(description)
         )
 
@@ -1836,14 +1886,15 @@
         rich_cmp(formatter([]))
 
     def test_list(self, rich_cmp: Any) -> None:
         jobs = [
             JobDescription(
                 status=JobStatus.PENDING,
                 id="job-42687e7c-6c76-4857-a6a7-1166f8295391",
+                project_name="myproject",
                 owner="owner",
                 cluster_name="default",
                 uri=URL("job://default/owner/job-42687e7c-6c76-4857-a6a7-1166f8295391"),
                 history=JobStatusHistory(
                     status=JobStatus.PENDING,
                     reason="ErrorReason",
                     description="ErrorDesc",
@@ -1860,14 +1911,15 @@
                 total_price_credits=Decimal("150"),
                 price_credits_per_hour=Decimal("15"),
             ),
             JobDescription(
                 status=JobStatus.PENDING,
                 id="job-cf33bd55-9e3b-4df7-a894-9c148a908a66",
                 name="this-job-has-a-name",
+                project_name="otherproject",
                 owner="owner",
                 cluster_name="default",
                 uri=URL("job://default/owner/job-cf33bd55-9e3b-4df7-a894-9c148a908a66"),
                 history=JobStatusHistory(
                     status=JobStatus.FAILED,
                     reason="ErrorReason",
                     description="ErrorDesc",
@@ -1899,14 +1951,15 @@
     ) -> JobDescription:
         remote_image = root.client.parse.remote_image(image)
         return JobDescription(
             status=status,
             id="job-1f5ab792-e534-4bb4-be56-8af1ce722692",
             name=name,
             owner="owner",
+            project_name="myproject",
             cluster_name="default",
             uri=URL("job://default/owner/job-1f5ab792-e534-4bb4-be56-8af1ce722692"),
             description="some",
             history=JobStatusHistory(
                 status=status,
                 reason="ErrorReason",
                 description="ErrorDesc",
@@ -1972,21 +2025,23 @@
         )
         assert row.status == Text(status, style="color")
         assert row.when == date
 
     def test_image_from_registry_parsing_short(
         self, root: Root, datetime_formatter: DatetimeFormatter
     ) -> None:
-        uri_fmtr = uri_formatter(username="bob", cluster_name="default", org_name=None)
+        uri_fmtr = uri_formatter(
+            project_name="test-project", cluster_name="default", org_name=None
+        )
         image_fmtr = image_formatter(uri_formatter=uri_fmtr)
         row = TabularJobRow.from_job(
             self._job_descr_with_status(
                 root,
                 JobStatus.PENDING,
-                "registry-dev.neu.ro/bob/swiss-box:red",
+                "registry-dev.neu.ro/test-project/swiss-box:red",
             ),
             "bob",
             image_formatter=image_fmtr,
             datetime_formatter=datetime_formatter,
         )
         assert row.image == "image:swiss-box:red"
         assert row.name == ""
@@ -2040,14 +2095,15 @@
         owner_printed: str,
         rich_cmp: Any,
     ) -> None:
         job = JobDescription(
             status=JobStatus.FAILED,
             id="j",
             owner=owner_name,
+            project_name="myproject",
             cluster_name="dc",
             uri=URL(f"job://dc/{owner_name}/j"),
             name="name",
             description="d",
             history=JobStatusHistory(
                 status=JobStatus.FAILED,
                 reason="ErrorReason",
@@ -2087,14 +2143,15 @@
     ) -> None:
         jobs = [
             JobDescription(
                 status=JobStatus.FAILED,
                 id="job-7ee153a7-249c-4be9-965a-ba3eafb67c82",
                 name="name1",
                 owner=owner_name,
+                project_name="myproject",
                 cluster_name="default",
                 uri=URL(
                     f"job://default/{owner_name}/"
                     f"job-7ee153a7-249c-4be9-965a-ba3eafb67c82"
                 ),
                 description="some description long long long long",
                 history=JobStatusHistory(
@@ -2118,14 +2175,15 @@
                 price_credits_per_hour=Decimal("15"),
             ),
             JobDescription(
                 status=JobStatus.PENDING,
                 id="job-7ee153a7-249c-4be9-965a-ba3eafb67c84",
                 name="name2",
                 owner=owner_name,
+                project_name="myproject",
                 cluster_name="default",
                 uri=URL(
                     f"job://default/{owner_name}/"
                     f"job-7ee153a7-249c-4be9-965a-ba3eafb67c84"
                 ),
                 description="some description",
                 history=JobStatusHistory(
@@ -2137,17 +2195,17 @@
                     finished_at=isoparse("2017-09-25T12:28:59.759433+00:00"),
                 ),
                 container=Container(
                     image=RemoteImage.new_neuro_image(
                         name="some-image-name",
                         tag="with-long-tag",
                         registry="https://registry.neu.ro",
-                        owner="bob",
                         cluster_name="test-cluster",
                         org_name=None,
+                        project_name="test-project",
                     ),
                     resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
                     command="ls -la /some/path",
                 ),
                 scheduler_enabled=True,
                 pass_config=True,
                 total_price_credits=Decimal("150"),
@@ -2165,14 +2223,15 @@
     def test_custom_columns(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         job = JobDescription(
             status=JobStatus.FAILED,
             id="j",
             owner="owner",
+            project_name="myproject",
             cluster_name="dc",
             uri=URL("job://dc/owner/j"),
             name="name",
             description="d",
             history=JobStatusHistory(
                 status=JobStatus.FAILED,
                 reason="ErrorReason",
@@ -2206,14 +2265,15 @@
     ) -> None:
         life_spans = [None, 0, 7 * 24 * 3600, 12345]
         jobs = [
             JobDescription(
                 status=JobStatus.FAILED,
                 id=f"job-{i}",
                 owner="owner",
+                project_name="myproject",
                 cluster_name="dc",
                 uri=URL("job://dc/owner/j"),
                 name="name",
                 description="d",
                 history=JobStatusHistory(
                     status=JobStatus.FAILED,
                     reason="ErrorReason",
@@ -2281,14 +2341,15 @@
             ),
         ]
         jobs = [
             JobDescription(
                 status=item.status,
                 owner="test-user",
                 cluster_name="default",
+                project_name="myproject",
                 id=f"job-{i}",
                 uri=URL(f"job://default/test-user/job-{i}"),
                 description=None,
                 history=item,
                 container=Container(
                     command="test-command",
                     image=RemoteImage.new_external_image(name="test-image"),
@@ -2316,14 +2377,15 @@
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         items = [None, "/working/dir"]
         jobs = [
             JobDescription(
                 status=JobStatus.FAILED,
                 owner="test-user",
+                project_name="myproject",
                 cluster_name="default",
                 id=f"job-{i}",
                 uri=URL(f"job://default/test-user/job-{i}"),
                 description=None,
                 history=JobStatusHistory(
                     status=JobStatus.FAILED,
                     reason="ErrorReason",
@@ -2358,14 +2420,15 @@
 
     def test_preset(self, rich_cmp: Any, datetime_formatter: DatetimeFormatter) -> None:
         items = [None, "cpu-small", "gpu-large"]
         jobs = [
             JobDescription(
                 status=JobStatus.FAILED,
                 owner="test-user",
+                project_name="myproject",
                 cluster_name="default",
                 id=f"job-{i}",
                 uri=URL(f"job://default/test-user/job-{i}"),
                 description=None,
                 history=JobStatusHistory(
                     status=JobStatus.FAILED,
                     reason="ErrorReason",
@@ -2402,14 +2465,15 @@
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         items = [None, "org1", "org2"]
         jobs = [
             JobDescription(
                 status=JobStatus.FAILED,
                 owner="test-user",
+                project_name="myproject",
                 cluster_name="default",
                 org_name=org_name,
                 id=f"job-{i}",
                 uri=URL(f"job://default/test-user/job-{i}"),
                 description=None,
                 history=JobStatusHistory(
                     status=JobStatus.FAILED,
@@ -2439,22 +2503,55 @@
             "test-user",
             columns,
             image_formatter=str,
             datetime_formatter=datetime_formatter,
         )
         rich_cmp(formatter(jobs))
 
+    def test_project_name(
+        self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
+    ) -> None:
+        projects = ["proj1", "proj2"]
+        owners = ["test-user", "someoneelse"]
+        jobs = []
+        for i, (proj, own) in enumerate(itertools.product(projects, owners)):
+            jobs.append(
+                make_job(
+                    JobStatus.RUNNING, "", name=str(i), project_name=proj, owner=own
+                )
+            )
+
+        columns = parse_ps_columns("id name cluster_name project_name owner image")
+        formatter = TabularJobsFormatter(
+            "test-user",
+            columns,
+            image_formatter=str,
+            datetime_formatter=datetime_formatter,
+        )
+        rich_cmp(formatter(jobs))
+
 
 class TestLifeSpanUpdateFormatter:
     async def test_not_finished(
-        self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
+        self,
+        rich_cmp: Any,
+        datetime_formatter: DatetimeFormatter,
+        monkeypatch: pytest.MonkeyPatch,
     ) -> None:
+        class MyDT(dt_module.datetime):
+            @classmethod
+            def now(cls, tz=None) -> datetime:  # type: ignore
+                return datetime(year=2023, month=3, day=21, tzinfo=tz)
+
+        monkeypatch.setattr(dt_module, "datetime", MyDT)
+
         job = JobDescription(
             status=JobStatus.RUNNING,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id=f"job-id",
             uri=URL(f"job://default/test-user/job-id"),
             description=None,
             history=JobStatusHistory(
                 status=JobStatus.RUNNING,
                 reason="ErrorReason",
@@ -2487,14 +2584,15 @@
             container=Container(
                 command="test-command",
                 image=RemoteImage.new_external_image(name="test-image"),
                 resources=Resources(16 * 2**20, 0.1, 0, None, False, None, None),
             ),
             scheduler_enabled=False,
             pass_config=True,
+            life_span=360000,
             total_price_credits=Decimal("150"),
             price_credits_per_hour=Decimal("15"),
         )
 
         formatter = LifeSpanUpdateFormatter(
             datetime_formatter=datetime_formatter,
         )
@@ -2502,14 +2600,15 @@
 
     async def test_finished(
         self, rich_cmp: Any, datetime_formatter: DatetimeFormatter
     ) -> None:
         job = JobDescription(
             status=JobStatus.SUCCEEDED,
             owner="test-user",
+            project_name="myproject",
             cluster_name="default",
             id=f"job-id",
             uri=URL(f"job://default/test-user/job-id"),
             description=None,
             history=JobStatusHistory(
                 status=JobStatus.SUCCEEDED,
                 reason="ErrorReason",
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_service_accounts.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_service_accounts.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,21 +9,27 @@
     ServiceAccountFormatter,
     ServiceAccountsFormatter,
     SimpleServiceAccountsFormatter,
 )
 from neuro_cli.formatters.utils import format_datetime_human
 
 
-def test_service_account_formatter(rich_cmp: Any) -> None:
+@pytest.mark.parametrize(
+    "org",
+    [None, "some-org"],
+)
+def test_service_account_formatter(rich_cmp: Any, org: Any) -> None:
     account = ServiceAccount(
         id="account",
         name="test1",
         role="test-role",
         owner="user",
         default_cluster="cluster",
+        default_project="some-project",
+        default_org=org,
         created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
     )
     fmtr = ServiceAccountFormatter(datetime_formatter=format_datetime_human)
     rich_cmp(fmtr(account))
 
 
 @pytest.fixture
@@ -31,38 +37,42 @@
     return [
         ServiceAccount(
             id="account-1",
             name="test1",
             role="test-role",
             owner="user",
             default_cluster="cluster",
+            default_project="test-project",
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         ),
         ServiceAccount(
             id="account-2",
             name="test2",
             role="test-role",
             owner="user",
             default_cluster="cluster",
+            default_project="test-project",
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         ),
         ServiceAccount(
             id="account-3",
             name="test3",
             role="test-role",
             owner="user",
             default_cluster="cluster",
+            default_project="test-project",
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         ),
         ServiceAccount(
             id="account-4",
             name="test4",
             role="test-role",
             owner="user",
             default_cluster="cluster",
+            default_project="test-project",
             created_at=isoparse("2017-03-04T12:28:59.759433+00:00"),
         ),
     ]
 
 
 def test_service_accounts_formatter_simple(
     service_accounts_list: List[ServiceAccount], rich_cmp: Any
```

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_storage_formatters.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_storage_formatters.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/formatters/test_utils.py` & `neuro-cli-23.7.0/tests/unit/formatters/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,129 +4,147 @@
 from yarl import URL
 
 from neuro_cli.formatters.utils import uri_formatter
 
 
 @pytest.mark.parametrize("scheme", ("storage", "image"))
 def test_uri_formatter_without_org(scheme: str) -> None:
-    fmtr = uri_formatter(username="user", cluster_name="cluster", org_name=None)
+    fmtr = uri_formatter(
+        project_name="test-project", cluster_name="cluster", org_name=None
+    )
     assert (
-        fmtr(URL(f"{scheme}://cluster/user/path/to/file")) == f"{scheme}:path/to/file"
+        fmtr(URL(f"{scheme}://cluster/test-project/path/to/file"))
+        == f"{scheme}:path/to/file"
     )
-    assert fmtr(URL(f"{scheme}://cluster/user/")) == f"{scheme}:"
-    assert fmtr(URL(f"{scheme}://cluster/user")) == f"{scheme}:"
+    assert fmtr(URL(f"{scheme}://cluster/test-project/")) == f"{scheme}:"
+    assert fmtr(URL(f"{scheme}://cluster/test-project")) == f"{scheme}:"
     assert fmtr(URL(f"{scheme}://cluster/")) == f"{scheme}:/"
     assert fmtr(URL(f"{scheme}://cluster")) == f"{scheme}:/"
     assert (
-        fmtr(URL(f"{scheme}://cluster/otheruser/path/to/file"))
-        == f"{scheme}:/otheruser/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/other-project/path/to/file"))
+        == f"{scheme}:/other-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/user/path/to/file"))
-        == f"{scheme}:/org/user/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/org/test-project/path/to/file"))
+        == f"{scheme}:/org/test-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/user/path/to/file"))
-        == f"{scheme}://othercluster/user/path/to/file"
+        fmtr(URL(f"{scheme}://othercluster/test-project/path/to/file"))
+        == f"{scheme}://othercluster/test-project/path/to/file"
     )
     assert fmtr(URL("user://cluster/user/rest")) == "user://cluster/user/rest"
 
 
 @pytest.mark.parametrize("scheme", ("storage", "image"))
 def test_uri_formatter_with_org(scheme: str) -> None:
-    fmtr = uri_formatter(username="user", cluster_name="cluster", org_name="org")
+    fmtr = uri_formatter(
+        project_name="test-project", cluster_name="cluster", org_name="org"
+    )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/user/path/to/file"))
+        fmtr(URL(f"{scheme}://cluster/org/test-project/path/to/file"))
         == f"{scheme}:path/to/file"
     )
-    assert fmtr(URL(f"{scheme}://cluster/org/user/")) == f"{scheme}:"
-    assert fmtr(URL(f"{scheme}://cluster/org/user")) == f"{scheme}:"
+    assert fmtr(URL(f"{scheme}://cluster/org/test-project/")) == f"{scheme}:"
+    assert fmtr(URL(f"{scheme}://cluster/org/test-project")) == f"{scheme}:"
     assert fmtr(URL(f"{scheme}://cluster/org/")) == f"{scheme}:/"
     assert fmtr(URL(f"{scheme}://cluster/org")) == f"{scheme}:/"
     assert fmtr(URL(f"{scheme}://cluster/")) == f"{scheme}://cluster/"
     assert fmtr(URL(f"{scheme}://cluster")) == f"{scheme}://cluster"
     assert (
-        fmtr(URL(f"{scheme}://cluster/user/path/to/file"))
-        == f"{scheme}://cluster/user/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/test-project/path/to/file"))
+        == f"{scheme}://cluster/test-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/otheruser/path/to/file"))
-        == f"{scheme}:/otheruser/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/org/other-project/path/to/file"))
+        == f"{scheme}:/other-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/otherorg/user/path/to/file"))
-        == f"{scheme}://cluster/otherorg/user/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/otherorg/test-project/path/to/file"))
+        == f"{scheme}://cluster/otherorg/test-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/org/user/path/to/file"))
-        == f"{scheme}://othercluster/org/user/path/to/file"
+        fmtr(URL(f"{scheme}://othercluster/org/test-project/path/to/file"))
+        == f"{scheme}://othercluster/org/test-project/path/to/file"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/user/path/to/file"))
-        == f"{scheme}://cluster/user/path/to/file"
+        fmtr(URL(f"{scheme}://cluster/test-project/path/to/file"))
+        == f"{scheme}://cluster/test-project/path/to/file"
+    )
+    assert (
+        fmtr(URL("user://cluster/org/test-project/rest"))
+        == "user://cluster/org/test-project/rest"
     )
-    assert fmtr(URL("user://cluster/org/user/rest")) == "user://cluster/org/user/rest"
 
 
 @pytest.mark.parametrize("org_name", (None, "org"))
 def test_global_uri_formatter(org_name: Optional[str]) -> None:
-    fmtr = uri_formatter(username="user", cluster_name="cluster", org_name=org_name)
+    fmtr = uri_formatter(
+        project_name="test-project", cluster_name="cluster", org_name=org_name
+    )
     assert fmtr(URL("user://cluster/user/rest")) == "user://cluster/user/rest"
     assert fmtr(URL("user://cluster/org/user/rest")) == "user://cluster/org/user/rest"
 
 
 @pytest.mark.parametrize("scheme", ("storage", "image"))
 def test_uri_formatter_special_chars_without_org(scheme: str) -> None:
-    fmtr = uri_formatter(username="user", cluster_name="cluster", org_name=None)
+    fmtr = uri_formatter(
+        project_name="test-project", cluster_name="cluster", org_name=None
+    )
     assert (
-        fmtr(URL(f"{scheme}://cluster/user/путь/к/файлу"))
+        fmtr(URL(f"{scheme}://cluster/test-project/путь/к/файлу"))
         == f"{scheme}:%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/otheruser/путь/к/файлу"))
-        == f"{scheme}:/otheruser/"
+        fmtr(URL(f"{scheme}://cluster/other-project/путь/к/файлу"))
+        == f"{scheme}:/other-project/"
         "%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/user/путь/к/файлу"))
-        == f"{scheme}://othercluster/user/"
+        fmtr(URL(f"{scheme}://othercluster/test-project/путь/к/файлу"))
+        == f"{scheme}://othercluster/test-project/"
         "%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
-    assert fmtr(URL(f"{scheme}://cluster/user/%2525%3f%23")) == f"{scheme}:%2525%3F%23"
     assert (
-        fmtr(URL(f"{scheme}://cluster/otheruser/%2525%3f%23"))
-        == f"{scheme}:/otheruser/%2525%3F%23"
+        fmtr(URL(f"{scheme}://cluster/test-project/%2525%3f%23"))
+        == f"{scheme}:%2525%3F%23"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/user/%2525%3f%23"))
-        == f"{scheme}://othercluster/user/%2525%3F%23"
+        fmtr(URL(f"{scheme}://cluster/other-project/%2525%3f%23"))
+        == f"{scheme}:/other-project/%2525%3F%23"
+    )
+    assert (
+        fmtr(URL(f"{scheme}://othercluster/other-project/%2525%3f%23"))
+        == f"{scheme}://othercluster/other-project/%2525%3F%23"
     )
 
 
 @pytest.mark.parametrize("scheme", ("storage", "image"))
 def test_uri_formatter_special_chars_with_org(scheme: str) -> None:
-    fmtr = uri_formatter(username="user", cluster_name="cluster", org_name="org")
+    fmtr = uri_formatter(
+        project_name="test-project", cluster_name="cluster", org_name="org"
+    )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/user/путь/к/файлу"))
+        fmtr(URL(f"{scheme}://cluster/org/test-project/путь/к/файлу"))
         == f"{scheme}:%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/otheruser/путь/к/файлу"))
-        == f"{scheme}:/otheruser/"
+        fmtr(URL(f"{scheme}://cluster/org/other-project/путь/к/файлу"))
+        == f"{scheme}:/other-project/"
         "%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/org/user/путь/к/файлу"))
-        == f"{scheme}://othercluster/org/user/"
+        fmtr(URL(f"{scheme}://othercluster/org/test-project/путь/к/файлу"))
+        == f"{scheme}://othercluster/org/test-project/"
         "%D0%BF%D1%83%D1%82%D1%8C/%D0%BA/%D1%84%D0%B0%D0%B9%D0%BB%D1%83"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/user/%2525%3f%23")) == f"{scheme}:%2525%3F%23"
+        fmtr(URL(f"{scheme}://cluster/org/test-project/%2525%3f%23"))
+        == f"{scheme}:%2525%3F%23"
     )
     assert (
-        fmtr(URL(f"{scheme}://cluster/org/otheruser/%2525%3f%23"))
-        == f"{scheme}:/otheruser/%2525%3F%23"
+        fmtr(URL(f"{scheme}://cluster/org/other-project/%2525%3f%23"))
+        == f"{scheme}:/other-project/%2525%3F%23"
     )
     assert (
-        fmtr(URL(f"{scheme}://othercluster/org/user/%2525%3f%23"))
-        == f"{scheme}://othercluster/org/user/%2525%3F%23"
+        fmtr(URL(f"{scheme}://othercluster/org/test-project/%2525%3f%23"))
+        == f"{scheme}://othercluster/org/test-project/%2525%3F%23"
     )
```

### Comparing `neuro-cli-23.2.0/tests/unit/test_admin.py` & `neuro-cli-23.7.0/tests/unit/test_admin.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_ael.py` & `neuro-cli-23.7.0/tests/unit/test_ael.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_alias.py` & `neuro-cli-23.7.0/tests/unit/test_alias.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_click_types.py` & `neuro-cli-23.7.0/tests/unit/test_click_types.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_click_utils.py` & `neuro-cli-23.7.0/tests/unit/test_click_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_config.py` & `neuro-cli-23.7.0/tests/unit/test_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from pathlib import Path
 from typing import Callable
 from unittest import mock
 
 import pytest
 from yarl import URL
 
-from neuro_sdk import Client, Cluster, Preset
+from neuro_sdk import Client, Cluster, Preset, Project
 
-from neuro_cli.config import prompt_cluster
+from neuro_cli.config import prompt_cluster, prompt_project
 from neuro_cli.root import Root
 from neuro_cli.utils import Command, Context
 
 
 async def cmd() -> None:
     pass
 
@@ -161,7 +161,132 @@
     fut = loop.create_future()
     fut.set_result("")
     session.prompt_async.return_value = fut
 
     ret = root.run(prompt_cluster(root, session=session))
     assert ret == "first"
     root.close()
+
+
+@pytest.mark.skipif(
+    sys.platform == "win32",
+    reason="Prompt_toolkit fails in github actions worker",
+)
+def test_prompt_project(make_client: Callable[..., Client]) -> None:
+    clusters = {
+        "default": Cluster(
+            name="default",
+            registry_url=URL("https://registry-dev.neu.ro"),
+            storage_url=URL("https://storage-dev.neu.ro"),
+            users_url=URL("https://users-dev.neu.ro"),
+            monitoring_url=URL("https://monitoring-dev.neu.ro"),
+            secrets_url=URL("https://secrets-dev.neu.ro"),
+            disks_url=URL("https://disks-dev.neu.ro"),
+            buckets_url=URL("https://buckets-dev.neu.ro"),
+            presets={
+                "cpu-small": Preset(
+                    credits_per_hour=Decimal("10"), cpu=1, memory=2**30
+                )
+            },
+            orgs=[None],
+        ),
+    }
+    project = Project(name="main", cluster_name="default", org_name=None, role="owner")
+    projects = {project.key: project}
+
+    root = Root(
+        color=False,
+        tty=False,
+        disable_pypi_version_check=True,
+        network_timeout=60,
+        config_path=Path("<config-path>"),
+        verbosity=0,
+        trace=False,
+        trace_hide_token=True,
+        force_trace_all=False,
+        command_path="",
+        command_params=[],
+        skip_gmp_stats=True,
+        show_traceback=False,
+        iso_datetime_format=False,
+        ctx=Context(Command(cmd, name="")),
+    )
+
+    async def _async_make_client() -> Client:
+        return make_client("https://neu.ro", clusters=clusters, projects=projects)
+
+    root._client = root.run(_async_make_client())
+
+    session = mock.Mock()
+    loop = root._runner._loop
+    assert loop is not None
+    fut = loop.create_future()
+    fut.set_result("main")
+    session.prompt_async.return_value = fut
+    ret = root.run(prompt_project(root, session=session))
+    assert ret == "main"
+    root.close()
+
+
+@pytest.mark.skipif(
+    sys.platform == "win32",
+    reason="Prompt_toolkit fails in github actions worker",
+)
+def test_prompt_project_default(make_client: Callable[..., Client]) -> None:
+    clusters = {
+        "default": Cluster(
+            name="default",
+            registry_url=URL("https://registry-dev.neu.ro"),
+            storage_url=URL("https://storage-dev.neu.ro"),
+            users_url=URL("https://users-dev.neu.ro"),
+            monitoring_url=URL("https://monitoring-dev.neu.ro"),
+            secrets_url=URL("https://secrets-dev.neu.ro"),
+            disks_url=URL("https://disks-dev.neu.ro"),
+            buckets_url=URL("https://buckets-dev.neu.ro"),
+            presets={
+                "cpu-small": Preset(
+                    credits_per_hour=Decimal("10"), cpu=1, memory=2**30
+                )
+            },
+            orgs=[None],
+        ),
+    }
+    project = Project(name="main", cluster_name="default", org_name=None, role="owner")
+    projects = {project.key: project}
+
+    root = Root(
+        color=False,
+        tty=False,
+        disable_pypi_version_check=True,
+        network_timeout=60,
+        config_path=Path("<config-path>"),
+        verbosity=0,
+        trace=False,
+        trace_hide_token=True,
+        force_trace_all=False,
+        command_path="",
+        command_params=[],
+        skip_gmp_stats=True,
+        show_traceback=False,
+        iso_datetime_format=False,
+        ctx=Context(Command(cmd, name="")),
+    )
+
+    async def _async_make_client() -> Client:
+        return make_client(
+            "https://neu.ro",
+            clusters=clusters,
+            projects=projects,
+            project_name=project.name,
+        )
+
+    root._client = root.run(_async_make_client())
+
+    session = mock.Mock()
+    loop = root._runner._loop
+    assert loop is not None
+    fut = loop.create_future()
+    fut.set_result("")
+    session.prompt_async.return_value = fut
+    ret = root.run(prompt_project(root, session=session))
+    assert ret == "main"
+    root.close()
```

### Comparing `neuro-cli-23.2.0/tests/unit/test_docker_helper.py` & `neuro-cli-23.7.0/tests/unit/test_docker_helper.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_job.py` & `neuro-cli-23.7.0/tests/unit/test_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,27 +186,27 @@
 
     assert root.client.parse._build_env([], [str(env_file1), str(env_file2)]) == {
         "ENV_VAR": "value2",
     }
 
 
 def test_extract_secret_env(root: Root) -> None:
-    username = root.client.username
+    project_name = root.client.config.project_name
     cluster_name = root.client.cluster_name
     env = {
         "ENV_VAR_1": "secret:value1",
         "ENV_VAR_2": "value2",
-        "ENV_VAR_3": "secret:/otheruser/value3",
+        "ENV_VAR_3": "secret:/otherproject/value3",
         "ENV_VAR_4": "value4",
-        "ENV_VAR_5": "secret://othercluster/otheruser/value5",
+        "ENV_VAR_5": "secret://othercluster/otherproject/value5",
     }
     assert root.client.parse._extract_secret_env(env) == {
-        "ENV_VAR_1": URL(f"secret://{cluster_name}/{username}/value1"),
-        "ENV_VAR_3": URL(f"secret://{cluster_name}/otheruser/value3"),
-        "ENV_VAR_5": URL(f"secret://othercluster/otheruser/value5"),
+        "ENV_VAR_1": URL(f"secret://{cluster_name}/{project_name}/value1"),
+        "ENV_VAR_3": URL(f"secret://{cluster_name}/otherproject/value3"),
+        "ENV_VAR_5": URL(f"secret://othercluster/otherproject/value5"),
     }
     assert env == {"ENV_VAR_2": "value2", "ENV_VAR_4": "value4"}
 
 
 async def test_calc_ps_columns_section_doesnt_exist(
     monkeypatch: Any, tmp_path: Path, make_client: _MakeClient
 ) -> None:
@@ -280,14 +280,15 @@
     assert _parse_cmd(cmd) == "bash -c 'ls -l && pwd'"
 
 
 def test_job_to_args_simple() -> None:
     job = JobDescription(
         status=JobStatus.FAILED,
         owner="test-user",
+        project_name="myproj",
         cluster_name="default",
         id=f"job",
         uri=URL(f"job://default/test-user/job"),
         description=None,
         history=JobStatusHistory(
             status=JobStatus.FAILED,
             reason="ErrorReason",
@@ -306,23 +307,27 @@
         preset_name="testing",
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
     assert _job_to_cli_args(job) == [
         "--preset",
         "testing",
+        "--project",
+        "myproj",
         "test-image",
+        "--",
         "test-command",
     ]
 
 
 def test_job_to_args_drop_env_when_pass_config() -> None:
     job = JobDescription(
         status=JobStatus.FAILED,
         owner="test-user",
+        project_name="myproj",
         cluster_name="default",
         id=f"job",
         uri=URL(f"job://default/test-user/job"),
         description=None,
         history=JobStatusHistory(
             status=JobStatus.FAILED,
             reason="ErrorReason",
@@ -345,25 +350,29 @@
         total_price_credits=Decimal("150"),
         price_credits_per_hour=Decimal("15"),
     )
     assert _job_to_cli_args(job) == [
         "--preset",
         "testing",
         "--pass-config",
+        "--project",
+        "myproj",
         "test-image",
+        "--",
         "test-command",
     ]
 
 
 def test_job_to_args_complex() -> None:
     job = JobDescription(
         status=JobStatus.FAILED,
         owner="test-user",
         name="test-job",
         tags=["tag-1", "tag-2"],
+        project_name="myproject",
         cluster_name="default",
         id=f"job",
         uri=URL(f"job://default/test-user/job"),
         description="test description",
         restart_policy=JobRestartPolicy.ALWAYS,
         history=JobStatusHistory(
             status=JobStatus.FAILED,
@@ -474,10 +483,49 @@
         "2d11h17m12s",
         "--pass-config",
         "--privileged",
         "--priority",
         "high",
         "--energy-schedule",
         "some-energy-schedule-name",
+        "--project",
+        "myproject",
         "test-image",
+        "--",
         "test-command",
     ]
+
+
+def test_job_to_args_no_cmd() -> None:
+    job = JobDescription(
+        status=JobStatus.FAILED,
+        owner="test-user",
+        project_name="proj",
+        cluster_name="default",
+        id=f"job",
+        uri=URL(f"job://default/test-user/job"),
+        description=None,
+        history=JobStatusHistory(
+            status=JobStatus.FAILED,
+            reason="ErrorReason",
+            description="ErrorDesc",
+            created_at=isoparse("2018-09-25T12:28:21.298672+00:00"),
+            started_at=isoparse("2018-09-25T12:28:59.759433+00:00"),
+            finished_at=datetime.now(timezone.utc) - timedelta(seconds=1),
+        ),
+        container=Container(
+            image=RemoteImage.new_external_image(name="test-image"),
+            resources=Resources(16, 0.1, 0, None, True, None, None),
+        ),
+        scheduler_enabled=False,
+        pass_config=False,
+        preset_name="testing",
+        total_price_credits=Decimal("150"),
+        price_credits_per_hour=Decimal("15"),
+    )
+    assert _job_to_cli_args(job) == [
+        "--preset",
+        "testing",
+        "--project",
+        "proj",
+        "test-image",
+    ]
```

### Comparing `neuro-cli-23.2.0/tests/unit/test_parse_utils.py` & `neuro-cli-23.7.0/tests/unit/test_parse_utils.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_root.py` & `neuro-cli-23.7.0/tests/unit/test_root.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_shell_completion.py` & `neuro-cli-23.7.0/tests/unit/test_shell_completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -196,15 +196,14 @@
 
 
 @skip_on_windows
 def test_storage_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Storage, "stat") as mocked_stat, mock.patch.object(
         Storage, "list"
     ) as mocked_list:
-
         tree = {
             URL("storage://default"): ["test-user", "other-user"],
             URL("storage://default/test-user"): ["folder", "file.txt"],
             URL("storage://default/test-user/folder"): ["folder2", "file2.txt"],
             URL("storage://default/other-user"): ["folder3", "file3.txt"],
             URL("storage://other-cluster"): ["test-user"],
         }
@@ -323,34 +322,70 @@
                 name="neuro-my-bucket",
                 created_at=datetime(2018, 1, 1, 3),
                 cluster_name="default",
                 owner="user",
                 provider=Bucket.Provider.AWS,
                 imported=False,
                 org_name=None,
+                project_name="project",
             )
             yield Bucket(
                 id="bucket-2",
                 name="neuro-public-bucket",
                 created_at=datetime(2018, 1, 1, 17, 2, 4),
                 cluster_name="default",
                 owner="public",
                 provider=Bucket.Provider.AWS,
                 imported=False,
                 org_name=None,
+                project_name="project",
             )
             yield Bucket(
                 id="bucket-3",
                 name="neuro-shared-bucket",
                 created_at=datetime(2018, 1, 1, 13, 1, 5),
                 cluster_name="default",
                 owner="another-user",
                 provider=Bucket.Provider.AWS,
                 imported=False,
                 org_name=None,
+                project_name="project",
+            )
+            yield Bucket(
+                id="bucket-4",
+                name="neuro-my-org-bucket",
+                created_at=datetime(2018, 1, 1, 3),
+                cluster_name="default",
+                owner="user",
+                provider=Bucket.Provider.AWS,
+                imported=False,
+                org_name="org",
+                project_name="project",
+            )
+            yield Bucket(
+                id="bucket-5",
+                name="neuro-public-org-bucket",
+                created_at=datetime(2018, 1, 1, 17, 2, 4),
+                cluster_name="default",
+                owner="public",
+                provider=Bucket.Provider.AWS,
+                imported=False,
+                org_name="org",
+                project_name="project",
+            )
+            yield Bucket(
+                id="bucket-6",
+                name="neuro-shared-org-bucket",
+                created_at=datetime(2018, 1, 1, 13, 1, 5),
+                cluster_name="default",
+                owner="another-user",
+                provider=Bucket.Provider.AWS,
+                imported=False,
+                org_name="org",
+                project_name="project",
             )
 
         async def blob_is_dir(uri: URL) -> bool:
             return ".txt" not in uri.name
 
         @asyncgeneratorcontextmanager
         async def list_blobs(uri: URL) -> AsyncIterator[BlobObject]:
@@ -467,14 +502,66 @@
             "uri\nfile1024.txt\n_\nblob:bucket-1/\n"
             "uri\notherfile.txt\n_\nblob:bucket-1/\n"
             "uri\nfile_bigger.txt\n_\nblob:bucket-1/\n"
             "uri\nfolder2/\n_\nblob:bucket-1/\n"
             "uri\nfolder23/\n_\nblob:bucket-1/"
         )
 
+        zsh_out, bash_out = run_autocomplete(["blob", "ls", "blob:/p"])
+        assert bash_out == "uri,project/,//default/"
+        assert zsh_out == "uri\nproject/\n_\nblob://default/"
+
+        zsh_out, bash_out = run_autocomplete(["blob", "ls", "blob:/project/"])
+        assert bash_out == (
+            "uri,bucket-1/,\n"
+            "uri,neuro-my-bucket/,\n"
+            "uri,bucket-2/,\n"
+            "uri,neuro-public-bucket/,\n"
+            "uri,bucket-3/,\n"
+            "uri,neuro-shared-bucket/,"
+        )
+        assert zsh_out == (
+            "uri\nbucket-1/\n_\nblob:\nuri\nneuro-my-bucket/\n_\nblob:\n"
+            "uri\nbucket-2/\n_\nblob:\n"
+            "uri\nneuro-public-bucket/\n_\nblob:\n"
+            "uri\nbucket-3/\n_\nblob:\n"
+            "uri\nneuro-shared-bucket/\n_\nblob:"
+        )
+
+        zsh_out, bash_out = run_autocomplete(["blob", "ls", "blob://default/"])
+        assert bash_out == "uri,project/,//default/\nuri,org/,//default/"
+        assert (
+            zsh_out
+            == "uri\nproject/\n_\nblob://default/\nuri\norg/\n_\nblob://default/"
+        )
+
+        zsh_out, bash_out = run_autocomplete(["blob", "ls", "blob://default/org/"])
+        assert bash_out == "uri,project/,//default/org/"
+        assert zsh_out == "uri\nproject/\n_\nblob://default/org/"
+
+        zsh_out, bash_out = run_autocomplete(
+            ["blob", "ls", "blob://default/org/project/"]
+        )
+        assert bash_out == (
+            "uri,bucket-4/,//default/org/project/\n"
+            "uri,neuro-my-org-bucket/,//default/org/project/\n"
+            "uri,bucket-5/,//default/org/project/\n"
+            "uri,neuro-public-org-bucket/,//default/org/project/\n"
+            "uri,bucket-6/,//default/org/project/\n"
+            "uri,neuro-shared-org-bucket/,//default/org/project/"
+        )
+        assert zsh_out == (
+            "uri\nbucket-4/\n_\nblob://default/org/project/\n"
+            "uri\nneuro-my-org-bucket/\n_\nblob://default/org/project/\n"
+            "uri\nbucket-5/\n_\nblob://default/org/project/\n"
+            "uri\nneuro-public-org-bucket/\n_\nblob://default/org/project/\n"
+            "uri\nbucket-6/\n_\nblob://default/org/project/\n"
+            "uri\nneuro-shared-org-bucket/\n_\nblob://default/org/project/"
+        )
+
         zsh_out, bash_out = run_autocomplete(["blob", "ls", "blob:bucket-1/f"])
         assert bash_out == (
             "uri,file1024.txt,bucket-1/\n"
             "uri,file_bigger.txt,bucket-1/\n"
             "uri,folder2/,bucket-1/\n"
             "uri,folder23/,bucket-1/"
         )
@@ -504,21 +591,25 @@
         assert bash_out == "uri,info.txt,bucket-1/folder2/"
         assert zsh_out == "uri\ninfo.txt\n_\nblob:bucket-1/folder2/"
 
 
 def make_job(
     job_id: str,
     name: Optional[str] = None,
+    org_name: Optional[str] = None,
     owner: str = "test-user",
     cluster_name: str = "default",
+    project_name: str = "test-project",
 ) -> JobDescription:
     return JobDescription(
         status=JobStatus.FAILED,
         owner=owner,
+        project_name=project_name,
         cluster_name=cluster_name,
+        org_name=org_name,
         id=job_id,
         name=name,
         uri=URL(f"job://{cluster_name}/{owner}/{job_id}"),
         description=None,
         history=JobStatusHistory(
             status=JobStatus.FAILED,
             reason="ErrorReason",
@@ -540,34 +631,51 @@
     )
 
 
 @skip_on_windows
 def test_job_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Jobs, "list") as mocked_list:
         jobs = [
-            make_job("job-0123-4567", owner="user"),
-            make_job("job-89ab-cdef", owner="user", name="jeronimo"),
-            make_job("job-0123-cdef", owner="other-user"),
-            make_job("job-89ab-4567", cluster_name="other", owner="user"),
+            make_job("job-0123-4567", owner="user", project_name="project"),
+            make_job(
+                "job-89ab-cdef", owner="user", name="jeronimo", project_name="project"
+            ),
+            make_job("job-0123-cdef", owner="other-user", project_name="project"),
+            make_job(
+                "job-0123-4567",
+                owner="other-user",
+                name="oeronimo",
+                project_name="project",
+            ),
+            make_job(
+                "job-89ab-4567",
+                cluster_name="other",
+                owner="user",
+                project_name="project",
+            ),
+            make_job("job-4567-cdef", owner="user", project_name="otherproject"),
         ]
 
         @asyncgeneratorcontextmanager
         async def list(
             *,
             since: Optional[datetime] = None,
             reverse: bool = False,
             limit: Optional[int] = None,
             cluster_name: Optional[str] = None,
             owners: Iterable[str] = (),
+            project_names: Iterable[str] = (),
         ) -> AsyncIterator[JobDescription]:
             for job in jobs:
                 if cluster_name and job.cluster_name != cluster_name:
                     continue
                 if owners and job.owner not in owners:
                     continue
+                if project_names and job.project_name not in project_names:
+                    continue
                 yield job
 
         mocked_list.side_effect = list
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "j"])
         assert bash_out == "uri,job:,"
         assert zsh_out == "uri\njob:\n_\n_"
@@ -578,58 +686,74 @@
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "je"])
         assert bash_out == "plain,jeronimo,"
         assert zsh_out == "plain\njeronimo\njob-89ab-cdef\n_"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:"])
         assert bash_out == (
-            "uri,job-0123-4567,\n" "uri,job-89ab-cdef,\n" "uri,jeronimo,"
+            "uri,job-0123-4567,\n"
+            "uri,job-89ab-cdef,\n"
+            "uri,jeronimo,\n"
+            "uri,job-0123-cdef,\n"
+            "uri,oeronimo,"
         )
         assert zsh_out == (
             "uri\njob-0123-4567\n_\njob:\n"
             "uri\njob-89ab-cdef\n_\njob:\n"
-            "uri\njeronimo\n_\njob:"
+            "uri\njeronimo\n_\njob:\n"
+            "uri\njob-0123-cdef\n_\njob:\n"
+            "uri\noeronimo\n_\njob:"
         )
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:j"])
         assert bash_out == (
-            "uri,job-0123-4567,\n" "uri,job-89ab-cdef,\n" "uri,jeronimo,"
+            "uri,job-0123-4567,\n"
+            "uri,job-89ab-cdef,\n"
+            "uri,jeronimo,\n"
+            "uri,job-0123-cdef,"
         )
         assert zsh_out == (
             "uri\njob-0123-4567\n_\njob:\n"
             "uri\njob-89ab-cdef\n_\njob:\n"
-            "uri\njeronimo\n_\njob:"
+            "uri\njeronimo\n_\njob:\n"
+            "uri\njob-0123-cdef\n_\njob:"
         )
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:je"])
         assert bash_out == "uri,jeronimo,"
         assert zsh_out == "uri\njeronimo\n_\njob:"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:/"])
-        assert bash_out == ("uri,user/,/\n" "uri,other-user/,/")
-        assert zsh_out == ("uri\nuser/\n_\njob:/\n" "uri\nother-user/\n_\njob:/")
+        assert bash_out == ("uri,project/,/\nuri,user/,/\n" "uri,otherproject/,/")
+        assert zsh_out == (
+            "uri\nproject/\n_\njob:/\n"
+            "uri\nuser/\n_\njob:/\n"
+            "uri\notherproject/\n_\njob:/"
+        )
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:/u"])
         assert bash_out == "uri,user/,/"
         assert zsh_out == "uri\nuser/\n_\njob:/"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job:/o"])
-        assert bash_out == "uri,other-user/,/"
-        assert zsh_out == "uri\nother-user/\n_\njob:/"
+        assert bash_out == "uri,otherproject/,/"
+        assert zsh_out == "uri\notherproject/\n_\njob:/"
 
-        zsh_out, bash_out = run_autocomplete(["job", "status", "job:/user/j"])
+        zsh_out, bash_out = run_autocomplete(["job", "status", "job:/project/j"])
         assert bash_out == (
-            "uri,job-0123-4567,/user/\n"
-            "uri,job-89ab-cdef,/user/\n"
-            "uri,jeronimo,/user/"
+            "uri,job-0123-4567,/project/\n"
+            "uri,job-89ab-cdef,/project/\n"
+            "uri,jeronimo,/project/\n"
+            "uri,job-0123-cdef,/project/"
         )
         assert zsh_out == (
-            "uri\njob-0123-4567\n_\njob:/user/\n"
-            "uri\njob-89ab-cdef\n_\njob:/user/\n"
-            "uri\njeronimo\n_\njob:/user/"
+            "uri\njob-0123-4567\n_\njob:/project/\n"
+            "uri\njob-89ab-cdef\n_\njob:/project/\n"
+            "uri\njeronimo\n_\njob:/project/\n"
+            "uri\njob-0123-cdef\n_\njob:/project/"
         )
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://"])
         assert bash_out == ("uri,default/,//\n" "uri,other/,//")
         assert zsh_out == ("uri\ndefault/\n_\njob://\n" "uri\nother/\n_\njob://")
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://d"])
@@ -637,92 +761,110 @@
         assert zsh_out == "uri\ndefault/\n_\njob://"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://o"])
         assert bash_out == "uri,other/,//"
         assert zsh_out == "uri\nother/\n_\njob://"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://default/"])
-        assert bash_out == ("uri,user/,//default/\n" "uri,other-user/,//default/")
+        assert bash_out == (
+            "uri,project/,//default/\n"
+            "uri,user/,//default/\n"
+            "uri,otherproject/,//default/"
+        )
         assert zsh_out == (
-            "uri\nuser/\n_\njob://default/\n" "uri\nother-user/\n_\njob://default/"
+            "uri\nproject/\n_\njob://default/\n"
+            "uri\nuser/\n_\njob://default/\n"
+            "uri\notherproject/\n_\njob://default/"
         )
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://other/"])
         assert bash_out == "uri,user/,//other/"
         assert zsh_out == "uri\nuser/\n_\njob://other/"
 
         zsh_out, bash_out = run_autocomplete(["job", "status", "job://default/u"])
         assert bash_out == "uri,user/,//default/"
         assert zsh_out == "uri\nuser/\n_\njob://default/"
 
-        zsh_out, bash_out = run_autocomplete(["job", "status", "job://default/user/"])
+        zsh_out, bash_out = run_autocomplete(
+            ["job", "status", "job://default/project/"]
+        )
         assert bash_out == (
-            "uri,job-0123-4567,//default/user/\n"
-            "uri,job-89ab-cdef,//default/user/\n"
-            "uri,jeronimo,//default/user/"
+            "uri,job-0123-4567,//default/project/\n"
+            "uri,job-89ab-cdef,//default/project/\n"
+            "uri,jeronimo,//default/project/\n"
+            "uri,job-0123-cdef,//default/project/\n"
+            "uri,oeronimo,//default/project/"
         )
         assert zsh_out == (
-            "uri\njob-0123-4567\n_\njob://default/user/\n"
-            "uri\njob-89ab-cdef\n_\njob://default/user/\n"
-            "uri\njeronimo\n_\njob://default/user/"
+            "uri\njob-0123-4567\n_\njob://default/project/\n"
+            "uri\njob-89ab-cdef\n_\njob://default/project/\n"
+            "uri\njeronimo\n_\njob://default/project/\n"
+            "uri\njob-0123-cdef\n_\njob://default/project/\n"
+            "uri\noeronimo\n_\njob://default/project/"
         )
 
-        zsh_out, bash_out = run_autocomplete(["job", "status", "job://default/user/je"])
-        assert bash_out == "uri,jeronimo,//default/user/"
-        assert zsh_out == "uri\njeronimo\n_\njob://default/user/"
+        zsh_out, bash_out = run_autocomplete(
+            ["job", "status", "job://default/project/je"]
+        )
+        assert bash_out == "uri,jeronimo,//default/project/"
+        assert zsh_out == "uri\njeronimo\n_\njob://default/project/"
+
+        zsh_out, bash_out = run_autocomplete(["job", "status", "job://default/otherpr"])
+        assert bash_out == "uri,otherproject/,//default/"
+        assert zsh_out == "uri\notherproject/\n_\njob://default/"
 
 
 @skip_on_windows
 def test_image_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Images, "list") as mocked_list:
         images = {
             "default": [
                 RemoteImage.new_neuro_image(
                     name="bananas",
                     registry="registry-dev.neu.ro",
-                    owner="user",
                     cluster_name="default",
                     org_name=None,
+                    project_name="project",
                 ),
                 RemoteImage.new_neuro_image(
                     name="lemons",
                     registry="registry-dev.neu.ro",
-                    owner="user",
                     cluster_name="default",
                     org_name=None,
+                    project_name="project",
                 ),
                 RemoteImage.new_neuro_image(
                     name="library/bananas",
                     registry="registry-dev.neu.ro",
-                    owner="user",
                     cluster_name="default",
                     org_name=None,
+                    project_name="project",
                 ),
                 RemoteImage.new_neuro_image(
                     name="library/bananas",
                     registry="registry-dev.neu.ro",
-                    owner="other-user",
                     cluster_name="default",
                     org_name=None,
+                    project_name="other-project",
                 ),
                 RemoteImage.new_neuro_image(
                     name="library/bananas",
                     registry="registry-dev.neu.ro",
-                    owner="user",
                     cluster_name="default",
                     org_name="org",
+                    project_name="project",
                 ),
             ],
             "other": [
                 RemoteImage.new_neuro_image(
                     name="library/bananas",
                     registry="registry2-dev.neu.ro",
-                    owner="user",
                     cluster_name="other",
                     org_name=None,
+                    project_name="project",
                 ),
             ],
         }
 
         async def list(cluster_name: str) -> List[RemoteImage]:
             return images[cluster_name]
 
@@ -746,51 +888,54 @@
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image:l"])
         assert bash_out == ("uri,lemons,\n" "uri,library/bananas,")
         assert zsh_out == ("uri\nlemons\n_\nimage:\n" "uri\nlibrary/bananas\n_\nimage:")
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image:/"])
         assert bash_out == (
-            "uri,user/bananas,/\n"
-            "uri,user/lemons,/\n"
-            "uri,user/library/bananas,/\n"
-            "uri,other-user/library/bananas,/\n"
-            "uri,org/user/library/bananas,/"
+            "uri,project/bananas,/\n"
+            "uri,project/lemons,/\n"
+            "uri,project/library/bananas,/\n"
+            "uri,other-project/library/bananas,/\n"
+            "uri,org/project/library/bananas,/"
         )
         assert zsh_out == (
-            "uri\nuser/bananas\n_\nimage:/\n"
-            "uri\nuser/lemons\n_\nimage:/\n"
-            "uri\nuser/library/bananas\n_\nimage:/\n"
-            "uri\nother-user/library/bananas\n_\nimage:/\n"
-            "uri\norg/user/library/bananas\n_\nimage:/"
+            "uri\nproject/bananas\n_\nimage:/\n"
+            "uri\nproject/lemons\n_\nimage:/\n"
+            "uri\nproject/library/bananas\n_\nimage:/\n"
+            "uri\nother-project/library/bananas\n_\nimage:/\n"
+            "uri\norg/project/library/bananas\n_\nimage:/"
         )
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/u"])
+        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/p"])
         assert bash_out == (
-            "uri,user/bananas,/\n" "uri,user/lemons,/\n" "uri,user/library/bananas,/"
+            "uri,project/bananas,/\n"
+            "uri,project/lemons,/\n"
+            "uri,project/library/bananas,/"
         )
         assert zsh_out == (
-            "uri\nuser/bananas\n_\nimage:/\n"
-            "uri\nuser/lemons\n_\nimage:/\n"
-            "uri\nuser/library/bananas\n_\nimage:/"
+            "uri\nproject/bananas\n_\nimage:/\n"
+            "uri\nproject/lemons\n_\nimage:/\n"
+            "uri\nproject/library/bananas\n_\nimage:/"
         )
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image:/o"])
         assert bash_out == (
-            "uri,other-user/library/bananas,/\n" "uri,org/user/library/bananas,/"
+            "uri,other-project/library/bananas,/\n" "uri,org/project/library/bananas,/"
         )
         assert zsh_out == (
-            "uri\nother-user/library/bananas\n_\nimage:/\n"
-            "uri\norg/user/library/bananas\n_\nimage:/"
+            "uri\nother-project/library/bananas\n_\nimage:/\n"
+            "uri\norg/project/library/bananas\n_\nimage:/"
         )
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/user/l"])
-        assert bash_out == ("uri,user/lemons,/\n" "uri,user/library/bananas,/")
+        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/project/l"])
+        assert bash_out == ("uri,project/lemons,/\n" "uri,project/library/bananas,/")
         assert zsh_out == (
-            "uri\nuser/lemons\n_\nimage:/\n" "uri\nuser/library/bananas\n_\nimage:/"
+            "uri\nproject/lemons\n_\nimage:/\n"
+            "uri\nproject/library/bananas\n_\nimage:/"
         )
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://"])
         assert bash_out == ("uri,default/,//\n" "uri,other/,//")
         assert zsh_out == ("uri\ndefault/\n_\nimage://\n" "uri\nother/\n_\nimage://")
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://d"])
@@ -799,83 +944,85 @@
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://o"])
         assert bash_out == "uri,other/,//"
         assert zsh_out == "uri\nother/\n_\nimage://"
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://default/"])
         assert bash_out == (
-            "uri,user/bananas,//default/\n"
-            "uri,user/lemons,//default/\n"
-            "uri,user/library/bananas,//default/\n"
-            "uri,other-user/library/bananas,//default/\n"
-            "uri,org/user/library/bananas,//default/"
+            "uri,project/bananas,//default/\n"
+            "uri,project/lemons,//default/\n"
+            "uri,project/library/bananas,//default/\n"
+            "uri,other-project/library/bananas,//default/\n"
+            "uri,org/project/library/bananas,//default/"
         )
         assert zsh_out == (
-            "uri\nuser/bananas\n_\nimage://default/\n"
-            "uri\nuser/lemons\n_\nimage://default/\n"
-            "uri\nuser/library/bananas\n_\nimage://default/\n"
-            "uri\nother-user/library/bananas\n_\nimage://default/\n"
-            "uri\norg/user/library/bananas\n_\nimage://default/"
+            "uri\nproject/bananas\n_\nimage://default/\n"
+            "uri\nproject/lemons\n_\nimage://default/\n"
+            "uri\nproject/library/bananas\n_\nimage://default/\n"
+            "uri\nother-project/library/bananas\n_\nimage://default/\n"
+            "uri\norg/project/library/bananas\n_\nimage://default/"
         )
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://other/"])
-        assert bash_out == ("uri,user/library/bananas,//other/")
-        assert zsh_out == ("uri\nuser/library/bananas\n_\nimage://other/")
+        assert bash_out == ("uri,project/library/bananas,//other/")
+        assert zsh_out == ("uri\nproject/library/bananas\n_\nimage://other/")
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image://default/o"])
         assert bash_out == (
-            "uri,other-user/library/bananas,//default/\n"
-            "uri,org/user/library/bananas,//default/"
+            "uri,other-project/library/bananas,//default/\n"
+            "uri,org/project/library/bananas,//default/"
         )
         assert zsh_out == (
-            "uri\nother-user/library/bananas\n_\nimage://default/\n"
-            "uri\norg/user/library/bananas\n_\nimage://default/"
+            "uri\nother-project/library/bananas\n_\nimage://default/\n"
+            "uri\norg/project/library/bananas\n_\nimage://default/"
         )
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image://default/user/"])
+        zsh_out, bash_out = run_autocomplete(
+            ["image", "size", "image://default/project/"]
+        )
         assert bash_out == (
-            "uri,user/bananas,//default/\n"
-            "uri,user/lemons,//default/\n"
-            "uri,user/library/bananas,//default/"
+            "uri,project/bananas,//default/\n"
+            "uri,project/lemons,//default/\n"
+            "uri,project/library/bananas,//default/"
         )
         assert zsh_out == (
-            "uri\nuser/bananas\n_\nimage://default/\n"
-            "uri\nuser/lemons\n_\nimage://default/\n"
-            "uri\nuser/library/bananas\n_\nimage://default/"
+            "uri\nproject/bananas\n_\nimage://default/\n"
+            "uri\nproject/lemons\n_\nimage://default/\n"
+            "uri\nproject/library/bananas\n_\nimage://default/"
         )
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/l"]
+            ["image", "size", "image://default/project/l"]
         )
         assert bash_out == (
-            "uri,user/lemons,//default/\n" "uri,user/library/bananas,//default/"
+            "uri,project/lemons,//default/\n" "uri,project/library/bananas,//default/"
         )
         assert zsh_out == (
-            "uri\nuser/lemons\n_\nimage://default/\n"
-            "uri\nuser/library/bananas\n_\nimage://default/"
+            "uri\nproject/lemons\n_\nimage://default/\n"
+            "uri\nproject/library/bananas\n_\nimage://default/"
         )
 
 
 @skip_on_windows
 def test_nonascii_image_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Images, "list") as mocked_list:
         images = [
             RemoteImage.new_neuro_image(
                 name="ima?ge",
                 registry="registry-dev.neu.ro",
-                owner="user",
                 cluster_name="default",
                 org_name=None,
+                project_name="project",
             ),
             RemoteImage.new_neuro_image(
                 name="образ",
                 registry="registry-dev.neu.ro",
-                owner="user",
                 cluster_name="default",
                 org_name=None,
+                project_name="project",
             ),
         ]
 
         async def list(cluster_name: str) -> List[RemoteImage]:
             if cluster_name == "default":
                 return images
             return []
@@ -899,77 +1046,79 @@
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image:%D0%BE%D0%B1"])
         assert bash_out == ("uri,%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,")
         assert zsh_out == ("uri\n%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage:")
 
         zsh_out, bash_out = run_autocomplete(["image", "size", "image:/"])
         assert bash_out == (
-            "uri,user/ima%3Fge,/\n" "uri,user/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,/"
+            "uri,project/ima%3Fge,/\n" "uri,project/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,/"
         )
         assert zsh_out == (
-            "uri\nuser/ima%3Fge\n_\nimage:/\n"
-            "uri\nuser/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage:/"
+            "uri\nproject/ima%3Fge\n_\nimage:/\n"
+            "uri\nproject/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage:/"
         )
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/user/im"])
-        assert bash_out == ("uri,user/ima%3Fge,/")
-        assert zsh_out == ("uri\nuser/ima%3Fge\n_\nimage:/")
+        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/project/im"])
+        assert bash_out == ("uri,project/ima%3Fge,/")
+        assert zsh_out == ("uri\nproject/ima%3Fge\n_\nimage:/")
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/user/об"])
-        assert bash_out == ("uri,user/об%D1%80%D0%B0%D0%B7,/")
-        assert zsh_out == ("uri\nuser/об%D1%80%D0%B0%D0%B7\n_\nimage:/")
+        zsh_out, bash_out = run_autocomplete(["image", "size", "image:/project/об"])
+        assert bash_out == ("uri,project/об%D1%80%D0%B0%D0%B7,/")
+        assert zsh_out == ("uri\nproject/об%D1%80%D0%B0%D0%B7\n_\nimage:/")
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image:/user/%D0%BE%D0%B1"]
+            ["image", "size", "image:/project/%D0%BE%D0%B1"]
         )
-        assert bash_out == ("uri,user/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,/")
-        assert zsh_out == ("uri\nuser/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage:/")
+        assert bash_out == ("uri,project/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,/")
+        assert zsh_out == ("uri\nproject/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage:/")
 
-        zsh_out, bash_out = run_autocomplete(["image", "size", "image://default/user/"])
+        zsh_out, bash_out = run_autocomplete(
+            ["image", "size", "image://default/project/"]
+        )
         assert bash_out == (
-            "uri,user/ima%3Fge,//default/\n"
-            "uri,user/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,//default/"
+            "uri,project/ima%3Fge,//default/\n"
+            "uri,project/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,//default/"
         )
         assert zsh_out == (
-            "uri\nuser/ima%3Fge\n_\nimage://default/\n"
-            "uri\nuser/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage://default/"
+            "uri\nproject/ima%3Fge\n_\nimage://default/\n"
+            "uri\nproject/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage://default/"
         )
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/im"]
+            ["image", "size", "image://default/project/im"]
         )
-        assert bash_out == ("uri,user/ima%3Fge,//default/")
-        assert zsh_out == ("uri\nuser/ima%3Fge\n_\nimage://default/")
+        assert bash_out == ("uri,project/ima%3Fge,//default/")
+        assert zsh_out == ("uri\nproject/ima%3Fge\n_\nimage://default/")
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/об"]
+            ["image", "size", "image://default/project/об"]
         )
-        assert bash_out == ("uri,user/об%D1%80%D0%B0%D0%B7,//default/")
-        assert zsh_out == ("uri\nuser/об%D1%80%D0%B0%D0%B7\n_\nimage://default/")
+        assert bash_out == ("uri,project/об%D1%80%D0%B0%D0%B7,//default/")
+        assert zsh_out == ("uri\nproject/об%D1%80%D0%B0%D0%B7\n_\nimage://default/")
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/%D0%BE%D0%B1"]
+            ["image", "size", "image://default/project/%D0%BE%D0%B1"]
         )
-        assert bash_out == ("uri,user/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,//default/")
+        assert bash_out == ("uri,project/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7,//default/")
         assert zsh_out == (
-            "uri\nuser/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage://default/"
+            "uri\nproject/%D0%BE%D0%B1%D1%80%D0%B0%D0%B7\n_\nimage://default/"
         )
 
 
 @skip_on_windows
 def test_image_tag_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Images, "list") as mocked_list, mock.patch.object(
         Images, "tags"
     ) as mocked_tags:
         image = RemoteImage.new_neuro_image(
             name="library/bananas",
             registry="registry-dev.neu.ro",
-            owner="other-user",
             cluster_name="default",
             org_name=None,
+            project_name="other-project",
         )
 
         async def list(cluster_name: str) -> List[RemoteImage]:
             return [image]
 
         async def tags(image: RemoteImage) -> List[RemoteImage]:
             return [
@@ -994,84 +1143,87 @@
         zsh_out, bash_out = run_autocomplete(
             ["image", "size", "image:library/bananas:b"]
         )
         assert bash_out == ("uri,beta,")
         assert zsh_out == ("uri\nbeta\n_\nimage:library/bananas:")
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image:/user/library/bananas:"]
+            ["image", "size", "image:/project/library/bananas:"]
         )
         assert bash_out == ("uri,alpha,\n" "uri,beta,\n" "uri,latest,")
         assert zsh_out == (
-            "uri\nalpha\n_\nimage:/user/library/bananas:\n"
-            "uri\nbeta\n_\nimage:/user/library/bananas:\n"
-            "uri\nlatest\n_\nimage:/user/library/bananas:"
+            "uri\nalpha\n_\nimage:/project/library/bananas:\n"
+            "uri\nbeta\n_\nimage:/project/library/bananas:\n"
+            "uri\nlatest\n_\nimage:/project/library/bananas:"
         )
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image:/user/library/bananas:b"]
+            ["image", "size", "image:/project/library/bananas:b"]
         )
         assert bash_out == ("uri,beta,")
-        assert zsh_out == ("uri\nbeta\n_\nimage:/user/library/bananas:")
+        assert zsh_out == ("uri\nbeta\n_\nimage:/project/library/bananas:")
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/library/bananas:"]
+            ["image", "size", "image://default/project/library/bananas:"]
         )
         assert bash_out == ("uri,alpha,\n" "uri,beta,\n" "uri,latest,")
         assert zsh_out == (
-            "uri\nalpha\n_\nimage://default/user/library/bananas:\n"
-            "uri\nbeta\n_\nimage://default/user/library/bananas:\n"
-            "uri\nlatest\n_\nimage://default/user/library/bananas:"
+            "uri\nalpha\n_\nimage://default/project/library/bananas:\n"
+            "uri\nbeta\n_\nimage://default/project/library/bananas:\n"
+            "uri\nlatest\n_\nimage://default/project/library/bananas:"
         )
 
         zsh_out, bash_out = run_autocomplete(
-            ["image", "size", "image://default/user/library/bananas:b"]
+            ["image", "size", "image://default/project/library/bananas:b"]
         )
         assert bash_out == ("uri,beta,")
-        assert zsh_out == ("uri\nbeta\n_\nimage://default/user/library/bananas:")
+        assert zsh_out == ("uri\nbeta\n_\nimage://default/project/library/bananas:")
 
 
 @skip_on_windows
 def test_disk_autocomplete(run_autocomplete: _RunAC) -> None:
     with mock.patch.object(Disks, "list") as mocked_list:
         created_at = datetime.now() - timedelta(days=1)
         last_usage = datetime.now()
         disks = {
             "default": [
                 Disk(
                     id="disk-123",
                     storage=500,
                     owner="user",
+                    project_name="test-project",
                     status=Disk.Status.READY,
                     cluster_name="default",
                     org_name=None,
                     created_at=created_at,
                     timeout_unused=None,
                     name=None,
                 ),
                 Disk(
                     id="disk-234",
                     storage=600,
                     owner="user",
                     status=Disk.Status.PENDING,
                     cluster_name="default",
                     org_name="test-org",
+                    project_name="another-project",
                     created_at=created_at,
                     last_usage=last_usage,
                     timeout_unused=timedelta(hours=1),
                     name="data-disk",
                 ),
             ],
             "other": [
                 Disk(
                     id="disk-345",
                     storage=600,
                     owner="user",
                     status=Disk.Status.PENDING,
                     cluster_name="other",
+                    project_name="test-project",
                     org_name="test-org",
                     created_at=created_at,
                     last_usage=last_usage,
                     timeout_unused=timedelta(hours=1),
                     name="data-disk2",
                 ),
             ],
@@ -1123,57 +1275,62 @@
                     name="test-bucket",
                     owner="user",
                     cluster_name="default",
                     created_at=created_at,
                     provider=Bucket.Provider.AWS,
                     imported=False,
                     org_name=None,
+                    project_name="test-project",
                 ),
                 Bucket(
                     id="bucket-2",
                     name="test-bucket-2",
                     owner="user",
                     cluster_name="default",
                     created_at=created_at,
                     provider=Bucket.Provider.AWS,
                     imported=False,
                     org_name=None,
+                    project_name="test-project",
                 ),
                 Bucket(
                     id="bucket-3",
                     name=None,
                     owner="user-2",
                     cluster_name="default",
                     created_at=created_at,
                     provider=Bucket.Provider.AWS,
                     imported=False,
                     org_name="test-org",
+                    project_name="test-project",
                 ),
                 Bucket(
                     id="bucket-4",
                     name=None,
                     owner="user",
                     cluster_name="default",
                     created_at=created_at,
                     provider=Bucket.Provider.AWS,
                     imported=False,
                     public=True,
                     org_name="test-org",
+                    project_name="test-project",
                 ),
             ],
             "other": [
                 Bucket(
                     id="bucket-5",
                     name="test-bucket-3",
                     owner="user",
                     cluster_name="other",
                     created_at=created_at,
                     provider=Bucket.Provider.AWS,
                     imported=False,
                     org_name=None,
+                    project_name="test-project",
                 ),
             ],
         }
 
         @asyncgeneratorcontextmanager
         async def list(cluster_name: Optional[str] = None) -> AsyncIterator[Bucket]:
             for bucket in buckets[cluster_name or "default"]:
@@ -1219,22 +1376,24 @@
         accounts = [
             ServiceAccount(
                 id="account-1",
                 name="test1",
                 role="test-role-1",
                 owner="user",
                 default_cluster="cluster1",
+                default_project="user",
                 created_at=created_at,
             ),
             ServiceAccount(
                 id="account-2",
                 name="test2",
                 role="test-role-2",
                 owner="user",
                 default_cluster="cluster2",
+                default_project="project",
                 created_at=created_at,
             ),
         ]
 
         @asyncgeneratorcontextmanager
         async def list() -> AsyncIterator[ServiceAccount]:
             for account in accounts:
```

### Comparing `neuro-cli-23.2.0/tests/unit/test_stats.py` & `neuro-cli-23.7.0/tests/unit/test_stats.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_storage.py` & `neuro-cli-23.7.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_storage_progress.py` & `neuro-cli-23.7.0/tests/unit/test_storage_progress.py`

 * *Files identical despite different names*

### Comparing `neuro-cli-23.2.0/tests/unit/test_utils.py` & `neuro-cli-23.7.0/tests/unit/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 _MakeClient = Callable[..., Client]
 
 
 def _job_entry(
     job_id: str,
     cluster_name: str = "default",
     owner: str = "user",
+    project_name: str = "project",
     org_name: Optional[str] = None,
 ) -> Dict[str, Any]:
     if org_name:
-        uri = f"job://{cluster_name}/{org_name}/{owner}/{job_id}"
+        uri = f"job://{cluster_name}/{org_name}/{project_name}/{job_id}"
     else:
-        uri = f"job://{cluster_name}/{owner}/{job_id}"
+        uri = f"job://{cluster_name}/{project_name}/{job_id}"
     return {
         "id": job_id,
         "owner": owner,
         "cluster_name": cluster_name,
         "org_name": org_name,
+        "project_name": project_name,
         "uri": uri,
         "status": "running",
         "history": {
             "status": "running",
             "reason": None,
             "description": None,
             "created_at": "2019-03-18T12:41:10.573468+00:00",
@@ -60,15 +62,15 @@
             "resources": {"cpu": 0.1, "memory": 2**30, "shm": True},
         },
         "ssh_auth_server": "ssh://nobody@ssh-auth-dev.neu.ro:22",
         "scheduler_enabled": True,
         "pass_config": False,
         "name": "my-job-name",
         "internal_hostname": f"{job_id}.{cluster_name}",
-        "internal_hostname_named": f"my-job-name--{owner}.{cluster_name}",
+        "internal_hostname_named": f"my-job-name--{project_name}.{cluster_name}",
         "total_price_credits": "150",
         "price_credits_per_hour": "15",
     }
 
 
 def _check_params(
     request: web.Request, **expected: Union[str, List[str], Set[str]]
@@ -91,15 +93,15 @@
     JSON: Dict[str, Any] = {"jobs": []}
     job_id = "job-81839be3-3ecf-4ec5-80d9-19b1588869db"
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_id,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -112,27 +114,27 @@
         resolved_ex = await resolve_job_ex(
             job_id, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_id, "default")
 
 
 @pytest.mark.parametrize("cluster_name", ["default", "other"])
-async def test_resolve_job_id__from_uri_with_owner_same_user__no_jobs_found(
+async def test_resolve_job_id__from_uri_with_same_project__no_jobs_found(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient, cluster_name: str
 ) -> None:
-    job_owner = "user"
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_project}/{job_name}"
     JSON: Dict[str, Any] = {"jobs": []}
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner=job_owner,
+            project_name=job_project,
             cluster_name=cluster_name,
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -144,27 +146,27 @@
         assert resolved == job_name
         resolved_ex = await resolve_job_ex(
             uri, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_name, cluster_name)
 
 
-async def test_resolve_job_id__from_uri_with_owner_other_user__no_jobs_found(
+async def test_resolve_job_id__from_uri_with_other_project__no_jobs_found(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    job_owner = "job-owner"
+    job_project = "other-test-project"
     job_name = "my-job-name"
-    uri = f"job://default/{job_owner}/{job_name}"
+    uri = f"job://default/{job_project}/{job_name}"
     JSON: Dict[str, Any] = {"jobs": []}
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner=job_owner,
+            project_name=job_project,
             cluster_name="default",
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -174,26 +176,26 @@
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(ValueError):
             await resolve_job(uri, client=client, status={JobStatus.RUNNING})
         with pytest.raises(ValueError):
             await resolve_job_ex(uri, client=client, status={JobStatus.RUNNING})
 
 
-async def test_resolve_job_id__from_uri_without_owner__no_jobs_found(
+async def test_resolve_job_id__from_uri_without_project__no_jobs_found(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     job_name = "my-job-name"
     uri = f"job:{job_name}"
     JSON: Dict[str, Any] = {"jobs": []}
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -210,21 +212,21 @@
 
 
 async def test_resolve_job_id__from_string__single_job_found(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     job_name = "test-job-name-555"
     job_id = "job-id-1"
-    JSON = {"jobs": [_job_entry(job_id, owner="user")]}
+    JSON = {"jobs": [_job_entry(job_id, project_name="test-project")]}
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -240,37 +242,35 @@
             job_name, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_id, "default")
 
 
 @pytest.mark.parametrize("cluster_name", ["default", "other"])
 @pytest.mark.parametrize("org_name", [None, "test-org"])
-@pytest.mark.parametrize(
-    "job_owner", ["job-owner", "user", "job-owner/service", "user/service"]
-)
-async def test_resolve_job_id__from_uri_with_owner__single_job_found(
+async def test_resolve_job_id__from_uri_with_same_project__single_job_found(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_name: str,
     org_name: Optional[str],
-    job_owner: str,
 ) -> None:
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_project}/{job_name}"
     job_id = "job-id-1"
-    JSON = {"jobs": [_job_entry(job_id, cluster_name=cluster_name, owner=job_owner)]}
+    JSON = {
+        "jobs": [
+            _job_entry(job_id, cluster_name=cluster_name, project_name=job_project)
+        ]
+    }
 
     async def handler(request: web.Request) -> web.Response:
-        expected_owners = (
-            [job_owner, "service"] if job_owner == "job-owner/service" else [job_owner]
-        )
         _check_params(
             request,
             name=job_name,
-            owner=expected_owners,
+            project_name=job_project,
             cluster_name=cluster_name,
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -284,46 +284,46 @@
             uri, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_id, cluster_name)
 
 
 @pytest.mark.parametrize("cluster_name", ["default", "other"])
 @pytest.mark.parametrize("org_name", [None, "test-org", "job-org"])
-@pytest.mark.parametrize(
-    "job_owner", ["job-owner", "user", "job-owner/service", "user/service"]
-)
 async def test_resolve_job_id__from_uri_with_org__single_job_found(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_name: str,
     org_name: Optional[str],
-    job_owner: str,
 ) -> None:
     job_org = "job-org"
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_org}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_org}/{job_project}/{job_name}"
     job_id = "job-id-1"
     JSON = {
         "jobs": [
             _job_entry(
-                job_id, cluster_name=cluster_name, owner=job_owner, org_name=job_org
+                job_id,
+                cluster_name=cluster_name,
+                org_name=job_org,
+                project_name=job_project,
             )
         ]
     }
 
     async def handler(request: web.Request) -> web.Response:
-        expected_owners = (
-            [f"{job_org}/{job_owner}", job_owner]
+        expected_projects = (
+            [f"{job_org}/{job_project}", job_project]
             if org_name != job_org
-            else [job_owner]
+            else [job_project]
         )
         _check_params(
             request,
             name=job_name,
-            owner=expected_owners,
+            project_name=expected_projects,
             cluster_name=cluster_name,
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -343,45 +343,48 @@
 @pytest.mark.parametrize("org_name", [None, "test-org"])
 async def test_resolve_job_id__from_uri__multiple_jobs_found(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_name: str,
     org_name: Optional[str],
 ) -> None:
-    job_org = f"job-owner"
-    job_owner = f"job-owner"
+    job_org = "job-org"
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_project}/{job_name}"
     job_ids = [f"job-id-{i}" for i in range(4)]
     JSON = {
         "jobs": [
             _job_entry(
                 job_ids[0],
                 cluster_name=cluster_name,
-                owner=job_owner,
+                project_name=job_project,
                 org_name="other-org",
             ),
             _job_entry(
-                job_ids[1], cluster_name=cluster_name, owner=job_owner, org_name=job_org
+                job_ids[1],
+                cluster_name=cluster_name,
+                project_name=job_project,
+                org_name=job_org,
             ),
-            _job_entry(job_ids[2], cluster_name=cluster_name, owner=job_owner),
+            _job_entry(job_ids[2], cluster_name=cluster_name, project_name=job_project),
             _job_entry(
                 job_ids[3],
                 cluster_name=cluster_name,
-                owner=job_owner,
                 org_name="other-org",
+                project_name=job_project,
             ),
         ]
     }
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner=job_owner,
+            project_name=job_project,
             cluster_name=cluster_name,
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -401,45 +404,48 @@
 @pytest.mark.parametrize("org_name", [None, "test-org"])
 async def test_resolve_job_id__from_uri_with_org__multiple_jobs_found(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     cluster_name: str,
     org_name: Optional[str],
 ) -> None:
-    job_org = f"job-owner"
-    job_owner = f"job-owner"
+    job_org = "job-org"
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_org}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_org}/{job_project}/{job_name}"
     job_ids = [f"job-id-{i}" for i in range(4)]
     JSON = {
         "jobs": [
             _job_entry(
                 job_ids[0],
                 cluster_name=cluster_name,
-                owner=job_owner,
+                project_name=job_project,
                 org_name="other-org",
             ),
-            _job_entry(job_ids[1], cluster_name=cluster_name, owner=job_owner),
+            _job_entry(job_ids[1], cluster_name=cluster_name, project_name=job_project),
             _job_entry(
-                job_ids[2], cluster_name=cluster_name, owner=job_owner, org_name=job_org
+                job_ids[2],
+                cluster_name=cluster_name,
+                project_name=job_project,
+                org_name=job_org,
             ),
             _job_entry(
                 job_ids[3],
                 cluster_name=cluster_name,
-                owner=job_owner,
+                project_name=job_project,
                 org_name="other-org",
             ),
         ]
     }
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner=[f"{job_org}/{job_owner}", job_owner],
+            project_name=[f"{job_org}/{job_project}", job_project],
             cluster_name=cluster_name,
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -452,29 +458,31 @@
         resolved_ex = await resolve_job_ex(
             uri, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_ids[2], cluster_name)
 
 
 @pytest.mark.parametrize("org_name", [None, "test-org"])
-async def test_resolve_job_id__from_uri_without_owner__single_job_found(
+async def test_resolve_job_id__from_uri_without_project__single_job_found(
     aiohttp_server: _TestServerFactory,
     make_client: _MakeClient,
     org_name: Optional[str],
 ) -> None:
     job_name = "my-job-name"
     uri = f"job:{job_name}"
     job_id = "job-id-1"
-    JSON = {"jobs": [_job_entry(job_id, owner="user", org_name=org_name)]}
+    JSON = {
+        "jobs": [_job_entry(job_id, project_name="test-project", org_name=org_name)]
+    }
 
     async def handler(request: web.Request) -> web.Response:
         _check_params(
             request,
             name=job_name,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         return web.json_response(JSON)
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -496,15 +504,15 @@
     job_id = "job-81839be3-3ecf-4ec5-80d9-19b1588869db"
     job_name = job_id
 
     async def handler(request: web.Request) -> NoReturn:
         _check_params(
             request,
             name=job_name,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         raise web.HTTPError()
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -519,26 +527,26 @@
         resolved_ex = await resolve_job_ex(
             job_name, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_id, "default")
 
 
 @pytest.mark.parametrize("cluster_name", ["default", "other"])
-async def test_resolve_job_id__from_uri_with_owner_same_user__server_error(
+async def test_resolve_job_id__from_uri_with_same_project__server_error(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient, cluster_name: str
 ) -> None:
-    job_owner = "user"
+    job_project = "test-project"
     job_name = "my-job-name"
-    uri = f"job://{cluster_name}/{job_owner}/{job_name}"
+    uri = f"job://{cluster_name}/{job_project}/{job_name}"
 
     async def handler(request: web.Request) -> NoReturn:
         _check_params(
             request,
             name=job_name,
-            owner=job_owner,
+            project_name=job_project,
             cluster_name=cluster_name,
             reverse="1",
         )
         raise web.HTTPError()
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -550,26 +558,26 @@
         assert resolved == job_name
         resolved_ex = await resolve_job_ex(
             uri, client=client, status={JobStatus.RUNNING}
         )
         assert resolved_ex == (job_name, cluster_name)
 
 
-async def test_resolve_job_id__from_uri_with_owner_other_user__server_error(
+async def test_resolve_job_id__from_uri_with_other_project__server_error(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
-    job_owner = "job-owner"
+    job_project = "other-test-project"
     job_name = "my-job-name"
-    uri = f"job://default/{job_owner}/{job_name}"
+    uri = f"job://default/{job_project}/{job_name}"
 
     async def handler(request: web.Request) -> NoReturn:
         _check_params(
             request,
             name=job_name,
-            owner=job_owner,
+            project_name=job_project,
             cluster_name="default",
             reverse="1",
         )
         raise web.HTTPError()
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -579,25 +587,25 @@
     async with make_client(srv.make_url("/")) as client:
         with pytest.raises(ValueError):
             await resolve_job(uri, client=client, status={JobStatus.RUNNING})
         with pytest.raises(ValueError):
             await resolve_job_ex(uri, client=client, status={JobStatus.RUNNING})
 
 
-async def test_resolve_job_id__from_uri_without_owner__server_error(
+async def test_resolve_job_id__from_uri_without_project__server_error(
     aiohttp_server: _TestServerFactory, make_client: _MakeClient
 ) -> None:
     job_name = "my-job-name"
     uri = f"job:{job_name}"
 
     async def handler(request: web.Request) -> NoReturn:
         _check_params(
             request,
             name=job_name,
-            owner="user",
+            project_name="test-project",
             cluster_name="default",
             reverse="1",
         )
         raise web.HTTPError()
 
     app = web.Application()
     app.router.add_get("/jobs", handler)
@@ -655,73 +663,80 @@
 def test_parse_file_resource_unsupported_scheme(root: Root) -> None:
     with pytest.raises(ValueError, match=r"Invalid scheme"):
         parse_file_resource("http://neu.ro", root)
     with pytest.raises(ValueError, match=r"Invalid scheme"):
         parse_file_resource("image:ubuntu", root)
 
 
-def test_parse_file_resource_user_less(root: Root) -> None:
+def test_parse_file_resource_project_less(root: Root) -> None:
     user_less_permission = parse_file_resource("storage:resource", root)
     assert user_less_permission == URL(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource"
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource"
     )
 
 
-def test_parse_file_resource_with_user(root: Root) -> None:
+def test_parse_file_resource_with_project(root: Root) -> None:
     full_permission = parse_file_resource(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource", root
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource",
+        root,
     )
     assert full_permission == URL(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource"
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource"
     )
     full_permission = parse_file_resource(f"storage://default/alice/resource", root)
     assert full_permission == URL(f"storage://default/alice/resource")
 
 
 def test_parse_file_resource_with_tilde(root: Root) -> None:
     with pytest.raises(ValueError, match=r"Cannot expand user for "):
         parse_file_resource(f"storage://~/resource", root)
 
 
 def test_parse_resource_for_sharing_image_no_tag(root: Root) -> None:
     uri = "image:ubuntu"
     parsed = parse_resource_for_sharing(uri, root)
     assert parsed == URL(
-        f"image://{root.client.cluster_name}/{root.client.username}/ubuntu"
+        f"image://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/ubuntu"
     )
 
 
 def test_parse_resource_for_sharing_image_non_ascii(root: Root) -> None:
     uri = "image:образ"
     parsed = parse_resource_for_sharing(uri, root)
     assert parsed == URL(
-        f"image://{root.client.cluster_name}/{root.client.username}/образ"
+        f"image://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/образ"
     )
-    assert parsed.path == f"/{root.client.username}/образ"
+    assert parsed.path == f"/{root.client.config.project_name}/образ"
 
 
 def test_parse_resource_for_sharing_image_percent_encoded(root: Root) -> None:
     uri = "image:%252d%3f%23"
     parsed = parse_resource_for_sharing(uri, root)
     assert parsed == URL(
-        f"image://{root.client.cluster_name}/{root.client.username}/%252d%3f%23"
+        f"image://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/%252d%3f%23"
     )
-    assert parsed.path == f"/{root.client.username}/%2d?#"
+    assert parsed.path == f"/{root.client.config.project_name}/%2d?#"
 
 
 def test_parse_resource_for_sharing_image_with_tag_fail(root: Root) -> None:
     uri = "image:ubuntu:latest"
     with pytest.raises(ValueError, match="tag is not allowed"):
         parse_resource_for_sharing(uri, root)
 
 
-def test_parse_resource_for_sharing_all_user_images(root: Root) -> None:
-    uri = "image:/otheruser"
+def test_parse_resource_for_sharing_all_project_images(root: Root) -> None:
+    uri = "image:/otherproject"
     parsed = parse_resource_for_sharing(uri, root)
-    assert parsed == URL(f"image://{root.client.cluster_name}/otheruser")
+    assert parsed == URL(f"image://{root.client.cluster_name}/otherproject")
 
 
 def _test_parse_resource_for_sharing_all_cluster_images(root: Root) -> None:
     uri = "image://"
     parsed = parse_resource_for_sharing(uri, root)
     assert parsed == URL(f"image://{root.client.cluster_name}/otheruser")
 
@@ -739,24 +754,28 @@
     with pytest.raises(ValueError, match=r"Invalid scheme"):
         parse_resource_for_sharing(r"c:scheme-less/resource", root)
 
 
 def test_parse_resource_for_sharing_user_less(root: Root) -> None:
     user_less_permission = parse_resource_for_sharing("storage:resource", root)
     assert user_less_permission == URL(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource"
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource"
     )
 
 
-def test_parse_resource_for_sharing_with_user(root: Root) -> None:
+def test_parse_resource_for_sharing_with_project(root: Root) -> None:
     full_permission = parse_resource_for_sharing(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource", root
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource",
+        root,
     )
     assert full_permission == URL(
-        f"storage://{root.client.cluster_name}/{root.client.username}/resource"
+        f"storage://{root.client.cluster_name}"
+        f"/{root.client.config.project_name}/resource"
     )
     full_permission = parse_resource_for_sharing(
         f"storage://default/alice/resource", root
     )
     assert full_permission == URL(f"storage://default/alice/resource")
```

