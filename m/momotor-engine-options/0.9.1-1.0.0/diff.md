# Comparing `tmp/momotor-engine-options-0.9.1.tar.gz` & `tmp/momotor-engine-options-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-options-0.9.1.tar", last modified: Thu Oct 27 06:26:52 2022, max compression
+gzip compressed data, was "momotor-engine-options-1.0.0.tar", last modified: Thu Jul  6 10:04:25 2023, max compression
```

## Comparing `momotor-engine-options-0.9.1.tar` & `momotor-engine-options-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/
--rw-r--r--   0 root         (0) root         (0)     1779 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      778 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2154 2022-10-06 09:17:27.000000 momotor-engine-options-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7456 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8228 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/dependencies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     7560 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/preflight.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3692 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/
--rw-rw-rw-   0 root         (0) root         (0)     5329 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/domain/tools/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/filter_files.py
--rw-rw-rw-   0 root         (0) root         (0)    12223 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-27 06:26:31.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2022-10-21 07:06:14.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/keyvalue.py
--rw-rw-rw-   0 root         (0) root         (0)     3552 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)    24419 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8308 2022-10-27 06:25:56.000000 momotor-engine-options-0.9.1/src/momotor/options/parser/selector.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/result_query.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/split.py
--rw-rw-rw-   0 root         (0) root         (0)     8926 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/task_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/
--rw-rw-rw-   0 root         (0) root         (0)      919 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6195 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12426 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/types.py
--rw-rw-rw-   0 root         (0) root         (0)     4780 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/tools/version.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2022-09-29 07:08:02.000000 momotor-engine-options-0.9.1/src/momotor/options/types.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-10-27 06:26:11.000000 momotor-engine-options-0.9.1/src/momotor/options/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1779 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1495 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      152 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-10-27 06:26:52.000000 momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      778 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2155 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7456 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8245 2023-06-19 07:15:31.000000 momotor-engine-options-1.0.0/src/momotor/options/dependencies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 10:04:04.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 10:04:04.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2023-06-19 07:15:31.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/preflight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3692 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     5329 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/domain/tools/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/filter_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    12223 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 10:04:04.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2022-10-21 07:06:14.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3534 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/keyvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3552 2022-10-27 06:25:56.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)    24941 2023-06-19 07:15:31.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2022-10-27 06:25:56.000000 momotor-engine-options-1.0.0/src/momotor/options/parser/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/result_query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     8918 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/src/momotor/options/task_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6195 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12442 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6076 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/src/momotor/options/tools/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-06 10:02:42.000000 momotor-engine-options-1.0.0/src/momotor/options/types.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-06 10:03:43.000000 momotor-engine-options-1.0.0/src/momotor/options/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:04:25.000000 momotor-engine-options-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7508 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_parser_modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_parser_placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)     9529 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_parser_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_parser_selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8100 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_utils_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2022-09-29 07:08:02.000000 momotor-engine-options-1.0.0/tests/test_utils_tasks.py
```

### Comparing `momotor-engine-options-0.9.1/PKG-INFO` & `momotor-engine-options-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 0.9.1
+Version: 1.0.0
 Summary: Momotor Engine Options Library
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.1/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/1.0.0/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content. 
 
 Momotor accepts digital content as a product bundle and generates a result bundle from this product under
```

### Comparing `momotor-engine-options-0.9.1/README.md` & `momotor-engine-options-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/setup.py` & `momotor-engine-options-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         'Source': 'https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/',
         'Tracker': 'https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues',
     },
     install_requires=[
         'momotor-bundles>=6.0,<8.0',
         'typing-extensions~=4.0',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     extras_require={
         'test': [
             'pytest',
             'pytest-cov',
             'pytest-doctestplus',
             'pytest-pythonpath',
         ],
@@ -54,14 +54,14 @@
     packages=find_namespace_packages(where='src', include=('momotor.*',)),
     package_dir={'': 'src'},
     zip_safe=False,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
     ],
 )
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/convert.py` & `momotor-engine-options-1.0.0/src/momotor/options/convert.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/dependencies.py` & `momotor-engine-options-1.0.0/src/momotor/options/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     if '*' in applied_id or '?' in applied_id:
         applied_id_re = make_result_id_re(applied_id)
         for task_id_str, task_id in task_ids_map.items():
             if applied_id_re.fullmatch(task_id_str):
                 yield task_id
 
     else:
