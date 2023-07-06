# Comparing `tmp/taskcluster-taskgraph-5.4.0.tar.gz` & `tmp/taskcluster-taskgraph-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcluster-taskgraph-5.4.0.tar", last modified: Tue Jun 13 13:57:11 2023, max compression
+gzip compressed data, was "dist/taskcluster-taskgraph-5.5.0.tar", last modified: Thu Jul  6 14:46:32 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.4.0.tar` & `taskcluster-taskgraph-5.5.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.762659 taskcluster-taskgraph-5.4.0/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    16725 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/LICENSE
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      175 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/MANIFEST.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      665 2023-06-13 13:57:11.758659 taskcluster-taskgraph-5.4.0/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3659 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/README.rst
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      602 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/pyproject.toml
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/requirements/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      177 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/base.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    20339 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/base.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       22 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/requirements/dev.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1281 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/requirements/dev.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       58 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/requirements/test.in
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9241 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/test.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       38 2023-06-13 13:57:11.762659 taskcluster-taskgraph-5.4.0/setup.cfg
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1555 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/setup.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.734659 taskcluster-taskgraph-5.4.0/src/
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      665 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3977 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       50 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      201 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)       10 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/src/taskgraph/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      729 2023-06-13 09:06:43.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      416 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1836 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1309 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1941 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1086 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13113 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9387 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10661 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/util.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4611 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/config.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5184 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/create.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12882 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7834 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2793 2022-08-29 09:00:10.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/files_changed.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      866 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15541 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/generator.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4680 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/graph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1185 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/default.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2147 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    26201 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/main.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9192 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/morph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      123 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18341 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2380 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11906 2022-11-08 15:09:41.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    29990 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)      896 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    30243 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    44960 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3324 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3240 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2434 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.746659 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      110 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5146 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2607 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      707 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7606 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10479 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6647 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/from_deps.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.746659 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    17271 2022-12-19 12:50:27.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6826 2022-10-13 13:09:44.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1220 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9814 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6015 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6019 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/notify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    51279 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.750659 taskcluster-taskgraph-5.4.0/src/taskgraph/util/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2855 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/archive.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2964 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3406 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2433 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2502 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11690 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1661 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/hash.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3419 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1331 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3184 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4466 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1576 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      787 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8323 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/schema.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1317 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/shell.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12445 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1969 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1417 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/templates.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3390 2022-08-26 12:55:10.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/time.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2687 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18534 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8947 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/verify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2498 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1029 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.758659 taskcluster-taskgraph-5.4.0/test/
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1584 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1670 2022-09-07 16:01:21.000000 taskcluster-taskgraph-5.4.0/test/test_actions_registry.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3654 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_create.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7688 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_decision.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3505 2022-08-29 09:00:10.000000 taskcluster-taskgraph-5.4.0/test/test_files_changed.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7588 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_generator.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7063 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_graph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7940 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_main.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2701 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_morph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15584 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_optimize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1727 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_optimize_strategies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13921 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_parameters.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2491 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12257 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_scripts_run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12046 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_target_tasks.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3759 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_taskgraph.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1812 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transform_docker_image.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      874 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_base.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1527 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_fetch.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5880 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_from_deps.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5181 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6291 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job_run_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7131 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job_toolchain.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6948 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_notify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    23573 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_task.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3596 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_attributes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1120 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/test/test_util_dependencies.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10212 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_docker.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2340 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_memoize.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7556 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_parameterization.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5906 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1045 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_python_path.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1234 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_readonlydict.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6961 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_schema.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10115 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     1677 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_templates.py
--rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     2239 2022-09-07 16:01:29.000000 taskcluster-taskgraph-5.4.0/test/test_util_time.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      913 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_treeherder.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)    14739 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_util_vcs.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4981 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_util_verify.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)      942 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_workertypes.py
--rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1591 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/LICENSE
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/MANIFEST.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/README.rst
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.5.0/pyproject.toml
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/requirements/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      177 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/requirements/base.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    20339 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/requirements/base.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/requirements/dev.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.5.0/requirements/dev.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.5.0/requirements/test.in
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9241 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/requirements/test.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/setup.cfg
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/setup.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      201 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-07-06 14:45:57.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1836 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9387 2023-06-12 19:54:30.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4611 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/config.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15541 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4680 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/graph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/loader/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/morph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    30813 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)    45018 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3240 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2434 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5146 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10479 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5897 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     9814 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    51678 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2592 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    18780 2023-07-06 14:16:59.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     8947 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2498 2023-06-21 19:54:32.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-07-06 14:46:32.000000 taskcluster-taskgraph-5.5.0/test/
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.5.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_actions_registry.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.5.0/test/test_create.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_decision.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_files_changed.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_generator.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_graph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.5.0/test/test_main.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_morph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.5.0/test/test_optimize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_optimize_strategies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_parameters.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.5.0/test/test_scripts_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_target_tasks.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_taskgraph.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_transform_docker_image.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_base.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_fetch.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6985 2023-07-06 14:31:47.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_job.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_notify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.5.0/test/test_transforms_task.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_attributes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.5.0/test/test_util_dependencies.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_docker.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_memoize.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_util_parameterization.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.5.0/test/test_util_python_path.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_readonlydict.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_schema.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_templates.py
+-rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_time.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_treeherder.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)    15598 2023-07-06 14:10:15.000000 taskcluster-taskgraph-5.5.0/test/test_util_vcs.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.5.0/test/test_util_verify.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_util_workertypes.py
+-rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.5.0/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `taskcluster-taskgraph-5.4.0/LICENSE` & `taskcluster-taskgraph-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/PKG-INFO` & `taskcluster-taskgraph-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.4.0
+Version: 5.5.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.4.0/README.rst` & `taskcluster-taskgraph-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/pyproject.toml` & `taskcluster-taskgraph-5.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/requirements/base.txt` & `taskcluster-taskgraph-5.5.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/requirements/dev.txt` & `taskcluster-taskgraph-5.5.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/requirements/test.txt` & `taskcluster-taskgraph-5.5.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/setup.py` & `taskcluster-taskgraph-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.4.0
+Version: 5.5.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.5.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.4.0"
+__version__ = "5.5.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/retrigger.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/config.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/create.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/main.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     util,
     vfs,
 )
 
 # Causes worker to purge caches on process exit and for task to retry.
 EXIT_PURGE_CACHE = 72
 
-testedwith = b"4.5 4.6 4.7 4.8 4.9 5.0 5.1 5.2 5.3 5.4 5.5 5.6 5.7 5.8 5.9"
+testedwith = (
+    b"4.5 4.6 4.7 4.8 4.9 5.0 5.1 5.2 5.3 5.4 5.5 5.6 5.7 5.8 5.9 6.0 6.1 6.2 6.3 6.4"
+)
 minimumhgversion = b"4.5"
 
 cmdtable = {}
 command = registrar.command(cmdtable)
 
 configtable = {}
 configitem = registrar.configitem(configtable)
@@ -492,14 +494,18 @@
         elif isinstance(e, ssl.SSLError):
             # Assume all SSL errors are due to the network, as Mercurial
             # should convert non-transport errors like cert validation failures
             # to error.Abort.
             ui.warn(b"ssl error: %s\n" % pycompat.bytestr(str(e)))
             handlenetworkfailure()
             return True
+        elif isinstance(e, urllibcompat.urlerr.httperror) and e.code >= 500:
+            ui.warn(b"http error: %s\n" % pycompat.bytestr(str(e.reason)))
+            handlenetworkfailure()
+            return True
         elif isinstance(e, urllibcompat.urlerr.urlerror):
             if isinstance(e.reason, socket.error):
                 ui.warn(b"socket error: %s\n" % pycompat.bytestr(str(e.reason)))
                 handlenetworkfailure()
                 return True
             else:
                 ui.warn(
@@ -802,15 +808,22 @@
             else:
                 ui.write(b"(setting sparse config to profile %s)\n" % sparse_profile)
 
             # If doing an incremental update, this will perform two updates:
             # one to change the sparse profile and another to update to the new
             # revision. This is not desired. But there's not a good API in
             # Mercurial to do this as one operation.
-            with repo.wlock(), repo.dirstate.parentchange(), timeit(
+            # TRACKING hg64 - Mercurial 6.4 and later require call to
+            # dirstate.changing_parents(repo)
+            def parentchange(repo):
+                if util.safehasattr(repo.dirstate, "changing_parents"):
+                    return repo.dirstate.changing_parents(repo)
+                return repo.dirstate.parentchange()
+
+            with repo.wlock(), parentchange(repo), timeit(
                 "sparse_update_config", "sparse-update-config"
             ):
                 # pylint --py3k: W1636
                 fcounts = list(
                     map(
                         len,
                         sparsemod._updateconfigandrefreshwdir(
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.5.0/src/taskgraph/run-task/run-task`

 * *Files 1% similar despite different names*

