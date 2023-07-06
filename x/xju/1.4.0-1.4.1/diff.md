# Comparing `tmp/xju-1.4.0.tar.gz` & `tmp/xju-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-1.4.0.tar", last modified: Wed Jul  5 10:32:10 2023, max compression
+gzip compressed data, was "xju-1.4.1.tar", last modified: Thu Jul  6 11:17:46 2023, max compression
```

## Comparing `xju-1.4.0.tar` & `xju-1.4.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-07-05 10:32:09.000000 xju-1.4.0/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)     9092 2023-07-05 10:32:10.205364 xju-1.4.0/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     7556 2023-07-05 10:32:09.000000 xju-1.4.0/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1742 2023-07-05 10:32:09.000000 xju-1.4.0/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-07-05 10:32:10.205364 xju-1.4.0/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.201364 xju-1.4.0/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.201364 xju-1.4.0/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-1.4.0/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-1.4.0/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju/cmc/
--rwxr-xr-x   0 xju       (1001) xju       (1001)     9781 2023-06-20 09:48:20.000000 xju-1.4.0/src/xju/cmc/AsyncDict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-1.4.0/src/xju/cmc/AsyncOpt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.4.0/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-06-11 03:07:27.000000 xju-1.4.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.4.0/src/xju/cmc/Dict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-1.4.0/src/xju/cmc/Opt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.4.0/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    41771 2023-06-21 01:30:26.000000 xju-1.4.0/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     8562 2023-06-26 21:01:25.000000 xju-1.4.0/src/xju/cmc/async_cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-1.4.0/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14657 2023-06-17 10:59:19.000000 xju-1.4.0/src/xju/cmc/cmclass.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.4.0/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.4.0/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.4.0/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.4.0/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.4.0/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.4.0/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.4.0/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.4.0/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.4.0/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.4.0/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.4.0/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.4.0/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.4.0/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.4.0/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.4.0/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.4.0/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    70831 2023-07-03 10:56:25.000000 xju-1.4.0/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    45743 2023-07-03 10:53:19.000000 xju-1.4.0/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.4.0/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.4.0/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.4.0/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.4.0/src/xju/misc.py.test
--r--r--r--   0 xju       (1001) xju       (1001)    22865 2023-06-11 07:25:02.000000 xju-1.4.0/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11796 2023-06-11 09:21:50.000000 xju-1.4.0/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.4.0/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.4.0/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.4.0/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.4.0/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:09.000000 xju-1.4.0/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.4.0/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.4.0/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.4.0/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.4.0/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7232 2023-07-02 10:20:30.000000 xju-1.4.0/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     5202 2023-06-21 01:07:25.000000 xju-1.4.0/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-05 10:32:10.205364 xju-1.4.0/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)     9092 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1380 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-07-05 10:32:10.000000 xju-1.4.0/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.071362 xju-1.4.1/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2023-07-06 11:17:45.000000 xju-1.4.1/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)     9160 2023-07-06 11:17:46.071362 xju-1.4.1/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     7624 2023-07-06 11:17:45.000000 xju-1.4.1/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1742 2023-07-06 11:17:45.000000 xju-1.4.1/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2023-07-06 11:17:46.071362 xju-1.4.1/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.067362 xju-1.4.1/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.067362 xju-1.4.1/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-1.4.1/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-1.4.1/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.071362 xju-1.4.1/src/xju/cmc/
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     9781 2023-06-20 09:48:20.000000 xju-1.4.1/src/xju/cmc/AsyncDict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-1.4.1/src/xju/cmc/AsyncOpt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-1.4.1/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-06-11 03:07:27.000000 xju-1.4.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-1.4.1/src/xju/cmc/Dict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-1.4.1/src/xju/cmc/Opt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-1.4.1/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    42000 2023-07-06 10:58:53.000000 xju-1.4.1/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8566 2023-07-06 10:59:56.000000 xju-1.4.1/src/xju/cmc/async_cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-1.4.1/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14657 2023-06-17 10:59:19.000000 xju-1.4.1/src/xju/cmc/cmclass.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.071362 xju-1.4.1/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-1.4.1/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-1.4.1/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-1.4.1/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-1.4.1/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-1.4.1/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-1.4.1/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-1.4.1/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18523 2023-03-11 11:23:08.000000 xju-1.4.1/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-1.4.1/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-1.4.1/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-1.4.1/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-1.4.1/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-1.4.1/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-1.4.1/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2022-10-22 04:11:35.000000 xju-1.4.1/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-1.4.1/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    70831 2023-07-03 10:56:25.000000 xju-1.4.1/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    45743 2023-07-03 10:53:19.000000 xju-1.4.1/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-1.4.1/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-1.4.1/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1278 2022-10-19 21:07:25.000000 xju-1.4.1/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-1.4.1/src/xju/misc.py.test
+-r--r--r--   0 xju       (1001) xju       (1001)    22865 2023-06-11 07:25:02.000000 xju-1.4.1/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11796 2023-06-11 09:21:50.000000 xju-1.4.1/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-1.4.1/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-1.4.1/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2023-04-30 10:35:38.000000 xju-1.4.1/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2023-03-18 10:39:02.000000 xju-1.4.1/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:45.000000 xju-1.4.1/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-1.4.1/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-1.4.1/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3280 2023-04-30 10:35:38.000000 xju-1.4.1/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2402 2023-03-11 10:39:44.000000 xju-1.4.1/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7232 2023-07-02 10:20:30.000000 xju-1.4.1/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     5202 2023-06-21 01:07:25.000000 xju-1.4.1/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2023-07-06 11:17:46.067362 xju-1.4.1/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)     9160 2023-07-06 11:17:46.000000 xju-1.4.1/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1380 2023-07-06 11:17:46.000000 xju-1.4.1/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2023-07-06 11:17:46.000000 xju-1.4.1/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2023-07-06 11:17:46.000000 xju-1.4.1/src/xju.egg-info/top_level.txt
```

### Comparing `xju-1.4.0/MIT-LICENCE` & `xju-1.4.1/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/PKG-INFO` & `xju-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.4.0
+Version: 1.4.1
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -188,14 +188,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.1 fix type hints on xju.cmc.async_cmclass and xju.cmc.cmclass
 - 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
