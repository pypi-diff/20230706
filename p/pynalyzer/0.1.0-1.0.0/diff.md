# Comparing `tmp/pynalyzer-0.1.0.tar.gz` & `tmp/pynalyzer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynalyzer-0.1.0.tar", max compression
+gzip compressed data, was "pynalyzer-1.0.0.tar", max compression
```

## Comparing `pynalyzer-0.1.0.tar` & `pynalyzer-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,20 @@
--rw-r--r--   0        0        0        0 2023-06-28 14:58:36.570838 pynalyzer-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-28 14:58:36.570838 pynalyzer-0.1.0/pynalyzer/__init__.py
--rw-r--r--   0        0        0      595 2023-06-28 15:05:28.961462 pynalyzer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 pynalyzer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:12:23.507916 pynalyzer-1.0.0/LICENSE
+-rw-r--r--   0        0        0     8255 2023-07-06 12:49:38.358014 pynalyzer-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:38.358014 pynalyzer-1.0.0/pynalyzer/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:38.358014 pynalyzer-1.0.0/pynalyzer/commands_handling/__init__.py
+-rw-r--r--   0        0        0      422 2023-07-06 12:49:38.358014 pynalyzer-1.0.0/pynalyzer/commands_handling/command_executor.py
+-rw-r--r--   0        0        0     1712 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/commands_handling/command_preparer.py
+-rw-r--r--   0        0        0      464 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/commands_handling/command_runner.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/configuration_parsing/__init__.py
+-rw-r--r--   0        0        0      197 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/configuration_parsing/configuration.py
+-rw-r--r--   0        0        0     1249 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/configuration_parsing/configuration_decoder.py
+-rw-r--r--   0        0        0     1259 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/configuration_parsing/configuration_parser.py
+-rw-r--r--   0        0        0      815 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/configuration_parsing/configuration_path_finder.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/scripts/__init__.py
+-rw-r--r--   0        0        0      895 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/scripts/entrypoint.py
+-rw-r--r--   0        0        0        0 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/utils/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/utils/constants.py
+-rw-r--r--   0        0        0      307 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/utils/converters.py
+-rw-r--r--   0        0        0     1006 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pynalyzer/utils/exceptions.py
+-rw-r--r--   0        0        0     2355 2023-07-06 12:49:38.359014 pynalyzer-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9723 1970-01-01 00:00:00.000000 pynalyzer-1.0.0/PKG-INFO
```

