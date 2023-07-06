# Comparing `tmp/otter-grader-4.3.4.tar.gz` & `tmp/otter-grader-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-4.3.4.tar", last modified: Wed Jun 21 05:13:00 2023, max compression
+gzip compressed data, was "otter-grader-4.4.0.tar", last modified: Thu Jul  6 03:08:29 2023, max compression
```

## Comparing `otter-grader-4.3.4.tar` & `otter-grader-4.4.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 05:12:29.000000 otter-grader-4.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-21 05:12:29.000000 otter-grader-4.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-21 05:13:00.167218 otter-grader-4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-21 05:12:29.000000 otter-grader-4.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/cell_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/v0/convert/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/convert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/convert/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/v0/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/r_adapter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.159218 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/assign/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/execute/execute_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/execute/execute_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/execute/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.155218 otter-grader-4.3.4/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/python/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-21 05:12:58.000000 otter-grader-4.3.4/otter/generate/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/python/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/python/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/r/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/r/requirements.r
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 05:12:58.000000 otter-grader-4.3.4/otter/generate/templates/r/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/r/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/r/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.163218 otter-grader-4.3.4/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-21 05:12:58.000000 otter-grader-4.3.4/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-21 05:12:30.000000 otter-grader-4.3.4/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-21 05:12:58.000000 otter-grader-4.3.4/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-21 05:12:59.000000 otter-grader-4.3.4/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-21 05:13:00.000000 otter-grader-4.3.4/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 05:12:59.000000 otter-grader-4.3.4/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-21 05:12:59.000000 otter-grader-4.3.4/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 05:12:59.000000 otter-grader-4.3.4/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 05:12:59.000000 otter-grader-4.3.4/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 05:12:58.000000 otter-grader-4.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 05:13:00.167218 otter-grader-4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-21 05:12:30.000000 otter-grader-4.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 05:13:00.167218 otter-grader-4.3.4/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 05:12:30.000000 otter-grader-4.3.4/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-06 03:07:57.000000 otter-grader-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-06 03:07:57.000000 otter-grader-4.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 03:08:29.214744 otter-grader-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-06 03:07:57.000000 otter-grader-4.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/cell_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/convert/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.202744 otter-grader-4.4.0/otter/assign/v0/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/r_adapter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/assign/v0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/execute_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/execute_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/execute/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.198744 otter-grader-4.4.0/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.206744 otter-grader-4.4.0/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/generate/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/requirements.r
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/generate/templates/r/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-06 03:07:57.000000 otter-grader-4.4.0/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 03:08:27.000000 otter-grader-4.4.0/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.210744 otter-grader-4.4.0/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-06 03:08:29.000000 otter-grader-4.4.0/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 03:08:28.000000 otter-grader-4.4.0/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-06 03:07:57.000000 otter-grader-4.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 03:08:29.214744 otter-grader-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-06 03:07:57.000000 otter-grader-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-06 03:08:27.000000 otter-grader-4.4.0/test/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:08:29.214744 otter-grader-4.4.0/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_grade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-06 03:07:57.000000 otter-grader-4.4.0/test/test_utils.py
```

### Comparing `otter-grader-4.3.4/LICENSE` & `otter-grader-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/PKG-INFO` & `otter-grader-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.3.4
+Version: 4.4.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.3.4/README.md` & `otter-grader-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/api.py` & `otter-grader-4.4.0/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/__init__.py` & `otter-grader-4.4.0/otter/assign/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         plugins, pc = assignment.plugins, None
         if plugins:
             LOGGER.debug("Processing plugins")
             pc = PluginCollection(plugins, "", {})
             pc.run("during_assign", assignment)
             if assignment.generate_enabled:
                 LOGGER.debug("Adding plugin configurations to Otter Generate configuration")
-                assignment.generate.plugins.extend(plugins)
+                assignment.generate.plugins = assignment.generate.plugins + plugins
 
         # generate Gradescope autograder zipfile
         if assignment.generate_enabled:
             LOGGER.info("Generating autograder zipfile")
             run_generate_autograder(assignment, username, password, plugin_collection=pc)
 
         # generate PDF of solutions
```

### Comparing `otter-grader-4.3.4/otter/assign/assignment.py` & `otter-grader-4.4.0/otter/assign/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/blocks.py` & `otter-grader-4.4.0/otter/assign/blocks.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/cell_factory.py` & `otter-grader-4.4.0/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/feature_toggle.py` & `otter-grader-4.4.0/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/notebook_transformer.py` & `otter-grader-4.4.0/otter/assign/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/output.py` & `otter-grader-4.4.0/otter/assign/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/plugins.py` & `otter-grader-4.4.0/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/question_config.py` & `otter-grader-4.4.0/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/r_adapter/cell_factory.py` & `otter-grader-4.4.0/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-4.4.0/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/r_adapter/solutions.py` & `otter-grader-4.4.0/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/r_adapter/tests_manager.py` & `otter-grader-4.4.0/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/solutions.py` & `otter-grader-4.4.0/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/tests_manager.py` & `otter-grader-4.4.0/otter/assign/tests_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,10 +378,14 @@
         if len(test_cases) == 0:
             if question.points is None and question.manual:
                 raise ValueError(
                     f"Point value unspecified for question with no test cases: {question.name}")
 
             return question.points if question.points is not None else 1
 
