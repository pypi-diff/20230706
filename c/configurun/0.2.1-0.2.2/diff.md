# Comparing `tmp/configurun-0.2.1.tar.gz` & `tmp/configurun-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configurun-0.2.1.tar", last modified: Tue Jul  4 23:26:10 2023, max compression
+gzip compressed data, was "configurun-0.2.2.tar", last modified: Thu Jul  6 16:11:10 2023, max compression
```

## Comparing `configurun-0.2.1.tar` & `configurun-0.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.245883 configurun-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-04 23:26:00.000000 configurun-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-04 23:26:00.000000 configurun-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-04 23:26:10.245883 configurun-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26717 2023-07-04 23:26:00.000000 configurun-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.233883 configurun-0.2.1/configurun/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.233883 configurun-0.2.1/configurun/app/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/create_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45879 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.237883 configurun-0.2.1/configurun/app/models/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/models/run_queue_console_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/models/run_queue_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/network_main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.237883 configurun-0.2.1/configurun/app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/ui/main_window_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/ui/network_login_widget_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/ui/run_queue_widget_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.237883 configurun-0.2.1/configurun/app/views/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/views/run_queue_tree_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.237883 configurun-0.2.1/configurun/app/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/widgets/network_login_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/app/widgets/run_queue_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.241883 configurun-0.2.1/configurun/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/method_call_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)    54072 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/run_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/run_queue_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/run_queue_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/classes/run_queue_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.241883 configurun-0.2.1/configurun/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/configuration/argparse_to_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/configuration/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/configuration/configuration_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.245883 configurun-0.2.1/configurun/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_configuration_sklearn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.245883 configurun-0.2.1/configurun/examples/example_options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_options/example_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_options/example_sklearn_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/examples/example_target_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.245883 configurun-0.2.1/configurun/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/res/app_resources_rc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.245883 configurun-0.2.1/configurun/server/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-04 23:26:00.000000 configurun-0.2.1/configurun/server/create_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 23:26:10.233883 configurun-0.2.1/configurun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-07-04 23:26:10.000000 configurun-0.2.1/configurun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-04 23:26:10.000000 configurun-0.2.1/configurun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 23:26:10.000000 configurun-0.2.1/configurun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-04 23:26:10.000000 configurun-0.2.1/configurun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-04 23:26:10.000000 configurun-0.2.1/configurun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 23:26:10.249883 configurun-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-04 23:26:00.000000 configurun-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.681369 configurun-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    27030 2023-07-06 16:11:01.000000 configurun-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 16:11:01.000000 configurun-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 16:11:10.681369 configurun-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-07-06 16:11:01.000000 configurun-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/create_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20340 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/run_queue_console_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/models/run_queue_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/network_main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23369 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/main_window_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/network_login_widget_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/ui/run_queue_widget_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/views/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/views/run_queue_tree_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun/app/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/network_login_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/app/widgets/run_queue_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/method_call_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54072 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/classes/run_queue_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/argparse_to_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32209 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/configuration/configuration_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_configuration_sklearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/examples/example_options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/example_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_options/example_sklearn_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/examples/example_target_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1155777 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/res/app_resources_rc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.677369 configurun-0.2.2/configurun/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-06 16:11:01.000000 configurun-0.2.2/configurun/server/create_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:11:10.673369 configurun-0.2.2/configurun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26554 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 16:11:10.000000 configurun-0.2.2/configurun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:11:10.681369 configurun-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-06 16:11:01.000000 configurun-0.2.2/setup.py
```

### Comparing `configurun-0.2.1/LICENSE` & `configurun-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/PKG-INFO` & `configurun-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: configurun
-Version: 0.2.1
-Summary: PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..
+Version: 0.2.2
+Summary: Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely.
 Home-page: https://github.com/Woutah/configurun
 Author: Wouter Stokman
 License: LGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Configurun
