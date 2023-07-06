# Comparing `tmp/gdtoolkit-4.0.1.tar.gz` & `tmp/gdtoolkit-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/godot-gdscript-toolkit/godot-gdscript-toolkit/dist/.tmp-rer1ho88/gdtoolkit-4.0.1.tar", last modified: Sat Apr 22 08:51:12 2023, max compression
+gzip compressed data, was "/home/runner/work/godot-gdscript-toolkit/godot-gdscript-toolkit/dist/.tmp-tj9r357v/gdtoolkit-4.1.0.tar", last modified: Thu Jul  6 21:19:34 2023, max compression
```

## Comparing `gdtoolkit-4.0.1.tar` & `gdtoolkit-4.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/class_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/const_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33975 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/expression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/function_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/safety_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/statement_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/formatter/var_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gd2py/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/gdradon/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/linter/
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/basic_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/class_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/design_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/format_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/if_return_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/misc_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/name_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/problem_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/linter/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/comments.lark
--rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/gdscript.lark
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/gdtoolkit/parser/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/gdtoolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 08:51:12.000000 gdtoolkit-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-22 08:50:57.000000 gdtoolkit-4.0.1/tests/test_ast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/common/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/common/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/class_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/const_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34037 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/expression_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/expression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/function_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/safety_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/statement_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/formatter/var_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit/gd2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/gd2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/gd2py/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit/gdradon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/gdradon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/gdradon/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/gdtoolkit/linter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/basic_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/class_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/design_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/format_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/if_return_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/misc_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/name_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/problem_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/linter/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/gdtoolkit/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/parser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/parser/comments.lark
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/parser/gdscript.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/gdtoolkit/parser/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 21:19:33.000000 gdtoolkit-4.1.0/gdtoolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:19:34.000000 gdtoolkit-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-06 21:19:23.000000 gdtoolkit-4.1.0/tests/test_ast.py
```

### Comparing `gdtoolkit-4.0.1/LICENSE` & `gdtoolkit-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/PKG-INFO` & `gdtoolkit-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtoolkit
-Version: 4.0.1
+Version: 4.1.0
 Summary: Independent set of tools for working with GDScript - parser, linter and formatter
 Home-page: https://github.com/Scony/godot-gdscript-toolkit
 Author: Pawel Lampe
 Author-email: pawel.lampe@gmail.com
 License: MIT
 Keywords: GODOT,GDSCRIPT,PARSER,LINTER,FORMATTER
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gdtoolkit-4.0.1/README.md` & `gdtoolkit-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/common/ast.py` & `gdtoolkit-4.1.0/gdtoolkit/common/ast.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/common/utils.py` & `gdtoolkit-4.1.0/gdtoolkit/common/utils.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/__init__.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/__main__.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,17 @@
                     given_code_parse_tree=code_parse_tree,
                     given_code_comment_parse_tree=comment_parse_tree,
                 )
     except lark.exceptions.UnexpectedToken as exception:
         success = False
         print(
             f"{file_path}:\n",
-            lark_unexpected_token_to_str(exception, code),
+            lark_unexpected_token_to_str(
+                exception, formatted_code if actually_formatted else code
+            ),
             sep="\n",
             file=sys.stderr,
         )
     except lark.exceptions.UnexpectedInput as exception:
         success = False
         print(
             f"{file_path}:\n",
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/annotation.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/annotation.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/block.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/block.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/class_statement.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/class_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         "pass_stmt": partial(format_simple_statement, "pass"),
         "enum_stmt": _format_enum_statement,
         "signal_stmt": _format_signal_statement,
         "extends_stmt": _format_extends_statement,
         "classname_stmt": _format_classname_statement,
         "classname_extends_stmt": _format_classname_extends_statement,
         "class_var_stmt": _format_var_statement,
+        "static_class_var_stmt": lambda s, c: _format_var_statement(
+            s.children[0], c, "static "
+        ),
         "const_stmt": format_const_statement,
         "docstr_stmt": _format_docstring_statement,
         "class_def": _format_class_statement,
         "func_def": _format_func_statement,
         "static_func_def": lambda s, c: _format_func_statement(
             s.children[0], c, "static "
         ),
@@ -116,16 +119,20 @@
                 optional_attributes,
             ),
         )
     ]
     return (formatted_lines, last_processed_line_no)
 
 
-def _format_var_statement(statement: Tree, context: Context) -> Outcome:
-    formatted_lines, last_processed_line = format_var_statement(statement, context)
+def _format_var_statement(
+    statement: Tree, context: Context, prefix: str = ""
+) -> Outcome:
+    formatted_lines, last_processed_line = format_var_statement(
+        statement, context, prefix
+    )
     concrete_var_statement = statement.children[0]
     if has_inline_property_body(concrete_var_statement):
         inline_property_body = concrete_var_statement.children[-1]
         formatted_lines = formatted_lines[:-1] + append_property_body_to_formatted_line(
             formatted_lines[-1], inline_property_body, context
         )
     return formatted_lines, last_processed_line
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/comments.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/comments.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/const_statement.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/const_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/constants.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/constants.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/context.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/context.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/exceptions.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/exceptions.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/expression.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,18 @@
     )
     formatted_lines += lines
     operator_expr_chain = zip(expression.children[1::2], expression.children[2::2])
     for operator, child in operator_expr_chain:
         lines = _format_concrete_expression(
             child,
             ExpressionContext(
-                f"{operator.value} ", get_line(child), "", get_end_line(child)
+                f"{expression_to_str(operator)} ",
+                get_line(child),
+                "",
+                get_end_line(child),
             ),
             context,
         )
         formatted_lines += lines
     return formatted_lines
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/expression_to_str.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/expression_to_str.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "and_test": _operator_chain_based_expression_to_str,
         "asless_and_test": _operator_chain_based_expression_to_str,
         "asless_actual_not_test": lambda e: "{}{}{}".format(
             expression_to_str(e.children[0]),
             "" if e.children[0].value == "!" else " ",
             expression_to_str(e.children[1]),
         ),
