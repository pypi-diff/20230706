# Comparing `tmp/bullmq-1.5.0.tar.gz` & `tmp/bullmq-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.5.0.tar", last modified: Tue Jul  4 17:28:42 2023, max compression
+gzip compressed data, was "bullmq-1.6.0.tar", last modified: Thu Jul  6 19:16:03 2023, max compression
```

## Comparing `bullmq-1.5.0.tar` & `bullmq-1.6.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.833291 bullmq-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 17:28:42.833291 bullmq-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 17:27:35.000000 bullmq-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.825291 bullmq-1.5.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-04 17:28:40.000000 bullmq-1.5.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.829291 bullmq-1.5.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-04 17:28:16.000000 bullmq-1.5.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.829291 bullmq-1.5.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-04 17:27:35.000000 bullmq-1.5.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:28:42.825291 bullmq-1.5.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 17:28:42.000000 bullmq-1.5.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-04 17:28:40.000000 bullmq-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:28:42.833291 bullmq-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-04 17:27:35.000000 bullmq-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.517049 bullmq-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 19:16:03.517049 bullmq-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 19:14:58.000000 bullmq-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.509049 bullmq-1.6.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-06 19:16:01.000000 bullmq-1.6.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.513049 bullmq-1.6.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 19:15:38.000000 bullmq-1.6.0/bullmq/commands/updateProgress-2.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.513049 bullmq-1.6.0/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.517049 bullmq-1.6.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-07-06 19:14:58.000000 bullmq-1.6.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:16:03.509049 bullmq-1.6.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 19:16:03.000000 bullmq-1.6.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-06 19:16:01.000000 bullmq-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:16:03.517049 bullmq-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-06 19:14:58.000000 bullmq-1.6.0/setup.py
```

### Comparing `bullmq-1.5.0/PKG-INFO` & `bullmq-1.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.5.0
+Version: 1.6.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.5.0/README.md` & `bullmq-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/backoffs.py` & `bullmq-1.6.0/bullmq/backoffs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         "exponential": lambda delay: lambda attempts_made, type, err, job: int(round(pow(2, attempts_made - 1) * delay))
     }    
 
     @staticmethod
     def normalize(backoff: int | BackoffOptions):
         if type(backoff) == int and math.isfinite(backoff):
             return {
-                "type": 'fixed',
+                "type": "fixed",
                 "delay": backoff
             }
         elif backoff:
             return backoff
 
     @staticmethod
     async def calculate(backoff: BackoffOptions, attempts_made: int, err, job, customStrategy):
```

### Comparing `bullmq-1.5.0/bullmq/commands/addJob-9.lua` & `bullmq-1.6.0/bullmq/commands/addJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.6.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.6.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.6.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/drain-4.lua` & `bullmq-1.6.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.6.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.6.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/getState-8.lua` & `bullmq-1.6.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.6.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.6.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.6.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.6.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.6.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.6.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.6.0/bullmq/commands/moveToFinished-13.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.6.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.6.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/pause-5.lua` & `bullmq-1.6.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/promote-7.lua` & `bullmq-1.6.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.6.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.6.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.6.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.6.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.6.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/event_emitter.py` & `bullmq-1.6.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/job.py` & `bullmq-1.6.0/bullmq/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from typing import List, Any, TYPE_CHECKING
 from bullmq.scripts import Scripts
 from bullmq.backoffs import Backoffs
 if TYPE_CHECKING:
     from bullmq.queue import Queue
 from bullmq.types import JobOptions