@@ -465,32 +465,31 @@
 
 # SSH-tunneling
 
 This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
 
 ## No-hop
 
-A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without permanently port forwarding any ports on the server-side.
 If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
 
 ```bash
 ssh -L 5454:localhost:5454 user@remote_host
 ```
 
 On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
 
 ## Hopping
-
 If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
 This example assumes we have:
 
 - `remote1`: directly accessible from our machine
 - `remote2`: only accessible from `remote1`
 - Using default Configurun-port `5454` on both the client and server-side
 
 We can then connect to `remote2` from our machine using the following command:
 
 ```bash
-ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+ssh -J <username1>@<remote1>, <username2>@<remote2> -L 5454:localhost:5454
 ```
 
-This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
+This example forwards `localhost:5454`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.2.1/README.md` & `configurun-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -455,32 +455,31 @@
 
 # SSH-tunneling
 
 This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
 
 ## No-hop
 
-A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without permanently port forwarding any ports on the server-side.
 If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
 
 ```bash
 ssh -L 5454:localhost:5454 user@remote_host
 ```
 
 On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
 
 ## Hopping
-
 If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
 This example assumes we have:
 
 - `remote1`: directly accessible from our machine
 - `remote2`: only accessible from `remote1`
 - Using default Configurun-port `5454` on both the client and server-side
 
 We can then connect to `remote2` from our machine using the following command:
 
 ```bash
-ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+ssh -J <username1>@<remote1>, <username2>@<remote2> -L 5454:localhost:5454
 ```
 
-This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
+This example forwards `localhost:5454`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.2.1/configurun/app/create_run.py` & `configurun-0.2.2/configurun/app/create_run.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/main_window.py` & `configurun-0.2.2/configurun/app/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 	"""
 	Source of the options. Used to determine whether the options should be saved to a file or to the queue.
 	"""
 	FILE = 0
 	QUEUE = 1
 
 
-class MainWindow():
+class MainWindow(QtCore.QObject):
 	"""
 	The main QT window for this app which provides the user with several tools to edit/manage/run machine learning
 	settings.
 
 	Should be provided with:
 		- A configuration model - manages the creation of new configurations & the ui
 		- A run queue - manages the running of the configurations
@@ -69,14 +69,15 @@
 			run_queue (RunQueue): The runqueue which manages running the configurations
 			window (QtWidgets.QMainWindow): The window in which the app should be built
 			workspace_path (str, optional): The base output-path used for the configurations, logfiles etc.
 				If empty, or folder does not exist, defaults to ~/Configurun/configurations/
 			settings_in_workspace_path (bool, optional): Whether to store the settings in the workspace path or in the default
 				QSettings location. Defaults to True
 		"""
