# Comparing `tmp/fractal_server-1.3.2a1.tar.gz` & `tmp/fractal_server-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.2a1.tar", max compression
+gzip compressed data, was "fractal_server-1.3.3.tar", max compression
```

## Comparing `fractal_server-1.3.2a1.tar` & `fractal_server-1.3.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1576 2023-06-23 06:18:06.498772 fractal_server-1.3.2a1/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-23 06:18:06.498772 fractal_server-1.3.2a1/README.md
--rw-r--r--   0        0        0       69 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-29 12:24:14.630163 fractal_server-1.3.2a1/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/__init__.py
--rw-r--r--   0        0        0     1242 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7622 2023-06-29 10:43:50.361229 fractal_server-1.3.2a1/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4990 2023-06-29 10:43:50.361229 fractal_server-1.3.2a1/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-06-27 14:30:25.873556 fractal_server-1.3.2a1/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0     5516 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    10831 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/api/v1/task_collection.py
--rw-r--r--   0        0        0     9246 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     5165 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/api/v1/workflowtask.py
--rw-r--r--   0        0        0     3081 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     2535 2023-06-29 11:35:58.311060 fractal_server-1.3.2a1/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5205 2023-06-29 10:31:41.253702 fractal_server-1.3.2a1/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0    10102 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19766 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42317 2023-06-29 10:43:50.365229 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-06-26 06:59:30.472776 fractal_server-1.3.2a1/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-06-26 06:59:32.128764 fractal_server-1.3.2a1/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       57 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-06-26 06:59:32.128764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-06-26 06:59:32.128764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-26 06:59:32.128764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     4082 2023-06-26 06:59:32.132763 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3551 2023-06-26 06:59:32.132763 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     1179 2023-06-26 06:59:32.140764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     2719 2023-06-26 06:59:32.140764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     3306 2023-06-26 06:59:32.144764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-06-26 06:59:32.148764 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     3896 2023-06-26 06:59:32.152763 fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-06-28 13:38:09.728212 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      620 2023-06-28 13:38:09.776211 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-06-28 13:38:09.800210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1255 2023-06-28 13:38:09.800210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1178 2023-06-28 13:38:09.800210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-06-28 13:38:09.804210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2806 2023-06-28 13:38:09.804210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1349 2023-06-28 13:38:09.808210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2685 2023-06-28 13:38:09.808210 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2925 2023-06-28 13:38:09.812209 fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-06-26 06:59:30.480776 fractal_server-1.3.2a1/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12432 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-06-27 14:30:25.873556 fractal_server-1.3.2a1/fractal_server/logger.py
--rw-r--r--   0        0        0     5935 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/main.py
--rw-r--r--   0        0        0       59 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/migrations/README
--rw-r--r--   0        0        0     2666 2023-06-29 12:21:21.012806 fractal_server-1.3.2a1/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-29 12:21:21.012806 fractal_server-1.3.2a1/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-06-29 12:21:21.012806 fractal_server-1.3.2a1/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-29 12:21:21.012806 fractal_server-1.3.2a1/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17583 2023-06-29 10:43:50.365229 fractal_server-1.3.2a1/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-06-23 06:18:06.502771 fractal_server-1.3.2a1/fractal_server/utils.py
--rw-r--r--   0        0        0     2704 2023-06-29 12:24:14.630163 fractal_server-1.3.2a1/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:06.498772 fractal_server-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-23 06:18:06.498772 fractal_server-1.3.3/README.md
+-rw-r--r--   0        0        0       69 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/.gitignore
+-rw-r--r--   0        0        0       22 2023-07-06 08:58:33.028530 fractal_server-1.3.3/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0     1242 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7622 2023-06-29 10:43:50.361229 fractal_server-1.3.3/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4990 2023-06-29 10:43:50.361229 fractal_server-1.3.3/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-06-27 14:30:25.873556 fractal_server-1.3.3/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0     5516 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    10831 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/task_collection.py
+-rw-r--r--   0        0        0     9246 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     5165 2023-06-29 10:31:41.253702 fractal_server-1.3.3/fractal_server/app/api/v1/workflowtask.py
+-rw-r--r--   0        0        0     3081 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     2535 2023-07-06 07:41:28.191331 fractal_server-1.3.3/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5207 2023-06-30 07:20:38.331243 fractal_server-1.3.3/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0    10102 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-07-06 08:55:51.562302 fractal_server-1.3.3/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42317 2023-06-29 10:43:50.365229 fractal_server-1.3.3/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-26 06:59:30.472776 fractal_server-1.3.3/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       57 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-26 06:59:32.128764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4082 2023-06-26 06:59:32.132763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3551 2023-06-26 06:59:32.132763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1179 2023-06-26 06:59:32.140764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-06-26 06:59:32.140764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3306 2023-06-26 06:59:32.144764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:32.148764 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3896 2023-06-26 06:59:32.152763 fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-06-28 13:38:09.728212 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      620 2023-06-28 13:38:09.776211 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1255 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1178 2023-06-28 13:38:09.800210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-06-28 13:38:09.804210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2806 2023-06-28 13:38:09.804210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1349 2023-06-28 13:38:09.808210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2685 2023-06-28 13:38:09.808210 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2925 2023-06-28 13:38:09.812209 fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-06-26 06:59:30.480776 fractal_server-1.3.3/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-06-27 14:30:25.873556 fractal_server-1.3.3/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-07-06 07:41:28.191331 fractal_server-1.3.3/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2666 2023-06-29 12:21:21.012806 fractal_server-1.3.3/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-29 13:31:45.976002 fractal_server-1.3.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-07-06 07:41:28.195330 fractal_server-1.3.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-29 13:31:45.976002 fractal_server-1.3.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17583 2023-06-29 10:43:50.365229 fractal_server-1.3.3/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-06-23 06:18:06.502771 fractal_server-1.3.3/fractal_server/utils.py
+-rw-r--r--   0        0        0     2703 2023-07-06 08:58:33.028530 fractal_server-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 fractal_server-1.3.3/PKG-INFO
```

### Comparing `fractal_server-1.3.2a1/LICENSE` & `fractal_server-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/README.md` & `fractal_server-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/__main__.py` & `fractal_server-1.3.3/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/alembic.ini` & `fractal_server-1.3.3/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/__init__.py` & `fractal_server-1.3.3/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/task_collection.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/api/v1/workflowtask.py` & `fractal_server-1.3.3/fractal_server/app/api/v1/workflowtask.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/db/__init__.py` & `fractal_server-1.3.3/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/job.py` & `fractal_server-1.3.3/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/project.py` & `fractal_server-1.3.3/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/security.py` & `fractal_server-1.3.3/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/state.py` & `fractal_server-1.3.3/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/task.py` & `fractal_server-1.3.3/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/models/workflow.py` & `fractal_server-1.3.3/fractal_server/app/models/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         if args is not None:
             for k, v in args.items():
                 actual_args[k] = v
         if not actual_args:
             actual_args = None
 
         # Combine meta (higher priority) and db_task.meta (lower priority)
