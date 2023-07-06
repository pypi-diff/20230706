# Comparing `tmp/nuclear-1.4.1.tar.gz` & `tmp/nuclear-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuclear-1.4.1.tar", last modified: Mon Apr 17 13:48:22 2023, max compression
+gzip compressed data, was "nuclear-1.4.2.tar", last modified: Thu Jul  6 10:51:27 2023, max compression
```

## Comparing `nuclear-1.4.1.tar` & `nuclear-1.4.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.939554 nuclear-1.4.1/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.1/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-04-17 13:48:22.939554 nuclear-1.4.1/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18082 2023-04-17 13:48:22.000000 nuclear-1.4.1/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      564 2023-04-07 09:00:07.000000 nuclear-1.4.1/nuclear/__init__.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/args/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/args_que.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/args/container.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/autocomplete/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/autocomplete/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/autocomplete/autocomplete.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.1/nuclear/autocomplete/install.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/builder/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/builder/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.1/nuclear/builder/builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.1/nuclear/builder/decorator_builder.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/builder/rule.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.1/nuclear/builder/rule_factory.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/builder/typedef.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/completers/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/completers/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/completers/file.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/help/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/help/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.1/nuclear/help/help.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/inspection/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.1/nuclear/inspection/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    11910 2023-04-12 16:51:53.000000 nuclear-1.4.1/nuclear/inspection/inspection.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/parser/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/context.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/error.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/parser/inject.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/internal_vars.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/keyword.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/matcher.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.1/nuclear/parser/parser.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/parser/transform.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.1/nuclear/parser/validate.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.1/nuclear/parser/value.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/shell/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.1/nuclear/shell/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.1/nuclear/shell/background_cmd.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.1/nuclear/shell/shell_utils.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/sublog/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.1/nuclear/sublog/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.1/nuclear/sublog/catch.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.1/nuclear/sublog/context_logger.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.1/nuclear/sublog/wrap_error.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear/types/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/boolean.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/filesystem.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/types/time.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.939554 nuclear-1.4.1/nuclear/utils/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.1/nuclear/utils/__init__.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.1/nuclear/utils/files.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/input.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.1/nuclear/utils/regex.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.1/nuclear/utils/shell.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/strings.py
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.1/nuclear/utils/time.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-04-17 13:46:38.000000 nuclear-1.4.1/nuclear/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-17 13:48:22.935554 nuclear-1.4.1/nuclear.egg-info/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-04-17 13:48:22.000000 nuclear-1.4.1/nuclear.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-04-17 13:48:22.939554 nuclear-1.4.1/setup.cfg
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.1/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2020-07-28 11:14:52.000000 nuclear-1.4.2/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-06 10:51:27.382318 nuclear-1.4.2/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18082 2023-07-06 10:51:27.000000 nuclear-1.4.2/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      564 2023-04-07 09:00:07.000000 nuclear-1.4.2/nuclear/__init__.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/args/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1399 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/args_que.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      504 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/args/container.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/autocomplete/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/autocomplete/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     4445 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/autocomplete/autocomplete.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     2175 2022-04-12 16:38:36.000000 nuclear-1.4.2/nuclear/autocomplete/install.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/builder/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/builder/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     9263 2022-04-13 09:01:27.000000 nuclear-1.4.2/nuclear/builder/builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3752 2022-04-13 09:02:59.000000 nuclear-1.4.2/nuclear/builder/decorator_builder.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2974 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/builder/rule.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11321 2022-04-13 09:13:28.000000 nuclear-1.4.2/nuclear/builder/rule_factory.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      227 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/builder/typedef.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/completers/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       33 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/completers/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      739 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/completers/file.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/help/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/help/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    11775 2023-03-13 13:40:47.000000 nuclear-1.4.2/nuclear/help/help.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear/inspection/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2023-04-03 14:03:48.000000 nuclear-1.4.2/nuclear/inspection/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    12596 2023-07-06 10:47:26.000000 nuclear-1.4.2/nuclear/inspection/inspection.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/parser/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      442 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/context.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      449 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/error.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1843 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/parser/inject.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      326 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/internal_vars.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      666 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/keyword.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1378 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/matcher.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)    12607 2022-05-12 13:06:55.000000 nuclear-1.4.2/nuclear/parser/parser.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      409 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/parser/transform.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3826 2021-12-11 21:16:15.000000 nuclear-1.4.2/nuclear/parser/validate.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1886 2022-05-13 09:22:45.000000 nuclear-1.4.2/nuclear/parser/value.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/shell/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      123 2022-05-16 13:47:34.000000 nuclear-1.4.2/nuclear/shell/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4734 2022-08-16 13:22:26.000000 nuclear-1.4.2/nuclear/shell/background_cmd.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     3676 2022-05-16 13:53:00.000000 nuclear-1.4.2/nuclear/shell/shell_utils.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/sublog/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      309 2022-06-08 11:51:00.000000 nuclear-1.4.2/nuclear/sublog/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3546 2022-06-08 12:00:57.000000 nuclear-1.4.2/nuclear/sublog/catch.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     4039 2022-04-13 09:02:02.000000 nuclear-1.4.2/nuclear/sublog/context_logger.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      843 2022-06-08 12:04:08.000000 nuclear-1.4.2/nuclear/sublog/wrap_error.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/types/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)       94 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/boolean.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      358 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/filesystem.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1189 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/types/time.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.382318 nuclear-1.4.2/nuclear/utils/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)        0 2022-04-12 16:16:19.000000 nuclear-1.4.2/nuclear/utils/__init__.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      116 2022-08-24 14:04:56.000000 nuclear-1.4.2/nuclear/utils/files.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      138 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/input.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)     1301 2022-08-24 13:59:25.000000 nuclear-1.4.2/nuclear/utils/regex.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      112 2022-04-12 16:39:09.000000 nuclear-1.4.2/nuclear/utils/shell.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      688 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/strings.py
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      362 2020-07-28 11:14:52.000000 nuclear-1.4.2/nuclear/utils/time.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2023-07-06 10:50:19.000000 nuclear-1.4.2/nuclear/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2023-07-06 10:51:27.378318 nuclear-1.4.2/nuclear.egg-info/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)    18534 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1496 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       48 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        8 2023-07-06 10:51:27.000000 nuclear-1.4.2/nuclear.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2023-07-06 10:51:27.382318 nuclear-1.4.2/setup.cfg
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      866 2022-04-13 08:25:38.000000 nuclear-1.4.2/setup.py
```

### Comparing `nuclear-1.4.1/LICENSE` & `nuclear-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/PKG-INFO` & `nuclear-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.1
+Version: 1.4.2
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nuclear-1.4.1/README.md` & `nuclear-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/__init__.py` & `nuclear-1.4.2/nuclear/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/args/args_que.py` & `nuclear-1.4.2/nuclear/args/args_que.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/autocomplete/autocomplete.py` & `nuclear-1.4.2/nuclear/autocomplete/autocomplete.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/autocomplete/install.py` & `nuclear-1.4.2/nuclear/autocomplete/install.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/builder/builder.py` & `nuclear-1.4.2/nuclear/builder/builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/builder/decorator_builder.py` & `nuclear-1.4.2/nuclear/builder/decorator_builder.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/builder/rule.py` & `nuclear-1.4.2/nuclear/builder/rule.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/builder/rule_factory.py` & `nuclear-1.4.2/nuclear/builder/rule_factory.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/completers/file.py` & `nuclear-1.4.2/nuclear/completers/file.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/help/help.py` & `nuclear-1.4.2/nuclear/help/help.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/inspection/inspection.py` & `nuclear-1.4.2/nuclear/inspection/inspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import sys
 from typing import Any, Dict, List, Optional, Type, Iterable, Union
 
 
 @dataclass
 class InspectConfig:
-    attr: bool
+    short: bool
     dunder: bool
     docs: bool
     long: bool
     code: bool
 
 
 @dataclass
@@ -26,57 +26,57 @@
     signature: Optional[str]
     doc: Optional[str]
 
 
 def inspect(
     obj: Any,
     *,
-    attr: bool = True,
+    short: bool = False,
     dunder: bool = False,
     docs: bool = True,
     long: bool = False,
     code: bool = False,
     all: bool = False,
 ):
     """
     Examine the object's information, such as its type, formatted value, variables, methods,
     documentation or source code.
     :param obj: object to inspect
-    :param attr: whether to print attributes (variables and methods)
+    :param short: whether to print short output without attributes (neither variables nor methods)
     :param dunder: whether to print dunder attributes
     :param docs: whether to print documentation for functions and classes
     :param long: whether to print non-abbreviated values and documentation
     :param code: whether to print source code of a function, method or class
     :param all: whether to include all information
     """
     print(inspect_format(
-        obj, attr=attr or all, dunder=dunder or all, long=long or all, docs=docs or all,
-        code=code or all))
+        obj, short=short, dunder=dunder or all, long=long or all, docs=docs or all, code=code or all
+    ))
 
 
 def insp(obj: Any, **kwargs):
     """Inspect object's attributes (variables and methods)"""
     inspect(obj, **kwargs)
 
 
 def ins(obj: Any, **kwargs):
     """Inspect object's short, elementary data: value, type, signature"""