+		super().__init__()
 		self.ui = Ui_MainWindow() # pylint: disable=C0103
 		self.ui.setupUi(window)
 
 		self.window = window
 		self._cur_source = None
 		self._queue_source_id = -1 #The id of the queue item which is currently selected (if cur_source == QUEUE)
 		self._default_splitter_states = {
```

### Comparing `configurun-0.2.1/configurun/app/models/run_queue_console_model.py` & `configurun-0.2.2/configurun/app/models/run_queue_console_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/models/run_queue_table_model.py` & `configurun-0.2.2/configurun/app/models/run_queue_table_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,32 +123,27 @@
 		self.beginResetModel() #Invalidate all data in current views
 		self._run_queue = new_run_queue
 
 		#============= Signal connections linking UI to RunQueue =============
 		for connection in self._run_queue_connections:
 			connection.disconnect()
 
+		#NOTE: runqueue connections are not qt-signals, insertions etc. are not necessarily done in the main thread
 		self._run_queue_connections.append(self._run_queue.queueChanged.connect(self._queue_changed))
 		self._run_queue_connections.append( #On item-insertion in runQueue
 			self._run_queue.allItemsDictInsertion.connect(self._handle_run_queue_insertion)
 		)
 		self._run_queue_connections.append( #On item deletion in runQueue
 			self._run_queue.allItemsDictRemoval.connect(self._handle_run_queue_deletion)
 		)
 		self._run_queue_connections.append(self._run_queue.itemDataChanged.connect(self._run_item_changed))
 		self._run_queue_connections.append(self._run_queue.resetTriggered.connect(self.reset_model))
 		self._run_queue_connections.append(self._run_queue.autoProcessingStateChanged.connect(
 			self.autoprocessing_state_changed))
 
-
-		# self._cur_queue_copy = self._run_queue.get_queue_snapshot_copy()
-		# self._cur_run_list_copy = self._run_queue.get_run_list_snapshot_copy()
-
-
-		# if also_instantiate:
 		self._reset_model()
 		self.endResetModel()
 
 	def stop_autoprocessing(self):
 		"""Signal current runqueue to stop autoqueueing"""
 		self._run_queue.stop_autoprocessing()
```

### Comparing `configurun-0.2.1/configurun/app/network_main_window.py` & `configurun-0.2.2/configurun/app/network_main_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 		- A run queue - manages the running of the configurations
 		- A window - the main window in which the app should be built
 		- workspace_path (str, optional) - the default path to use for the configuration, logfiles etc. If empty, or
 			folder does not exist, defaults to ~/Configurun/configurations/
 		- settings_in_workspace_path (bool, optional) - Whether to store the settings in the workspace path or in the
 			default QSettings location. Defaults to True
 	"""
+	_authenConnectionStateChanged = QtCore.Signal(bool) #Emitted when the connection state changes (True=authenticated)
+		# Copy used to make sure that the signal emitted from the run_queue is emitted in the qt-main thread
+		# (since it's a non-qt signal using PySignal). 
 
 	def __init__(self,
 				configuration_model : ConfigurationModel,
 				run_queue_client : RunQueueClient,
 				window : QtWidgets.QMainWindow,
 				workspace_path : str = "",
 				settings_in_workspace_path : bool = True
@@ -98,16 +101,25 @@
 
 		self.network_connection_parent = QtWidgets.QWidget()
 		self.network_connection_widget = NetworkLoginWidget(self.network_connection_parent, self._settings)
 		self.connection_window.setCentralWidget(self.network_connection_parent)
 		self.server_connection_state_changed(self._run_queue.is_connected_and_authenticated()) #Set initial state
 
 
+		#========= Link runqueue signals to UI updates ===========
+		#NOTE: authenConnectionChanged is a non-main-thread non-qt-signal
+		# as such, we must make sure that updates to the UI are done in the main thread by using a single-shot timer
+		self._authenConnectionStateChanged.connect(self.server_connection_state_changed)
+		self._run_queue.authenConnectionStateChanged.connect(
+			lambda connected : self._authenConnectionStateChanged.emit(connected)
+		)
+
+
+
 		#=========== Link connection view buttons to connection window ==============
-		self._run_queue.authenConnectionStateChanged.connect(self.server_connection_state_changed)
 		self.network_connection_widget.connectClicked.connect(self.connect_to_server)
 		self.network_connection_widget.disconnectClicked.connect(self.disconnect_from_server)
 		self.network_connection_widget.cancelClicked.connect(lambda *_: self.connection_window.close())
 		self.network_connection_widget.cancelClicked.connect(lambda *_: self.network_connection_widget.save_histories())
 
 		self.network_connection_widget.connectClicked.connect(
 			lambda *_: self.network_connection_widget.save_histories()
@@ -171,15 +183,15 @@
 
 			self.run_queue_table_model.reset_model() #Re-request all data from the server
 			self.window.statusBar().showMessage(f"Connected to {cur_ip}:{cur_port}", timeout=0) #Show message until next msg
 
 		else:
 			self.network_connection_widget.client_disconnected()
 			self.connection_window.activateWindow()
-			self.connection_window.show()
+			self.connection_window.show() #Goes wrong here
 			self.window.statusBar().showMessage("Not Connected", timeout=0) #Show message until next msg
 
 
 
 
 	def close_event(self, event: QtGui.QCloseEvent) -> None:
 		self.network_connection_widget.save_histories() #Also save file-edit history
```

### Comparing `configurun-0.2.1/configurun/app/ui/main_window_ui.py` & `configurun-0.2.2/configurun/app/ui/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/ui/network_login_widget_ui.py` & `configurun-0.2.2/configurun/app/ui/network_login_widget_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/ui/run_queue_widget_ui.py` & `configurun-0.2.2/configurun/app/ui/run_queue_widget_ui.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/views/run_queue_tree_view.py` & `configurun-0.2.2/configurun/app/views/run_queue_tree_view.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/widgets/network_login_widget.py` & `configurun-0.2.2/configurun/app/widgets/network_login_widget.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/app/widgets/run_queue_widget.py` & `configurun-0.2.2/configurun/app/widgets/run_queue_widget.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/classes/method_call_interceptor.py` & `configurun-0.2.2/configurun/classes/method_call_interceptor.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/classes/run_queue.py` & `configurun-0.2.2/configurun/classes/run_queue.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/classes/run_queue_client.py` & `configurun-0.2.2/configurun/classes/run_queue_client.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/classes/run_queue_datatypes.py` & `configurun-0.2.2/configurun/classes/run_queue_datatypes.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/classes/run_queue_server.py` & `configurun-0.2.2/configurun/classes/run_queue_server.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/configuration/argparse_to_dataclass.py` & `configurun-0.2.2/configurun/configuration/argparse_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/configuration/base_options.py` & `configurun-0.2.2/configurun/configuration/base_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/configuration/configuration.py` & `configurun-0.2.2/configurun/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/configuration/configuration_model.py` & `configurun-0.2.2/configurun/configuration/configuration_model.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_argparse.py` & `configurun-0.2.2/configurun/examples/example_argparse.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_configuration.py` & `configurun-0.2.2/configurun/examples/example_configuration.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_configuration_sklearn.py` & `configurun-0.2.2/configurun/examples/example_configuration_sklearn.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_options/example_options.py` & `configurun-0.2.2/configurun/examples/example_options/example_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_options/example_sklearn_options.py` & `configurun-0.2.2/configurun/examples/example_options/example_sklearn_options.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/examples/example_target_function.py` & `configurun-0.2.2/configurun/examples/example_target_function.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/res/app_resources_rc.py` & `configurun-0.2.2/configurun/res/app_resources_rc.py`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/configurun/server/create_server.py` & `configurun-0.2.2/configurun/server/create_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 	run_queue_server.terminate() #Disconnect all, stop running and save progress
 	# app.quit()
 
 	log.info("Server cleanup complete, exiting")
 
 def run_server(
 			target_function : typing.Callable,
+			password : str,
 			workspace_path : str = "",
 			run_queue_n_processes : int = 1,
-			password : str = "",
 			hostname : str = "localhost",
 			port : int = 5454,
 			log_level : int = logging.INFO,
 			run_queue_kwargs : typing.Optional[typing.Dict[str, typing.Any]] = None
 		):
 	"""
 	WARNING: RUNNING A SERVER ALLOWS OTHER MACHINES ON THIS NETWORK TO EXECUTE ARBITRARY CODE IF THEY KNOW THE PASSWORD
@@ -99,14 +99,14 @@
 		run_queue_server.run()
 		log.info("Server started, listening for client connections...")
 		while True:
 				time.sleep(1)
 
 	except KeyboardInterrupt:
 		log.info("Received keyboard interrupt, now attempting to cleanup server and close app...")
-	except Exception as e:
-		log.exception(f"{type(e).__name__}: {e}")
+	except Exception as exception: #pylint: disable=broad-except
+		log.exception(f"{type(exception).__name__}: {exception}")
 		log.info("Due to the above unhandled exception, now attempting to cleanup server and close app...")
 	finally:
 		if run_queue_server:
 			_cleanup_server(run_queue_server)
 		exit(0)
```

### Comparing `configurun-0.2.1/configurun.egg-info/PKG-INFO` & `configurun-0.2.2/configurun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: configurun
-Version: 0.2.1
-Summary: PySide6 based user-interface tools to create and manage machine learning training/testing-configurations and run them automatically and/or remotely..
+Version: 0.2.2
+Summary: Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely.
 Home-page: https://github.com/Woutah/configurun
 Author: Wouter Stokman
 License: LGPLv2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Configurun
@@ -465,32 +465,31 @@
 
 # SSH-tunneling
 
 This section contains a quick tutorial on how to use SSH-tunnels to connect to a remote server-instance in case we're not running client and server on the same machine/network.
 
 ## No-hop
 
-A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without opening up any ports on the server-side.
+A SSH-tunnel can be used to forward `localhost:5454` on the client-instance-side to `<remote>:5454` on the server side so we connect to the server instance without permanently port forwarding any ports on the server-side.
 If we can directly SSH into the target machine, we can connect the ports as follows (assuming we're using the default `5454`-port in both the server and client configuration):
 
 ```bash
 ssh -L 5454:localhost:5454 user@remote_host
 ```
 
 On the client-side, we can then connect to the server-instance by using `localhost:5454` as the host and the password we set in the server-instance.
 
 ## Hopping
-
 If we cannot directly access the remote-machine, we can use a 2-step SSH-tunnel to connect to the server-instance.
 This example assumes we have:
 
 - `remote1`: directly accessible from our machine
 - `remote2`: only accessible from `remote1`
 - Using default Configurun-port `5454` on both the client and server-side
 
 We can then connect to `remote2` from our machine using the following command:
 
 ```bash
-ssh -L 5454:localhost:61521 <username>@<remote1-ip> ssh -L 61521:localhost:5454 -N <remote2-ip>
+ssh -J <username1>@<remote1>, <username2>@<remote2> -L 5454:localhost:5454
 ```
 
-This example forwards `localhost:5454`->`remote1:61521`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
+This example forwards `localhost:5454`->`remote2:5454`, so we can connect to the server-instance on `remote2` by using `localhost:5454` as the host and the password we set in the server-instance.
```

### Comparing `configurun-0.2.1/configurun.egg-info/SOURCES.txt` & `configurun-0.2.2/configurun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configurun-0.2.1/setup.py` & `configurun-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """The setup script."""
 from setuptools import setup, find_packages
 
 
 setup(
 	name = "configurun",
-	version= "0.2.1",
+	version= "0.2.2",
 	packages=find_packages('.'),
-    description=("PySide6 based user-interface tools to create and manage machine learning "
-                 "training/testing-configurations and run them automatically and/or remotely.."),
+    description=("Cross-platform user-interface tools to create and manage (machine learning) configurations and run them automatically and remotely."),
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author="Wouter Stokman",
     url="https://github.com/Woutah/configurun",
     license="LGPLv2",
     include_package_data=True,
     install_requires=[ #Generated using pipreqs
         'PySide6>=6.0.0', # Qt for Python, works for 6.5.1.1
         'pathos>=0.3.0', #Works for 0.3.0
         'setuptools>=65.0.0', #Works for 65.5.0
 		'dill>=0.3.0', #Works for 0.3.6
 		'multiprocess>=0.70.00', #Works for 0.70.14
 		'numpydoc>=1.4.0', #Works for 1.5.0
 		'pycryptodome>=3.10.0', #Works for 3.18.0
-        'pyside6-utils==1.2.0',
+        'pyside6-utils>=1.2.0',
         'PySignal>=1.1.1' #Works for 1.1.1,
 	]
 )
```