```

### Comparing `xju-1.4.0/README.rst` & `xju-1.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.1 fix type hints on xju.cmc.async_cmclass and xju.cmc.cmclass
 - 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
```

### Comparing `xju-1.4.0/pyproject.toml` & `xju-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "1.4.0"
+version = "1.4.1"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `xju-1.4.0/src/xju/assert_.py` & `xju-1.4.1/src/xju/assert_.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/assert_.py.test` & `xju-1.4.1/src/xju/assert_.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/AsyncDict.py.test` & `xju-1.4.1/src/xju/cmc/AsyncDict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/AsyncOpt.py.test` & `xju-1.4.1/src/xju/cmc/AsyncOpt.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-1.4.1/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test` & `xju-1.4.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/Dict.py.test` & `xju-1.4.1/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/Opt.py.test` & `xju-1.4.1/src/xju/cmc/Opt.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-1.4.1/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/__init__.py` & `xju-1.4.1/src/xju/cmc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 from xju.time import Duration
 from xju.xn import in_function_context, in_context
 from xju.assert_ import Assert
 
 T = TypeVar('T')
 U = TypeVar('U')
 
-def cmclass(cls:Type[contextlib.AbstractContextManager[T]]) -> Type[contextlib.AbstractContextManager[T]]:
+T_CMT = TypeVar('T_CMT', bound=Type[contextlib.AbstractContextManager])
+
+def cmclass(cls:T_CMT) -> T_CMT:
     '''Class decorator that adds context management __enter__ and __exit__
        that enter and exit all type-hinted attributes implementing contextlib.AbstractContextManager
        then any existing __enter__.
        Note that to satisfy mypy, the decorated class must already
        implement contextlib.AbstractContextManager and the preferred way to do that is
        to inherit from xju.cmc.CM - see cmc.py.test for examples.
        See also async_cmclass, which provides an asyncio equivalent.
@@ -578,25 +580,28 @@
         pass
 
     def notify_all(self, l:Lock) -> None:
         assert l.m == self.m and l.active
         self.c.notify_all()
     pass
 
-def async_cmclass(cls:Type[contextlib.AbstractAsyncContextManager[T]]) -> Type[contextlib.AbstractAsyncContextManager[T]]:
+ACMT = TypeVar('ACMT', bound=contextlib.AbstractAsyncContextManager)
+T_ACMT = TypeVar('T_ACMT', bound=Type[contextlib.AbstractAsyncContextManager])
+
+def async_cmclass(cls:T_ACMT) -> T_ACMT:
     '''Class decorator that adds async context management __aenter__ and __aexit__
        that enter and exit all type-hinted attributes implementing 
        contextlib.AbstractAsyncContextManager and contextlib.AbstractContextManager
        then any existing __aenter__.
        Note that to satisfy mypy, the decorated class must already
        implement contextlib.AbstractAsyncContextManager and the preferred way to do that is
        to inherit from xju.cmc.AsyncCM - see cmc.py.test for examples.
     '''
-    base_classes_to_enter = _make_base_classes_to_enter(cls)
-    attrs_to_enter = _make_attrs_to_enter(cls)
+    base_classes_to_enter = _make_base_classes_to_enter(cls) # type: ignore  # mypy 1.4.1 gets confused
+    attrs_to_enter = _make_attrs_to_enter(cls) # type: ignore  # mypy 1.4.1 gets confused
     # need a unique place to keep resources acquired by enter so exit can
     # exit them, only want resources for self, not subclasses (which do their own
     # handling). Note replacing . with _ could lead to clashes but there's no
     # way to avoid all clashes.
     resources_attr_name=f'xju_cmc_async_cmclass_resources_{cls.__module__}.{cls.__name__}'.replace('.','_')
     orig_enter=cls.__dict__.get('__aenter__')
     async def aenter(self,
@@ -1080,59 +1085,64 @@
 
     def notify_all(self, l:AsyncLock):
         assert l.m == self.m and l.active
         self.c.notify_all()
     pass
 
 def _make_base_classes_to_enter(
-        cls: Type[contextlib.AbstractAsyncContextManager[T]]
-) -> list[Callable[[contextlib.AbstractAsyncContextManager[T]],contextlib.AbstractAsyncContextManager]]:
-    result: list[Callable[[contextlib.AbstractAsyncContextManager[T]],contextlib.AbstractAsyncContextManager]] = []
+        cls: Type[ACMT]
+) -> list[Callable[[ACMT],contextlib.AbstractAsyncContextManager[None]]]:
+    result: list[Callable[[ACMT],contextlib.AbstractAsyncContextManager[None]]] = []
     for base_class in cls.__bases__:
         if base_class is not AsyncCM and issubclass(base_class, contextlib.AbstractAsyncContextManager):
-            result.append(_make_async_class_cm(base_class))
+            result.append(
+                _make_async_class_cm(base_class))  # type: ignore  # above assert...
+            # ... says that base_class is a subclass of AbstractAsyncContextManager i.e. an ACMT,
+            # but mypy 1.4.1 says "Argument 1 to "_make_async_class_cm" has incompatible
+            # type "type[AbstractAsyncContextManager[Any]]"; expected "type[ACMT]"
             pass
         assert not issubclass(cls, CM), cls
         pass
     return result
 
 def _make_async_class_cm(
-        cls:Type[contextlib.AbstractAsyncContextManager]
-) -> Callable[[contextlib.AbstractAsyncContextManager],contextlib.AbstractAsyncContextManager]:
-    def result(x:contextlib.AbstractAsyncContextManager) -> contextlib.AbstractAsyncContextManager:
+        cls:Type[ACMT]
+) -> Callable[[ACMT],contextlib.AbstractAsyncContextManager[None]]:
+    def result(x:contextlib.AbstractAsyncContextManager) -> contextlib.AbstractAsyncContextManager[None]:
         return _AsyncClassCm(cls, x)
     return result
             
 @dataclass
-class _AsyncClassCm(contextlib.AbstractAsyncContextManager):
+class _AsyncClassCm(contextlib.AbstractAsyncContextManager[None]):
     '''target object {x} subclass {cls} context management methods
        - so for x: X where X(Y), __ClassCM(Y, x) will call Y.__enter__
          and Y.__exit__ directly avoiding any X.__enter__/__exit__
          overrides'''
-    cls:Type[contextlib.AbstractAsyncContextManager]
-    x:contextlib.AbstractAsyncContextManager
+    cls:Type[contextlib.AbstractAsyncContextManager[Any]]
+    x:Any
 
-    async def __aenter__(self):
-        return await self.cls.__aenter__(self.x)
+    async def __aenter__(self) -> None:
+        assert isinstance(self.x, self.cls)
+        await self.cls.__aenter__(self.x)
     async def __aexit__(self, t, e, b):
         return await self.cls.__aexit__(self.x, t, e, b)
     pass
 
 def _make_attrs_to_enter(
-        cls: Type[contextlib.AbstractAsyncContextManager[T]]
+        cls: Type[ACMT]
 ) -> dict[
     str,
     Callable[
-        [contextlib.AbstractAsyncContextManager[T]],contextlib.AbstractAsyncContextManager
+        [ACMT],contextlib.AbstractAsyncContextManager
     ]
 ]:
     result: dict[
         str,
         Callable[
-            [contextlib.AbstractAsyncContextManager[T]],contextlib.AbstractAsyncContextManager
+            [ACMT],contextlib.AbstractAsyncContextManager
         ]
     ] = {}
     for n, t in cls.__annotations__.items():
         if _is_subclass(n, t, contextlib.AbstractAsyncContextManager):
             result[n]=_make_async_attr_class_cm(n)
         elif _is_subclass(n, t, contextlib.AbstractContextManager):
             result[n]=_make_async_sync_attr_class_cm(n)
```

