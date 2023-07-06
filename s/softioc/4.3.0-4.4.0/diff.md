# Comparing `tmp/softioc-4.3.0.tar.gz` & `tmp/softioc-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softioc-4.3.0.tar", last modified: Tue Apr  4 08:28:25 2023, max compression
+gzip compressed data, was "softioc-4.4.0.tar", last modified: Thu Jul  6 13:50:51 2023, max compression
```

## Comparing `softioc-4.3.0.tar` & `softioc-4.4.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.171734 softioc-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 08:28:06.000000 softioc-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-04 08:28:25.171734 softioc-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-04 08:28:06.000000 softioc-4.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-04 08:28:06.000000 softioc-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-04 08:28:25.171734 softioc-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-04 08:28:06.000000 softioc-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.155734 softioc-4.3.0/softioc/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-04 08:28:25.171734 softioc-4.3.0/softioc/_version_git.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/access.acf
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/asyncio_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/cothread_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/device.dbd
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/device_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/extension.c
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.151734 softioc-4.3.0/softioc/iocStats/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.159734 softioc-4.3.0/softioc/iocStats/devIocStats/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStats.dbd
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStats.h
--rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsAnalog.c
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsString.c
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsSub.c
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsWaveform.c
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/devVxStats.dbd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.147734 softioc-4.3.0/softioc/iocStats/devIocStats/os/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.159734 softioc-4.3.0/softioc/iocStats/devIocStats/os/Darwin/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/Darwin/devIocStatsOSD.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.159734 softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUtilization.c
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdFdUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdMemUsage.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.159734 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/devIocStatsOSD.h
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdBootInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdCpuUtilization.c
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdFdUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdHostInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdMemUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdSystemInfo.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.167734 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/devIocStatsOSD.h
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdBootInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdClustInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdCpuUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdCpuUtilization.c
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdFdUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdHostInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdIFErrors.c
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdMemUsage.c
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdPIDInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdPwdInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdSuspTasks.c
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdSystemInfo.c
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdWorkspaceUsage.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.151734 softioc-4.3.0/softioc/iocStats/iocAdmin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.171734 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/access.db
--rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/access.doc
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/ioc.template
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminRTEMS.substitutions
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminScanMon.substitutions
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminSoft.substitutions
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminVxWorks.substitutions
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocCluster.template
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocEnvVar.template
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocGeneralTime.template
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocQueue.db
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocRTEMSOnly.template
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocRTOS.template
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocScanMon.template
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocScanMonSum.template
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-04 08:28:07.000000 softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocVxWorksOnly.template
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/pvlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/pythonSoftIoc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-04 08:28:06.000000 softioc-4.3.0/softioc/softioc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.155734 softioc-4.3.0/softioc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:28:24.000000 softioc-4.3.0/softioc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 08:28:25.000000 softioc-4.3.0/softioc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:28:25.171734 softioc-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-04 08:28:06.000000 softioc-4.3.0/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-04 08:28:06.000000 softioc-4.3.0/tests/test_cothread.py
--rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-04-04 08:28:06.000000 softioc-4.3.0/tests/test_record_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-04-04 08:28:06.000000 softioc-4.3.0/tests/test_records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.051078 softioc-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 13:50:35.000000 softioc-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-06 13:50:51.051078 softioc-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-06 13:50:35.000000 softioc-4.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-06 13:50:35.000000 softioc-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-06 13:50:51.051078 softioc-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-06 13:50:35.000000 softioc-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.023078 softioc-4.4.0/softioc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-06 13:50:51.051078 softioc-4.4.0/softioc/_version_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/access.acf
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/asyncio_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/cothread_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/device.dbd
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/device_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/extension.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.015077 softioc-4.4.0/softioc/iocStats/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.031078 softioc-4.4.0/softioc/iocStats/devIocStats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStats.dbd
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStats.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsAnalog.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsString.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsSub.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsWaveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/devVxStats.dbd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.015077 softioc-4.4.0/softioc/iocStats/devIocStats/os/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.031078 softioc-4.4.0/softioc/iocStats/devIocStats/os/Darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/Darwin/devIocStatsOSD.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.031078 softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUtilization.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdFdUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdMemUsage.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.035078 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/devIocStatsOSD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdBootInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdCpuUtilization.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdFdUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdHostInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdMemUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdSystemInfo.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.043078 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/devIocStatsOSD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdBootInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdClustInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdCpuUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdCpuUtilization.c
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdFdUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdHostInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdIFErrors.c
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdMemUsage.c
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdPIDInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdPwdInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdSuspTasks.c
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdSystemInfo.c
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdWorkspaceUsage.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.015077 softioc-4.4.0/softioc/iocStats/iocAdmin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.047078 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/access.db
+-rw-r--r--   0 runner    (1001) docker     (123)    32256 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/access.doc
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/ioc.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminRTEMS.substitutions
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminScanMon.substitutions
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminSoft.substitutions
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminVxWorks.substitutions
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocCluster.template
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocEnvVar.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocGeneralTime.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocQueue.db
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocRTEMSOnly.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocRTOS.template
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocScanMon.template
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocScanMonSum.template
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-06 13:50:36.000000 softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocVxWorksOnly.template
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/pvlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/pythonSoftIoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-07-06 13:50:35.000000 softioc-4.4.0/softioc/softioc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.027078 softioc-4.4.0/softioc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-06 13:50:51.000000 softioc-4.4.0/softioc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:50:50.000000 softioc-4.4.0/softioc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:50:51.051078 softioc-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-06 13:50:35.000000 softioc-4.4.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-06 13:50:35.000000 softioc-4.4.0/tests/test_cothread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-06 13:50:35.000000 softioc-4.4.0/tests/test_deviocstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34351 2023-07-06 13:50:35.000000 softioc-4.4.0/tests/test_record_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27787 2023-07-06 13:50:35.000000 softioc-4.4.0/tests/test_records.py
```

### Comparing `softioc-4.3.0/LICENSE` & `softioc-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/PKG-INFO` & `softioc-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softioc
-Version: 4.3.0
+Version: 4.4.0
 Summary: Embed an EPICS IOC in a Python process
 Home-page: https://github.com/dls-controls/pythonSoftIOC
 Author: Michael Abbott
 Author-email: Michael.Abbott@diamond.ac.uk
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `softioc-4.3.0/README.rst` & `softioc-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/setup.cfg` & `softioc-4.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,23 @@
 	iocStats/devIocStats/os/WIN32/*
 	iocStats/devIocStats/os/Linux/*
 
 [options.extras_require]
 useful = 
 	cothread
 	scipy
-	aioca >=1.3
+	aioca >=1.6
 dev = 
 	pytest-cov
 	pytest-flake8
+	flake8 <5.0.0
+	sphinx ==4.3.2
 	sphinx-rtd-theme-github-versions
 	pytest-asyncio
-	aioca >=1.3
+	aioca >=1.6
 	cothread; sys_platform != "win32"
 	p4p
 
 [flake8]
 max-line-length = 80
 extend-ignore = 
 	F401 F403 F405  # Allow from module import *
```