-        task_id = task_ids_map.get(applied_id)
-        if task_id:
-            yield task_id
+        dep_task_id = task_ids_map.get(applied_id)
+        if dep_task_id:
+            yield dep_task_id
         elif applied_id == depend_id_str:
             raise InvalidDependencies(
-                f"Task {task_id!r} depends on non-existent task(s) {depend_id_str!r}"
+                f"Task {str(task_id)!r} depends on non-existent task(s) {depend_id_str!r}"
             )
 
 
 def _reorder_taskids(task_ids: typing.Container[StepTaskId], ordering: typing.Iterable[StepTaskId]) \
         -> typing.Tuple[StepTaskId, ...]:
 
     # Convert a container of StepTaskIds into a tuple, using the order given by `ordering`
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/preflight.py` & `momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/preflight.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 )
 
 # Properties for 'pass-secret' and 'fail-secret' actions
 SECRET_PROPERTIES = {
     'secret': True,
 }
 
+# Properties for 'pass-hidden' and 'fail-hidden' actions
+HIDDEN_PROPERTIES = {
+    **SECRET_PROPERTIES,
+    'hidden': True,
+}
+
 # Properties for 'skip' action
 SKIP_PROPERTIES = {
     'skipped': True,
 }
 
 # Properties for the 'skip-error' action
 SKIP_ERROR_PROPERTIES = {
@@ -84,16 +90,18 @@
 
 ActionType = typing.Tuple[Outcome, typing.Dict]
 
 PREFLIGHT_ACTIONS: typing.Dict[str, typing.Optional[ActionType]] = {
     'run': None,
     'pass': (Outcome.PASS, {}),
     'pass-secret': (Outcome.PASS, SECRET_PROPERTIES),
+    'pass-hidden': (Outcome.PASS, HIDDEN_PROPERTIES),
     'fail': (Outcome.FAIL, {}),
     'fail-secret': (Outcome.FAIL, SECRET_PROPERTIES),
+    'fail-hidden': (Outcome.FAIL, HIDDEN_PROPERTIES),
     'skip': (Outcome.SKIP, SKIP_PROPERTIES),
     'error': (Outcome.ERROR, {}),
     'skip-error': (Outcome.SKIP, SKIP_ERROR_PROPERTIES),
 }
 
 
 def create_preflight_result(
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tasks.py` & `momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/domain/scheduler/tools.py` & `momotor-engine-options-1.0.0/src/momotor/options/domain/scheduler/tools.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/domain/tools/__init__.py` & `momotor-engine-options-1.0.0/src/momotor/options/domain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/filter_files.py` & `momotor-engine-options-1.0.0/src/momotor/options/filter_files.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/option.py` & `momotor-engine-options-1.0.0/src/momotor/options/option.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/consts.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/consts.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/keyvalue.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/keyvalue.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/modifier.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/modifier.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/placeholders.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/reference.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,15 +379,15 @@
 
         _test = lambda obj: obj.outcome_enum == outcome
 
     for obj, ref in objects:
         if ref and ref.name:
             # noinspection PyProtectedMember
             raise ValueError(
-                f"{ref._source!r} is not valid: name or class {ref.name!r} not allowed"
+                f"{ref._source!r} is not valid, name or class {ref.name!r} not allowed"
             )
 
         result = (obj,) if _test(obj) else tuple()
         yield ReferenceMatch(obj, result)
 
 
 def _match_prop_reference(
@@ -397,23 +397,24 @@
 
     for obj, ref in objects:
         if ref is None:
             raise ValueError("a name is required")
         elif ref.name is None:
             # noinspection PyProtectedMember
             raise ValueError(
-                f"{ref._source!r} is not valid: a name is required"
+                f"{ref._source!r} is not valid, a name is required"
             )
 
         name = ref.name
         if task_id:
             try:
                 name = apply_task_number(name, task_id)
             except InvalidDependencies as e:
-                raise ValueError(f"{ref._source!r} is not valid: {e!s}")
+                # noinspection PyProtectedMember
+                raise ValueError(f"{ref._source!r} is not valid, {e!s}")
 
         properties = obj.properties.filter(name=name)
         yield ReferenceMatch(obj, properties)
 
 
 def _match_file_reference(
         objects: typing.Iterable[typing.Tuple[typing.Union[ProviderElement, FilesMixin], Reference]],
@@ -425,21 +426,23 @@
         if ref and ref.name:
             class_, name = _split_name_class(ref.name)
             if task_id:
                 if class_:
                     try:
                         class_ = apply_task_number(class_, task_id)
                     except InvalidDependencies as e:
-                        raise ValueError(f"{ref._source!r} class is not valid: {e!s}")
+                        # noinspection PyProtectedMember
+                        raise ValueError(f"{ref._source!r} class is not valid, {e!s}")
 
                 if name:
                     try:
                         name = apply_task_number(name, task_id)
                     except InvalidDependencies as e:
-                        raise ValueError(f"{ref._source!r} name is not valid: {e!s}")
+                        # noinspection PyProtectedMember
+                        raise ValueError(f"{ref._source!r} name is not valid, {e!s}")
 
             filters = {}
             if name:
                 filters['name__glob'] = name
             if class_:
                 filters['class_'] = class_
 
@@ -455,30 +458,32 @@
 
     for obj, ref in objects:
         if ref is None:
             raise ValueError("a name is required")
         elif ref.name is None:
             # noinspection PyProtectedMember
             raise ValueError(
-                f"{ref._source!r} is not valid: a name is required"
+                f"{ref._source!r} is not valid, a name is required"
             )
 
         name, domain = _split_name_domain(ref.name)
         if task_id:
             if name:
                 try:
                     name = apply_task_number(name, task_id)
                 except InvalidDependencies as e:
-                    raise ValueError(f"{ref._source!r} name is not valid: {e!s}")
+                    # noinspection PyProtectedMember
+                    raise ValueError(f"{ref._source!r} name is not valid, {e!s}")
 
             if domain:
                 try:
                     domain = apply_task_number(domain, task_id)
                 except InvalidDependencies as e:
-                    raise ValueError(f"{ref._source!r} domain is not valid: {e!s}")
+                    # noinspection PyProtectedMember
+                    raise ValueError(f"{ref._source!r} domain is not valid, {e!s}")
 
         options = obj.options.filter(name=name, domain=merge_domains(domain, Option.DEFAULT_DOMAIN))
         yield ReferenceMatch(obj, options)
 
 
 DEFAULT_VALID_PROVIDERS = {
     None: ('result', {'result'}),
@@ -496,15 +501,15 @@
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[type_]
     else:
         default_provider, valid_providers = DEFAULT_VALID_PROVIDERS[None]
 
     for ref in refs:
         provider = ref.provider or default_provider
         if provider is None:
-            raise ValueError(f"no provider")
+            raise ValueError("no provider")
 
         if valid_providers is not None and provider not in valid_providers:
             raise ValueError(f"invalid provider {provider!r}")
 
         if provider == 'recipe' and bundles.recipe:
             if ref.id:
                 raise ValueError('`id` not allowed for @recipe provider')
@@ -580,25 +585,26 @@
              the :token:`~reference:type`,
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     :raises ValueError: the reference cannot be parsed
     """
     reference = reference.strip()
 
-    type_, refs, remainder = parse_reference(reference)
     try:
+        type_, refs, remainder = parse_reference(reference)
+
         if type_:
             items = tuple(generate_reference(type_, refs, bundles))
         else:
             items = tuple()
 
-    except ValueError as exc:
-        raise ValueError(f"Invalid {type_!r} reference {reference!r}: {exc}")
+        return type_, items, remainder
 
-    return type_, items, remainder
+    except ValueError as exc:
+        raise ValueError(f"Invalid {type_!r} reference {reference!r}: {exc}") from None
 
 
 def select_by_prop_reference(reference: str, results: ResultsBundle = None, task_id: StepTaskId = None) \
         -> typing.Tuple[typing.Tuple[ReferenceMatch], str]:
     """ Parse a property :token:`~reference:reference` string and collect the referenced properties.
 
     This is similar to the ``prop[...]`` :ref:`reference syntax <reference>`,
@@ -612,41 +618,41 @@
              a string with the rest of the `reference` string remaining after parsing.
     """
     reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('prop', refs, Providers(results=results, task_id=task_id))
-    except ValueError as exc:
-        raise ValueError(f"Invalid property reference {reference!r}: {exc}")
+        return tuple(_match_prop_reference(objects, task_id)), remainder
 
-    return tuple(_match_prop_reference(objects, task_id)), remainder
+    except ValueError as exc:
+        raise ValueError(f"Invalid property reference {reference!r}: {exc}") from None
 
 
 def select_by_file_reference(reference: str, bundles: Providers) -> typing.Tuple[typing.Tuple[ReferenceMatch], str]:
     """ Parse a file :token:`~reference:reference` string and collect the referenced files.
 
     This is similar to the ``file[...]`` :ref:`reference syntax <reference>`,
     but does not require the ``file`` nor the square brackets.
 
     :param reference: The reference to parse
-    :param bundles: The bundles to resolve the references too
+    :param bundles: The bundles to resolve the references to
     :return: a 2-tuple containing
              a tuple of :py:class:`ReferenceMatch` objects, and
              a string with the rest of the `reference` string remaining after parsing.
     """
     reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('file', refs, bundles)
-    except ValueError as exc:
-        raise ValueError(f"Invalid file reference {reference!r}: {exc}")
+        return tuple(_match_file_reference(objects, bundles.task_id)), remainder
 
-    return tuple(_match_file_reference(objects, bundles.task_id)), remainder
+    except ValueError as exc:
+        raise ValueError(f"Invalid file reference {reference!r}: {exc}") from None
 
 
 def select_by_opt_reference(reference: str, bundles: Providers) -> typing.Tuple[typing.Tuple[ReferenceMatch], str]:
     """ Parse an option :token:`~reference:reference` string and collect the referenced options.
 
     This is similar to the ``opt[...]`` :ref:`reference syntax <reference>`,
     but does not require the ``opt`` nor the square brackets.
@@ -658,45 +664,49 @@
              a string with the rest of the `reference` string remaining after parsing.
     """
     reference = reference.strip()
     refs, remainder = _split_options(reference)
 
     try:
         objects = _get_bundle_objects('opt', refs, bundles)
-    except ValueError as exc:
-        raise ValueError(f"Invalid option reference {reference!r}: {exc}")
+        return tuple(_match_opt_reference(objects, bundles.task_id)), remainder
 
-    return tuple(_match_opt_reference(objects, bundles.task_id)), remainder
+    except ValueError as exc:
+        raise ValueError(f"Invalid option reference {reference!r}: {exc}") from None
 
 
 def resolve_reference_value(
         value_reference: str, bundles: Providers, *,
         default_mod: str = 'join'
 ) -> typing.Tuple[typing.Union[str, int, float, bool, None], str]:
     """ Resolve a :ref:`reference value <reference value>` string into the value
 
     :param value_reference: The :token:`~reference_value:value_reference`
-    :param bundles: The bundles to resolve the references too
+    :param bundles: The bundles to resolve the references to
     :param default_mod: The default :token:`~reference_value:mod`
     :return: The resolved value
     """
-    value_reference = value_reference.strip()
-    mod, remaining = parse_mod(value_reference)
-    type_, refs, remaining = parse_reference(remaining)
-
-    if not type_:
-        return None, value_reference
-
-    matches = tuple(
-        generate_reference(type_, refs, bundles)
-    )
-
-    attr = VALUE_ATTR.get(type_, VALUE_ATTR[None])
-
-    values = collections.deque()
-    for match in matches:
-        if match.values:
-            values.extend(getattr(value, attr, None) for value in match.values)
-        else:
-            values.append(None)
+    try:
+        value_reference = value_reference.strip()
+        mod, remaining = parse_mod(value_reference)
+        type_, refs, remaining = parse_reference(remaining)
+
+        if not type_:
+            return None, value_reference
+
+        matches = tuple(
+            generate_reference(type_, refs, bundles)
+        )
+
+        attr = VALUE_ATTR.get(type_, VALUE_ATTR[None])
+
+        values = collections.deque()
+        for match in matches:
+            if match.values:
+                values.extend(getattr(value, attr, None) for value in match.values)
+            else:
+                values.append(None)
+
+        return apply_combiner_modifier(mod or default_mod, values), remaining
 
-    return apply_combiner_modifier(mod or default_mod, values), remaining
+    except ValueError as exc:
+        raise ValueError(f"Invalid option reference {value_reference!r}: {exc}") from None
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/parser/selector.py` & `momotor-engine-options-1.0.0/src/momotor/options/parser/selector.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/providers.py` & `momotor-engine-options-1.0.0/src/momotor/options/providers.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/result_query.py` & `momotor-engine-options-1.0.0/src/momotor/options/result_query.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/split.py` & `momotor-engine-options-1.0.0/src/momotor/options/split.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/task_id.py` & `momotor-engine-options-1.0.0/src/momotor/options/task_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,25 +161,27 @@
 
     Examples:
 
     >>> tid = StepTaskId('step', (4, 5, 6))
     >>> apply_task_number('test', tid)
     'test'
 
-    # Basic usages
+    Basic usage
+
     >>> apply_task_number('test.$0', tid)
     'test.4'
 
     >>> apply_task_number('test-$0.$1', tid)
     'test-4.5'
 
     >>> apply_task_number('test$1_$2', tid)
     'test5_6'
 
-    # Arithmatic
+    Arithmetic
+
     >>> apply_task_number('test.$0-5.$1-5.$2-5', tid)
     'test.#NEG.0.1'
 
     >>> apply_task_number('test.$0+1.$1+1.$2+1', tid)
     'test.5.6.7'
 
     >>> apply_task_number('test.$0*2.$1*2.$2*2', tid)
@@ -199,15 +201,16 @@
 
     >>> apply_task_number('test.$0+$1+$2', tid)
     'test.15'
 
     >>> apply_task_number('test.$1/0', tid)
     'test.#INF'
 
-    # The $@ placeholder
+    The $@ placeholder
+
     >>> apply_task_number('test.$@', tid)
     'test.4.5.6'
 
     >>> apply_task_number('test-$@tail', tid)
     'test-4.5.6tail'
 
     >>> apply_task_number('test-$@-tail', tid)
@@ -215,29 +218,31 @@
 
     >>> apply_task_number('test-$@.tail', tid)
     'test-4.5.6.tail'
 
     >>> apply_task_number('test-$@999', tid)
     'test-4.5.6999'
 
-    # Escaping $ and operators
+    Escaping $ and operators
 
     >>> apply_task_number('test-\$0', tid)
     'test-$0'
 
     >>> apply_task_number('test.$0\-$1', tid)
     'test.4-5'
 
-    # Invalid references
+    Invalid references
+
     >>> apply_task_number('test.$9', tid)
     Traceback (most recent call last):
     ...
     momotor.bundles.exception.InvalidDependencies: Task 'step.4.5.6' has invalid dependency 'test.$9'
 
-    # Other special cases
+    Other special cases
+
     >>> apply_task_number('test-$X', tid)
     'test-$X'
 
     >>> apply_task_number('test.$1$2', tid)
     'test.56'
 
     >>> apply_task_number('test.$1^4', tid)
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/tools/__init__.py` & `momotor-engine-options-1.0.0/src/momotor/options/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/tools/registry.py` & `momotor-engine-options-1.0.0/src/momotor/options/tools/registry.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/tools/tool.py` & `momotor-engine-options-1.0.0/src/momotor/options/tools/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias  # Python 3.10+
 
 import collections
 import dataclasses
 import functools
 import logging
 import os
 import pathlib
```

### Comparing `momotor-engine-options-0.9.1/src/momotor/options/tools/version.py` & `momotor-engine-options-1.0.0/src/momotor/options/tools/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 import dataclasses
 import functools
 import typing
 
 
+def _partial_tuple(left: tuple, right: tuple) -> bool:
+    """ Returns True if `left` is equal to or a partial version of `right`.
+    """
+    if len(left) > len(right):
+        return False
+
+    for le, re in zip(left, right):
+        if le != re:
+            if isinstance(le, tuple) and isinstance(re, tuple):
+                if not _partial_tuple(le, re):
+                    return False
+            else:
+                return False
+
+    return True
+
+
 @functools.total_ordering
 @dataclasses.dataclass(frozen=True, init=False)
 class ToolVersion:
     """ Represents a tool version string (i.e., a string with dotted version-number parts)
-    and makes it possible to order these.
+    and makes it possible to order these. Also handles sub-version suffixes like 1.0-0, 1.0-1, 1.0-2, etc.
 
     :py:const:`ToolVersion.DEFAULT` is a version constant which is always better than any other version number
 
     >>> _test = lambda x, y: (x < y, x == y, x > y)
 
     >>> _test(ToolVersion('1'), ToolVersion('2'))
     (True, False, False)
@@ -39,14 +56,26 @@
 
     >>> _test(ToolVersion('1.00'), ToolVersion('1.0'))
     (False, True, False)
 
     >>> _test(ToolVersion('1.09'), ToolVersion('1.10'))
     (True, False, False)
 
+    >>> _test(ToolVersion('1.0'), ToolVersion('1.0-0'))
+    (True, False, False)
+
+    >>> _test(ToolVersion('1.0'), ToolVersion('1.0-1'))
+    (True, False, False)
+
+    >>> _test(ToolVersion('1.0-0'), ToolVersion('1.0-1'))
+    (True, False, False)
+
+    >>> _test(ToolVersion('1.0-0'), ToolVersion('1.1'))
+    (True, False, False)
+
     >>> _test(ToolVersion(ToolVersion.DEFAULT), ToolVersion('1'))
     (False, False, True)
 
     >>> _test(ToolVersion('1'), ToolVersion(ToolVersion.DEFAULT))
     (True, False, False)
 
     >>> _test(ToolVersion(ToolVersion.DEFAULT), ToolVersion(ToolVersion.DEFAULT))
@@ -55,37 +84,37 @@
     """
     #: Constant indicating a default version
     DEFAULT: typing.ClassVar[str] = '_'
 
     #: The original value
     value: str
 
-    _version: typing.Tuple[typing.Union[str, int]] = dataclasses.field(repr=False)
+    _version: typing.Tuple[typing.Union[str, typing.Tuple[int]]] = dataclasses.field(repr=False)
 
     def __init__(self, value: str):
         if not isinstance(value, str):
             raise TypeError
         elif not value:
             raise ValueError
 
         object.__setattr__(self, 'value', value)
         object.__setattr__(self, '_version', None)
 
     @property
-    def version(self) -> typing.Tuple[typing.Union[str, int]]:
-        """ A tuple representing the :py:attr:`value` split on the dot character (``.``)
+    def version(self) -> typing.Tuple[typing.Union[str, typing.Tuple[int]]]:
+        """ A tuple representing the :py:attr:`value` split on the dot and dash characters (``.``, ``-``)
         and each part converted to :py:class:`int` if possible, and otherwise an :py:class:`str`.
 
         The special value :py:const:`~ToolVersion.DEFAULT` is converted into an empty tuple.
         """
         def _convert(value):
             if value != self.DEFAULT:
                 for part in value.split('.'):
                     try:
-                        yield int(part)
+                        yield tuple(int(subpart) for subpart in part.split('-'))
                     except ValueError:
                         yield part
 
         if self._version is None:
             object.__setattr__(self, '_version', tuple(_convert(self.value)))
 
         return self._version
@@ -95,14 +124,20 @@
 
         >>> ToolVersion('1').is_partial(ToolVersion('1'))
         True
 
         >>> ToolVersion('1').is_partial(ToolVersion('1.0'))
         True
 
+        >>> ToolVersion('1').is_partial(ToolVersion('1.0-0'))
+        True
+
+        >>> ToolVersion('1.0').is_partial(ToolVersion('1.0-0'))
+        True
+
         >>> ToolVersion('1.0').is_partial(ToolVersion('1'))
         False
 
         >>> ToolVersion('2').is_partial(ToolVersion('1.0'))
         False
 
         >>> ToolVersion('1').is_partial(default_tool_version)
@@ -111,16 +146,15 @@
         >>> default_tool_version.is_partial(ToolVersion('1'))
         True
 
         >>> default_tool_version.is_partial(default_tool_version)
         True
 
         """
-        self_version, other_version = self.version, other.version
-        return other_version[:len(self_version)] == self_version
+        return _partial_tuple(self.version, other.version)
 
     def is_default(self) -> bool:
         return self.value == self.DEFAULT
 
     def __eq__(self, other: "ToolVersion") -> bool:
         return self.version == other.version
 
@@ -132,16 +166,24 @@
             return True
 
         # Python throws a TypeError when attempting to do __lt__ between different types
         # (i.e., `self.version < other.version` will not work for all cases), so we check each element pair
         # separately
         for el1, el2 in zip(self.version, other.version):
             if el1 != el2:
-                if type(el1) == type(el2):
+                if isinstance(el1, tuple) and isinstance(el2, tuple):
+                    for p1, p2 in zip(el1, el2):
+                        if p1 != p2:
+                            return p1 < p2
+
+                    return len(el1) < len(el2)
+
+                elif isinstance(el1, str) and isinstance(el2, str):
                     return el1 < el2
+
                 else:
                     return isinstance(el1, str)  # named versions are less than numeric versions
 
         return len(self.version) < len(other.version)
 
     def __hash__(self):
         return hash(self.version)
```

### Comparing `momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/PKG-INFO` & `momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 0.9.1
+Version: 1.0.0
 Summary: Momotor Engine Options Library
 Home-page: https://momotor.org/
 Author: Erik Scheffers
 Author-email: e.t.j.scheffers@tue.nl
-Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/0.9.1/
+Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/release/1.0.0/
 Project-URL: Source, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: docs
 
 This package is a part of [Momotor](https://momotor.org/), a tool for automated processing of digital content. 
 
 Momotor accepts digital content as a product bundle and generates a result bundle from this product under
```

### Comparing `momotor-engine-options-0.9.1/src/momotor_engine_options.egg-info/SOURCES.txt` & `momotor-engine-options-1.0.0/src/momotor_engine_options.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -32,8 +32,15 @@
 src/momotor/options/tools/types.py
 src/momotor/options/tools/version.py
 src/momotor_engine_options.egg-info/PKG-INFO
 src/momotor_engine_options.egg-info/SOURCES.txt
 src/momotor_engine_options.egg-info/dependency_links.txt
 src/momotor_engine_options.egg-info/not-zip-safe
 src/momotor_engine_options.egg-info/requires.txt
-src/momotor_engine_options.egg-info/top_level.txt
+src/momotor_engine_options.egg-info/top_level.txt
+tests/test_option_definition.py
+tests/test_parser_modifier.py
+tests/test_parser_placeholders.py
+tests/test_parser_reference.py
+tests/test_parser_selector.py
+tests/test_utils_dependencies.py
+tests/test_utils_tasks.py
```

