# Comparing `tmp/anylearn-0.17.7rc1.tar.gz` & `tmp/anylearn-0.18.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylearn-0.17.7rc1.tar", last modified: Thu Jun  8 10:32:24 2023, max compression
+gzip compressed data, was "anylearn-0.18.0rc1.tar", last modified: Thu Jul  6 03:38:15 2023, max compression
```

## Comparing `anylearn-0.17.7rc1.tar` & `anylearn-0.18.0rc1.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.777131 anylearn-0.17.7rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 10:32:24.777131 anylearn-0.17.7rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.749129 anylearn-0.17.7rc1/anylearn/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.749129 anylearn-0.17.7rc1/anylearn/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/analyzers/artifact_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/anylearnctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.753130 anylearn-0.17.7rc1/anylearn/applications/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/algorithm_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/dataset_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/git_progress_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22943 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/hpo_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    37837 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/quickstart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/train_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/applications/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.757130 anylearn-0.17.7rc1/anylearn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/add_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/add_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/anylearn_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/cli/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.757130 anylearn-0.17.7rc1/anylearn/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.757130 anylearn-0.17.7rc1/anylearn/interfaces/quota/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/quota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/quota/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.757130 anylearn-0.17.7rc1/anylearn/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/resource/resource_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.761130 anylearn-0.17.7rc1/anylearn/interfaces/service/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/service/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/service/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/train_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/interfaces/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.761130 anylearn-0.17.7rc1/anylearn/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.761130 anylearn-0.17.7rc1/anylearn/sdk/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/artifacts/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/sdk/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.761130 anylearn-0.17.7rc1/anylearn/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.765130 anylearn-0.17.7rc1/anylearn/storage/db/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.765130 anylearn-0.17.7rc1/anylearn/storage/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.765130 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.765130 anylearn-0.17.7rc1/anylearn/storage/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/storage/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.769131 anylearn-0.17.7rc1/anylearn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/anylearn/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.749129 anylearn-0.17.7rc1/anylearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 10:32:24.000000 anylearn-0.17.7rc1/anylearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:32:24.777131 anylearn-0.17.7rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.769131 anylearn-0.17.7rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.769131 anylearn-0.17.7rc1/tests/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/analyzers/test_artifact_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.769131 anylearn-0.17.7rc1/tests/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/applications/test_quick_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.773131 anylearn-0.17.7rc1/tests/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.773131 anylearn-0.17.7rc1/tests/interfaces/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_resource_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/resource/test_resource_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/test_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/test_train_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/interfaces/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:24.773131 anylearn-0.17.7rc1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:32:08.000000 anylearn-0.17.7rc1/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.012536 anylearn-0.18.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 03:38:15.012536 anylearn-0.18.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.976535 anylearn-0.18.0rc1/anylearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.976535 anylearn-0.18.0rc1/anylearn/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/analyzers/artifact_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/anylearnctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.980535 anylearn-0.18.0rc1/anylearn/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/algorithm_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/dataset_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/git_progress_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22943 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/hpo_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38251 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/train_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/applications/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.984535 anylearn-0.18.0rc1/anylearn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/add_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/add_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/anylearn_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.988535 anylearn-0.18.0rc1/anylearn/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.988535 anylearn-0.18.0rc1/anylearn/interfaces/quota/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/quota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/quota/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.992535 anylearn-0.18.0rc1/anylearn/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12843 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/resource/resource_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.992535 anylearn-0.18.0rc1/anylearn/interfaces/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/service/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25688 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/train_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/interfaces/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.992535 anylearn-0.18.0rc1/anylearn/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.996535 anylearn-0.18.0rc1/anylearn/sdk/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/artifacts/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/sdk/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.996535 anylearn-0.18.0rc1/anylearn/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.996535 anylearn-0.18.0rc1/anylearn/storage/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14765 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.000536 anylearn-0.18.0rc1/anylearn/storage/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.000536 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.000536 anylearn-0.18.0rc1/anylearn/storage/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/storage/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.004536 anylearn-0.18.0rc1/anylearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/anylearn/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:14.976535 anylearn-0.18.0rc1/anylearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 03:38:14.000000 anylearn-0.18.0rc1/anylearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:38:15.012536 anylearn-0.18.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.004536 anylearn-0.18.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.004536 anylearn-0.18.0rc1/tests/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/analyzers/test_artifact_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.008536 anylearn-0.18.0rc1/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/applications/test_quick_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.008536 anylearn-0.18.0rc1/tests/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.012536 anylearn-0.18.0rc1/tests/interfaces/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_resource_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/resource/test_resource_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/test_train_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/interfaces/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:15.012536 anylearn-0.18.0rc1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:38:06.000000 anylearn-0.18.0rc1/tests/utils/__init__.py
```

### Comparing `anylearn-0.17.7rc1/PKG-INFO` & `anylearn-0.18.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.17.7rc1
+Version: 0.18.0rc1
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.17.7rc1/README.md` & `anylearn-0.18.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/__init__.py` & `anylearn-0.18.0rc1/anylearn/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/analyzers/artifact_collector.py` & `anylearn-0.18.0rc1/anylearn/analyzers/artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/anylearnctl.py` & `anylearn-0.18.0rc1/anylearn/anylearnctl.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/algorithm_manager.py` & `anylearn-0.18.0rc1/anylearn/applications/algorithm_manager.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/dataset_manager.py` & `anylearn-0.18.0rc1/anylearn/applications/dataset_manager.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/git_progress_printer.py` & `anylearn-0.18.0rc1/anylearn/applications/git_progress_printer.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/hpo.py` & `anylearn-0.18.0rc1/anylearn/applications/hpo.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/hpo_experiment.py` & `anylearn-0.18.0rc1/anylearn/applications/hpo_experiment.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/quickstart.py` & `anylearn-0.18.0rc1/anylearn/applications/quickstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,14 +227,15 @@
 
 def _create_train_task(name: str,
                        algorithm: Algorithm,
                        project: Project,
                        hyperparams: dict,
                        hyperparams_prefix: str="--",
                        hyperparams_delimeter: str=" ",
+                       envs: Optional[Dict[str, str]]=None,
                        mounts: Optional[Union[Dict[str, List[Resource]], Dict[str, Resource]]]=None,
                        artifacts: Optional[List[Artifact]]=None,
                        algorithm_git_ref: Optional[str]=None,
                        resource_request: Optional[List[Dict[str, Dict[str, int]]]]=None,
                        description: Optional[str]=None,			
                        entrypoint: Optional[str]=None,
                        output: Optional[str]=None,
@@ -247,25 +248,27 @@
     for k, v in mounts.items():
         if isinstance(v, list):
             resource_ids.update([v_item.id for v_item in v])
             train_params[k] = [f"\"${v_item.id}\"" for v_item in v]
         else:
             resource_ids.add(v.id)
             train_params[k] = f"\"${v.id}\""
+    envs_json_str = json.dumps(envs) if envs else ""
     for artifact in artifacts:
         resource_ids.add(artifact.id)
     train_task = TrainTask(
         name=name,
         project_id=project.id,
         algorithm_id=algorithm.id,
         algorithm_git_ref=algorithm_git_ref,
         files=list(resource_ids),
         train_params=json.dumps(train_params),
         train_params_prefix=hyperparams_prefix,
         train_params_delimeter=hyperparams_delimeter,
+        envs=envs_json_str,
         resource_request=resource_request,
         description=description,
         num_nodes=num_nodes,
         nproc_per_node=nproc_per_node,
         mirror_id=get_mirror_by_name(mirror_name).id,
     )
     if entrypoint is not None:
@@ -323,14 +326,15 @@
 
 
 def run(
     algorithm_cloud_name: str,
     algorithm_entrypoint: str,
     algorithm_output: Optional[str]='./output/',
     algorithm_hyperparams: dict={},
+    algorithm_envs: Optional[Dict[str, str]]=None,
     dataset_cloud_names: Optional[List[str]]=None,
     model_cloud_names: Optional[List[str]]=None,
     project_name: Optional[str]=None,
     task_name: Optional[str]=None,
     image_name: Optional[str]="QUICKSTART",
     quota_group_request: Optional[Dict[str, int]]=None,
 ) -> Optional[TrainTask]:
@@ -372,14 +376,15 @@
 
 
 def upload_and_run(
     algorithm_cloud_name: str,
     algorithm_entrypoint: str,
     algorithm_output: Optional[str]='./output/',
     algorithm_hyperparams: dict={},
+    algorithm_envs: Optional[Dict[str, str]]=None,
     algorithm_local_dir: Optional[Union[str, Path]]='.',
     algorithm_force_update: bool=False,
     dataset_cloud_names: Optional[List[str]]=None,
     model_cloud_names: Optional[List[str]]=None,
     project_name: Optional[str]=None,
     task_name: Optional[str]=None,
     image_name: Optional[str]="QUICKSTART",
@@ -436,14 +441,15 @@
                 resource_polling: Union[float, int]=5,
                 hyperparams: dict={},
                 hyperparams_prefix: str="--",
                 hyperparams_delimeter: str=" ",
                 algorithm_hyperparams: dict={},
                 algorithm_hyperparams_prefix: str="--",
                 algorithm_hyperparams_delimeter: str=" ",
+                algorithm_envs: Optional[Dict[str, str]]=None,
                 resource_request: Optional[List[Dict[str, Dict[str, int]]]]=None,
                 quota_group_name: Optional[str]=None,
                 quota_group_request: Optional[Dict[str, int]]=None,
                 task_name: Optional[str]=None,
                 task_description: Optional[str]=None,
                 num_nodes: Optional[int]=1,
                 nproc_per_node: Optional[int]=1):
@@ -653,14 +659,16 @@
         如需要标识类参数（flag），可将参数的值设为空字符串，如 :obj:`{'my-flag': ''}` ，等价于 :obj:`--my-flag` 传入训练命令。
         默认为空字典。
     algorithm_hyperparams_prefix : :obj:`str`, optional
         训练超参数键前标识，可支持hydra特殊命令行传参格式的诸如 :obj:`+key1` 、 :obj:`++key2` 、 空前置 :obj:`key3` 等需求，
         默认为 :obj:`--` 。
     algorithm_hyperparams_delimeter :obj:`str`, optional
         训练超参数键值间的分隔符，默认为空格 :obj:` ` 。
+    algorithm_envs : :obj:`dict`, optional
+        训练环境变量字典。
     resource_request : :obj:`List[Dict[str, Dict[str, int]]]`, optional
         训练所需计算资源的请求。
         如未填，则使用Anylearn后端的 :obj:`default` 资源组中的默认资源套餐。
         自0.17.0版本起，此参数被标记为废弃，将于0.18.0版本中移除。
         请使用 :obj:`quota_group_request` 作为替代。
         
         .. deprecated:: 0.17.0
@@ -891,14 +899,15 @@
         name=train_task_name,
         algorithm=algo,
         algorithm_git_ref=algorithm_git_ref or current_sha,
         project=project,
         hyperparams=_hyperparams,
         hyperparams_prefix=_hyperparams_prefix,
         hyperparams_delimeter=_hyperparams_delimeter,
+        envs=algorithm_envs,
         mounts=mounts,
         artifacts=artifacts,
         resource_request=resource_request,
         description=task_description,
         num_nodes=num_nodes,
         nproc_per_node=nproc_per_node,
         entrypoint=_entrypoint,
```

### Comparing `anylearn-0.17.7rc1/anylearn/applications/tracking.py` & `anylearn-0.18.0rc1/anylearn/applications/tracking.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/train_profile.py` & `anylearn-0.18.0rc1/anylearn/applications/train_profile.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/applications/utils.py` & `anylearn-0.18.0rc1/anylearn/applications/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/add_algorithm.py` & `anylearn-0.18.0rc1/anylearn/cli/add_algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/add_dataset.py` & `anylearn-0.18.0rc1/anylearn/cli/add_dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/anylearn_cli_config.py` & `anylearn-0.18.0rc1/anylearn/cli/anylearn_cli_config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/cli.py` & `anylearn-0.18.0rc1/anylearn/cli/cli.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/config.py` & `anylearn-0.18.0rc1/anylearn/cli/config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/download.py` & `anylearn-0.18.0rc1/anylearn/cli/download.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/push.py` & `anylearn-0.18.0rc1/anylearn/cli/push.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/quota.py` & `anylearn-0.18.0rc1/anylearn/cli/quota.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/rm.py` & `anylearn-0.18.0rc1/anylearn/cli/rm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/run.py` & `anylearn-0.18.0rc1/anylearn/cli/run.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/task.py` & `anylearn-0.18.0rc1/anylearn/cli/task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/utils.py` & `anylearn-0.18.0rc1/anylearn/cli/utils.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/cli/view.py` & `anylearn-0.18.0rc1/anylearn/cli/view.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/config.py` & `anylearn-0.18.0rc1/anylearn/config.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/env.py` & `anylearn-0.18.0rc1/anylearn/env.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/__init__.py` & `anylearn-0.18.0rc1/anylearn/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/base.py` & `anylearn-0.18.0rc1/anylearn/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/mirror.py` & `anylearn-0.18.0rc1/anylearn/interfaces/mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/project.py` & `anylearn-0.18.0rc1/anylearn/interfaces/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/quota/group.py` & `anylearn-0.18.0rc1/anylearn/interfaces/quota/group.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/algorithm.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/dataset.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/file.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/model.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/resource.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/resource_downloader.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/resource/resource_uploader.py` & `anylearn-0.18.0rc1/anylearn/interfaces/resource/resource_uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/service/record.py` & `anylearn-0.18.0rc1/anylearn/interfaces/service/record.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/service/service.py` & `anylearn-0.18.0rc1/anylearn/interfaces/service/service.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/train_task.py` & `anylearn-0.18.0rc1/anylearn/interfaces/train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/interfaces/user.py` & `anylearn-0.18.0rc1/anylearn/interfaces/user.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/__init__.py` & `anylearn-0.18.0rc1/anylearn/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/algorithm.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/artifact.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/compression.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/compression.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/dataset.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/file.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/artifacts/model.py` & `anylearn-0.18.0rc1/anylearn/sdk/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/project.py` & `anylearn-0.18.0rc1/anylearn/sdk/project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/sdk/task.py` & `anylearn-0.18.0rc1/anylearn/sdk/task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/db.py` & `anylearn-0.18.0rc1/anylearn/storage/db/db.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/alembic.ini` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/env.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/6dfd859f129e_add_train_hpo_id_hpo_final_metric.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/848203d98d73_recreate_resource_tables_for_checksum.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/c1ee06d84c12_create_local_train_profile_table.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/c22620b97e39_create_local_hpo_experiment_table.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py` & `anylearn-0.18.0rc1/anylearn/storage/db/migrations/versions/ed56a42729b7_alter_train_profile_datasetid_nullable.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/storage/db/models.py` & `anylearn-0.18.0rc1/anylearn/storage/db/models.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/utils/api.py` & `anylearn-0.18.0rc1/anylearn/utils/api.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/utils/errors.py` & `anylearn-0.18.0rc1/anylearn/utils/errors.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn/utils/func.py` & `anylearn-0.18.0rc1/anylearn/utils/func.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/anylearn.egg-info/PKG-INFO` & `anylearn-0.18.0rc1/anylearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylearn
-Version: 0.17.7rc1
+Version: 0.18.0rc1
 Summary: Anylearn Python SDK
 Author: Dmagine
 Author-email: anylearn@nelbds.org.cn
 License: Proprietary
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

### Comparing `anylearn-0.17.7rc1/anylearn.egg-info/SOURCES.txt` & `anylearn-0.18.0rc1/anylearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/setup.py` & `anylearn-0.18.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 
 import setuptools
 
 
-CLIENT_VERSION = "0.17.7rc1"
+CLIENT_VERSION = "0.18.0rc1"
 PACKAGE_NAME = "anylearn"
 
 try:
     with io.open("README.md", encoding="utf-8") as f:
         LONG_DESCRIPTION = f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = ""
```

### Comparing `anylearn-0.17.7rc1/tests/analyzers/test_artifact_collector.py` & `anylearn-0.18.0rc1/tests/analyzers/test_artifact_collector.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/applications/test_quick_train.py` & `anylearn-0.18.0rc1/tests/applications/test_quick_train.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/base_test_case.py` & `anylearn-0.18.0rc1/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_algorithm.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_dataset.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_dataset.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_file.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_file.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_model.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_model.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_resource.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_resource.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_resource_downloader.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_resource_downloader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/resource/test_resource_uploader.py` & `anylearn-0.18.0rc1/tests/interfaces/resource/test_resource_uploader.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/test_db.py` & `anylearn-0.18.0rc1/tests/interfaces/test_db.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/test_mirror.py` & `anylearn-0.18.0rc1/tests/interfaces/test_mirror.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/test_project.py` & `anylearn-0.18.0rc1/tests/interfaces/test_project.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/test_train_task.py` & `anylearn-0.18.0rc1/tests/interfaces/test_train_task.py`

 * *Files identical despite different names*

### Comparing `anylearn-0.17.7rc1/tests/interfaces/test_user.py` & `anylearn-0.18.0rc1/tests/interfaces/test_user.py`

 * *Files identical despite different names*