-        wt_meta = db_task.meta.copy() or {}
+        wt_meta = (db_task.meta or {}).copy()
         wt_meta.update(meta or {})
         if not wt_meta:
             wt_meta = None
 
         # Create DB entry
         wf_task = WorkflowTask(task_id=task_id, args=actual_args, meta=wt_meta)
         db.add(wf_task)
```

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.3/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_common.py` & `fractal_server-1.3.3/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.3/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.3/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.3/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.3/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.3/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/runner/common.py` & `fractal_server-1.3.3/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/app/security/__init__.py` & `fractal_server-1.3.3/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.3/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.3/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/README.md` & `fractal_server-1.3.3/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.3/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.3/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.3/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.3/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/project.py` & `fractal_server-1.3.3/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/state.py` & `fractal_server-1.3.3/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/task.py` & `fractal_server-1.3.3/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.3/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/user.py` & `fractal_server-1.3.3/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.3/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.3/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/config.py` & `fractal_server-1.3.3/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/logger.py` & `fractal_server-1.3.3/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/main.py` & `fractal_server-1.3.3/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/migrations/env.py` & `fractal_server-1.3.3/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.3/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/syringe.py` & `fractal_server-1.3.3/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/tasks/collection.py` & `fractal_server-1.3.3/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/fractal_server/utils.py` & `fractal_server-1.3.3/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.2a1/pyproject.toml` & `fractal_server-1.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.2a1"
+version = "1.3.3"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -20,15 +20,15 @@
 aiosqlite = "^0.17.0"
 fastapi-users = {extras = ["oauth"], version = "^10.1"}
 alembic = "^1.9.1"
 uvicorn = "^0.20.0"
 sqlalchemy = "^1.4"
 SQLAlchemy-Utils = "^0.38.3"
 greenlet = "*"
-pydantic = ">=1.10.8"
+pydantic = ">=1.10.8,<2"
 
 clusterfutures = { version = "^0.5", optional = true}
 cloudpickle = {version = ">=2.2.1 <2.3.0", optional = true}
 
 asyncpg = { version = "^0.27.0", optional = true }
 psycopg2 = { version = "^2.9.5", optional = true }
 gunicorn = { version = "^20.1.0", optional = true }
@@ -73,15 +73,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.2a1"
+current_version = "1.3.3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.2a1/PKG-INFO` & `fractal_server-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.2a1
+Version: 1.3.3
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -22,15 +22,15 @@
 Requires-Dist: cloudpickle (>=2.2.1,<2.3.0) ; extra == "slurm"
 Requires-Dist: clusterfutures (>=0.5,<0.6) ; extra == "slurm"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: fastapi-users[oauth] (>=10.1,<11.0)
 Requires-Dist: greenlet
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
-Requires-Dist: pydantic (>=1.10.8)
+Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Fractal Server
```

