# Comparing `tmp/fractal_client-1.3.0a3.tar.gz` & `tmp/fractal_client-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.0a3.tar", max compression
+gzip compressed data, was "fractal_client-1.3.1.tar", max compression
```

## Comparing `fractal_client-1.3.0a3.tar` & `fractal_client-1.3.1.tar`

### file list

```diff
@@ -1,106 +1,20 @@
--rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a3/LICENSE
--rw-r--r--   0        0        0     2492 2023-06-13 10:01:05.958774 fractal_client-1.3.0a3/README.md
--rw-r--r--   0        0        0       24 2023-06-13 10:01:20.162621 fractal_client-1.3.0a3/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a3/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a3/fractal/authclient.py
--rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a3/fractal/client.py
--rw-r--r--   0        0        0    12216 2023-06-12 14:05:40.809583 fractal_client-1.3.0a3/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a3/fractal/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a3/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_project.py
--rw-r--r--   0        0        0     6659 2023-06-13 10:01:05.958774 fractal_client-1.3.0a3/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_user.py
--rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a3/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a3/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a3/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a3/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
--rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
--rw-r--r--   0        0        0     4068 2023-06-12 13:01:03.378002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
--rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     2705 2023-06-12 13:01:03.386002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     3292 2023-06-12 13:01:03.390002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a3/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      415 2023-06-12 13:01:14.929878 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      606 2023-06-12 13:01:14.961878 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3382 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1241 2023-06-12 13:01:03.562000 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1241 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1164 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1763 2023-06-12 13:01:15.173875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2792 2023-06-12 13:01:15.173875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1335 2023-06-12 13:01:03.566000 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1335 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2671 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2911 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a3/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a3/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a3/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a3/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a3/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a3/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a3/fractal/interface.py
--rw-r--r--   0        0        0    23275 2023-06-13 10:01:03.054806 fractal_client-1.3.0a3/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a3/fractal/response.py
--rw-r--r--   0        0        0     1851 2023-06-13 10:01:20.162621 fractal_client-1.3.0a3/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 fractal_client-1.3.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-06-23 06:18:32.718024 fractal_client-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2492 2023-06-23 06:18:32.718024 fractal_client-1.3.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-06 08:56:49.429672 fractal_client-1.3.1/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/client.py
+-rw-r--r--   0        0        0    12348 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     7260 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_user.py
+-rw-r--r--   0        0        0    10027 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0     1285 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/interface.py
+-rw-r--r--   0        0        0    23932 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-06-23 06:18:32.722024 fractal_client-1.3.1/fractal/response.py
+-rw-r--r--   0        0        0     1850 2023-07-06 08:56:49.429672 fractal_client-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 fractal_client-1.3.1/PKG-INFO
```

### Comparing `fractal_client-1.3.0a3/LICENSE` & `fractal_client-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/README.md` & `fractal_client-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/authclient.py` & `fractal_client-1.3.1/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/client.py` & `fractal_client-1.3.1/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/__init__.py` & `fractal_client-1.3.1/fractal/cmd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,28 +160,32 @@
             "name",
             "command",
             "source",
             "input_type",
             "output_type",
             "version",
             "meta_file",
+            "args_schema",
+            "args_schema_version",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await post_task(client, batch=batch, **function_kwargs)
     elif subcmd == "edit":
         parameters = [
             "id",
             "name",
             "version",
             "new_name",
             "new_command",
             "new_input_type",
             "new_output_type",
             "new_version",
             "meta_file",
+            "new_args_schema",
+            "new_args_schema_version",
         ]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await patch_task(client, **function_kwargs)
     elif subcmd == "delete":
         parameters = ["id", "name", "version"]
         function_kwargs = get_kwargs(parameters, kwargs)
         iface = await delete_task(client, **function_kwargs)