-        resolved_test_cases = TestFile.resolve_test_file_points(question.points, test_cases)
+        try:
+            resolved_test_cases = TestFile.resolve_test_file_points(question.points, test_cases)
+        except Exception as e:
+            raise type(e)(f"Error in \"{question.name}\" test cases: {e}")
+
         points = round(sum(tc.points for tc in resolved_test_cases), 5)
         return int(points) if points % 1 == 0 else points
```

### Comparing `otter-grader-4.3.4/otter/assign/utils.py` & `otter-grader-4.4.0/otter/assign/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/__init__.py` & `otter-grader-4.4.0/otter/assign/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/assignment.py` & `otter-grader-4.4.0/otter/assign/v0/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/cell_generators.py` & `otter-grader-4.4.0/otter/assign/v0/cell_generators.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/constants.py` & `otter-grader-4.4.0/otter/assign/v0/constants.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/convert/__main__.py` & `otter-grader-4.4.0/otter/assign/v0/convert/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/convert/notebook_transformer.py` & `otter-grader-4.4.0/otter/assign/v0/convert/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/notebook_transformer.py` & `otter-grader-4.4.0/otter/assign/v0/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/output.py` & `otter-grader-4.4.0/otter/assign/v0/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/plugins.py` & `otter-grader-4.4.0/otter/assign/v0/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/questions.py` & `otter-grader-4.4.0/otter/assign/v0/questions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/r_adapter/tests.py` & `otter-grader-4.4.0/otter/assign/v0/r_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py` & `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/output.py` & `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/solutions.py` & `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/tests.py` & `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/rmarkdown_adapter/utils.py` & `otter-grader-4.4.0/otter/assign/v0/rmarkdown_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/solutions.py` & `otter-grader-4.4.0/otter/assign/v0/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/tests.py` & `otter-grader-4.4.0/otter/assign/v0/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/assign/v0/utils.py` & `otter-grader-4.4.0/otter/assign/v0/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/check/__init__.py` & `otter-grader-4.4.0/otter/check/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/check/logs.py` & `otter-grader-4.4.0/otter/check/logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/check/notebook.py` & `otter-grader-4.4.0/otter/check/notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/check/utils.py` & `otter-grader-4.4.0/otter/check/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/check/validate_export/__main__.py` & `otter-grader-4.4.0/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/cli.py` & `otter-grader-4.4.0/otter/cli.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/execute/__init__.py` & `otter-grader-4.4.0/otter/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/execute/checker.py` & `otter-grader-4.4.0/otter/execute/checker.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/execute/execute_log.py` & `otter-grader-4.4.0/otter/execute/execute_log.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/execute/execute_notebook.py` & `otter-grader-4.4.0/otter/execute/execute_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/execute/transforms.py` & `otter-grader-4.4.0/otter/execute/transforms.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/__init__.py` & `otter-grader-4.4.0/otter/export/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/__init__.py` & `otter-grader-4.4.0/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/base_exporter.py` & `otter-grader-4.4.0/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-4.4.0/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_html.tpl` & `otter-grader-4.4.0/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-4.4.0/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-4.4.0/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-4.4.0/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/utils.py` & `otter-grader-4.4.0/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/via_html.py` & `otter-grader-4.4.0/otter/export/exporters/via_html.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/export/exporters/via_latex.py` & `otter-grader-4.4.0/otter/export/exporters/via_latex.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/generate/__init__.py` & `otter-grader-4.4.0/otter/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/generate/templates/python/setup.sh` & `otter-grader-4.4.0/otter/generate/templates/python/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/generate/templates/r/setup.sh` & `otter-grader-4.4.0/otter/generate/templates/r/setup.sh`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/generate/token.py` & `otter-grader-4.4.0/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/generate/utils.py` & `otter-grader-4.4.0/otter/generate/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/grade/Dockerfile` & `otter-grader-4.4.0/otter/grade/Dockerfile`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/grade/__init__.py` & `otter-grader-4.4.0/otter/grade/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/grade/containers.py` & `otter-grader-4.4.0/otter/grade/containers.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/grade/utils.py` & `otter-grader-4.4.0/otter/grade/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/plugins/__init__.py` & `otter-grader-4.4.0/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/plugins/abstract_plugin.py` & `otter-grader-4.4.0/otter/plugins/abstract_plugin.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-4.4.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/plugins/builtin/grade_override.py` & `otter-grader-4.4.0/otter/plugins/builtin/grade_override.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             curr_dir = os.getcwd()
             os.chdir(assignment.master.parent)
 
         cfg_idx = [self.IMPORTABLE_NAME in c.keys() for c in otter_config["plugins"] if isinstance(c, dict)].index(True)
         creds_path = otter_config["plugins"][cfg_idx][self.IMPORTABLE_NAME]["credentials_json_path"]
         with open(creds_path, encoding="utf-8") as f:
             creds = json.load(f)