### Comparing `xju-1.4.0/src/xju/cmc/async_cmclass.py.test` & `xju-1.4.1/src/xju/cmc/async_cmclass.py.test`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
             if self.xe:
                 log(f'E exit {self.name}')
                 raise self.xe
             log(f'- aexit {self.name}')
         except Exception:
             raise in_context(f'aexit {self.name}') from None
         pass
+    pass
 
 @async_cmclass
 class Aggregate(AsyncCM):
     name: str
     a: AsyncResource
     b: Resource
     c: AsyncResource
@@ -154,17 +155,18 @@
     try:
         await base.__aexit__(None,None,None)
     except Exception as e:
         Assert(readable_repr(e))=='xju.cmc.AsyncCM.__aexit__ not overridden, have you forgotten @async_cmclass on __main__.NotOverridden?'
     else:
         assert False
         pass
-    
-    async with Aggregate('A') as a:
-        Assert(a.name)=='A'
+
+    a=Aggregate('A')
+    Assert(a.name)=='A'
+    async with a:
         Assert(_log)==[
             '+ aenter A.a', '- aenter A.a',
             '+ enter A.b', '- enter A.b',
             '+ aenter A.c', '- aenter A.c'
         ]
         try:
             a.c = AsyncResource('fred',None,None)
```

### Comparing `xju-1.4.0/src/xju/cmc/cmc.py.test` & `xju-1.4.1/src/xju/cmc/cmc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/cmclass.py.test` & `xju-1.4.1/src/xju/cmc/cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/FileLock.py.test` & `xju-1.4.1/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/FileMode.py.test` & `xju-1.4.1/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/FilePosition.py.test` & `xju-1.4.1/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/FileReader.py.test` & `xju-1.4.1/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/FileWriter.py.test` & `xju-1.4.1/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/Pipe.py.test` & `xju-1.4.1/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-1.4.1/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/io/__init__.py` & `xju-1.4.1/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/perflog.py` & `xju-1.4.1/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/perflog.py.test` & `xju-1.4.1/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/signal.py` & `xju-1.4.1/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/signal.py.test` & `xju-1.4.1/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/tstore.py` & `xju-1.4.1/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmc/tstore.py.test` & `xju-1.4.1/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmd.py` & `xju-1.4.1/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/cmd.py.test` & `xju-1.4.1/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/json_codec.py` & `xju-1.4.1/src/xju/json_codec.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/json_codec.py.test` & `xju-1.4.1/src/xju/json_codec.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/jsonschema.py` & `xju-1.4.1/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/jsonschema.py.test` & `xju-1.4.1/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/misc.py` & `xju-1.4.1/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/misc.py.test` & `xju-1.4.1/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/newtype.py` & `xju-1.4.1/src/xju/newtype.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/newtype.py.test` & `xju-1.4.1/src/xju/newtype.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/patch.py` & `xju-1.4.1/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/patch.py.test` & `xju-1.4.1/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/pq.py` & `xju-1.4.1/src/xju/pq.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/pq.py.test` & `xju-1.4.1/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/rfc2616.py` & `xju-1.4.1/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/rfc2616.py.test` & `xju-1.4.1/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/time.py` & `xju-1.4.1/src/xju/time.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/time.py.test` & `xju-1.4.1/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/xn.py` & `xju-1.4.1/src/xju/xn.py`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju/xn.py.test` & `xju-1.4.1/src/xju/xn.py.test`

 * *Files identical despite different names*

### Comparing `xju-1.4.0/src/xju.egg-info/PKG-INFO` & `xju-1.4.1/src/xju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 1.4.0
+Version: 1.4.1
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -188,14 +188,15 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 1.4.1 fix type hints on xju.cmc.async_cmclass and xju.cmc.cmclass
 - 1.4.0 add Enum support to xju.json_codec
 - 1.3.0 add xju.cmc.AsyncDict, like xju.cmc.Dict but async
 - 1.3.0 xju.cmc.AsyncOpt/Opt async context manager that holds an optional async context manager
 - 1.3.0 xju.cmc.Opt context manager that holds an optional context manager
 - 1.3.0 python xju.cmc add async_cmclass, like xju.cmc.cmclass; handles both async and non-async attrs
 - 1.3.0 strip leading whitespace from doc strings, for compatibility with code formatters like black
 - 1.2.13 xju.newtype Literals now handle more than one value, e.g. Literal['fred','jock']
```

### Comparing `xju-1.4.0/src/xju.egg-info/SOURCES.txt` & `xju-1.4.1/src/xju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