```

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_aux_task_caching.py` & `fractal_client-1.3.1/fractal/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_dataset.py` & `fractal_client-1.3.1/fractal/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_job.py` & `fractal_client-1.3.1/fractal/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_project.py` & `fractal_client-1.3.1/fractal/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_task.py` & `fractal_client-1.3.1/fractal/cmd/_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,24 +106,32 @@
     client: AuthClient,
     *,
     name: str,
     command: str,
     source: str,
     input_type: str = "Any",
     output_type: str = "Any",
+    batch: bool = False,
     version: Optional[str] = None,
     meta_file: Optional[str] = None,
-    batch: bool = False,
+    args_schema: Optional[str] = None,
+    args_schema_version: Optional[str] = None,
 ) -> BaseInterface:
     optionals = {}
     if version:
         optionals["version"] = version
     if meta_file:
         with open(meta_file, "r") as f:
             optionals["meta"] = json.load(f)
+    if args_schema:
+        with open(args_schema, "r") as f:
+            optionals["args_schema"] = json.load(f)
+    if args_schema_version:
+        optionals["args_schema_version"] = args_schema_version
+
     payload = TaskCreate(
         name=name,
         command=command,
         source=source,
         input_type=input_type,
         output_type=output_type,
         **optionals,
@@ -145,14 +153,16 @@
     version: Optional[str] = None,
     new_name: Optional[str] = None,
     new_command: Optional[str] = None,
     new_input_type: Optional[str] = None,
     new_output_type: Optional[str] = None,
     new_version: Optional[str] = None,
     meta_file: Optional[str] = None,
+    new_args_schema: Optional[str] = None,
+    new_args_schema_version: Optional[str] = None,
 ) -> BaseInterface:
 
     if id:
         if version:
             logging.error(
                 "Too many arguments: cannot provide both `id` and `version`."
             )
@@ -176,14 +186,19 @@
     if new_command:
         update["command"] = new_command
     if new_version:
         update["version"] = new_version
     if meta_file:
         with open(meta_file, "r") as f:
             update["meta"] = json.load(f)
+    if new_args_schema:
+        with open(new_args_schema, "r") as f:
+            update["args_schema"] = json.load(f)
+    if new_args_schema_version:
+        update["args_schema_version"] = new_args_schema_version
 
     task_update = TaskUpdate(**update)
     payload = task_update.dict(exclude_unset=True)
     if not payload:
         return PrintInterface(retcode=1, data="Nothing to update")
 
     res = await client.patch(f"{settings.BASE_URL}/task/{id}", json=payload)
```

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_user.py` & `fractal_client-1.3.1/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/cmd/_workflow.py` & `fractal_client-1.3.1/fractal/cmd/_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -250,14 +250,15 @@
             f"apply/?{query_parameters}"
         ),
         json=apply_wf_create.dict(exclude_unset=True),
     )
     apply_wf_read = check_response(
         res, expected_status_code=202, coerce=ApplyWorkflowRead
     )
+
     return RichJsonInterface(retcode=0, data=apply_wf_read.sanitised_dict())
 
 
 async def workflow_import(
     client: AuthClient, *, project_id: int, json_file: str, batch: bool = False
 ) -> BaseInterface:
     with Path(json_file).open("r") as f:
@@ -266,14 +267,28 @@
     res = await client.post(
         f"{settings.BASE_URL}/project/{project_id}/workflow/import/",
         json=workflow.dict(exclude_unset=True),
     )
     wf_read = check_response(
         res, expected_status_code=201, coerce=WorkflowRead
     )
+
+    warnings = [
+        workflow_task.task.source
+        for workflow_task in wf_read.task_list
+        if workflow_task.task.owner
+    ]
+    if warnings:
+        sources_str = ", ".join([f"'{s}'" for s in warnings])
+        logging.warning(
+            "This workflow includes custom tasks (the ones with sources: "
+            f"{sources_str}), which are not meant to be portable; "
+            "importing this workflow may not work as expected."
+        )
+
     if batch:
         datastr = f"{wf_read.id}"
         for wftask in wf_read.task_list:
             datastr += f" {wftask.id}"
         return PrintInterface(retcode=0, data=datastr)
     else:
         return RichJsonInterface(retcode=0, data=wf_read.dict())
@@ -291,12 +306,28 @@
             f"{settings.BASE_URL}/project/{project_id}/"
             f"workflow/{workflow_id}/export/"
         ),
     )
     workflow = check_response(
         res, expected_status_code=200, coerce=WorkflowExport
     )
+
+    warnings = [
+        workflow_task.task.source
+        for workflow_task in workflow.task_list
+        if not workflow_task.task.source.startswith(
+            ("pip_local:", "pip_remote:")
+        )
+    ]
+    if warnings:
+        sources_str = ", ".join([f"'{s}'" for s in warnings])
+        logging.warning(
+            "This workflow includes custom tasks (the ones with sources: "
+            f"{sources_str}), which are not meant to be portable; "
+            "re-importing this workflow may not work as expected."
+        )
+
     with Path(json_file).open("w") as f:
         json.dump(workflow.dict(), f, indent=2)
     return PrintInterface(
         retcode=0, data=f"Workflow {workflow_id} exported at {json_file}"
     )