+from bullmq.utils import get_parent_key
 
 import json
 import time
 import traceback
 
 
 optsDecodeMap = {
@@ -30,28 +31,32 @@
     def __init__(self, queue: Queue, name: str, data: Any, opts: JobOptions = {}):
         self.name = name
         self.id = opts.get("jobId", None)
         self.progress = 0
         self.timestamp = opts.get("timestamp", round(time.time() * 1000))
         final_opts = {"attempts": 0, "delay": 0}
         final_opts.update(opts or {})
+        final_opts.update({"backoff": Backoffs.normalize(opts.get('backoff'))})
         self.discarded = False
         self.opts = final_opts
         self.queue = queue
         self.delay = opts.get("delay", 0)
         self.attempts = opts.get("attempts", 1)
         self.attemptsMade = 0
         self.data = data
         self.removeOnComplete = opts.get("removeOnComplete", True)
         self.removeOnFail = opts.get("removeOnFail", False)
         self.processedOn = 0
         self.finishedOn = 0
         self.returnvalue = None
         self.failedReason = None
         self.repeatJobKey = None
+        parent = opts.get("parent")
+        self.parentKey = get_parent_key(parent)
+        self.parent = {"id": parent.get("id"), "queueKey": parent.get("queue")} if parent else None
         self.stacktrace: List[str] = []
         self.scripts = Scripts(queue.prefix, queue.name, queue.redisConnection)
 
     def updateData(self, data):
         self.data = data
         return self.scripts.updateData(self.id, data)
 
@@ -139,14 +144,20 @@
                 self.stacktrace = self.stacktrace[-(stackTraceLimit-1):stackTraceLimit]
 
         keys, args = self.scripts.saveStacktraceArgs(
             self.id, json.dumps(self.stacktrace, separators=(',', ':')), err)
 
         await self.scripts.commands["saveStacktrace"](keys=keys, args=args, client=pipe)
 
+    def moveToWaitingChildren(self, token, opts:dict):
+        return self.scripts.moveToWaitingChildren(self.id, token, opts)
+
+    @property
+    def queueQualifiedName(self):
+        return f"{self.queue.prefix}:{self.queue.name}"
 
     @staticmethod
     def fromJSON(queue: Queue, rawData: dict, jobId: str | None = None):
         """
         Instantiates a Job from a JobJsonRaw object (coming from a deserialized JSON object)
 
         @param queue: the queue where the job belongs to.
@@ -177,21 +188,19 @@
 
         returnvalue = rawData.get("returnvalue")
         if type(returnvalue) == str:
             job.returnvalue = getReturnValue(returnvalue)
 
         job.stacktrace = json.loads(rawData.get("stacktrace", "[]"))
 
-        # if (json.parentKey) {
-        #   job.parentKey = json.parentKey;
-        # }
-
-        # if (json.parent) {
-        #   job.parent = JSON.parse(json.parent);
-        # }
+        if rawData.get("parentKey"):
+            job.parentKey = rawData.get("parentKey")
+
+        if rawData.get("parent"):
+           job.parent = json.loads(rawData.get("parent"))
 
         return job
 
     @staticmethod
     async def fromId(queue: Queue, jobId: str):
         key = f"{queue.prefix}:{queue.name}:{jobId}"
         raw_data = await queue.client.hgetall(key)
```

### Comparing `bullmq-1.5.0/bullmq/queue.py` & `bullmq-1.6.0/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/redis_connection.py` & `bullmq-1.6.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/scripts.py` & `bullmq-1.6.0/bullmq/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     This class is used to load and execute Lua scripts.
     It is a wrapper around the Redis client.
 """
 
 from __future__ import annotations
 from redis import Redis
 from bullmq.error_code import ErrorCode
-from bullmq.utils import isRedisVersionLowerThan
+from bullmq.utils import isRedisVersionLowerThan, get_parent_key
 from typing import Any, TYPE_CHECKING
 if TYPE_CHECKING:
     from bullmq.job import Job
     from bullmq.redis_connection import RedisConnection
 
 import time
 import json
@@ -37,27 +37,28 @@
             "getRanges": self.redisClient.register_script(self.getScript("getRanges-1.lua")),
             "getState": self.redisClient.register_script(self.getScript("getState-8.lua")),
             "getStateV2": self.redisClient.register_script(self.getScript("getStateV2-8.lua")),
             "moveStalledJobsToWait": self.redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
             "moveToActive": self.redisClient.register_script(self.getScript("moveToActive-10.lua")),
             "moveToDelayed": self.redisClient.register_script(self.getScript("moveToDelayed-8.lua")),
             "moveToFinished": self.redisClient.register_script(self.getScript("moveToFinished-13.lua")),
+            "moveToWaitingChildren": self.redisClient.register_script(self.getScript("moveToWaitingChildren-4.lua")),
             "obliterate": self.redisClient.register_script(self.getScript("obliterate-2.lua")),
             "pause": self.redisClient.register_script(self.getScript("pause-5.lua")),
             "removeJob": self.redisClient.register_script(self.getScript("removeJob-1.lua")),
             "reprocessJob": self.redisClient.register_script(self.getScript("reprocessJob-6.lua")),
             "retryJob": self.redisClient.register_script(self.getScript("retryJob-9.lua")),
             "retryJobs": self.redisClient.register_script(self.getScript("retryJobs-6.lua")),
             "saveStacktrace": self.redisClient.register_script(self.getScript("saveStacktrace-1.lua")),
             "updateData": self.redisClient.register_script(self.getScript("updateData-1.lua")),
             "updateProgress": self.redisClient.register_script(self.getScript("updateProgress-2.lua")),
         }
 
         # loop all the names and add them to the keys object