+
         otter_config["plugins"][cfg_idx][self.IMPORTABLE_NAME]["service_account_credentials"] = creds
 
         if assignment is not None:
             os.chdir(curr_dir)
 
     def before_grading(self, config):
         """
```

### Comparing `otter-grader-4.3.4/otter/plugins/builtin/rate_limiting.py` & `otter-grader-4.4.0/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/__init__.py` & `otter-grader-4.4.0/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/__init__.py` & `otter-grader-4.4.0/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/autograder_config.py` & `otter-grader-4.4.0/otter/run/run_autograder/autograder_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/runners/__init__.py` & `otter-grader-4.4.0/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-4.4.0/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-4.4.0/otter/run/run_autograder/runners/python_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-4.4.0/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/test_files/__init__.py` & `otter-grader-4.4.0/otter/test_files/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/test_files/abstract_test.py` & `otter-grader-4.4.0/otter/test_files/abstract_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
             else:
                 point_values.append(None)
 
         pre_specified = sum(p for p in point_values if p is not None)
         if total_points is not None:
             if pre_specified > total_points:
-                raise ValueError(f"More points specified in test cases that allowed for test")
+                raise ValueError(f"More points specified in test cases than allowed for test")
 
             else:
                 try:
                     per_remaining = (total_points - pre_specified) / sum(1 for p in point_values if p is None)
                 except ZeroDivisionError:
                     per_remaining = 0.0
```

### Comparing `otter-grader-4.3.4/otter/test_files/exception_test.py` & `otter-grader-4.4.0/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/test_files/metadata_test.py` & `otter-grader-4.4.0/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/test_files/ok_test.py` & `otter-grader-4.4.0/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/utils.py` & `otter-grader-4.4.0/otter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/otter/version.py` & `otter-grader-4.4.0/otter/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "4.3.4"
+__version__ = "4.4.0"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-4.3.4/otter_grader.egg-info/PKG-INFO` & `otter-grader-4.4.0/otter_grader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.3.4
+Version: 4.4.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.3.4/otter_grader.egg-info/SOURCES.txt` & `otter-grader-4.4.0/otter_grader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/setup.py` & `otter-grader-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_assign.py` & `otter-grader-4.4.0/test/test_assign.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,14 +219,34 @@
 
     # sum(4 / 11 for _ in range(11)) evaluates to 4.000000000000001 in Python, so this will
     # check that the per-test-case point values are correctly rounded.
     points = tests_mgr.determine_question_point_value(question)
     assert points == 4
 
 
+def test_determine_question_point_value_error_message():
+    """
+    Tests that error messages for point value validations contain the question name.
+    """
+    question = QuestionConfig({"name": "q1", "points": 1, "manual": False})
+    tests_mgr = AssignmentTestsManager(Assignment())
+    for _ in range(2):
+        tests_mgr._add_test_case(question, TestCase("", "", False, 1, "", ""))
+
+    exception = None
+    try:
+        tests_mgr.determine_question_point_value(question)
+    except Exception as e:
+        exception = e
+
+    assert str(exception) == "Error in \"q1\" test cases: More points specified in test cases " \
+        "than allowed for test"
+    assert type(exception) == ValueError
+
+
 def test_jupyterlite(generate_master_notebook):
     """
     """
     master_nb_path = generate_master_notebook({
         "runs_on": "jupyterlite",
         "tests": {"url_prefix": "https://domain.tld/tests/"}
     })
```

### Comparing `otter-grader-4.3.4/test/test_check.py` & `otter-grader-4.4.0/test/test_check.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_export.py` & `otter-grader-4.4.0/test/test_export.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_generate/test_autograder.py` & `otter-grader-4.4.0/test/test_generate/test_autograder.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_generate/test_token.py` & `otter-grader-4.4.0/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_grade.py` & `otter-grader-4.4.0/test/test_grade.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_logs.py` & `otter-grader-4.4.0/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_notebook.py` & `otter-grader-4.4.0/test/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.3.4/test/test_run.py` & `otter-grader-4.4.0/test/test_run.py`

 * *Files identical despite different names*