```

### Comparing `fractal_client-1.3.0a3/fractal/common/README.md` & `fractal_client-1.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,48 @@
-# Fractal Common
-
-[![CI Status](https://github.com/fractal-analytics-platform/fractal-common/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-common/actions/workflows/ci.yml)
+Metadata-Version: 2.1
+Name: fractal-client
+Version: 1.3.1
+Summary: Client component of the Fractal analytics platform
+Home-page: https://github.com/fractal-analytics-platform/fractal
+License: BSD-3-Clause
+Author: Tommaso Comparin
+Author-email: tommaso.comparin@exact-lab.it
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
+Requires-Dist: fastapi-users (>=10.4.1,<11.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: pydantic (>=1.10.8,<2)
+Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Description-Content-Type: text/markdown
+
+# Fractal Client
+
+[![PyPI version](https://img.shields.io/pypi/v/fractal-client?color=gree)](https://pypi.org/project/fractal-client/)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal/actions/workflows/ci.yml)
+[![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal/blob/python-coverage-comment-action-data/htmlcov/index.html)
+[![Documentation Status](https://github.com/fractal-analytics-platform/fractal/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 Fractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.
 
 ![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)
 
 Fractal provides distributed workflows that convert TBs of image data into OME-Zarr files. The platform then processes the 3D image data by applying tasks like illumination correction, maximum intensity projection, 3D segmentation using [cellpose](https://cellpose.readthedocs.io/en/latest/) and measurements using [napari workflows](https://github.com/haesleinhuepf/napari-workflows). The pyramidal OME-Zarr files enable interactive visualization in the napari viewer.
 
-This is the **common repository**, containing resources that are shared by the server and client components. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).
+This is the repository that contains the **Fractal client**. Find more information about Fractal in general and the other repositories at the [Fractal home page](https://fractal-analytics-platform.github.io).
+
+## Documentation
 
-**IMPORTANT: This repository must only be used as a git submodule.**
+See https://fractal-analytics-platform.github.io/fractal.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](https://exact-lab.it).
+
```

### Comparing `fractal_client-1.3.0a3/fractal/config.py` & `fractal_client-1.3.1/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/interface.py` & `fractal_client-1.3.1/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/fractal/parser.py` & `fractal_client-1.3.1/fractal/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,14 +366,27 @@
     help="Task version",
 )
 task_new_parser.add_argument(
     "--meta-file",
     help="Path to JSON file with additional parameters useful for execution",
     type=str,
 )
+task_new_parser.add_argument(
+    "--args-schema",
+    help="Path to file containing JSON Schema for task arguments",
+    type=str,
+)
+task_new_parser.add_argument(
+    "--args-schema-version",
+    help=(
+        "Label encoding how the task-arguments JSON Schema was generated "
+        "(e.g. `pydantic_v1`)."
+    ),
+    type=str,
+)
 
 # task edit
 task_edit_parser = task_subparsers.add_parser(
     "edit",
     description="Edit task",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
@@ -420,15 +433,26 @@
     ),
 )
 task_edit_parser.add_argument(
     "--new-version",
     type=str,
     help="New version",
 )
-
+task_edit_parser.add_argument(
+    "--new-args-schema",
+    help="Path to file containing the new JSON Schema for task arguments",
+    type=str,
+)
+task_edit_parser.add_argument(
+    "--new-args-schema-version",
+    help=(
+        "New label encoding how the task-arguments JSON Schema was generated."
+    ),
+    type=str,
+)
 
 # task delete
 task_delete_parser = task_subparsers.add_parser(
     "delete",
     description="Delete task",
     argument_default=ap.SUPPRESS,
     allow_abbrev=False,
```

### Comparing `fractal_client-1.3.0a3/fractal/response.py` & `fractal_client-1.3.1/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a3/pyproject.toml` & `fractal_client-1.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.0a3"
+version = "1.3.1"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -16,15 +16,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.20.0"
 rich = "^12.5.1"
 httpx = "^0.23.0"
 PyJWT = "^2.4.0"
-pydantic = ">=1.10.8"
+pydantic = ">=1.10.8,<2"
 fastapi-users = "^10.4.1"
 
 [tool.poetry.group.dev.dependencies]
 sqlmodel = "^0.0.8"
 devtools = "^0.9.0"
 pytest = "^7.1.2"
 bumpver = "^2022.1118"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.0a3"
+current_version = "1.3.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