```diff
@@ -10,41 +10,38 @@
 
 It performs actions as requested from the arguments. Then it executes
 the requested process and prints its output, prefixing it with the
 current time to improve log usefulness.
 """
 
 import sys
-from typing import Optional
 
 if sys.version_info[0:2] < (3, 5):
     print("run-task requires Python 3.5+")
     sys.exit(1)
 
-
 import argparse
 import datetime
 import errno
 import io
 import json
 import os
-from pathlib import Path
 import platform
 import re
 import shutil
 import signal
 import socket
 import stat
 import subprocess
 import time
-
 import urllib.error
 import urllib.request
-
+from pathlib import Path
 from threading import Thread
+from typing import Optional
 
 SECRET_BASEURL_TPL = "http://taskcluster/secrets/v1/secret/{}"
 
 GITHUB_SSH_FINGERPRINT = (
     b"github.com ssh-rsa "
     b"AAAAB3NzaC1yc2EAAAADAQABAAABgQCj7ndNxQowgcQnjshcLrqPEiiphnt+VTTvDP6mHBL9j1aNUkY"
     b"4Ue1gvwnGLVlOhGeYrnZaMgRK6+PKCUXaDbC7qtbW8gIkhL7aGCsOr/C56SJMy/BCZfxd1nWzAOxSDP"
@@ -707,14 +704,15 @@
 
         run_required_command(b"vcs", args, cwd=destination_path)
 
         args = [
             "git",
             "submodule",
             "update",
+            "--force",  # Overrides any potential local changes
         ]
 
         run_required_command(b"vcs", args, cwd=destination_path)
 
     _clean_git_checkout(destination_path)
 
     args = ["git", "rev-parse", "--verify", "HEAD"]
@@ -922,15 +920,14 @@
         "repo-type": repo_type,
         "ssh-secret-name": private_key_secret,
         "pip-requirements": pip_requirements,
     }
 
 
 def vcs_checkout_from_args(options):
-
     if not options["checkout"]:
         if options["ref"] and not options["revision"]:
             print("task should be defined in terms of non-symbolic revision")
             sys.exit(1)
         return
 
     revision = options["revision"]
@@ -1068,18 +1065,18 @@
                 break
             print_line(prefix, data)
 
     monitor_process = Thread(target=capture_output)
     monitor_process.start()
     return process
 
+
 def _display_python_version():
     print_line(
-        b"setup",
-        b"Python version: "+ bytes(platform.python_version(), 'utf-8')
+        b"setup", b"Python version: %s\n" % platform.python_version().encode("utf-8")
     )
 
 
 def main(args):
     os.environ["TASK_WORKDIR"] = os.getcwd()
     print_line(
         b"setup",
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/task.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,39 +56,14 @@
         )
 
     else:
         # Caches not implemented
         pass
 
 
-def docker_worker_add_workspace_cache(config, job, taskdesc, extra=None):
-    """Add the workspace cache.
-
-    Args:
-        config (TransformConfig): Transform configuration object.
-        job (dict): Task's job description.
-        taskdesc (dict): Target task description to modify.
-        extra (str): Optional context passed in that supports extending the cache
-            key name to avoid undesired conflicts with other caches.
-    """
-    cache_name = "{}-build-{}-{}-workspace".format(
-        config.params["project"],
-        taskdesc["attributes"]["build_platform"],
-        taskdesc["attributes"]["build_type"],
-    )
-    if extra:
-        cache_name = f"{cache_name}-{extra}"
-
-    mount_point = "{workdir}/workspace".format(**job["run"])
-
-    # Don't enable the workspace cache when we can't guarantee its
-    # behavior, like on Try.
-    add_cache(job, taskdesc, cache_name, mount_point, skip_untrusted=True)
-
-
 def add_artifacts(config, job, taskdesc, path):
     taskdesc["worker"].setdefault("artifacts", []).append(
         {
             "name": get_artifact_prefix(taskdesc),
             "path": path,
             "type": "directory",
         }
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/transforms/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -613,14 +613,19 @@
                 Optional("format"): Any("rar", "tar.bz2", "tar.gz", "zip"),
             }
         ],
         # environment variables
         Required("env"): {str: taskref_or_string},
         # the maximum time to run, in seconds
         Required("max-run-time"): int,
+        # the exit status code(s) that indicates the task should be retried
+        Optional("retry-exit-status"): [int],
+        # the exit status code(s) that indicates the caches used by the task
+        # should be purged
+        Optional("purge-caches-exit-status"): [int],
         # os user groups for test task workers
         Optional("os-groups"): [str],
         # feature for test task to run as administarotr
         Optional("run-as-administrator"): bool,
         # optional features
         Required("chain-of-trust"): bool,
         Optional("taskcluster-proxy"): bool,
@@ -635,14 +640,16 @@
         "command": worker["command"],
         "maxRunTime": worker["max-run-time"],
     }
 
     on_exit_status = {}
     if "retry-exit-status" in worker:
         on_exit_status["retry"] = worker["retry-exit-status"]
+    if "purge-caches-exit-status" in worker:
+        on_exit_status["purgeCaches"] = worker["purge-caches-exit-status"]
     if worker["os"] == "windows":
         on_exit_status.setdefault("retry", []).extend(
             [
                 # These codes (on windows) indicate a process interruption,
                 # rather than a task run failure. See bug 1544403.
                 1073807364,  # process force-killed due to system shutdown
                 3221225786,  # sigint (any interrupt)
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
 @group_by("single")
 def group_by_single(config, tasks):
     for task in tasks:
         yield [task]
 
 
+@group_by("all")
+def group_by_all(config, tasks):
+    return [[task for task in tasks]]
+
+
 @group_by("attribute", schema=Schema(str))
 def group_by_attribute(config, tasks, attr):
     groups = {}
     for task in tasks:
         val = task.attributes.get(attr)
         if not val:
             continue
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,18 @@
     @abstractmethod
     def update(self, ref):
         """Update the working directory to the specified reference."""
 
     @abstractmethod
     def find_latest_common_revision(self, base_ref_or_rev, head_rev):
         """Find the latest revision that is common to both the given
-        ``head_rev`` and ``base_ref_or_rev``"""
+        ``head_rev`` and ``base_ref_or_rev``.
+
+        If no common revision exists, ``Repository.NULL_REVISION`` will
+        be returned."""
 
     @abstractmethod
     def does_revision_exist_locally(self, revision):
         """Check whether this revision exists in the local repository.
 
         If this function returns an unexpected value, then make sure
         the revision was fetched from the remote repository."""
@@ -292,21 +295,22 @@
         # means we are clean.
         return not len(self.run(*args).strip())
 
     def update(self, ref):
         return self.run("update", "--check", ref)
 
     def find_latest_common_revision(self, base_ref_or_rev, head_rev):
-        return self.run(
+        ancestor = self.run(
             "log",
             "-r",
             f"last(ancestors('{base_ref_or_rev}') and ancestors('{head_rev}'))",
             "--template",
             "{node}",
         ).strip()
+        return ancestor or self.NULL_REVISION
 
     def does_revision_exist_locally(self, revision):
         try:
             return bool(self.run("log", "-r", revision).strip())
         except subprocess.CalledProcessError as e:
             # Error code 255 comes with the message:
             # "abort: unknown revision $REVISION"
@@ -478,15 +482,18 @@
         # means we are clean.
         return not len(self.run(*args).strip())
 
     def update(self, ref):
         self.run("checkout", ref)
 
     def find_latest_common_revision(self, base_ref_or_rev, head_rev):
-        return self.run("merge-base", base_ref_or_rev, head_rev).strip()
+        try:
+            return self.run("merge-base", base_ref_or_rev, head_rev).strip()
+        except subprocess.CalledProcessError:
+            return self.NULL_REVISION
 
     def does_revision_exist_locally(self, revision):
         try:
             return self.run("cat-file", "-t", revision).strip() == "commit"
         except subprocess.CalledProcessError as e:
             # Error code 128 comes with the message:
             # "git cat-file: could not get object info"
```

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.5.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.5.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_actions_registry.py` & `taskcluster-taskgraph-5.5.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_create.py` & `taskcluster-taskgraph-5.5.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_decision.py` & `taskcluster-taskgraph-5.5.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_files_changed.py` & `taskcluster-taskgraph-5.5.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_generator.py` & `taskcluster-taskgraph-5.5.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_graph.py` & `taskcluster-taskgraph-5.5.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_main.py` & `taskcluster-taskgraph-5.5.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_morph.py` & `taskcluster-taskgraph-5.5.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_optimize.py` & `taskcluster-taskgraph-5.5.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.5.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_parameters.py` & `taskcluster-taskgraph-5.5.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.5.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.5.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_target_tasks.py` & `taskcluster-taskgraph-5.5.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_taskgraph.py` & `taskcluster-taskgraph-5.5.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.5.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_base.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_from_deps.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,26 @@
     assert task["attributes"] == {
         "build-type": "win",
         "kind": "foo",
         "primary-kind-dependency": "foo",
     }
 
 