+        "not_in_op": lambda _: "not in",
         "content_test": _operator_chain_based_expression_to_str,
         "asless_content_test": _operator_chain_based_expression_to_str,
         "comparison": _operator_chain_based_expression_to_str,
         "asless_comparison": _operator_chain_based_expression_to_str,
         "bitw_or": _operator_chain_based_expression_to_str,
         "asless_bitw_or": _operator_chain_based_expression_to_str,
         "bitw_xor": _operator_chain_based_expression_to_str,
@@ -179,15 +180,15 @@
     }[expression.data](expression)
 
 
 def _operator_chain_based_expression_to_str(expression: Tree) -> str:
     operator_expr_chain = zip(expression.children[1::2], expression.children[2::2])
 
     def _padding(operator):
-        return "" if operator.value == "." else " "
+        return "" if expression_to_str(operator).startswith(".") else " "
 
     chain = [
         "{}{}{}{}".format(
             _padding(operator),
             expression_to_str(operator),
             _padding(operator),
             expression_to_str(expr),
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/expression_utils.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/expression_utils.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/formatter.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/function_statement.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/function_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/property.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/property.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/safety_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/safety_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/formatter/var_statement.py` & `gdtoolkit-4.1.0/gdtoolkit/formatter/var_statement.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/gd2py/__init__.py` & `gdtoolkit-4.1.0/gdtoolkit/gd2py/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/gd2py/__main__.py` & `gdtoolkit-4.1.0/gdtoolkit/gd2py/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/gdradon/__main__.py` & `gdtoolkit-4.1.0/gdtoolkit/gdradon/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/__init__.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/__init__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/__main__.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/basic_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/basic_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/class_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/class_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/design_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/design_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/format_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/format_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/if_return_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/if_return_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/misc_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/misc_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/linter/name_checks.py` & `gdtoolkit-4.1.0/gdtoolkit/linter/name_checks.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/parser/__main__.py` & `gdtoolkit-4.1.0/gdtoolkit/parser/__main__.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit/parser/gdscript.lark` & `gdtoolkit-4.1.0/gdtoolkit/parser/gdscript.lark`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ?single_class_stmt: pass_stmt
                   | enum_stmt
                   | signal_stmt
                   | extends_stmt
                   | classname_extends_stmt
                   | classname_stmt
                   | class_var_stmt
+                  | "static" class_var_stmt -> static_class_var_stmt
                   | const_stmt
                   | docstr_stmt
 ?compound_class_stmt: class_def
                     | property_body_def
                     | func_def
                     | "static" func_def -> static_func_def
 annotation: "@" NAME [annotation_args]
@@ -169,17 +170,19 @@
           | actual_type_cast (("and" | "&&") asless_not_test)+
 !?asless_and_test: asless_not_test (("and" | "&&") asless_not_test)*
 ?not_test: content_test
          | asless_actual_not_test
 !?asless_actual_not_test: ("not" | "!") asless_not_test
 ?asless_not_test: asless_content_test
                 | asless_actual_not_test
-!?content_test: comparison ("in" asless_comparison)*
-              | actual_type_cast ("in" asless_comparison)+
-!?asless_content_test: asless_comparison ("in" asless_comparison)*
+not_in_op: "not" "in"
+!_content_test_op: not_in_op | "in"
+!?content_test: comparison (_content_test_op asless_comparison)*
+              | actual_type_cast (_content_test_op asless_comparison)+
+!?asless_content_test: asless_comparison (_content_test_op asless_comparison)*
 ?comparison: bitw_or [_comp_op asless_bitw_or]
            | actual_type_cast _comp_op asless_bitw_or
 ?asless_comparison: asless_bitw_or [_comp_op asless_bitw_or]
 !_comp_op: ">" | "<" | "==" | "!=" | "<=" | ">="
 !?bitw_or: bitw_xor ("|" asless_bitw_xor)*
          | actual_type_cast ("|" asless_bitw_xor)+
 !?asless_bitw_or: asless_bitw_xor ("|" asless_bitw_xor)*
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit/parser/parser.py` & `gdtoolkit-4.1.0/gdtoolkit/parser/parser.py`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/gdtoolkit.egg-info/PKG-INFO` & `gdtoolkit-4.1.0/gdtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtoolkit
-Version: 4.0.1
+Version: 4.1.0
 Summary: Independent set of tools for working with GDScript - parser, linter and formatter
 Home-page: https://github.com/Scony/godot-gdscript-toolkit
 Author: Pawel Lampe
 Author-email: pawel.lampe@gmail.com
 License: MIT
 Keywords: GODOT,GDSCRIPT,PARSER,LINTER,FORMATTER
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gdtoolkit-4.0.1/gdtoolkit.egg-info/SOURCES.txt` & `gdtoolkit-4.1.0/gdtoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdtoolkit-4.0.1/setup.py` & `gdtoolkit-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name="gdtoolkit",
-    version="4.0.1",
+    version="4.1.0",
     description="Independent set of tools for working with GDScript - parser, linter and formatter",
     keywords=["GODOT", "GDSCRIPT", "PARSER", "LINTER", "FORMATTER"],
     url="https://github.com/Scony/godot-gdscript-toolkit",
     author="Pawel Lampe",
     author_email="pawel.lampe@gmail.com",
     license="MIT",
     packages=[
```

### Comparing `gdtoolkit-4.0.1/tests/test_ast.py` & `gdtoolkit-4.1.0/tests/test_ast.py`

 * *Files identical despite different names*