### Comparing `softioc-4.3.0/setup.py` & `softioc-4.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,38 +37,47 @@
     "osdBootInfo.c",
     "osdSystemInfo.c",
     "osdHostInfo.c",
     "osdPIDInfo.c",
 ]
 
 devIocStats_src = os.path.join("softioc", "iocStats", "devIocStats")
+devIocStats_posix = os.path.join(devIocStats_src, "os", "posix")
 devIocStats_os = os.path.join(devIocStats_src, "os", get_config_var('OS_CLASS'))
 devIocStats_default = os.path.join(devIocStats_src, "os", "default")
 
 for f in devIocStats_OSI:
     sources.append(os.path.join(devIocStats_src, f))
 for f in devIocStats_OSD:
     if os.path.exists(os.path.join(devIocStats_os, f)):
         sources.append(os.path.join(devIocStats_os, f))
     else:
         sources.append(os.path.join(devIocStats_default, f))
 
+include_dirs = [
+    epicscorelibs.path.include_path,
+    devIocStats_src,
+    devIocStats_os,
+    devIocStats_default
+]
+
+if get_config_var("POSIX"):
+    # If we're on a POSIX system, insert the POSIX folder into the list after
+    # the os-specific one so that os-specific header files are used first.
+    include_dirs.insert(
+        include_dirs.index(devIocStats_os) + 1,
+        devIocStats_posix
+    )
+
 # Extension with all our C code
 ext = Extension(
     name='softioc._extension',
     sources = sources,
-    include_dirs=[
-        epicscorelibs.path.include_path,
-        devIocStats_src, devIocStats_os, devIocStats_default
-    ],
+    include_dirs = include_dirs,
     dsos = [
-        'epicscorelibs.lib.qsrv',
-        'epicscorelibs.lib.pvAccessIOC',
-        'epicscorelibs.lib.pvAccess',
-        'epicscorelibs.lib.pvData',
         'epicscorelibs.lib.dbRecStd',
         'epicscorelibs.lib.dbCore',
         'epicscorelibs.lib.ca',
         'epicscorelibs.lib.Com',
     ],
     define_macros = get_config_var('CPPFLAGS'),
     extra_compile_args = get_config_var('CFLAGS') + ["-std=c99"],
@@ -91,12 +100,13 @@
 setup(
     cmdclass=dict(develop=Develop, **get_cmdclass()),
     version=__version__,
     ext_modules = [ext],
     install_requires = [
         # Dependency version declared in pyproject.toml
         epicscorelibs.version.abi_requires(),
+        "pvxslibs>=1.2.2",
         "numpy",
         "epicsdbbuilder>=1.4"
     ],
     zip_safe = False,  # setuptools_dso is not compatible with eggs!
 )
```

### Comparing `softioc-4.3.0/softioc/__init__.py` & `softioc-4.4.0/softioc/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 '''Python soft IOC module.'''
 import os
+import ctypes
 
-from epicscorelibs import path
+from setuptools_dso.runtime import find_dso
+import epicscorelibs.path
+import pvxslibs.path
 from epicscorelibs.ioc import \
     iocshRegisterCommon, registerRecordDeviceDriver, pdbbase
 
 # Do this as early as possible, in case we happen to use cothread
 # This will set the CATOOLS_LIBCA_PATH environment variable in case we use
 # cothread.catools. It works even if we don't have cothread installed
 import epicscorelibs.path.cothread  # noqa
@@ -13,16 +16,19 @@
 # This import will also pull in the extension, which is needed
 # before we call iocshRegisterCommon
 from .imports import dbLoadDatabase
 from ._version_git import __version__
 
 # Need to do this before calling anything in device.py
 iocshRegisterCommon()
-for dbd in ('base.dbd', 'PVAServerRegister.dbd', 'qsrv.dbd'):
-    dbLoadDatabase(dbd, os.path.join(path.base_path, 'dbd'), None)
+base_dbd_path = os.path.join(epicscorelibs.path.base_path, 'dbd')
+dbLoadDatabase('base.dbd', base_dbd_path, None)
+dbLoadDatabase('pvxsIoc.dbd', pvxslibs.path.dbd_path, None)
 iocStats = os.path.join(os.path.dirname(__file__), "iocStats", "devIocStats")
 dbLoadDatabase('devIocStats.dbd', iocStats, None)
 
+ctypes.CDLL(find_dso('pvxslibs.lib.pvxsIoc'), ctypes.RTLD_GLOBAL)
+os.environ.setdefault('PVXS_QSRV_ENABLE', 'YES')
 if registerRecordDeviceDriver(pdbbase):
     raise RuntimeError('Error registering')
 
 __all__ = ['__version__']
```

### Comparing `softioc-4.3.0/softioc/__main__.py` & `softioc-4.4.0/softioc/__main__.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/_version_git.py` & `softioc-4.4.0/softioc/_version_git.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # versiongit-1.0 (https://github.com/dls-controls/versiongit)
 import os
 import re
 import sys
 from subprocess import STDOUT, CalledProcessError, check_output
 
 # These will be filled in if git archive is run or by setup.py cmdclasses
-GIT_REFS = 'tag: 4.3.0'
-GIT_SHA1 = 'b22b497'
+GIT_REFS = 'tag: 4.4.0'
+GIT_SHA1 = '07b1168'
 
 # Git describe gives us sha1, last version-like tag, and commits since then
 CMD = "git describe --tags --dirty --always --long --match=[0-9]*[-.][0-9]*"
 
 
 def get_version_from_git(path=None):
     """Try to parse version from git describe, fallback to git archive tags"""
```

### Comparing `softioc-4.3.0/softioc/alarm.py` & `softioc-4.4.0/softioc/alarm.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/asyncio_dispatcher.py` & `softioc-4.4.0/softioc/asyncio_dispatcher.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/builder.py` & `softioc-4.4.0/softioc/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,28 +257,31 @@
         length = len(fields['initial_value'].encode(errors = 'replace')) + 1
     else:
         # Default length of 256
         length = 256
 
     fields.setdefault('initial_value', '')
     fields['_wf_nelm'] = length
-    fields['_wf_dtype'] = numpy.dtype('uint8')
+    fields['_wf_dtype'] = numpy.dtype('int8')
 
     fields['NELM'] = length
-    fields['FTVL'] = 'UCHAR'
+    fields['FTVL'] = 'CHAR'
 
+def qform_string(rec):
+    rec.add_info("Q:form", "String")
+    return rec
 
 def longStringIn(name, **fields):
     _long_string(fields)
     _set_in_defaults(fields)
-    return PythonDevice.long_stringin(name, **fields)
+    return qform_string(PythonDevice.long_stringin(name, **fields))
 
 def longStringOut(name, **fields):
     _long_string(fields)
-    return PythonDevice.long_stringout(name, **fields)
+    return qform_string(PythonDevice.long_stringout(name, **fields))
 
 
 
 # ----------------------------------------------------------------------------
 #  Support routines for builder
 
 def LoadDatabase():
```

### Comparing `softioc-4.3.0/softioc/cothread_dispatcher.py` & `softioc-4.4.0/softioc/cothread_dispatcher.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/device.dbd` & `softioc-4.4.0/softioc/device.dbd`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/device.py` & `softioc-4.4.0/softioc/device.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/device_core.py` & `softioc-4.4.0/softioc/device_core.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/extension.c` & `softioc-4.4.0/softioc/extension.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/fields.py` & `softioc-4.4.0/softioc/fields.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/imports.py` & `softioc-4.4.0/softioc/imports.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/Makefile` & `softioc-4.4.0/softioc/iocStats/devIocStats/Makefile`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStats.h` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStats.h`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsAnalog.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsAnalog.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsString.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsString.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsSub.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsSub.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsTest.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsTest.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/devIocStatsWaveform.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/devIocStatsWaveform.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/Darwin/devIocStatsOSD.h` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/Darwin/devIocStatsOSD.h`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUtilization.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdCpuUtilization.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdFdUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdFdUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/Linux/osdMemUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/Linux/osdMemUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/devIocStatsOSD.h` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/devIocStatsOSD.h`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdBootInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdBootInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdCpuUtilization.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdCpuUtilization.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdFdUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdFdUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdHostInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdHostInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdMemUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdMemUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/WIN32/osdSystemInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/WIN32/osdSystemInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/devIocStatsOSD.h` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/devIocStatsOSD.h`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdBootInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdBootInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdClustInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdClustInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdCpuUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdCpuUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdCpuUtilization.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdCpuUtilization.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdFdUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdFdUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdHostInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdHostInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdIFErrors.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdIFErrors.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdMemUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdMemUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdPIDInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdPIDInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdPwdInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdPwdInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdSuspTasks.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdSuspTasks.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdSystemInfo.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdSystemInfo.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/devIocStats/os/default/osdWorkspaceUsage.c` & `softioc-4.4.0/softioc/iocStats/devIocStats/os/default/osdWorkspaceUsage.c`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/Makefile` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/Makefile`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/access.db` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/access.db`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/access.doc` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/access.doc`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/ioc.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/ioc.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminRTEMS.substitutions` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminRTEMS.substitutions`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminScanMon.substitutions` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminScanMon.substitutions`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminSoft.substitutions` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminSoft.substitutions`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocAdminVxWorks.substitutions` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocAdminVxWorks.substitutions`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocCluster.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocCluster.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocGeneralTime.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocGeneralTime.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocQueue.db` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocQueue.db`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocRTEMSOnly.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocRTEMSOnly.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocRTOS.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocRTOS.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocScanMon.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocScanMon.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocScanMonSum.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocScanMonSum.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/iocStats/iocAdmin/Db/iocVxWorksOnly.template` & `softioc-4.4.0/softioc/iocStats/iocAdmin/Db/iocVxWorksOnly.template`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc/pythonSoftIoc.py` & `softioc-4.4.0/softioc/pythonSoftIoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,15 @@
     # Some further "Duck typing" for the builder: the following are required
     # for links to work properly.
 
     def __call__(self, *specifiers):
         return self.__builder(*specifiers)
 
     def __str__(self):
-        return str(self.__builder)
-
+        return self.__device._name
 
 
 class PythonDevice(object):
     DbdFileList = ['device']
 
     @classmethod
     def __init_class__(cls):
```

### Comparing `softioc-4.3.0/softioc/softioc.py` & `softioc-4.4.0/softioc/softioc.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/softioc.egg-info/PKG-INFO` & `softioc-4.4.0/softioc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softioc
-Version: 4.3.0
+Version: 4.4.0
 Summary: Embed an EPICS IOC in a Python process
 Home-page: https://github.com/dls-controls/pythonSoftIOC
 Author: Michael Abbott
 Author-email: Michael.Abbott@diamond.ac.uk
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `softioc-4.3.0/softioc.egg-info/SOURCES.txt` & `softioc-4.4.0/softioc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,9 +77,10 @@
 softioc/iocStats/iocAdmin/Db/iocRTEMSOnly.template
 softioc/iocStats/iocAdmin/Db/iocRTOS.template
 softioc/iocStats/iocAdmin/Db/iocScanMon.template
 softioc/iocStats/iocAdmin/Db/iocScanMonSum.template
 softioc/iocStats/iocAdmin/Db/iocVxWorksOnly.template
 tests/test_asyncio.py
 tests/test_cothread.py
+tests/test_deviocstats.py
 tests/test_record_values.py
 tests/test_records.py
```

### Comparing `softioc-4.3.0/tests/test_asyncio.py` & `softioc-4.4.0/tests/test_asyncio.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,20 @@
         assert ai_val == 23.45
         assert ai_val.severity == 3
         assert ai_val.status == 7  # STATE_ALARM
         # Check pvaccess works
         from p4p.client.asyncio import Context
         with Context("pva") as ctx:
             assert await ctx.get(pre + ":AI") == 23.45
+            long_pv = pre + ":AVERYLONGRECORDSUFFIXTOMAKELONGPV"
+            long_str = "A long string that is more than 40 characters long"
+            assert await ctx.get(long_pv) == long_str
+            assert await ctx.get(long_pv + ".NAME") == long_pv
+            await ctx.put(pre + ":LONGSTRING", long_str)
+            assert await ctx.get(pre + ":LONGSTRING") == long_str
 
         conn.send("D")  # "Done"
         select_and_recv(conn, "D")  # "Done"
 
     # Stop
     out, err = asyncio_ioc.proc.communicate(b"exit\n", timeout=5)
     out = out.decode()
```

### Comparing `softioc-4.3.0/tests/test_cothread.py` & `softioc-4.4.0/tests/test_cothread.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/tests/test_record_values.py` & `softioc-4.4.0/tests/test_record_values.py`

 * *Files identical despite different names*

### Comparing `softioc-4.3.0/tests/test_records.py` & `softioc-4.4.0/tests/test_records.py`

 * *Files 3% similar despite different names*

```diff
@@ -285,14 +285,72 @@
         select_and_recv(parent_conn, "D")
     finally:
         process.join(timeout=TIMEOUT)
         if process.exitcode is None:
             pytest.fail("Process did not terminate")
 
 
+def str_ioc_test_func(device_name, conn):
+    builder.SetDeviceName(device_name)
+
+    record_name = "MyAI"
+
+    full_name = device_name + ":" + record_name
+
+    ai = builder.aIn(record_name)
+
+
+    log("CHILD: Created ai record: ", ai.__str__())
+
+    assert (
+        ai.__str__() == full_name
+    ), f"Record name {ai.__str__()} before LoadDatabase did not match " \
+       f"expected string {full_name}"
+
+    builder.LoadDatabase()
+
+    assert (
+        ai.__str__() == full_name
+    ), f"Record name {ai.__str__()} after LoadDatabase did not match " \
+       f"expected string {full_name}"
+
+    dispatcher = asyncio_dispatcher.AsyncioDispatcher()
+    softioc.iocInit(dispatcher)
+
+    assert (
+        ai.__str__() == full_name
+    ), f"Record name {ai.__str__()} after iocInit did not match expected " \
+       f"string {full_name}"
+
+    conn.send("R")  # "Ready"
+    log("CHILD: Sent R over Connection to Parent")
+
+
+
+def test_record_wrapper_str():
+    """Test that the __str__ method on the RecordWrapper behaves as expected,
+    both before and after loading the record database"""
+
+    ctx = get_multiprocessing_context()
+    parent_conn, child_conn = ctx.Pipe()
+
+    device_name = create_random_prefix()
+
+    ioc_process = ctx.Process(
+        target=str_ioc_test_func,
+        args=(device_name, child_conn),
+    )
+
+    ioc_process.start()
+
+
+    # Wait for message that IOC has started
+    # If we never receive R it probably means an assert failed
+    select_and_recv(parent_conn, "R")
+
 
 def validate_fixture_names(params):
     """Provide nice names for the out_records fixture in TestValidate class"""
     return params[0].__name__
 
 class TestValidate:
     """Tests related to the validate callback"""
```