+def assert_group_by_all(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 1
+    assert tasks[0]["dependencies"] == {"foo": "a", "bar": "bar-b"}
+
+
+def assert_group_by_all_dupe_allowed(tasks):
+    handle_exception(tasks)
+    assert len(tasks) == 1
+    assert tasks[0]["dependencies"] == {"a": "a", "b": "b", "c": "c"}
+
+
 @pytest.mark.parametrize(
     "task, kind_config, deps",
     (
         pytest.param(
             # task
             {"from-deps": {}},
             # kind config
@@ -174,14 +186,45 @@
                 ),
                 "b": make_task(
                     "b", attributes={"build-type": "win", "kind": "foo"}, kind="foo"
                 ),
             },
             id="copy_attributes",
         ),
+        pytest.param(
+            # task
+            {
+                "from-deps": {
+                    "group-by": "all",
+                }
+            },
+            # kind config
+            None,
+            # deps
+            None,
+            id="group_by_all",
+        ),
+        pytest.param(
+            # task
+            {
+                "from-deps": {
+                    "unique-kinds": False,
+                    "group-by": "all",
+                }
+            },
+            # kind config
+            None,
+            # deps
+            {
+                "a": make_task("a", kind="foo"),
+                "b": make_task("b", kind="foo"),
+                "c": make_task("c", kind="foo"),
+            },
+            id="group_by_all_dupe_allowed",
+        ),
     ),
 )
 def test_transforms(
     request, make_transform_config, run_transform, task, kind_config, deps
 ):
     task.setdefault("name", "task")
     task.setdefault("description", "description")