-        names = ["", "active", "wait", "paused", "completed", "failed", "delayed",
+        names = ["", "active", "wait", "waiting-children", "paused", "completed", "failed", "delayed",
                  "stalled", "limiter", "prioritized", "id", "stalled-check", "meta", "pc", "events", "waiting-children"]
         for name in names:
             self.keys[name] = self.toKey(name)
 
     def toKey(self, name: str):
         return f"{self.prefix}:{self.queueName}:{name}"
 
@@ -71,39 +72,66 @@
         return data
 
     def getKeys(self, keys: list[str]):
         def mapKey(key):
             return self.keys[key]
         return list(map(mapKey, keys))
 
-    def addJob(self, job: Job):
-        """
-        Add an item to the queue
-        """
-        packedArgs = msgpack.packb(
-            [self.keys[""], job.id or "", job.name, job.timestamp], use_bin_type=True)
+    def addJobArgs(self, job: Job, waiting_children_key):
         #  We are still lacking some arguments here:
         #  ARGV[1] msgpacked arguments array
-        #         [1]  key prefix,
-        #         [2]  custom id (will not generate one automatically)
-        #         [3]  name
-        #         [4]  timestamp
-        #         [5]  parentKey?
-        #         [6]  waitChildrenKey key.
-        #         [7]  parent dependencies key.
-        #         [8]  parent? {id, queueKey}
         #         [9]  repeat job key
 
         jsonData = json.dumps(job.data, separators=(',', ':'))
         packedOpts = msgpack.packb(job.opts)
 
         keys = self.getKeys(['wait', 'paused', 'meta', 'id',
                             'delayed', 'prioritized', 'completed', 'events', 'pc'])
+        parent = job.parent
+        parentKey = job.parentKey
+
+        packedArgs = msgpack.packb(
+            [self.keys[""], job.id or "", job.name, job.timestamp, job.parentKey,
+                waiting_children_key,
+                f"{parentKey}:dependencies" if parentKey else None, parent],use_bin_type=True)
+        
+        args = [packedArgs, jsonData, packedOpts]
+
+        return (keys,args)
+
+    def addJob(self, job: Job):
+        """
+        Add an item to the queue
+        """
+        keys, args = self.addJobArgs(job, None)
+
+        return self.commands["addJob"](keys=keys, args=args)
 
-        return self.commands["addJob"](keys=keys, args=[packedArgs, jsonData, packedOpts])
+    def moveToWaitingChildrenArgs(self, job_id, token, opts):
+        keys = [self.toKey(job_id) + ":lock",
+                self.keys['active'],
+                self.keys['waiting-children'],
+                self.toKey(job_id)]
+        child_key = opts.get("child") if opts else None
+        args = [token, get_parent_key(child_key) or "", round(time.time() * 1000), job_id]
+
+        return (keys, args)
+
+    async def moveToWaitingChildren(self, job_id, token, opts):
+        keys, args = self.moveToWaitingChildrenArgs(job_id, token, opts)
+        result = await self.commands["moveToWaitingChildren"](keys=keys, args=args)
+
+        if result is not None:
+            if result == 1:
+                return False
+            elif result == 0:
+                return True
+            elif result < 0:
+                raise self.finishedErrors(result, job_id, 'moveToWaitingChildren', 'active')
+        return None
 
     def getRangesArgs(self, types, start: int = 0, end: int = 1, asc: bool = False):
         transformed_types = []
         for type in types:
             transformed_types.append("wait" if type == "waiting" else type)
 
         keys = self.getKeys([''])
```

### Comparing `bullmq-1.5.0/bullmq/timer.py` & `bullmq-1.6.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/types/job_options.py` & `bullmq-1.6.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/types/worker_options.py` & `bullmq-1.6.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.5.0/bullmq/worker.py` & `bullmq-1.6.0/bullmq/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Callable
 from uuid import uuid4
+from bullmq.custom_errors import WaitingChildrenError
 from bullmq.scripts import Scripts
 from bullmq.redis_connection import RedisConnection
 from bullmq.event_emitter import EventEmitter
 from bullmq.job import Job
 from bullmq.timer import Timer
 from bullmq.types import WorkerOptions
 from bullmq.utils import isRedisVersionLowerThan, extract_result
@@ -120,15 +121,18 @@
 
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
                 await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", False), token, self.opts, fetchNext=not self.closing)
+                job.returnvalue = result
             self.emit("completed", job, result)
+        except WaitingChildrenError:
+            return
         except Exception as err:
             try:
                 print("Error processing job", err)
                 if not self.forceClosing:
                     await job.moveToFailed(err, token)
 
                 self.emit("failed", job, err)
```

### Comparing `bullmq-1.5.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.6.0/bullmq.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.5.0
+Version: 1.6.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.5.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.6.0/bullmq.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 bullmq/commands/removeRepeatable-2.lua
 bullmq/commands/reprocessJob-6.lua
 bullmq/commands/retryJob-9.lua
 bullmq/commands/retryJobs-6.lua
 bullmq/commands/saveStacktrace-1.lua
 bullmq/commands/updateData-1.lua
 bullmq/commands/updateProgress-2.lua
+bullmq/custom_errors/__init__.py
+bullmq/custom_errors/waiting_children_error.py
 bullmq/types/__init__.py
 bullmq/types/backoff_options.py
 bullmq/types/job_options.py
 bullmq/types/keep_jobs.py
 bullmq/types/queue_options.py
 bullmq/types/retry_job_options.py
 bullmq/types/worker_options.py
```

### Comparing `bullmq-1.5.0/pyproject.toml` & `bullmq-1.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.5.0"
+version = "1.6.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 classifiers=[
     'Development Status :: 3 - Alpha',
```