-    inspect(obj, attr=False, **kwargs)
+    inspect(obj, short=True, **kwargs)
 
 
 def inspect_format(
     obj: Any,
     *,
-    attr: bool = True,
+    short: bool = False,
     dunder: bool = False,
     docs: bool = True,
     long: bool = False,
     code: bool = False,
 ) -> str:
-    config = InspectConfig(attr=attr, dunder=dunder, docs=docs, long=long, code=code)
+    config = InspectConfig(short=short, dunder=dunder, docs=docs, long=long, code=code)
 
     str_value = _format_value(obj)
     str_type = _format_type(type(obj))
     output: List[str] = [
         f'{STYLE_BRIGHT_BLUE}value:{RESET} {str_value}',
         f'{STYLE_BRIGHT_BLUE}type:{RESET} {STYLE_BRIGHT_YELLOW}{str_type}{RESET}',
     ]
@@ -94,15 +94,15 @@
             output.extend([f'{STYLE_GRAY}"""', doc, f'"""{RESET}'])
 
     if config.code and (std_inspect.isclass(obj) or callable(obj)):
         source = _get_source_code(obj)
         if source:
             output.append(f'{STYLE_BRIGHT_BLUE}source code:{RESET}\n{source}')
 
-    if config.attr:
+    if not config.short:
         attributes = sorted(_iter_attributes(obj, config), key=lambda attr: attr.name)
         output.extend(_render_attrs_section(attributes, config))
 
     if sys.stdout.isatty():  # horizontal bar
         terminal_width = os.get_terminal_size().columns
         output.insert(0, STYLE_BLUE + '─' * terminal_width + RESET)
         output.append(STYLE_BLUE + '─' * terminal_width + RESET)
@@ -112,32 +112,41 @@
         text = _strip_color(text)
     return text
 
 
 def _iter_attributes(obj: Any, config: InspectConfig) -> Iterable[InspectAttribute]:
     keys = dir(obj)
     for key in keys:
-        value = getattr(obj, key)
-        callable_ = callable(value)
         dunder = key.startswith('__') and key.endswith('__')
+        if dunder and not config.dunder:
+            continue
         private = key.startswith('_') and not dunder
+        value = _get_attribute_value(obj, key)
+        callable_ = callable(value)
         signature = _get_callable_signature(key, value) if callable_ else None
         doc = _get_doc(value, long=config.long) if callable_ else None
         yield InspectAttribute(
             name=key,
             value=value,
             type=type(value),
             callable=callable_,
             dunder=dunder,
             private=private,
             signature=signature,
             doc=doc,
         )
 
 
+def _get_attribute_value(obj: Any, key: str) -> Any:
+    try:
+        return getattr(obj, key)
+    except AttributeError as e:
+        return e
+
+
 def _get_callable_signature(name: str, obj: Any) -> Optional[str]:
     try:
         _signature = str(std_inspect.signature(obj))
     except (ValueError, TypeError):
         _signature = "(…)"
     
     if std_inspect.isclass(obj):
@@ -203,17 +212,17 @@
 
 def _format_value(value: Any, indent: int = 0) -> str:
     if isinstance(value, str):
         return f"{STYLE_GREEN}'{value}'{RESET}"
     if value is None:
         return f'{STYLE_MAGENTA}None{RESET}'
     if value is True:
-        return f'{STYLE_GREEN}True{RESET}'
+        return f'{STYLE_BRIGHT_GREEN}True{RESET}'
     if value is False:
-        return f'{STYLE_RED}False{RESET}'
+        return f'{STYLE_BRIGHT_RED}False{RESET}'
     if isinstance(value, (int, float)):
         return f'{STYLE_RED}{value}{RESET}'
     if isinstance(value, dict):
         return _format_dict_value(value, indent=indent+1)
     if isinstance(value, list):
         return _format_list_value(value, indent=indent+1)
     return str(value)
@@ -315,24 +324,26 @@
         self._print_help()
         return ''
         
     def __str__(self) -> str:
         return '<nuclear Wat Inspector object>'
     
     def _print_help(self):
-        print("""
-Try `wat / object`, `wat(**options) / object` or `wat(object, **options)` to inspect an object.
-options are:
-  attr=False to hide attributes (variables and methods)
-  dunder=True to print dunder attributes
-  docs=False to hide documentation for functions and classes
-  long=True to print non-abbreviated values and documentation
-  code=True to print source code of a function, method or class
-  all=True to include all information
-""".strip())
+        text = f"""
+Try `{STYLE_YELLOW}wat / object{RESET}`, `{STYLE_YELLOW}wat(**options) / object{RESET}` or `{STYLE_YELLOW}wat(object, **options){RESET}` to inspect an {STYLE_YELLOW}object{RESET}. Options are:
+  {STYLE_GREEN}short={STYLE_BRIGHT_GREEN}True{RESET} to hide attributes (variables and methods)
+  {STYLE_GREEN}dunder={STYLE_BRIGHT_GREEN}True{RESET} to print dunder attributes
+  {STYLE_GREEN}docs={STYLE_BRIGHT_RED}False{RESET} to hide documentation for functions and classes
+  {STYLE_GREEN}long={STYLE_BRIGHT_GREEN}True{RESET} to print non-abbreviated values and documentation
+  {STYLE_GREEN}code={STYLE_BRIGHT_GREEN}True{RESET} to print source code of a function, method or class
+  {STYLE_GREEN}all={STYLE_BRIGHT_GREEN}True{RESET} to include all information
+""".strip()
+        if not sys.stdout.isatty():
+            text = _strip_color(text)
+        print(text)
 
     def _react_with(self, other: Any) -> None:
         inspect(other, **self._params)
     
     def __call__(self, *args: Any, **kwargs: Any) -> Union['Wat', None]:
         if args:
             inspect(*args, **kwargs)
```

### Comparing `nuclear-1.4.1/nuclear/parser/inject.py` & `nuclear-1.4.2/nuclear/parser/inject.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/parser/keyword.py` & `nuclear-1.4.2/nuclear/parser/keyword.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/parser/matcher.py` & `nuclear-1.4.2/nuclear/parser/matcher.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/parser/parser.py` & `nuclear-1.4.2/nuclear/parser/parser.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/parser/validate.py` & `nuclear-1.4.2/nuclear/parser/validate.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/parser/value.py` & `nuclear-1.4.2/nuclear/parser/value.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/shell/background_cmd.py` & `nuclear-1.4.2/nuclear/shell/background_cmd.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/shell/shell_utils.py` & `nuclear-1.4.2/nuclear/shell/shell_utils.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/sublog/catch.py` & `nuclear-1.4.2/nuclear/sublog/catch.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/sublog/context_logger.py` & `nuclear-1.4.2/nuclear/sublog/context_logger.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/sublog/wrap_error.py` & `nuclear-1.4.2/nuclear/sublog/wrap_error.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/types/time.py` & `nuclear-1.4.2/nuclear/types/time.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/utils/regex.py` & `nuclear-1.4.2/nuclear/utils/regex.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear/utils/strings.py` & `nuclear-1.4.2/nuclear/utils/strings.py`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/nuclear.egg-info/PKG-INFO` & `nuclear-1.4.2/nuclear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclear
-Version: 1.4.1
+Version: 1.4.2
 Summary: Declarative parser for command line interfaces
 Home-page: https://github.com/igrek51/nuclear
 Author: igrek51
 Author-email: igrek51.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nuclear-1.4.1/nuclear.egg-info/SOURCES.txt` & `nuclear-1.4.2/nuclear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclear-1.4.1/setup.py` & `nuclear-1.4.2/setup.py`

 * *Files identical despite different names*