```

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_job.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_transforms_task.py` & `taskcluster-taskgraph-5.5.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_attributes.py` & `taskcluster-taskgraph-5.5.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-5.5.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_docker.py` & `taskcluster-taskgraph-5.5.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_memoize.py` & `taskcluster-taskgraph-5.5.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.5.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_path.py` & `taskcluster-taskgraph-5.5.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_python_path.py` & `taskcluster-taskgraph-5.5.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.5.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_schema.py` & `taskcluster-taskgraph-5.5.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.5.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_templates.py` & `taskcluster-taskgraph-5.5.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_time.py` & `taskcluster-taskgraph-5.5.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.5.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_vcs.py` & `taskcluster-taskgraph-5.5.0/test/test_util_vcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,23 +417,47 @@
 
     if repo.tool == "git":
         base_ref = f"{remote_name}/{repo.branch}"
         assert (
             repo.find_latest_common_revision(base_ref, repo.head_rev)
             == expected_latest_common_revision
         )
-    else:
+
+        # Test no common ancestors
+        repo.run("checkout", "--orphan", "new_branch")
+        repo.run("add", ".")
+        repo.run("commit", "-m", "Add another new revision")
+        base_ref = f"{remote_name}/{repo.branch}"
+        assert (
+            repo.find_latest_common_revision(base_ref, repo.head_rev)
+            == Repository.NULL_REVISION
+        )
+    elif repo.tool == "hg":
         # hg doesn't have the concept of remote branches
         assert (
             repo.find_latest_common_revision(
                 expected_latest_common_revision, repo.head_rev
             )
             == expected_latest_common_revision
         )
 
+        # Test no common ancestors
+        repo.run("update", Repository.NULL_REVISION)
+        with open(os.path.join(repo.path, "some_file"), "w") as f:
+            f.write("some content")
+
+        repo.run("add", ".")
+        repo.run("commit", "-m", "Add another new revision")
+        assert (
+            repo.find_latest_common_revision(
+                repo.head_rev, expected_latest_common_revision
+            )
+            == Repository.NULL_REVISION
+        )
+
 
 def test_does_revision_exist_locally(repo):
     first_revision = repo.head_rev
 
     with open(os.path.join(repo.path, "some_file"), "w") as f:
         f.write("some content")
```

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_verify.py` & `taskcluster-taskgraph-5.5.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.5.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.4.0/test/test_util_yaml.py` & `taskcluster-taskgraph-5.5.0/test/test_util_yaml.py`

 * *Files identical despite different names*

